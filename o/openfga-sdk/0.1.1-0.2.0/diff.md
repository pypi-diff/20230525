# Comparing `tmp/openfga-sdk-0.1.1.tar.gz` & `tmp/openfga-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfga-sdk-0.1.1.tar", last modified: Tue Jan 17 22:59:55 2023, max compression
+gzip compressed data, was "openfga-sdk-0.2.0.tar", last modified: Thu May 25 21:13:18 2023, max compression
```

## Comparing `openfga-sdk-0.1.1.tar` & `openfga-sdk-0.2.0.tar`

### file list

```diff
@@ -1,82 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 22:59:55.964293 openfga-sdk-0.1.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10176 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)    38733 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32334 2023-01-17 22:59:55.964293 openfga-sdk-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    31454 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 22:59:55.960293 openfga-sdk-0.1.1/openfga_sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4433 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 22:59:55.960293 openfga-sdk-0.1.1/openfga_sdk/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/api/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   117021 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/api/open_fga_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28946 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/api_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20173 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8106 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6822 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 22:59:55.964293 openfga-sdk-0.1.1/openfga_sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3904 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3657 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/any.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4864 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/assertion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5459 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/authorization_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6648 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/check_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/check_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3759 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/computed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4103 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/contextual_tuple_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3930 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/create_store_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5854 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/create_store_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4706 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/difference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7342 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/error_code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4979 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/expand_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3768 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/expand_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5794 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/get_store_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3819 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/internal_error_code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4607 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/internal_error_message_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5206 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/leaf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7926 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/list_objects_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3865 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/list_objects_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4742 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/list_stores_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3873 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6248 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/nodes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3495 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/not_found_error_code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4460 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/object_relation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4643 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/path_unknown_error_message_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4970 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/read_assertions_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4232 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/read_authorization_model_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/read_authorization_models_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4793 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/read_changes_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/read_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4670 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/read_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4303 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/relation_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5303 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/relation_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4940 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/store.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4340 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/tuple.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5254 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/tuple_change.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5687 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/tuple_key.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4023 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/tuple_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3323 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/tuple_operation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4735 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/tuple_to_userset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5327 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/type_definition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7712 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/userset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/userset_tree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4508 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/userset_tree_difference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4667 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/userset_tree_tuple_to_userset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3747 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/usersets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4607 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/validation_error_message_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4130 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/write_assertions_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5205 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/write_authorization_model_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4258 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/write_authorization_model_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5411 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/models/write_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10640 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/openfga_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 22:59:55.960293 openfga-sdk-0.1.1/openfga_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32334 2023-01-17 22:59:55.000000 openfga-sdk-0.1.1/openfga_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-01-17 22:59:55.000000 openfga-sdk-0.1.1/openfga_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 22:59:55.000000 openfga-sdk-0.1.1/openfga_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-17 22:59:55.000000 openfga-sdk-0.1.1/openfga_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-17 22:59:55.000000 openfga-sdk-0.1.1/openfga_sdk.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-01-17 22:59:55.964293 openfga-sdk-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 22:59:55.964293 openfga-sdk-0.1.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11039 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/test/test_credentials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50047 2023-01-17 22:59:47.000000 openfga-sdk-0.1.1/test/test_open_fga_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.647523 openfga-sdk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)   136821 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34636 2023-05-25 21:13:18.647523 openfga-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.639523 openfga-sdk-0.2.0/openfga_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.639523 openfga-sdk-0.2.0/openfga_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121526 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/api/open_fga_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29760 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.639523 openfga-sdk-0.2.0/openfga_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32165 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.639523 openfga-sdk-0.2.0/openfga_sdk/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/batch_check_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/check_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/expand_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/list_objects_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/list_relations_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/read_changes_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/write_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/write_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/write_single_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/client/models/write_transaction_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.647523 openfga-sdk-0.2.0/openfga_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/authorization_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/check_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/check_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/computed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/contextual_tuple_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/create_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/create_store_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/expand_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/expand_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/get_store_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/internal_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/internal_error_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/leaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/list_objects_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/list_objects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/list_stores_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/not_found_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/object_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/path_unknown_error_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/read_assertions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/read_authorization_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/read_authorization_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/read_changes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/read_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/read_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/relation_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/relation_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/tuple_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/tuple_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/tuple_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/tuple_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/tuple_to_userset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/type_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/userset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/userset_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/userset_tree_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/userset_tree_tuple_to_userset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/usersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/validation_error_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/write_assertions_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/write_authorization_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/write_authorization_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/models/write_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/openfga_sdk/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.639523 openfga-sdk-0.2.0/openfga_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34636 2023-05-25 21:13:18.000000 openfga-sdk-0.2.0/openfga_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-25 21:13:18.000000 openfga-sdk-0.2.0/openfga_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:13:18.000000 openfga-sdk-0.2.0/openfga_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 21:13:18.000000 openfga-sdk-0.2.0/openfga_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 21:13:18.000000 openfga-sdk-0.2.0/openfga_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 21:13:18.647523 openfga-sdk-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:13:18.647523 openfga-sdk-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    96026 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/test/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50837 2023-05-25 21:13:08.000000 openfga-sdk-0.2.0/test/test_open_fga_api.py
```

### Comparing `openfga-sdk-0.1.1/LICENSE` & `openfga-sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/README.md` & `openfga-sdk-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,70 @@
+Metadata-Version: 2.1
+Name: openfga-sdk
+Version: 0.2.0
+Summary: A high performance and flexible authorization/permission engine built for developers and inspired by Google Zanzibar.
+Home-page: https://github.com/openfga/python-sdk
+Author: OpenFGA (https://openfga.dev)
+Author-email: community@openfga.dev
+License: Apache-2.0
+Keywords: openfga,authorization,fga,fine-grained-authorization,rebac,zanzibar
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE.txt
+
 # Python SDK for OpenFGA
 
 [![pypi](https://img.shields.io/pypi/v/openfga_sdk.svg?style=flat)](https://pypi.org/project/openfga_sdk)
 [![Release](https://img.shields.io/github/v/release/openfga/python-sdk?sort=semver&color=green)](https://github.com/openfga/python-sdk/releases)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
-[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B4989%2Fgithub.com%2Fopenfga%2Fpython-sdk.svg?type=shield)](https://app.fossa.com/reports/824fbc44-7513-4496-84a4-f7ffb3fa23f7)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fopenfga%2Fpython-sdk.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fopenfga%2Fpython-sdk?ref=badge_shield)
 [![Discord Server](https://img.shields.io/discord/759188666072825867?color=7289da&logo=discord "Discord Server")](https://discord.com/channels/759188666072825867/930524706854031421)
 [![Twitter](https://img.shields.io/twitter/follow/openfga?color=%23179CF0&logo=twitter&style=flat-square "@openfga on Twitter")](https://twitter.com/openfga)
 
 This is an autogenerated python SDK for OpenFGA. It provides a wrapper around the [OpenFGA API definition](https://openfga.dev/api).
 
 ## Table of Contents
 
 - [About OpenFGA](#about)
 - [Resources](#resources)
 - [Installation](#installation)
 - [Getting Started](#getting-started)
   - [Initializing the API Client](#initializing-the-api-client)
   - [Get your Store ID](#get-your-store-id)
   - [Calling the API](#calling-the-api)
-    - [List All Stores](#list-stores)
-    - [Create a Store](#create-store)
-    - [Get a Store](#get-store)
-    - [Delete a Store](#delete-store)
-    - [Write Authorization Model](#write-authorization-model)
-    - [Read a Single Authorization Model](#read-a-single-authorization-model)
-    - [Read Authorization Model IDs](#read-authorization-model-ids)
-    - [Check](#check)
-    - [Write Tuples](#write-tuples)
-    - [Delete Tuples](#delete-tuples)
-    - [Expand](#expand)
-    - [Read Tuples](#read-tuples)
-    - [Read Changes (Watch)](#read-changes-watch)
-    - [List Objects](#list-objects)
+    - [Stores](#stores)
+      - [List All Stores](#list-stores)
+      - [Create a Store](#create-store)
+      - [Get a Store](#get-store)
+      - [Delete a Store](#delete-store)
+    - [Authorization Models](#authorization-models)
+      - [Read Authorization Models](#read-authorization-models)
+      - [Write Authorization Model](#write-authorization-model)
+      - [Read a Single Authorization Model](#read-a-single-authorization-model)
+      - [Read the Latest Authorization Model](#read-the-latest-authorization-model)
+    - [Relationship Tuples](#relationship-tuples)
+      - [Read Relationship Tuple Changes (Watch)](#read-relationship-tuple-changes-watch)
+      - [Read Relationship Tuples](#read-relationship-tuples)
+      - [Write (Create and Delete) Relationship Tuples](#write-create-and-delete-relationship-tuples)
+    - [Relationship Queries](#relationship-queries)
+      - [Check](#check)
+      - [Batch Check](#batch-check)
+      - [Expand](#expand)
+      - [List Objects](#list-objects)
+      - [List Relations](#list-relations)
+    - [Assertions](#assertions)
+      - [Read Assertions](#read-assertions)
+      - [Write Assertions](#write-assertions)
   - [API Endpoints](#api-endpoints)
   - [Models](#models)
 - [Contributing](#contributing)
   - [Issues](#issues)
   - [Pull Requests](#pull-requests)
 - [License](#license)
 
@@ -104,567 +133,627 @@
 
 ## Getting Started
 
 ### Initializing the API Client
 
 [Learn how to initialize your SDK](https://openfga.dev/docs/getting-started/setup-sdk-client)
 
-#### No Authentication ####
+The documentation below refers to the `OpenFgaClient`, to read the documentation for `OpenFgaApi`, check out the [`v0.1.1` documentation](https://github.com/openfga/python-sdk/tree/v0.1.1#readme).
 
-##### Without Store ID #####
+> The OpenFgaClient will by default retry API requests up to 15 times on 429 and 5xx errors.
 
-To configure the SDK API client without store ID, we can initialize the api client by specifying the scheme and host.
+#### No Credentials
 
 ```python
 import openfga_sdk
-from openfga_sdk.api import open_fga_api
-
-configuration = openfga_sdk.Configuration(
-    api_scheme = 'https',
-    api_host = 'api.fga.example'
-)
-
-async def api_setup():
-    # Enter a context with an instance of the API client
-    async with openfga_sdk.ApiClient(configuration) as api_client:
-        # Create an instance of the API class
-        api_instance = open_fga_api.OpenFgaApi(api_client)
-
-```
+from openfga_sdk.client import OpenFgaClient
 
-##### With Store ID #####
 
-To configure the SDK API client store ID, we can initialize the api client by specifying the scheme, host and store_id.
-
-```python
-import openfga_sdk
-from openfga_sdk.api import open_fga_api
-
-configuration = openfga_sdk.Configuration(
-    api_scheme = 'https',
-    api_host = 'api.fga.example',
-    store_id = 'YOUR_STORE_ID'
-)
-
-async def api_setup():
-    # Enter a context with an instance of the API client
-    async with openfga_sdk.ApiClient(configuration) as api_client:
-        # Create an instance of the API class
-        api_instance = open_fga_api.OpenFgaApi(api_client)
+async def main():
+    configuration = openfga_sdk.ClientConfiguration(
+        api_scheme = OPENFGA_API_SCHEME, # optional, defaults to "https"
+        api_host = OPENFGA_API_HOST, # required, define without the scheme (e.g. api.fga.example instead of https://api.fga.example)
+        store_id = OPENFGA_STORE_ID, # optional, not needed when calling `CreateStore` or `ListStores`
+        authorization_model_id = OPENFGA_AUTHORIZATION_MODEL_ID, # Optional, can be overridden per request
+    )
+    # Enter a context with an instance of the OpenFgaClient
+    async with OpenFgaClient(configuration) as fga_client:
+        api_response = await fga_client.read_authorization_models()
+        await fga_client.close()
 
 ```
 
-Another possibility is to use the existing configuration and add store id in its configuration
+#### API Token
 
 ```python
 import openfga_sdk
-from openfga_sdk.api import open_fga_api
-
-configuration = openfga_sdk.Configuration(
-    api_scheme = 'https',
-    api_host = 'api.fga.example'
-)
+from openfga_sdk.client import OpenFgaClient
+from openfga_sdk.credentials import Credentials, CredentialConfiguration
 
-async def api_setup():
-    configuration.store_id = 'YOUR_STORE_ID'
 
-    # Enter a context with an instance of the API client
-    async with openfga_sdk.ApiClient(configuration) as api_client:
-        # Create an instance of the API class
-        api_instance = open_fga_api.OpenFgaApi(api_client)
+async def main():
+    configuration = openfga_sdk.ClientConfiguration(
+        api_scheme = OPENFGA_API_SCHEME, # optional, defaults to "https"
+        api_host = OPENFGA_API_HOST, # required, define without the scheme (e.g. api.fga.example instead of https://api.fga.example)
+        store_id = OPENFGA_STORE_ID, # optional, not needed when calling `CreateStore` or `ListStores`
+        authorization_model_id = OPENFGA_AUTHORIZATION_MODEL_ID, # Optional, can be overridden per request
+        credentials = Credentials(
+            method='api_token',
+            configuration=CredentialConfiguration(
+                api_token= OPENFGA_API_TOKEN,
+            )
+        )
+    )
+    # Enter a context with an instance of the OpenFgaClient
+    async with OpenFgaClient(configuration) as fga_client:
+        api_response = await fga_client.read_authorization_models()
+        await fga_client.close()
 
 ```
 
-#### Authentication via API Token ####
-
-To configure the SDK API client with authentication via API TOKEN, we can initialize the api client by specifying the scheme, host and credentials.
+#### Client Credentials
 
 ```python
 import openfga_sdk
-from openfga_sdk.api import open_fga_api
+from openfga_sdk.client import OpenFgaClient
 from openfga_sdk.credentials import Credentials, CredentialConfiguration
 
-credentials = Credentials(method='api_token', configuration=CredentialConfiguration(api_token='TOKEN1'))
-configuration = openfga_sdk.Configuration(
-    api_scheme = 'https',
-    api_host = 'api.fga.example',
-    credentials = credentials
-)
 
-async def api_setup():
-    # Enter a context with an instance of the API client
-    async with openfga_sdk.ApiClient(configuration) as api_client:
-        # Create an instance of the API class
-        api_instance = open_fga_api.OpenFgaApi(api_client)
+async def main():
+    configuration = openfga_sdk.ClientConfiguration(
+        api_scheme = OPENFGA_API_SCHEME, # optional, defaults to "https"
+        api_host = OPENFGA_API_HOST, # required, define without the scheme (e.g. api.fga.example instead of https://api.fga.example)
+        store_id = OPENFGA_STORE_ID, # optional, not needed when calling `CreateStore` or `ListStores`
+        authorization_model_id = OPENFGA_AUTHORIZATION_MODEL_ID, # Optional, can be overridden per request
+        credentials = Credentials(
+            method='client_credentials',
+            configuration=CredentialConfiguration(
+                api_issuer= OPENFGA_API_TOKEN_ISSUER,
+                api_audience= OPENFGA_API_AUDIENCE,
+                client_id= OPENFGA_CLIENT_ID,
+                client_secret= OPENFGA_CLIENT_SECRET,
+            )
+        )
+    )
+    # Enter a context with an instance of the OpenFgaClient
+    async with OpenFgaClient(configuration) as fga_client:
+        api_response = await fga_client.read_authorization_models()
+        await fga_client.close()
 
 ```
 
 
 ### Get your Store ID
 
 You need your store id to call the OpenFGA API (unless it is to call the [CreateStore](#create-store) or [ListStores](#list-stores) methods).
 
 If your server is configured with [authentication enabled](https://openfga.dev/docs/getting-started/setup-openfga#configuring-authentication), you also need to have your credentials ready.
 
 ### Calling the API
 
-#### List Stores
+#### Stores
+
+##### List Stores
+
+Get a paginated list of stores.
 
 [API Documentation](https://openfga.dev/api/service/docs/api#/Stores/ListStores)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-)
+options = {"page_size": 25, "continuation_token": "eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ=="}
+response = await fga_client.get_store(options)
+# response = ListStoresResponse(...)
+# response.stores = [Store({"id": "01FQH7V8BEG3GPQW93KTRFR8JB", "name": "FGA Demo Store", "created_at": "2022-01-01T00:00:00.000Z", "updated_at": "2022-01-01T00:00:00.000Z"})]
+```
 
-# Get all stores
-async def list_stores():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
 
-    response = await api_instance.list_stores()
-    # response = ListStoreResponse(...)
-    # response.stores = [Store({"id": "01FQH7V8BEG3GPQW93KTRFR8JB", "name": "FGA Demo Store", "created_at": "2022-01-01T00:00:00.000Z", "updated_at": "2022-01-01T00:00:00.000Z"})]
-    await api_client.close()
-```
+##### Create Store
 
-#### Create Store
+Create and initialize a store.
 
 [API Documentation](https://openfga.dev/api/service/docs/api#/Stores/CreateStore)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
+body = CreateStoreRequest(
+    name = "FGA Demo Store",
 )
-
-# Create a store
-async def create_store():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-
-    body = CreateStoreRequest(
-        name = "FGA Demo Store",
-    )
-    response = await api_instance.create_store(body)
-    # response.id = "01FQH7V8BEG3GPQW93KTRFR8JB"
-    await api_client.close()
+response = await fga_client.create_store(body)
+# response.id = "01FQH7V8BEG3GPQW93KTRFR8JB"
 ```
 
 
-#### Get Store
+##### Get Store
+
+Get information about the current store.
 
 [API Documentation](https://openfga.dev/api/service/docs/api#/Stores/GetStore)
 
 > Requires a client initialized with a storeId
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
-
-# Get a store
-async def get_store():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-
-    response = await api_instance.get_store()
-    # response = Store({"id": "01FQH7V8BEG3GPQW93KTRFR8JB", "name": "FGA Demo Store", "created_at": "2022-01-01T00:00:00.000Z", "updated_at": "2022-01-01T00:00:00.000Z"})
-    await api_client.close()
+response = await fga_client.get_store()
+# response = Store({"id": "01FQH7V8BEG3GPQW93KTRFR8JB", "name": "FGA Demo Store", "created_at": "2022-01-01T00:00:00.000Z", "updated_at": "2022-01-01T00:00:00.000Z"})
 ```
 
 
-#### Delete Store
+##### Delete Store
+
+Delete a store.
 
 [API Documentation](https://openfga.dev/api/service/docs/api#/Stores/DeleteStore)
 
 > Requires a client initialized with a storeId
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
+response = await fga_client.delete_store()
+```
+
 
-# Delete a store
-async def delete_store():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
+#### Authorization Models
 
-    await api_instance.delete_store()
-    await api_client.close()
+##### Read Authorization Models
+
+Read all authorization models in the store.
+
+[API Documentation](https://openfga.dev/api/service#/Authorization%20Models/ReadAuthorizationModels)
+
+```python
+options = {"page_size": 25, "continuation_token": "eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ=="}
+response = await fga_client.read_authorization_models(options)
+# response.authorization_models = [AuthorizationModel(id='01GXSA8YR785C4FYS3C0RTG7B1', schema_version = '1.1', type_definitions=type_definitions[...], AuthorizationModel(id='01GXSBM5PVYHCJNRNKXMB4QZTW', schema_version = '1.1', type_definitions=type_definitions[...])]
 ```
 
-#### Write Authorization Model
 
-[API Documentation](https://openfga.dev/api/service#/Authorization%20Models/WriteAuthorizationModel)
+##### Write Authorization Model
 
-> Requires a client initialized with a storeId
+Create a new authorization model.
+
+[API Documentation](https://openfga.dev/api/service#/Authorization%20Models/WriteAuthorizationModel)
 
 > Note: To learn how to build your authorization model, check the Docs at https://openfga.dev/docs.
 
 > Learn more about [the OpenFGA configuration language](https://openfga.dev/docs/configuration-language).
 
+> You can use the [OpenFGA Syntax Transformer](https://github.com/openfga/syntax-transformer) to convert between the friendly DSL and the JSON authorization model.
+
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
-
-# Create a new authorization model
-async def write_authorization_model():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    type_definitions = WriteAuthorizationModelRequest(
-        type_definitions=[
-            TypeDefinition(
-                type="user",
-            ),
-            TypeDefinition(
-                type="document",
-                relations=dict(
-                    writer=Userset(
-                        this=dict(),
-                    ),
-                    viewer=Userset(
-                        union=Usersets(
-                            child=[
-                                Userset(this=dict()),
-                                Userset(computed_userset=ObjectRelation(
-                                    object="",
-                                    relation="writer",
-                                )),
-                            ],
-                        ),
+body = WriteAuthorizationModelRequest(
+    schema_version = "1.1",
+    type_definitions=[
+        TypeDefinition(
+            type="user",
+        ),
+        TypeDefinition(
+            type="document",
+            relations=dict(
+                writer=Userset(
+                    this=dict(),
+                ),
+                viewer=Userset(
+                    union=Usersets(
+                        child=[
+                            Userset(this=dict()),
+                            Userset(computed_userset=ObjectRelation(
+                                object="",
+                                relation="writer",
+                            )),
+                        ],
                     ),
-                )
-            ),
-        ],
-    )
+                ),
+            )
+        ),
+    ],
+)
 
-    response = await api_instance.write_authorization_model(type_definitions)
-    # response.authorization_model_id = "1uHxCSuTP0VKPYSnkq1pbb1jeZw"
-    await api_client.close()
+response = await fga_client.write_authorization_model(body)
+# response.authorization_model_id = "01GXSA8YR785C4FYS3C0RTG7B1"
 ```
 
 
-#### Read a Single Authorization Model
+##### Read a Single Authorization Model
+
+Read a particular authorization model.
 
 [API Documentation](https://openfga.dev/api/service#/Authorization%20Models/ReadAuthorizationModel)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
 
-# Return a particular version of an authorization model
-async def read_authorization_id():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    id = "1uHxCSuTP0VKPYSnkq1pbb1jeZw" #  Assuming `1uHxCSuTP0VKPYSnkq1pbb1jeZw` is an id of an existing model
-
-    response = await api_instance.read_authorization_model(id)
-    # response.authorization_model =  AuthorizationModel(id='1uHxCSuTP0VKPYSnkq1pbb1jeZw', type_definitions=type_definitions[...])
-    await api_client.close()
+response = await fga_client.read_authorization_model(id)
+# response.authorization_model =  AuthorizationModel(id='01GXSA8YR785C4FYS3C0RTG7B1', schema_version = '1.1', type_definitions=type_definitions[...])
 ```
 
-#### Read Authorization Model IDs
+##### Read the Latest Authorization Model
 
-[API Documentation](https://openfga.dev/api/service#/Authorization%20Models/ReadAuthorizationModels)
+Reads the latest authorization model (note: this ignores the model id in configuration).
+
+[API Documentation](https://openfga.dev/api/service#/Authorization%20Models/ReadAuthorizationModel)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
+response = await fga_client.read_latest_authorization_model()
+# response.authorization_model =  AuthorizationModel(id='01GXSA8YR785C4FYS3C0RTG7B1', schema_version = '1.1', type_definitions=type_definitions[...])
+```
 
-# Return all the authorization models for a particular store
-async def read_authorization_models():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
 
-    response = await api_instance.read_authorization_models()
-    # response.authorization_models = [AuthorizationModel(id='1uHxCSuTP0VKPYSnkq1pbb1jeZw', type_definitions=type_definitions[...], AuthorizationModel(id='GtQpMohWezFmIbyXxVEocOCxxgq', type_definitions=type_definitions[...])]
-    await api_client.close()
-```
+#### Relationship Tuples
 
+##### Read Relationship Tuple Changes (Watch)
 
-#### Check
+Reads the list of historical relationship tuple writes and deletes.
 
-[API Documentation](https://openfga.dev/api/service#/Relationship%20Queries/Check)
+[API Documentation](https://openfga.dev/api/service#/Relationship%20Tuples/ReadChanges)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
-
-# Check whether a user is authorized to access an object
-async def check():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    body = CheckRequest(
-        tuple_key=TupleKey(
-            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-            relation="viewer",
-            object="document:roadmap",
-        ),
-        authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
-    )
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "page_size": "25",
+    "continuation_token": "eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ=="
+}
+body = ClientReadChangesRequest("document")
 
-    response = await api_instance.check(body)
-    # response.allowed = True
-    await api_client.close()
+response = await api_instance.read_changes(body, options)
+# response.continuation_token = ...
+# response.changes = [TupleChange(tuple_key=TupleKey(object="...",relation="...",user="..."),operation=TupleOperation("TUPLE_OPERATION_WRITE"),timestamp=datetime.fromisoformat("..."))]
 ```
 
+##### Read Relationship Tuples
 
-#### Write Tuples
+Reads the relationship tuples stored in the database. It does not evaluate nor exclude invalid tuples according to the authorization model.
 
-[API Documentation](https://openfga.dev/api/service#/Relationship%20Tuples/Write)
+[API Documentation](https://openfga.dev/api/service#/Relationship%20Tuples/Read)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
-
-# Add tuples from the store
-async def write():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    body = WriteRequest(
-        writes=TupleKeys(
-            tuple_keys=[
-                TupleKey(
-                    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-                    relation="viewer",
-                    object="document:roadmap",
-                ),
-            ],
-        ),
-        authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
-    )
+# Find if a relationship tuple stating that a certain user is a viewer of certain document
+body = TupleKey(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="viewer",
+    object="document:roadmap",
+)
 
-    response = await api_instance.write(body)
-    await api_client.close()
+# Find all relationship tuples where a certain user has a relationship as any relation to a certain document
+body = TupleKey(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    object="document:roadmap",
+)
+
+# Find all relationship tuples where a certain user is a viewer of any document
+body = TupleKey(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="viewer",
+    object="document:",
+)
+
+# Find all relationship tuples where any user has a relationship as any relation with a particular document
+body = TupleKey(
+    object="document:roadmap",
+)
+
+// Read all stored relationship tuples
+body := ReadRequest()
+
+response = await api_instance.read(body)
+# response = ReadResponse({"tuples": [Tuple({"key": TupleKey({"user":"...","relation":"...","object":"..."}), "timestamp": datetime.fromisoformat("...") })]})
 ```
 
-#### Delete Tuples
+
+##### Write (Create and Delete) Relationship Tuples
+
+Create and/or delete relationship tuples to update the system state.
 
 [API Documentation](https://openfga.dev/api/service#/Relationship%20Tuples/Write)
 
+###### Transaction mode (default)
+
+By default, write runs in a transaction mode where any invalid operation (deleting a non-existing tuple, creating an existing tuple, one of the tuples was invalid) or a server error will fail the entire operation.
+
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
-
-# Delete tuples from the store
-async def delete():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    body = WriteRequest(
-        deletes=TupleKeys(
-            tuple_keys=[
-                TupleKey(
-                    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-                    relation="viewer",
-                    object="document:roadmap",
-                ),
-            ],
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = ClientWriteRequest(
+    writes=[
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="viewer",
+            object="document:roadmap",
         ),
-        authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
-    ) 
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="viewer",
+            object="document:budget",
+        ),
+    ],
+    deletes=[
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="writer",
+            object="document:roadmap",
+        ),
+    ],
+)
 
-    response = await api_instance.write(body)
-    await api_client.close()
+response = await fga_client.write(body, options)
 ```
 
-#### Expand
+Convenience `write_tuples` and `delete_tuples` methods are also available.
 
-[API Documentation](https://openfga.dev/api/service#/Relationship%20Queries/Expand)
+###### Non-transaction mode
 
-```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
+The SDK will split the writes into separate requests and send them sequentially to avoid violating rate limits.
 
-# Expand all relationships in userset tree format, and following userset rewrite rules.  Useful to reason about and debug a certain relationship
-async def expand():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    body = ExpandRequest(
-        tuple_key=TupleKey(
+```python
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1",
+    "transaction": WriteTransactionOpts(
+        disabled=True,
+        max_parallel_requests=10, # Maximum number of requests to issue in parallel
+        max_per_chunk=1, # Maximum number of requests to be sent in a transaction in a particular chunk
+    )
+}
+body = ClientWriteRequest(
+    writes=[
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
             relation="viewer",
             object="document:roadmap",
         ),
-        authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
-    )
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="viewer",
+            object="document:budget",
+        ),
+    ],
+    deletes=[
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="writer",
+            object="document:roadmap",
+        ),
+    ],
+)
 
-    response = await api_instance.expand(body)
-    # response = ExpandResponse({"tree": UsersetTree({"root": Node({"name": "document:roadmap#viewer", "leaf": Leaf({"users": Users({"users": ["user:81684243-9356-4421-8fbf-a4f8d36aa31b", "user:f52a4f7a-054d-47ff-bb6e-3ac81269988f"]})})})})})
-    await api_client.close()
+response = await fga_client.write(body, options)
 ```
 
-#### Read Changes
+#### Relationship Queries
 
-[API Documentation](https://openfga.dev/api/service#/Relationship%20Tuples/Read)
+##### Check
+
+Check if a user has a particular relation with an object.
+
+[API Documentation](https://openfga.dev/api/service#/Relationship%20Queries/Check)
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = ClientCheckRequest(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="writer",
+    object="document:roadmap",
 )
 
-async def read():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-
-    # Find if a relationship tuple stating that a certain user is a viewer of certain document
-    body = ReadRequest(
-        tuple_key=TupleKey(
+response = await fga_client.check(body, options)
+# response.allowed = True
+```
+
+
+##### Batch Check
+
+Run a set of [checks](#check). Batch Check will return `allowed: false` if it encounters an error, and will return the error in the body.
+If 429s or 5xxs are encountered, the underlying check will retry up to 15 times before giving up.
+
+```python
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = [ClientCheckRequest(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="viewer",
+    object="document:roadmap",
+    contextual_tuples=[ # optional
+        ClientTuple(
             user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-            relation="viewer",
+            relation="editor",
             object="document:roadmap",
         ),
-    ) 
-
-    # Find all relationship tuples where a certain user has a relationship as any relation to a certain document
-    body = ReadRequest(
-        tuple_key=TupleKey(
+    ]
+), ClientCheckRequest(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="admin",
+    object="document:roadmap",
+    contextual_tuples=[ # optional
+        ClientTuple(
             user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="editor",
             object="document:roadmap",
         ),
-    ) 
+    ]
+), ClientCheckRequest(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="creator",
+    object="document:roadmap",
+), ClientCheckRequest(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="deleter",
+    object="document:roadmap",
+)]
+
+response = await fga_client.batch_check(body, options)
+# response.responses = [{
+#   allowed: false,
+#   request: {
+#     user: "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+#     relation: "viewer",
+#     object: "document:roadmap",
+#     contextual_tuples: [{
+#       user: "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+#       relation: "editor",
+#       object: "document:roadmap"
+#     }]
+#   }
+# }, {
+#   allowed: false,
+#   request: {
+#     user: "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+#     relation: "admin",
+#     object: "document:roadmap",
+#     contextual_tuples: [{
+#       user: "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+#       relation: "editor",
+#       object: "document:roadmap"
+#     }]
+#   }
+# }, {
+#   allowed: false,
+#   request: {
+#     user: "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+#     relation: "creator",
+#     object: "document:roadmap",
+#   },
+#   error: <FgaError ...>
+# }, {
+#   allowed: true,
+#   request: {
+#     user: "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+#     relation: "deleter",
+#     object: "document:roadmap",
+#   }},
+# ]
+```
 
-    # Find all relationship tuples where a certain user is a viewer of any document
-    body = ReadRequest(
-        tuple_key=TupleKey(
-            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-            relation="viewer",
-            object="document:",
-        ),
-    )
+#### Expand
 
-    # Find all relationship tuples where any user has a relationship as any relation with a particular document
-    body = ReadRequest(
-        tuple_key=TupleKey(
-            object="document:roadmap",
-        ),
-    )
+Expands the relationships in userset tree format.
 
-    // Read all stored relationship tuples
-    body := ReadRequest()
+[API Documentation](https://openfga.dev/api/service#/Relationship%20Queries/Expand)
+
+```python
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = ClientExpandRequest(
+    relation="viewer",
+    object="document:roadmap",
+)
 
-    response = await api_instance.read(body)
-    # response = ReadResponse({"tuples": [Tuple({"key": TupleKey({"user":"...","relation":"...","object":"..."}), "timestamp": datetime.fromisoformat("...") })]})
-    await api_client.close()
+response = await fga_client.expand(body. options)
+# response = ExpandResponse({"tree": UsersetTree({"root": Node({"name": "document:roadmap#viewer", "leaf": Leaf({"users": Users({"users": ["user:81684243-9356-4421-8fbf-a4f8d36aa31b", "user:f52a4f7a-054d-47ff-bb6e-3ac81269988f"]})})})})})
 ```
 
-#### Read Changes (Watch)
 
-[API Documentation](https://openfga.dev/api/service#/Relationship%20Tuples/ReadChanges)
+##### List Objects
 
-```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
+List the objects of a particular type a user has access to.
 
-# Return a list of all the tuple changes
-async def read_changes():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
+[API Documentation](https://openfga.dev/api/service#/Relationship%20Queries/ListObjects)
 
-    type = "document"
-    page_size = 25
-    continuation_token = "eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ=="
+```python
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = ClientListObjectsRequest(
+    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation="viewer",
+    type="document",
+    contextual_tuples=[ # optional
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="writer",
+            object="document:budget",
+        ),
+    ]
+)
 
-    response = await api_instance.read_changes(type=type, page_size=page_size, continuation_token=continuation_token)
-    # response.continuation_token = ...
-    # response.changes = [TupleChange(tuple_key=TupleKey(object="...",relation="...",user="..."),operation=TupleOperation("TUPLE_OPERATION_WRITE"),timestamp=datetime.fromisoformat("..."))]
-    await api_client.close()
+response = await api_instance.list_objects(body)
+# response.objects = ["document:roadmap"]
 ```
 
-#### List Objects
+##### List Relations
 
-[API Documentation](https://openfga.dev/api/service#/Relationship%20Queries/ListObjects)
+List the relations a user has on an object.
 
 ```python
-configuration = openfga_sdk.Configuration(
-    api_scheme = os.environ.get(OPENFGA_API_SCHEME),
-    api_host = os.environ.get(OPENFGA_API_HOST),
-    store_id = os.environ.get(OPENFGA_STORE_ID),
-)
-
-# ListObjects lists all of the object ids for objects of the provided type that the given user has a specific relation with.
-async def list_objects():
-    # Create an instance of the API class
-    api_client = openfga_sdk.ApiClient(configuration)
-    api_instance = open_fga_api.OpenFgaApi(api_client)
-    body = ListObjectsRequest(
-        authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
-        user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-        relation="viewer",
-        type="document",
-        contextual_tuples=ContextualTupleKeys( # optional
-            tuple_keys=[
-                TupleKey(
-                    user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
-                    relation="writer",
-                    object="document:budget",
-                ),
-            ],
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = ClientListRelationsRequest(
+    user = "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    object = "document:roadmap",
+    relations = ["can_view", "can_edit", "can_delete", "can_rename"],
+    contextual_tuples=[ # optional
+        ClientTuple(
+            user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+            relation="writer",
+            object="document:budget",
         ),
-    )
+    ]
+)
+var response = await fga_client.list_relations(body, options);
+
+// response.relations = ["can_view", "can_edit"]
+```
+
+#### Assertions
+
+##### Read Assertions
+
+Read assertions for a particular authorization model.
+
+[API Documentation](https://openfga.dev/api/service#/Assertions/Read%20Assertions)
+
+```csharp
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+response = await fga_client.read_assertions(options);
+```
+
+##### Write Assertions
+
+Update the assertions for a particular authorization model.
+
+[API Documentation](https://openfga.dev/api/service#/Assertions/Write%20Assertions)
 
-    response = await api_instance.list_objects(body)
-    # response.objects = ["document:roadmap"]
-    await api_client.close()
+```csharp
+options = {
+    # You can rely on the model id set in the configuration or override it for this specific request
+    "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"
+}
+body = [ClientAssertion(
+    user = "user:81684243-9356-4421-8fbf-a4f8d36aa31b",
+    relation = "viewer",
+    object = "document:roadmap",
+    expectation = true,
+)];
+response = await fga_client.write_assertions(body, options);
 ```
 
 
 ### API Endpoints
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *OpenFgaApi* | [**check**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#check) | **POST** /stores/{store_id}/check | Check whether a user is authorized to access an object
 *OpenFgaApi* | [**create_store**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#create_store) | **POST** /stores | Create a store
 *OpenFgaApi* | [**delete_store**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#delete_store) | **DELETE** /stores/{store_id} | Delete a store
 *OpenFgaApi* | [**expand**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#expand) | **POST** /stores/{store_id}/expand | Expand all relationships in userset tree format, and following userset rewrite rules.  Useful to reason about and debug a certain relationship
 *OpenFgaApi* | [**get_store**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#get_store) | **GET** /stores/{store_id} | Get a store
-*OpenFgaApi* | [**list_objects**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#list_objects) | **POST** /stores/{store_id}/list-objects | [EXPERIMENTAL] Get all objects of the given type that the user has a relation with
+*OpenFgaApi* | [**list_objects**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#list_objects) | **POST** /stores/{store_id}/list-objects | List all objects of the given type that the user has a relation with
 *OpenFgaApi* | [**list_stores**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#list_stores) | **GET** /stores | List all stores
 *OpenFgaApi* | [**read**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#read) | **POST** /stores/{store_id}/read | Get tuples from the store that matches a query, without following userset rewrite rules
 *OpenFgaApi* | [**read_assertions**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#read_assertions) | **GET** /stores/{store_id}/assertions/{authorization_model_id} | Read assertions for an authorization model ID
 *OpenFgaApi* | [**read_authorization_model**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#read_authorization_model) | **GET** /stores/{store_id}/authorization-models/{id} | Return a particular version of an authorization model
 *OpenFgaApi* | [**read_authorization_models**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#read_authorization_models) | **GET** /stores/{store_id}/authorization-models | Return all the authorization models for a particular store
 *OpenFgaApi* | [**read_changes**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#read_changes) | **GET** /stores/{store_id}/changes | Return a list of all the tuple changes
 *OpenFgaApi* | [**write**](https://github.com/openfga/python-sdk/blob/main/docs/OpenFgaApi.md#write) | **POST** /stores/{store_id}/write | Add or delete tuples from the store
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/__init__.py` & `openfga-sdk-0.2.0/openfga_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,18 @@
    Documentation: https://openfga.dev/docs
    Support: https://discord.gg/8naAwJfWN6
    License: [Apache-2.0](https://github.com/openfga/python-sdk/blob/main/LICENSE)
 
    NOTE: This file was auto generated by OpenAPI Generator (https://openapi-generator.tech). DO NOT EDIT.
 """
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
+
+from openfga_sdk.client.client import OpenFgaClient
+from openfga_sdk.client.configuration import ClientConfiguration
 
 # import apis into sdk package
 from openfga_sdk.api.open_fga_api import OpenFgaApi
 
 # import ApiClient
 from openfga_sdk.api_client import ApiClient
 from openfga_sdk.configuration import Configuration
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/api/open_fga_api.py` & `openfga-sdk-0.2.0/openfga_sdk/api/open_fga_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     async def close(self):
         await self.api_client.close()
 
     async def check(self, body, **kwargs):  # noqa: E501
         """Check whether a user is authorized to access an object  # noqa: E501
 
-        The Check API queries to check if the user has a certain relationship with an object in a certain store. A `contextual_tuples` object may also be included in the body of the request. This object contains one field `tuple_keys`, which is an array of tuple keys. You may also provide an `authorization_model_id` in the body. This will be used to assert that the input `tuple_key` is valid for the model specified. If not specified, the assertion will be made against the latest authorization model ID. The response will return whether the relationship exists in the field `allowed`.  ## Example In order to check if user `user:anne` of type `user` has a `reader` relationship with object `document:2021-budget` given the following contextual tuple ```json {   \"user\": \"user:anne\",   \"relation\": \"member\",   \"object\": \"time_slot:office_hours\" } ``` the Check API can be used with the following request body: ```json {   \"tuple_key\": {     \"user\": \"user:anne\",     \"relation\": \"reader\",     \"object\": \"document:2021-budget\"   },   \"contextual_tuples\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"member\",         \"object\": \"time_slot:office_hours\"       }     ]   } } ``` OpenFGA's response will include `{ \"allowed\": true }` if there is a relationship and `{ \"allowed\": false }` if there isn't.  # noqa: E501
+        The Check API queries to check if the user has a certain relationship with an object in a certain store. A `contextual_tuples` object may also be included in the body of the request. This object contains one field `tuple_keys`, which is an array of tuple keys. You may also provide an `authorization_model_id` in the body. This will be used to assert that the input `tuple_key` is valid for the model specified. If not specified, the assertion will be made against the latest authorization model ID. It is strongly recommended to specify authorization model id for better performance. The response will return whether the relationship exists in the field `allowed`.  ## Example In order to check if user `user:anne` of type `user` has a `reader` relationship with object `document:2021-budget` given the following contextual tuple ```json {   \"user\": \"user:anne\",   \"relation\": \"member\",   \"object\": \"time_slot:office_hours\" } ``` the Check API can be used with the following request body: ```json {   \"tuple_key\": {     \"user\": \"user:anne\",     \"relation\": \"reader\",     \"object\": \"document:2021-budget\"   },   \"contextual_tuples\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"member\",         \"object\": \"time_slot:office_hours\"       }     ]   },   \"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\" } ``` OpenFGA's response will include `{ \"allowed\": true }` if there is a relationship and `{ \"allowed\": false }` if there isn't.  # noqa: E501
 
         >>> thread = await api.check(body)
 
         :param body: (required)
         :type body: CheckRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -72,15 +72,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return await(self.check_with_http_info(body, **kwargs))  # noqa: E501
 
     async def check_with_http_info(self, body, **kwargs):  # noqa: E501
         """Check whether a user is authorized to access an object  # noqa: E501
 
-        The Check API queries to check if the user has a certain relationship with an object in a certain store. A `contextual_tuples` object may also be included in the body of the request. This object contains one field `tuple_keys`, which is an array of tuple keys. You may also provide an `authorization_model_id` in the body. This will be used to assert that the input `tuple_key` is valid for the model specified. If not specified, the assertion will be made against the latest authorization model ID. The response will return whether the relationship exists in the field `allowed`.  ## Example In order to check if user `user:anne` of type `user` has a `reader` relationship with object `document:2021-budget` given the following contextual tuple ```json {   \"user\": \"user:anne\",   \"relation\": \"member\",   \"object\": \"time_slot:office_hours\" } ``` the Check API can be used with the following request body: ```json {   \"tuple_key\": {     \"user\": \"user:anne\",     \"relation\": \"reader\",     \"object\": \"document:2021-budget\"   },   \"contextual_tuples\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"member\",         \"object\": \"time_slot:office_hours\"       }     ]   } } ``` OpenFGA's response will include `{ \"allowed\": true }` if there is a relationship and `{ \"allowed\": false }` if there isn't.  # noqa: E501
+        The Check API queries to check if the user has a certain relationship with an object in a certain store. A `contextual_tuples` object may also be included in the body of the request. This object contains one field `tuple_keys`, which is an array of tuple keys. You may also provide an `authorization_model_id` in the body. This will be used to assert that the input `tuple_key` is valid for the model specified. If not specified, the assertion will be made against the latest authorization model ID. It is strongly recommended to specify authorization model id for better performance. The response will return whether the relationship exists in the field `allowed`.  ## Example In order to check if user `user:anne` of type `user` has a `reader` relationship with object `document:2021-budget` given the following contextual tuple ```json {   \"user\": \"user:anne\",   \"relation\": \"member\",   \"object\": \"time_slot:office_hours\" } ``` the Check API can be used with the following request body: ```json {   \"tuple_key\": {     \"user\": \"user:anne\",     \"relation\": \"reader\",     \"object\": \"document:2021-budget\"   },   \"contextual_tuples\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"member\",         \"object\": \"time_slot:office_hours\"       }     ]   },   \"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\" } ``` OpenFGA's response will include `{ \"allowed\": true }` if there is a relationship and `{ \"allowed\": false }` if there isn't.  # noqa: E501
 
         >>> thread = api.check_with_http_info(body)
 
         :param body: (required)
         :type body: CheckRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -94,14 +94,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(CheckResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -117,15 +118,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -184,14 +186,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def create_store(self, body, **kwargs):  # noqa: E501
         """Create a store  # noqa: E501
 
         Create a unique OpenFGA store which will be used to store authorization models and relationship tuples.  # noqa: E501
@@ -239,14 +242,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(CreateStoreResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -262,15 +266,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -322,14 +327,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def delete_store(self, **kwargs):  # noqa: E501
         """Delete a store  # noqa: E501
 
         Delete an OpenFGA store. This does not delete the data associated with the store, like tuples or authorization models.  # noqa: E501
@@ -373,14 +379,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
@@ -394,15 +401,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -446,21 +454,22 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def expand(self, body, **kwargs):  # noqa: E501
         """Expand all relationships in userset tree format, and following userset rewrite rules.  Useful to reason about and debug a certain relationship  # noqa: E501
 
-        The Expand API will return all users and usersets that have certain relationship with an object in a certain store. This is different from the `/stores/{store_id}/read` API in that both users and computed usersets are returned. Body parameters `tuple_key.object` and `tuple_key.relation` are all required. The response will return a tree whose leaves are the specific users and usersets. Union, intersection and difference operator are located in the intermediate nodes.  ## Example To expand all users that have the `reader` relationship with object `document:2021-budget`, use the Expand API with the following request body ```json {   \"tuple_key\": {     \"object\": \"document:2021-budget\",     \"relation\": \"reader\"   } } ``` OpenFGA's response will be a userset tree of the users and usersets that have read access to the document. ```json {   \"tree\":{     \"root\":{       \"type\":\"document:2021-budget#reader\",       \"union\":{         \"nodes\":[           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"users\":{                 \"users\":[                   \"user:bob\"                 ]               }             }           },           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"computed\":{                 \"userset\":\"document:2021-budget#writer\"               }             }           }         ]       }     }   } } ``` The caller can then call expand API for the `writer` relationship for the `document:2021-budget`.  # noqa: E501
+        The Expand API will return all users and usersets that have certain relationship with an object in a certain store. This is different from the `/stores/{store_id}/read` API in that both users and computed usersets are returned. Body parameters `tuple_key.object` and `tuple_key.relation` are all required. The response will return a tree whose leaves are the specific users and usersets. Union, intersection and difference operator are located in the intermediate nodes.  ## Example To expand all users that have the `reader` relationship with object `document:2021-budget`, use the Expand API with the following request body ```json {   \"tuple_key\": {     \"object\": \"document:2021-budget\",     \"relation\": \"reader\"   },   \"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\" } ``` OpenFGA's response will be a userset tree of the users and usersets that have read access to the document. ```json {   \"tree\":{     \"root\":{       \"type\":\"document:2021-budget#reader\",       \"union\":{         \"nodes\":[           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"users\":{                 \"users\":[                   \"user:bob\"                 ]               }             }           },           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"computed\":{                 \"userset\":\"document:2021-budget#writer\"               }             }           }         ]       }     }   } } ``` The caller can then call expand API for the `writer` relationship for the `document:2021-budget`.  # noqa: E501
 
         >>> thread = await api.expand(body)
 
         :param body: (required)
         :type body: ExpandRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -479,15 +488,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return await(self.expand_with_http_info(body, **kwargs))  # noqa: E501
 
     async def expand_with_http_info(self, body, **kwargs):  # noqa: E501
         """Expand all relationships in userset tree format, and following userset rewrite rules.  Useful to reason about and debug a certain relationship  # noqa: E501
 
-        The Expand API will return all users and usersets that have certain relationship with an object in a certain store. This is different from the `/stores/{store_id}/read` API in that both users and computed usersets are returned. Body parameters `tuple_key.object` and `tuple_key.relation` are all required. The response will return a tree whose leaves are the specific users and usersets. Union, intersection and difference operator are located in the intermediate nodes.  ## Example To expand all users that have the `reader` relationship with object `document:2021-budget`, use the Expand API with the following request body ```json {   \"tuple_key\": {     \"object\": \"document:2021-budget\",     \"relation\": \"reader\"   } } ``` OpenFGA's response will be a userset tree of the users and usersets that have read access to the document. ```json {   \"tree\":{     \"root\":{       \"type\":\"document:2021-budget#reader\",       \"union\":{         \"nodes\":[           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"users\":{                 \"users\":[                   \"user:bob\"                 ]               }             }           },           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"computed\":{                 \"userset\":\"document:2021-budget#writer\"               }             }           }         ]       }     }   } } ``` The caller can then call expand API for the `writer` relationship for the `document:2021-budget`.  # noqa: E501
+        The Expand API will return all users and usersets that have certain relationship with an object in a certain store. This is different from the `/stores/{store_id}/read` API in that both users and computed usersets are returned. Body parameters `tuple_key.object` and `tuple_key.relation` are all required. The response will return a tree whose leaves are the specific users and usersets. Union, intersection and difference operator are located in the intermediate nodes.  ## Example To expand all users that have the `reader` relationship with object `document:2021-budget`, use the Expand API with the following request body ```json {   \"tuple_key\": {     \"object\": \"document:2021-budget\",     \"relation\": \"reader\"   },   \"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\" } ``` OpenFGA's response will be a userset tree of the users and usersets that have read access to the document. ```json {   \"tree\":{     \"root\":{       \"type\":\"document:2021-budget#reader\",       \"union\":{         \"nodes\":[           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"users\":{                 \"users\":[                   \"user:bob\"                 ]               }             }           },           {             \"type\":\"document:2021-budget#reader\",             \"leaf\":{               \"computed\":{                 \"userset\":\"document:2021-budget#writer\"               }             }           }         ]       }     }   } } ``` The caller can then call expand API for the `writer` relationship for the `document:2021-budget`.  # noqa: E501
 
         >>> thread = api.expand_with_http_info(body)
 
         :param body: (required)
         :type body: ExpandRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -501,14 +510,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ExpandResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -524,15 +534,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -591,14 +602,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def get_store(self, **kwargs):  # noqa: E501
         """Get a store  # noqa: E501
 
         Returns an OpenFGA store by its identifier  # noqa: E501
@@ -642,14 +654,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(GetStoreResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -663,15 +676,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -720,21 +734,22 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def list_objects(self, body, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] Get all objects of the given type that the user has a relation with  # noqa: E501
+        """List all objects of the given type that the user has a relation with  # noqa: E501
 
-        The ListObjects API returns a list of all the objects of the given type that the user has a relation with. To achieve this, both the store tuples and the authorization model are used. An `authorization_model_id` may be specified in the body. If it is, it will be used to decide the underlying implementation used. If it is not specified, the latest authorization model ID will be used. You may also specify `contextual_tuples` that will be treated as regular tuples. The response will contain the related objects in an array in the \"objects\" field of the response and they will be strings in the object format `<type>:<id>` (e.g. \"document:roadmap\")    # noqa: E501
+        The ListObjects API returns a list of all the objects of the given type that the user has a relation with. To achieve this, both the store tuples and the authorization model are used. An `authorization_model_id` may be specified in the body. If it is, it will be used to decide the underlying implementation used. If it is not specified, the latest authorization model ID will be used. It is strongly recommended to specify authorization model id for better performance. You may also specify `contextual_tuples` that will be treated as regular tuples. The response will contain the related objects in an array in the \"objects\" field of the response and they will be strings in the object format `<type>:<id>` (e.g. \"document:roadmap\"). The number of objects in the response array will be limited by the execution timeout specified in the flag OPENFGA_LIST_OBJECTS_DEADLINE and by the upper bound specified in the flag OPENFGA_LIST_OBJECTS_MAX_RESULTS, whichever is hit first.  Note: If you have `and` or `but not` in your model while using ListObjects, checkout the [caveats](https://openfga.dev/docs/interacting/relationship-queries#caveats-and-when-not-to-use-it-3).   # noqa: E501
 
         >>> thread = await api.list_objects(body)
 
         :param body: (required)
         :type body: ListObjectsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -751,17 +766,17 @@
                  returns the request thread.
         :rtype: ListObjectsResponse
         """
         kwargs['_return_http_data_only'] = True
         return await(self.list_objects_with_http_info(body, **kwargs))  # noqa: E501
 
     async def list_objects_with_http_info(self, body, **kwargs):  # noqa: E501
-        """[EXPERIMENTAL] Get all objects of the given type that the user has a relation with  # noqa: E501
+        """List all objects of the given type that the user has a relation with  # noqa: E501
 
-        The ListObjects API returns a list of all the objects of the given type that the user has a relation with. To achieve this, both the store tuples and the authorization model are used. An `authorization_model_id` may be specified in the body. If it is, it will be used to decide the underlying implementation used. If it is not specified, the latest authorization model ID will be used. You may also specify `contextual_tuples` that will be treated as regular tuples. The response will contain the related objects in an array in the \"objects\" field of the response and they will be strings in the object format `<type>:<id>` (e.g. \"document:roadmap\")    # noqa: E501
+        The ListObjects API returns a list of all the objects of the given type that the user has a relation with. To achieve this, both the store tuples and the authorization model are used. An `authorization_model_id` may be specified in the body. If it is, it will be used to decide the underlying implementation used. If it is not specified, the latest authorization model ID will be used. It is strongly recommended to specify authorization model id for better performance. You may also specify `contextual_tuples` that will be treated as regular tuples. The response will contain the related objects in an array in the \"objects\" field of the response and they will be strings in the object format `<type>:<id>` (e.g. \"document:roadmap\"). The number of objects in the response array will be limited by the execution timeout specified in the flag OPENFGA_LIST_OBJECTS_DEADLINE and by the upper bound specified in the flag OPENFGA_LIST_OBJECTS_MAX_RESULTS, whichever is hit first.  Note: If you have `and` or `but not` in your model while using ListObjects, checkout the [caveats](https://openfga.dev/docs/interacting/relationship-queries#caveats-and-when-not-to-use-it-3).   # noqa: E501
 
         >>> thread = api.list_objects_with_http_info(body)
 
         :param body: (required)
         :type body: ListObjectsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -775,14 +790,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ListObjectsResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -798,15 +814,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -865,14 +882,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def list_stores(self, **kwargs):  # noqa: E501
         """List all stores  # noqa: E501
 
         Returns a paginated list of OpenFGA stores.  # noqa: E501
@@ -924,14 +942,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ListStoresResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -947,15 +966,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1004,14 +1024,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def read(self, body, **kwargs):  # noqa: E501
         """Get tuples from the store that matches a query, without following userset rewrite rules  # noqa: E501
 
         The Read API will return the tuples for a certain store that match a query filter specified in the body of the request. It is different from the `/stores/{store_id}/expand` API in that it only returns relationship tuples that are stored in the system and satisfy the query.  In the body: 1. tuple_key is optional.  If tuple_key is not specified, it will return all tuples in the store.2. `tuple_key.object` is mandatory if tuple_key is specified. It can be a full object (e.g., `type:object_id`) or type only (e.g., `type:`). 3. `tuple_key.user` is mandatory if tuple_key is specified in the case the `tuple_key.object` is a type only. ## Examples ### Query for all objects in a type definition To query for all objects that `user:bob` has `reader` relationship in the document type definition, call read API with body of ```json {  \"tuple_key\": {      \"user\": \"user:bob\",      \"relation\": \"reader\",      \"object\": \"document:\"   } } ``` The API will return tuples and an optional continuation token, something like ```json {   \"tuples\": [     {       \"key\": {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       },       \"timestamp\": \"2021-10-06T15:32:11.128Z\"     }   ] } ``` This means that `user:bob` has a `reader` relationship with 1 document `document:2021-budget`. ### Query for all stored relationship tuples that have a particular relation and object To query for all users that have `reader` relationship with `document:2021-budget`, call read API with body of  ```json {   \"tuple_key\": {      \"object\": \"document:2021-budget\",      \"relation\": \"reader\"    } } ``` The API will return something like  ```json {   \"tuples\": [     {       \"key\": {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       },       \"timestamp\": \"2021-10-06T15:32:11.128Z\"     }   ] } ``` This means that `document:2021-budget` has 1 `reader` (`user:bob`).  Note that the API will not return writers such as `user:anne` even when all writers are readers.  This is because only direct relationship are returned for the READ API. ### Query for all users with all relationships for a particular document To query for all users that have any relationship with `document:2021-budget`, call read API with body of  ```json {   \"tuple_key\": {       \"object\": \"document:2021-budget\"    } } ``` The API will return something like  ```json {   \"tuples\": [     {       \"key\": {         \"user\": \"user:anne\",         \"relation\": \"writer\",         \"object\": \"document:2021-budget\"       },       \"timestamp\": \"2021-10-05T13:42:12.356Z\"     },     {       \"key\": {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       },       \"timestamp\": \"2021-10-06T15:32:11.128Z\"     }   ] } ``` This means that `document:2021-budget` has 1 `reader` (`user:bob`) and 1 `writer` (`user:anne`).   # noqa: E501
@@ -1059,14 +1080,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ReadResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -1082,15 +1104,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1149,14 +1172,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def read_assertions(self, authorization_model_id, **kwargs):  # noqa: E501
         """Read assertions for an authorization model ID  # noqa: E501
 
         The ReadAssertions API will return, for a given authorization model id, all the assertions stored for it. An assertion is an object that contains a tuple key, and the expectation of whether a call to the Check API of that tuple key will return true or false.   # noqa: E501
@@ -1204,14 +1228,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ReadAssertionsResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -1227,15 +1252,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1291,14 +1317,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def read_authorization_model(self, id, **kwargs):  # noqa: E501
         """Return a particular version of an authorization model  # noqa: E501
 
         The ReadAuthorizationModel API returns an authorization model by its identifier. The response will return the authorization model for the particular version.  ## Example To retrieve the authorization model with ID `01G5JAVJ41T49E9TT3SKVS7X1J` for the store, call the GET authorization-models by ID API with `01G5JAVJ41T49E9TT3SKVS7X1J` as the `id` path parameter.  The API will return: ```json {   \"authorization_model\":{     \"id\":\"01G5JAVJ41T49E9TT3SKVS7X1J\",     \"type_definitions\":[       {         \"type\":\"user\"       },       {         \"type\":\"document\",         \"relations\":{           \"reader\":{             \"union\":{               \"child\":[                 {                   \"this\":{}                 },                 {                   \"computedUserset\":{                     \"object\":\"\",                     \"relation\":\"writer\"                   }                 }               ]             }           },           \"writer\":{             \"this\":{}           }         }       }     ]   } } ``` In the above example, there are 2 types (`user` and `document`). The `document` type has 2 relations (`writer` and `reader`).  # noqa: E501
@@ -1346,14 +1373,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ReadAuthorizationModelResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -1369,15 +1397,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1432,14 +1461,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def read_authorization_models(self, **kwargs):  # noqa: E501
         """Return all the authorization models for a particular store  # noqa: E501
 
         The ReadAuthorizationModels API will return all the authorization models for a certain store. OpenFGA's response will contain an array of all authorization models, sorted in descending order of creation.  ## Example Assume that a store's authorization model has been configured twice. To get all the authorization models that have been created in this store, call GET authorization-models. The API will return a response that looks like: ```json {   \"authorization_models\": [     {       \"id\": \"01G50QVV17PECNVAHX1GG4Y5NC\",       \"type_definitions\": [...]     },     {       \"id\": \"01G4ZW8F4A07AKQ8RHSVG9RW04\",       \"type_definitions\": [...]     },   ] } ``` If there are more authorization models available, the response will contain an extra field `continuation_token`: ```json {   \"authorization_models\": [     {       \"id\": \"01G50QVV17PECNVAHX1GG4Y5NC\",       \"type_definitions\": [...]     },     {       \"id\": \"01G4ZW8F4A07AKQ8RHSVG9RW04\",       \"type_definitions\": [...]     },   ],   \"continuation_token\": \"eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ==\" } ```   # noqa: E501
@@ -1491,14 +1521,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ReadAuthorizationModelsResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -1514,15 +1545,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1575,14 +1607,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def read_changes(self, **kwargs):  # noqa: E501
         """Return a list of all the tuple changes  # noqa: E501
 
         The ReadChanges API will return a paginated list of tuple changes (additions and deletions) that occurred in a given store, sorted by ascending time. The response will include a continuation token that is used to get the next set of changes. If there are no changes after the provided continuation token, the same token will be returned in order for it to be used when new changes are recorded. If the store never had any tuples added or removed, this token will be empty. You can use the `type` parameter to only get the list of tuple changes that affect objects of that type.   # noqa: E501
@@ -1638,14 +1671,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ReadChangesResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -1662,15 +1696,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1725,21 +1760,22 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def write(self, body, **kwargs):  # noqa: E501
         """Add or delete tuples from the store  # noqa: E501
 
-        The Write API will update the tuples for a certain store. Tuples and type definitions allow OpenFGA to determine whether a relationship exists between an object and an user. In the body, `writes` adds new tuples while `deletes` removes existing tuples. The API is not idempotent: if, later on, you try to add the same tuple, or if you try to delete a non-existing tuple, it will throw an error. An `authorization_model_id` may be specified in the body. If it is, it will be used to assert that each written tuple (not deleted) is valid for the model specified. If it is not specified, the latest authorization model ID will be used. ## Example ### Adding relationships To add `user:anne` as a `writer` for `document:2021-budget`, call write API with the following  ```json {   \"writes\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"writer\",         \"object\": \"document:2021-budget\"       }     ]   } } ``` ### Removing relationships To remove `user:bob` as a `reader` for `document:2021-budget`, call write API with the following  ```json {   \"deletes\": {     \"tuple_keys\": [       {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       }     ]   } } ```   # noqa: E501
+        The Write API will update the tuples for a certain store. Tuples and type definitions allow OpenFGA to determine whether a relationship exists between an object and an user. In the body, `writes` adds new tuples while `deletes` removes existing tuples. The API is not idempotent: if, later on, you try to add the same tuple, or if you try to delete a non-existing tuple, it will throw an error. An `authorization_model_id` may be specified in the body. If it is, it will be used to assert that each written tuple (not deleted) is valid for the model specified. If it is not specified, the latest authorization model ID will be used. ## Example ### Adding relationships To add `user:anne` as a `writer` for `document:2021-budget`, call write API with the following  ```json {   \"writes\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"writer\",         \"object\": \"document:2021-budget\"       }     ]   },   \"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\" } ``` ### Removing relationships To remove `user:bob` as a `reader` for `document:2021-budget`, call write API with the following  ```json {   \"deletes\": {     \"tuple_keys\": [       {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       }     ]   } } ```   # noqa: E501
 
         >>> thread = await api.write(body)
 
         :param body: (required)
         :type body: WriteRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1758,15 +1794,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return await(self.write_with_http_info(body, **kwargs))  # noqa: E501
 
     async def write_with_http_info(self, body, **kwargs):  # noqa: E501
         """Add or delete tuples from the store  # noqa: E501
 
-        The Write API will update the tuples for a certain store. Tuples and type definitions allow OpenFGA to determine whether a relationship exists between an object and an user. In the body, `writes` adds new tuples while `deletes` removes existing tuples. The API is not idempotent: if, later on, you try to add the same tuple, or if you try to delete a non-existing tuple, it will throw an error. An `authorization_model_id` may be specified in the body. If it is, it will be used to assert that each written tuple (not deleted) is valid for the model specified. If it is not specified, the latest authorization model ID will be used. ## Example ### Adding relationships To add `user:anne` as a `writer` for `document:2021-budget`, call write API with the following  ```json {   \"writes\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"writer\",         \"object\": \"document:2021-budget\"       }     ]   } } ``` ### Removing relationships To remove `user:bob` as a `reader` for `document:2021-budget`, call write API with the following  ```json {   \"deletes\": {     \"tuple_keys\": [       {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       }     ]   } } ```   # noqa: E501
+        The Write API will update the tuples for a certain store. Tuples and type definitions allow OpenFGA to determine whether a relationship exists between an object and an user. In the body, `writes` adds new tuples while `deletes` removes existing tuples. The API is not idempotent: if, later on, you try to add the same tuple, or if you try to delete a non-existing tuple, it will throw an error. An `authorization_model_id` may be specified in the body. If it is, it will be used to assert that each written tuple (not deleted) is valid for the model specified. If it is not specified, the latest authorization model ID will be used. ## Example ### Adding relationships To add `user:anne` as a `writer` for `document:2021-budget`, call write API with the following  ```json {   \"writes\": {     \"tuple_keys\": [       {         \"user\": \"user:anne\",         \"relation\": \"writer\",         \"object\": \"document:2021-budget\"       }     ]   },   \"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\" } ``` ### Removing relationships To remove `user:bob` as a `reader` for `document:2021-budget`, call write API with the following  ```json {   \"deletes\": {     \"tuple_keys\": [       {         \"user\": \"user:bob\",         \"relation\": \"reader\",         \"object\": \"document:2021-budget\"       }     ]   } } ```   # noqa: E501
 
         >>> thread = api.write_with_http_info(body)
 
         :param body: (required)
         :type body: WriteRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -1780,14 +1816,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
@@ -1803,15 +1840,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -1870,14 +1908,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def write_assertions(self, authorization_model_id, body, **kwargs):  # noqa: E501
         """Upsert assertions for an authorization model ID  # noqa: E501
 
         The WriteAssertions API will upsert new assertions for an authorization model id, or overwrite the existing ones. An assertion is an object that contains a tuple key, and the expectation of whether a call to the Check API of that tuple key will return true or false.   # noqa: E501
@@ -1929,14 +1968,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
@@ -1954,15 +1994,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -2023,14 +2064,15 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
 
     async def write_authorization_model(self, body, **kwargs):  # noqa: E501
         """Create a new authorization model  # noqa: E501
 
         The WriteAuthorizationModel API will add a new authorization model to a store. Each item in the `type_definitions` array is a type definition as specified in the field `type_definition`. The response will return the authorization model's ID in the `id` field.  ## Example To add an authorization model with `user` and `document` type definitions, call POST authorization-models API with the body:  ```json {   \"type_definitions\":[     {       \"type\":\"user\"     },     {       \"type\":\"document\",       \"relations\":{         \"reader\":{           \"union\":{             \"child\":[               {                 \"this\":{}               },               {                 \"computedUserset\":{                   \"object\":\"\",                   \"relation\":\"writer\"                 }               }             ]           }         },         \"writer\":{           \"this\":{}         }       }     }   ] } ``` OpenFGA's response will include the version id for this authorization model, which will look like  ``` {\"authorization_model_id\": \"01G50QVV17PECNVAHX1GG4Y5NC\"} ```   # noqa: E501
@@ -2078,14 +2120,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_param: if specified, override the retry parameters specified in configuration
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(WriteAuthorizationModelResponse, status_code(int), headers(HTTPHeaderDict))
         """
@@ -2101,15 +2144,16 @@
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
                 '_request_auth',
                 '_content_type',
-                '_headers'
+                '_headers',
+                '_retry_parms'
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise FgaValidationException(
                     "Got an unexpected keyword argument '%s'"
@@ -2168,9 +2212,10 @@
             files=local_var_files,
             response_types_map=response_types_map,
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
+            _retry_params=local_var_params.get('_retry_params'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth')))
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/api_client.py` & `openfga-sdk-0.2.0/openfga_sdk/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         self.user_agent = 'openfga-sdk {sdkId}/{packageVersion}'.replace(
-            '{sdkId}', '').replace('{packageVersion}', '0.1.1')
+            '{sdkId}', 'python').replace('{packageVersion}', '0.2.0')
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
@@ -134,15 +134,15 @@
 
     async def __call_api(
             self, resource_path, method, path_params=None,
             query_params=None, header_params=None, body=None, post_params=None,
             response_types_map=None, auth_settings=None,
             _return_http_data_only=None, collection_formats=None,
             _preload_content=True, _request_timeout=None, _host=None,
-            _request_auth=None):
+            _request_auth=None, _retry_params=None):
 
         self.configuration.is_valid()
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
@@ -194,14 +194,19 @@
             # use server/host defined in path or operation instead
             url = self.configuration.api_scheme + '://' + _host + resource_path
 
         max_retry = self.configuration.retry_params.max_retry if (
             self.configuration.retry_params is not None and self.configuration.retry_params.max_retry is not None) else 0
         min_wait_in_ms = self.configuration.retry_params.min_wait_in_ms if (
             self.configuration.retry_params is not None and self.configuration.retry_params.min_wait_in_ms is not None) else 0
+        if _retry_params is not None:
+            if _retry_params.max_retry is not None:
+                max_retry = _retry_params.max_retry
+            if _retry_params.min_wait_in_ms is not None:
+                max_retry = _retry_params.min_wait_in_ms
         for x in range(max_retry + 1):
             try:
                 # perform request and return response
                 response_data = await self.request(
                     method, url, query_params=query_params, headers=header_params,
                     post_params=post_params, body=body,
                     _preload_content=_preload_content,
@@ -328,16 +333,16 @@
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
-            if klass.startswith('dict('):
-                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
+            if klass.startswith('dict['):
+                sub_kls = re.match(r'dict\[([^,]*), (.*)\]', klass).group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -356,15 +361,16 @@
 
     async def call_api(self, resource_path, method,
                        path_params=None, query_params=None, header_params=None,
                        body=None, post_params=None, files=None,
                        response_types_map=None, auth_settings=None,
                        async_req=None, _return_http_data_only=None,
                        collection_formats=None, _preload_content=True,
-                       _request_timeout=None, _host=None, _request_auth=None):
+                       _request_timeout=None, _host=None, _request_auth=None,
+                       _retry_params=None):
         """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async_req request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
@@ -388,14 +394,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
+        :param _retry_params: If specified, override the default retry parameters
         :type _request_token: dict, optional
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
@@ -403,28 +410,28 @@
         if not async_req:
             return await(self.__call_api(resource_path, method,
                                          path_params, query_params, header_params,
                                          body, post_params,
                                          response_types_map, auth_settings,
                                          _return_http_data_only, collection_formats,
                                          _preload_content, _request_timeout, _host,
-                                         _request_auth))
+                                         _request_auth, _retry_params))
 
         return self.pool.apply_async(self.__call_api, (resource_path,
                                                        method, path_params,
                                                        query_params,
                                                        header_params, body,
                                                        post_params,
                                                        response_types_map,
                                                        auth_settings,
                                                        _return_http_data_only,
                                                        collection_formats,
                                                        _preload_content,
                                                        _request_timeout,
-                                                       _host, _request_auth))
+                                                       _host, _request_auth, _retry_params))
 
     async def request(self, method, url, query_params=None, headers=None,
                       post_params=None, body=None, _preload_content=True,
                       _request_timeout=None):
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
             return await(self.rest_client.GET(url,
@@ -673,14 +680,15 @@
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
+        kwargs["local_vars_configuration"] = self.configuration
         instance = klass(**kwargs)
 
         if has_discriminator:
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
@@ -693,7 +701,19 @@
         """
         configuration = self.configuration
         if configuration.store_id is None or configuration.store_id == '':
             raise FgaValidationException(
                 'store_id is required but not configured'
             )
         return configuration.store_id
+
+    def set_store_id(self, value):
+        """
+        Update the store ID in the configuration
+        """
+        self.configuration.store_id = value
+
+    def get_store_id(self):
+        """
+        Return the store id (if any) store in the configuration
+        """
+        return self.configuration.store_id
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/configuration.py` & `openfga-sdk-0.2.0/openfga_sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 import urllib3
 
 import six
 from six.moves import http_client as httplib
 from urllib.parse import urlparse
 from openfga_sdk.exceptions import FgaValidationException, ApiValueError
+from openfga_sdk.validation import is_well_formed_ulid_string
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -38,15 +39,15 @@
 
     Retry configuration in case of HTTP too many request
 
     :param max_retry: Maximum number of retry
     :param min_wait_in_ms: Minimum wait (in ms) between retry
     """
 
-    def __init__(self, max_retry=3, min_wait_in_ms=100):
+    def __init__(self, max_retry=15, min_wait_in_ms=100):
         self._max_retry = max_retry
         self._min_wait_in_ms = min_wait_in_ms
 
     @property
     def max_retry(self):
         """
         Return the maximum number of retry
@@ -434,15 +435,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.1.1".\
+               "SDK Package Version: 0.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
@@ -515,14 +516,19 @@
             raise ApiValueError('api_host `{}` is invalid'.format(self.api_host))
         if (parsed_url.path != ''):
             raise ApiValueError(
                 'api_host `{}` is not expected to have path specified'.format(self.api_scheme))
         if (parsed_url.query != ''):
             raise ApiValueError(
                 'api_host `{}` is not expected to have query specified'.format(self.api_scheme))
+
+        if self.store_id is not None and self.store_id != "" and is_well_formed_ulid_string(self.store_id) is False:
+            raise FgaValidationException(
+                "store_id ('%s') is not in a valid ulid format" % self.store_id)
+
         if self._credentials is not None:
             self._credentials.validate_credentials_config()
 
     @property
     def api_scheme(self):
         """Return connection is https or http."""
         return self._scheme
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/credentials.py` & `openfga-sdk-0.2.0/openfga_sdk/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         body = {
             'client_id': self.configuration.client_id,
             'client_secret': self.configuration.client_secret,
             'audience': self.configuration.api_audience,
             'grant_type': "client_credentials",
         }
         headers = urllib3.response.HTTPHeaderDict(
-            {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk (python) 0.1.1'})
+            {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk (python) 0.2.0'})
         raw_response = await client.POST(token_url, headers=headers, body=body)
         if 200 <= raw_response.status <= 299:
             try:
                 api_response = json.loads(raw_response.data)
             except:  # noqa: E722
                 raise AuthenticationError(http_resp=raw_response)
             if not api_response.get('expires_in') or not api_response.get('access_token'):
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/exceptions.py` & `openfga-sdk-0.2.0/openfga_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/__init__.py` & `openfga-sdk-0.2.0/openfga_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/any.py` & `openfga-sdk-0.2.0/openfga_sdk/models/any.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/assertion.py` & `openfga-sdk-0.2.0/openfga_sdk/models/assertion.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/authorization_model.py` & `openfga-sdk-0.2.0/openfga_sdk/models/authorization_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,15 @@
         self._id = None
         self._schema_version = None
         self._type_definitions = None
         self.discriminator = None
 
         if id is not None:
             self.id = id
-        if schema_version is not None:
-            self.schema_version = schema_version
+        self.schema_version = schema_version
         if type_definitions is not None:
             self.type_definitions = type_definitions
 
     @property
     def id(self):
         """Gets the id of this AuthorizationModel.  # noqa: E501
 
@@ -102,14 +101,16 @@
     def schema_version(self, schema_version):
         """Sets the schema_version of this AuthorizationModel.
 
 
         :param schema_version: The schema_version of this AuthorizationModel.  # noqa: E501
         :type schema_version: str
         """
+        if self.local_vars_configuration.client_side_validation and schema_version is None:  # noqa: E501
+            raise ValueError("Invalid value for `schema_version`, must not be `None`")  # noqa: E501
 
         self._schema_version = schema_version
 
     @property
     def type_definitions(self):
         """Gets the type_definitions of this AuthorizationModel.  # noqa: E501
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/check_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/check_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/check_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/check_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/computed.py` & `openfga-sdk-0.2.0/openfga_sdk/models/computed.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/contextual_tuple_keys.py` & `openfga-sdk-0.2.0/openfga_sdk/models/contextual_tuple_keys.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/create_store_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/create_store_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/create_store_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/create_store_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/difference.py` & `openfga-sdk-0.2.0/openfga_sdk/models/difference.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/error_code.py` & `openfga-sdk-0.2.0/openfga_sdk/models/error_code.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/expand_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/expand_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/expand_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/expand_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/get_store_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/get_store_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/internal_error_code.py` & `openfga-sdk-0.2.0/openfga_sdk/models/internal_error_code.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/internal_error_message_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/internal_error_message_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/leaf.py` & `openfga-sdk-0.2.0/openfga_sdk/models/leaf.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/list_objects_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/list_objects_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/list_objects_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/list_objects_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/list_stores_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/list_stores_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/metadata.py` & `openfga-sdk-0.2.0/openfga_sdk/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'relations': 'dict(str, RelationMetadata)'
+        'relations': 'dict[str, RelationMetadata]'
     }
 
     attribute_map = {
         'relations': 'relations'
     }
 
     def __init__(self, relations=None, local_vars_configuration=None):  # noqa: E501
@@ -59,25 +59,25 @@
 
     @property
     def relations(self):
         """Gets the relations of this Metadata.  # noqa: E501
 
 
         :return: The relations of this Metadata.  # noqa: E501
-        :rtype: dict(str, RelationMetadata)
+        :rtype: dict[str, RelationMetadata]
         """
         return self._relations
 
     @relations.setter
     def relations(self, relations):
         """Sets the relations of this Metadata.
 
 
         :param relations: The relations of this Metadata.  # noqa: E501
-        :type relations: dict(str, RelationMetadata)
+        :type relations: dict[str, RelationMetadata]
         """
 
         self._relations = relations
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/node.py` & `openfga-sdk-0.2.0/openfga_sdk/models/node.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/nodes.py` & `openfga-sdk-0.2.0/openfga_sdk/models/nodes.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/not_found_error_code.py` & `openfga-sdk-0.2.0/openfga_sdk/models/not_found_error_code.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/object_relation.py` & `openfga-sdk-0.2.0/openfga_sdk/models/object_relation.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/path_unknown_error_message_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/path_unknown_error_message_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/read_assertions_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/read_assertions_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/read_authorization_model_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/read_authorization_model_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/read_authorization_models_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/read_authorization_models_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/read_changes_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/read_changes_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/read_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/read_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/read_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/read_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/relation_metadata.py` & `openfga-sdk-0.2.0/openfga_sdk/models/relation_metadata.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/relation_reference.py` & `openfga-sdk-0.2.0/openfga_sdk/models/relation_reference.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/status.py` & `openfga-sdk-0.2.0/openfga_sdk/models/status.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/store.py` & `openfga-sdk-0.2.0/openfga_sdk/models/store.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/tuple.py` & `openfga-sdk-0.2.0/openfga_sdk/models/tuple.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/tuple_change.py` & `openfga-sdk-0.2.0/openfga_sdk/models/tuple_change.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/tuple_key.py` & `openfga-sdk-0.2.0/openfga_sdk/models/tuple_key.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/tuple_keys.py` & `openfga-sdk-0.2.0/openfga_sdk/models/tuple_keys.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/tuple_operation.py` & `openfga-sdk-0.2.0/openfga_sdk/models/tuple_operation.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/tuple_to_userset.py` & `openfga-sdk-0.2.0/openfga_sdk/models/tuple_to_userset.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/type_definition.py` & `openfga-sdk-0.2.0/openfga_sdk/models/type_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'type': 'str',
-        'relations': 'dict(str, Userset)',
+        'relations': 'dict[str, Userset]',
         'metadata': 'Metadata'
     }
 
     attribute_map = {
         'type': 'type',
         'relations': 'relations',
         'metadata': 'metadata'
@@ -91,25 +91,25 @@
 
     @property
     def relations(self):
         """Gets the relations of this TypeDefinition.  # noqa: E501
 
 
         :return: The relations of this TypeDefinition.  # noqa: E501
-        :rtype: dict(str, Userset)
+        :rtype: dict[str, Userset]
         """
         return self._relations
 
     @relations.setter
     def relations(self, relations):
         """Sets the relations of this TypeDefinition.
 
 
         :param relations: The relations of this TypeDefinition.  # noqa: E501
-        :type relations: dict(str, Userset)
+        :type relations: dict[str, Userset]
         """
 
         self._relations = relations
 
     @property
     def metadata(self):
         """Gets the metadata of this TypeDefinition.  # noqa: E501
```

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/users.py` & `openfga-sdk-0.2.0/openfga_sdk/models/users.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/userset.py` & `openfga-sdk-0.2.0/openfga_sdk/models/userset.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/userset_tree.py` & `openfga-sdk-0.2.0/openfga_sdk/models/userset_tree.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/userset_tree_difference.py` & `openfga-sdk-0.2.0/openfga_sdk/models/userset_tree_difference.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/userset_tree_tuple_to_userset.py` & `openfga-sdk-0.2.0/openfga_sdk/models/userset_tree_tuple_to_userset.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/usersets.py` & `openfga-sdk-0.2.0/openfga_sdk/models/usersets.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/validation_error_message_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/validation_error_message_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/write_assertions_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/write_assertions_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/write_authorization_model_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/write_authorization_model_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/write_authorization_model_response.py` & `openfga-sdk-0.2.0/openfga_sdk/models/write_authorization_model_response.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/models/write_request.py` & `openfga-sdk-0.2.0/openfga_sdk/models/write_request.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/openfga_sdk/rest.py` & `openfga-sdk-0.2.0/openfga_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `openfga-sdk-0.1.1/setup.py` & `openfga-sdk-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
    NOTE: This file was auto generated by OpenAPI Generator (https://openapi-generator.tech). DO NOT EDIT.
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "openfga-sdk"
-VERSION = "0.1.1"
+VERSION = "0.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -40,21 +40,20 @@
     author="OpenFGA (https://openfga.dev)",
     author_email="community@openfga.dev",
     url="https://github.com/openfga/python-sdk",
     classifiers=[
       'Development Status :: 5 - Production/Stable',
       'Intended Audience :: Developers',
       'License :: OSI Approved :: Apache Software License',
-      'Programming Language :: Python :: 3.9',
       'Programming Language :: Python :: 3.10',
       'Programming Language :: Python :: 3.11',
       'Programming Language :: Python :: 3.12',
     ],
     keywords=["openfga", "authorization", "fga", "fine-grained-authorization", "rebac", "zanzibar"],
     install_requires=REQUIRES,
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="Apache-2.0",
     long_description_content_type='text/markdown',
     long_description=long_description
 )
```

### Comparing `openfga-sdk-0.1.1/test/test_credentials.py` & `openfga-sdk-0.2.0/test/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         current_time = datetime.now()
         auth_header = await credential.get_authentication_header(client)
         self.assertEqual(auth_header, {'Authorization': 'Bearer AABBCCDD'})
         self.assertEqual(credential._access_token, 'AABBCCDD')
         self.assertGreaterEqual(credential._access_expiry_time,
                                 current_time + timedelta(seconds=int(120)))
         expected_header = urllib3.response.HTTPHeaderDict(
-            {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk (python) 0.1.1'})
+            {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk (python) 0.2.0'})
         mock_request.assert_called_once_with(
             'POST',
             'https://www.testme.com/oauth/token',
             headers=expected_header,
             query_params=None, post_params=None, _preload_content=True, _request_timeout=None,
             body={"client_id": "myclientid", "client_secret": "mysecret",
                   "audience": "myaudience", "grant_type": "client_credentials"}
```

### Comparing `openfga-sdk-0.1.1/test/test_open_fga_api.py` & `openfga-sdk-0.2.0/test/test_open_fga_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 from openfga_sdk.models.usersets import Usersets
 from openfga_sdk.models.validation_error_message_response import ValidationErrorMessageResponse
 from openfga_sdk.models.write_assertions_request import WriteAssertionsRequest
 from openfga_sdk.models.write_authorization_model_request import WriteAuthorizationModelRequest
 from openfga_sdk.models.write_authorization_model_response import WriteAuthorizationModelResponse
 from openfga_sdk.models.write_request import WriteRequest
 
-store_id = 'd12345abc'
+store_id = '01H0H015178Y2V4CX10C2KGHF4'
 request_id = 'x1y2z3'
 
 # Helper function to construct mock response
 
 
 def http_mock_response(body, status):
     headers = urllib3.response.HTTPHeaderDict({
@@ -120,30 +120,30 @@
             api_instance = open_fga_api.OpenFgaApi(api_client)
             body = CheckRequest(
                 tuple_key=TupleKey(
                     object="document:2021-budget",
                     relation="reader",
                     user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
                 ),
-                authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
+                authorization_model_id="01GXSA8YR785C4FYS3C0RTG7B1",
             )
             api_response = await api_instance.check(
                 body=body,
             )
             self.assertIsInstance(api_response, CheckResponse)
             self.assertTrue(api_response.allowed)
             # Make sure the API was called with the right data
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/check',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/check',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={"tuple_key": {"object": "document:2021-budget",
-                                    "relation": "reader", "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}, "authorization_model_id": "1uHxCSuTP0VKPYSnkq1pbb1jeZw"},
+                                    "relation": "reader", "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}, "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"},
                 _preload_content=ANY,
                 _request_timeout=None
             )
             await api_client.close()
 
     @patch.object(rest.RESTClientObject, 'request')
     async def test_create_store(self, mock_request):
@@ -193,15 +193,15 @@
         configuration = self.configuration
         configuration.store_id = store_id
         async with openfga_sdk.ApiClient(configuration) as api_client:
             api_instance = open_fga_api.OpenFgaApi(api_client)
             await api_instance.delete_store()
             mock_request.assert_called_once_with(
                 'DELETE',
-                'http://api.fga.example/stores/d12345abc',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4',
                 headers=ANY,
                 query_params=[],
                 body=None,
                 _preload_content=ANY,
                 _request_timeout=None
             )
             await api_client.close()
@@ -221,65 +221,65 @@
         async with openfga_sdk.ApiClient(configuration) as api_client:
             api_instance = open_fga_api.OpenFgaApi(api_client)
             body = ExpandRequest(
                 tuple_key=TupleKey(
                     object="document:budget",
                     relation="reader",
                 ),
-                authorization_model_id="1uHxCSuTP0VKPYSnkq1pbb1jeZw",
+                authorization_model_id="01GXSA8YR785C4FYS3C0RTG7B1",
             )
             api_response = await api_instance.expand(
                 body=body,
             )
             self.assertIsInstance(api_response, ExpandResponse)
             curUsers = Users(users=["user:81684243-9356-4421-8fbf-a4f8d36aa31b"])
             leaf = Leaf(users=curUsers)
             node = Node(name="document:budget#reader", leaf=leaf)
             userTree = UsersetTree(node)
             expected_response = ExpandResponse(userTree)
             self.assertEqual(api_response, expected_response)
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/expand',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/expand',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={"tuple_key": {"object": "document:budget", "relation": "reader"},
-                      "authorization_model_id": "1uHxCSuTP0VKPYSnkq1pbb1jeZw"},
+                      "authorization_model_id": "01GXSA8YR785C4FYS3C0RTG7B1"},
                 _preload_content=ANY,
                 _request_timeout=None
             )
             await api_client.close()
 
     @patch.object(rest.RESTClientObject, 'request')
     async def test_get_store(self, mock_request):
         """Test case for get_store
 
         Get a store  # noqa: E501
         """
         response_body = '''{
-  "id": "d12345abc",
+  "id": "01H0H015178Y2V4CX10C2KGHF4",
   "name": "test_store",
   "created_at": "2022-07-25T20:45:10.485Z",
   "updated_at": "2022-07-25T20:45:10.485Z"
 }
             '''
         mock_request.return_value = mock_response(response_body, 200)
         configuration = self.configuration
         configuration.store_id = store_id
         async with openfga_sdk.ApiClient(configuration) as api_client:
             api_instance = open_fga_api.OpenFgaApi(api_client)
             # Get a store
             api_response = await api_instance.get_store()
             self.assertIsInstance(api_response, GetStoreResponse)
-            self.assertEqual(api_response.id, 'd12345abc')
+            self.assertEqual(api_response.id, '01H0H015178Y2V4CX10C2KGHF4')
             self.assertEqual(api_response.name, 'test_store')
             mock_request.assert_called_once_with(
                 'GET',
-                'http://api.fga.example/stores/d12345abc',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4',
                 headers=ANY,
                 query_params=[],
                 _preload_content=ANY,
                 _request_timeout=None
             )
             await api_client.close()
 
@@ -309,15 +309,15 @@
             )
             # Get all stores
             api_response = await api_instance.list_objects(body)
             self.assertIsInstance(api_response, ListObjectsResponse)
             self.assertEqual(api_response.objects, ['document:abcd1234'])
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/list-objects',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/list-objects',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={'authorization_model_id': '01G5JAVJ41T49E9TT3SKVS7X1J',
                       'type': 'document', 'relation': 'reader', 'user': 'user:81684243-9356-4421-8fbf-a4f8d36aa31b'},
                 _preload_content=ANY,
                 _request_timeout=None
@@ -432,15 +432,15 @@
             key = TupleKey(user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
                            relation="reader", object="document:2021-budget")
             timestamp = datetime.fromisoformat("2021-10-06T15:32:11.128+00:00")
             expected_data = ReadResponse(tuples=[Tuple(key=key, timestamp=timestamp)])
             self.assertEqual(api_response, expected_data)
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/read',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/read',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={"tuple_key": {"object": "document:2021-budget", "relation": "reader", "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"},
                       "page_size": 50, "continuation_token": "eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ=="},
                 _preload_content=ANY,
                 _request_timeout=None
@@ -484,15 +484,15 @@
                     user="user:81684243-9356-4421-8fbf-a4f8d36aa31b",
                 ),
                 expectation=True,
             )
             self.assertEqual(api_response.assertions, [assertion])
             mock_request.assert_called_once_with(
                 'GET',
-                'http://api.fga.example/stores/d12345abc/assertions/01G5JAVJ41T49E9TT3SKVS7X1J',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/assertions/01G5JAVJ41T49E9TT3SKVS7X1J',
                 headers=ANY,
                 query_params=[],
                 _preload_content=ANY,
                 _request_timeout=None
             )
 
     @patch.object(rest.RESTClientObject, 'request')
@@ -501,14 +501,15 @@
 
         Return a particular version of an authorization model  # noqa: E501
         """
         response_body = '''
 {
   "authorization_model": {
     "id": "01G5JAVJ41T49E9TT3SKVS7X1J",
+    "schema_version":"1.1",
     "type_definitions": [
       {
         "type": "document",
         "relations": {
           "reader": {
             "union": {
               "child": [
@@ -563,20 +564,20 @@
                         ),
                         writer=Userset(
                             this=dict(),
                         ),
                     )
                 )
             ]
-            authorization_model = AuthorizationModel(id='01G5JAVJ41T49E9TT3SKVS7X1J',
+            authorization_model = AuthorizationModel(id='01G5JAVJ41T49E9TT3SKVS7X1J', schema_version="1.1",
                                                      type_definitions=type_definitions)
             self.assertEqual(api_response.authorization_model, authorization_model)
             mock_request.assert_called_once_with(
                 'GET',
-                'http://api.fga.example/stores/d12345abc/authorization-models/01G5JAVJ41T49E9TT3SKVS7X1J',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/authorization-models/01G5JAVJ41T49E9TT3SKVS7X1J',
                 headers=ANY,
                 query_params=[],
                 _preload_content=ANY,
                 _request_timeout=None
             )
 
     @patch.object(rest.RESTClientObject, 'request')
@@ -623,15 +624,15 @@
                 timestamp=datetime.fromisoformat("2022-07-26T15:55:55.809+00:00"))
             read_changes = ReadChangesResponse(
                 continuation_token='eyJwayI6IkxBVEVTVF9OU0NPTkZJR19hdXRoMHN0b3JlIiwic2siOiIxem1qbXF3MWZLZExTcUoyN01MdTdqTjh0cWgifQ==',
                 changes=[changes])
             self.assertEqual(api_response, read_changes)
             mock_request.assert_called_once_with(
                 'GET',
-                'http://api.fga.example/stores/d12345abc/changes',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/changes',
                 headers=ANY,
                 query_params=[('type', 'document'), ('page_size', 1),
                               ('continuation_token', 'abcdefg')],
                 _preload_content=ANY,
                 _request_timeout=None
             )
 
@@ -665,15 +666,15 @@
                 authorization_model_id="01G5JAVJ41T49E9TT3SKVS7X1J",
             )
             await api_instance.write(
                 body,
             )
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/write',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/write',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={"writes": {"tuple_keys": [{"object": "document:2021-budget", "relation": "reader",
                                                  "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}]}, "authorization_model_id": "01G5JAVJ41T49E9TT3SKVS7X1J"},
                 _preload_content=ANY,
                 _request_timeout=None
@@ -709,15 +710,15 @@
                 authorization_model_id="01G5JAVJ41T49E9TT3SKVS7X1J",
             )
             await api_instance.write(
                 body,
             )
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/write',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/write',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={"deletes": {"tuple_keys": [{"object": "document:2021-budget", "relation": "reader",
                                                   "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}]}, "authorization_model_id": "01G5JAVJ41T49E9TT3SKVS7X1J"},
                 _preload_content=ANY,
                 _request_timeout=None
@@ -754,15 +755,15 @@
             # Upsert assertions for an authorization model ID
             await api_instance.write_assertions(
                 authorization_model_id="xyz0123",
                 body=body,
             )
             mock_request.assert_called_once_with(
                 'PUT',
-                'http://api.fga.example/stores/d12345abc/assertions/xyz0123',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/assertions/xyz0123',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
                 body={"assertions": [{"expectation": True, "tuple_key": {
                     "object": "document:2021-budget", "relation": "reader", "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}}]},
                 _preload_content=ANY,
                 _request_timeout=None
@@ -780,14 +781,15 @@
         configuration.store_id = store_id
         async with openfga_sdk.ApiClient(configuration) as api_client:
             # Create an instance of the API class
             api_instance = open_fga_api.OpenFgaApi(api_client)
 
             # example passing only required values which don't have defaults set
             body = WriteAuthorizationModelRequest(
+                schema_version="1.1",
                 type_definitions=[
                     TypeDefinition(
                         type="document",
                         relations=dict(
                             writer=Userset(
                                 this=dict(),
                             ),
@@ -813,20 +815,20 @@
             self.assertIsInstance(api_response, WriteAuthorizationModelResponse)
             expected_response = WriteAuthorizationModelResponse(
                 authorization_model_id='01G5JAVJ41T49E9TT3SKVS7X1J'
             )
             self.assertEqual(api_response, expected_response)
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/authorization-models',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/authorization-models',
                 headers=ANY,
                 query_params=[],
                 post_params=[],
-                body={"type_definitions": [{"type": "document", "relations": {"writer": {"this": {}}, "reader": {
-                    "union": {"child": [{"this": {}}, {"computedUserset": {"object": "", "relation": "writer"}}]}}}}]},
+                body={"schema_version": "1.1", "type_definitions": [{"type": "document", "relations": {"writer": {"this": {
+                }}, "reader": {"union": {"child": [{"this": {}}, {"computedUserset": {"object": "", "relation": "writer"}}]}}}}]},
                 _preload_content=ANY,
                 _request_timeout=None
             )
 
     def test_default_scheme(self):
         """
         Ensure default scheme is https
@@ -900,14 +902,25 @@
         """
         configuration = openfga_sdk.Configuration(
             api_host='localhost?mypath=foo',
             api_scheme='http'
         )
         self.assertRaises(ApiValueError, configuration.is_valid)
 
+    def test_configuration_store_id_invalid(self):
+        """
+        Test whether ApiValueError is raised if host has query
+        """
+        configuration = openfga_sdk.Configuration(
+            api_host='localhost',
+            api_scheme='http',
+            store_id="abcd"
+        )
+        self.assertRaises(FgaValidationException, configuration.is_valid)
+
     async def test_bad_configuration_read_authorization_model(self):
         """
         Test whether FgaValidationException is raised for API (reading authorization models)
         with configuration is having incorrect API scheme
         """
         configuration = openfga_sdk.Configuration(
             api_scheme='bad',
@@ -1157,18 +1170,18 @@
             api_response = await api_instance.check(
                 body=body,
             )
             self.assertIsInstance(api_response, CheckResponse)
             self.assertTrue(api_response.allowed)
             # Make sure the API was called with the right data
             expectedHeader = urllib3.response.HTTPHeaderDict(
-                {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk /0.1.1', 'Authorization': 'Bearer TOKEN1'})
+                {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk python/0.2.0', 'Authorization': 'Bearer TOKEN1'})
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/check',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/check',
                 headers=expectedHeader,
                 query_params=[],
                 post_params=[],
                 body={"tuple_key": {"object": "document:2021-budget", "relation": "reader",
                                     "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}},
                 _preload_content=ANY,
                 _request_timeout=None
@@ -1200,18 +1213,18 @@
             api_response = await api_instance.check(
                 body=body,
             )
             self.assertIsInstance(api_response, CheckResponse)
             self.assertTrue(api_response.allowed)
             # Make sure the API was called with the right data
             expectedHeader = urllib3.response.HTTPHeaderDict(
-                {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk /0.1.1', 'Custom Header': 'custom value'})
+                {'Accept': 'application/json', 'Content-Type': 'application/json', 'User-Agent': 'openfga-sdk python/0.2.0', 'Custom Header': 'custom value'})
             mock_request.assert_called_once_with(
                 'POST',
-                'http://api.fga.example/stores/d12345abc/check',
+                'http://api.fga.example/stores/01H0H015178Y2V4CX10C2KGHF4/check',
                 headers=expectedHeader,
                 query_params=[],
                 post_params=[],
                 body={"tuple_key": {"object": "document:2021-budget", "relation": "reader",
                                     "user": "user:81684243-9356-4421-8fbf-a4f8d36aa31b"}},
                 _preload_content=ANY,
                 _request_timeout=None
```

