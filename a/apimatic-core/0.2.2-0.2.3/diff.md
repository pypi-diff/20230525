# Comparing `tmp/apimatic-core-0.2.2.tar.gz` & `tmp/apimatic-core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimatic-core-0.2.2.tar", last modified: Tue Apr  4 08:47:32 2023, max compression
+gzip compressed data, was "apimatic-core-0.2.3.tar", last modified: Thu May 25 12:18:56 2023, max compression
```

## Comparing `apimatic-core-0.2.2.tar` & `apimatic-core-0.2.3.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.572251 apimatic-core-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-04 08:47:32.572251 apimatic-core-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/api_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/header_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/authentication/multiple/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/multiple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/multiple/and_auth_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/multiple/auth_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/multiple/or_auth_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/multiple/single_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/authentication/query_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/configurations/endpoint_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/configurations/global_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/decorators/lazy_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/factories/http_response_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core/http/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/apimatic_core/http/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/configurations/http_client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/http_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/apimatic_core/http/request/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/request/http_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/apimatic_core/http/response/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/response/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/http/response/http_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/apimatic_core/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/logger/endpoint_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/request_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/apimatic_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/array_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/datetime_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/error_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/file_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/types/xml_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/apimatic_core/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/utilities/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/utilities/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/utilities/comparison_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/utilities/file_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/apimatic_core/utilities/xml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.560251 apimatic-core-0.2.2/apimatic_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-04 08:47:32.000000 apimatic-core-0.2.2/apimatic_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-04 08:47:32.000000 apimatic-core-0.2.2/apimatic_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:47:32.000000 apimatic-core-0.2.2/apimatic_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-04 08:47:32.000000 apimatic-core-0.2.2/apimatic_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 08:47:32.000000 apimatic-core-0.2.2/apimatic_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:47:32.572251 apimatic-core-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/tests/apimatic_core/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/tests/apimatic_core/api_call_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/api_call_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/api_call_tests/test_api_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/tests/apimatic_core/api_logger_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/api_logger_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/api_logger_tests/test_api_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.564251 apimatic-core-0.2.2/tests/apimatic_core/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/custom_header_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/custom_query_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/mocks/callables/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/callables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/callables/base_uri_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/global_test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/local_test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/nested_model_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/mocks/http/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/http/http_response_catcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/mocks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/logger/api_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/cat_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/days.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/dog_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/grand_parent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/one_of_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/wolf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/mocks/models/xml_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/request_builder_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/request_builder_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/request_builder_tests/test_request_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.568251 apimatic-core-0.2.2/tests/apimatic_core/response_handler_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/response_handler_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/response_handler_tests/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:47:32.572251 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   126287 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_comparison_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_file_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-04-04 08:47:15.000000 apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.091068 apimatic-core-0.2.3/apimatic_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/api_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.091068 apimatic-core-0.2.3/apimatic_core/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/header_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/authentication/multiple/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/and_auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/or_auth_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/multiple/single_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/authentication/query_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/configurations/endpoint_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/configurations/global_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/decorators/lazy_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/factories/http_response_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/configurations/http_client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/http_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/request/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/request/http_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/http/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/response/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/http/response/http_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.095068 apimatic-core-0.2.3/apimatic_core/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/logger/endpoint_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/request_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/apimatic_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/array_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/datetime_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/error_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/file_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/types/xml_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/apimatic_core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/comparison_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/apimatic_core/utilities/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.091068 apimatic-core-0.2.3/apimatic_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 12:18:56.000000 apimatic-core-0.2.3/apimatic_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/test_api_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/test_api_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.099068 apimatic-core-0.2.3/tests/apimatic_core/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/custom_header_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/custom_query_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/base_uri_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/global_test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/local_test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/nested_model_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/http/http_response_catcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.103068 apimatic-core-0.2.3/tests/apimatic_core/mocks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/logger/api_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/cat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/dog_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/grand_parent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/one_of_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/wolf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/mocks/models/xml_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45307 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/test_request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:18:56.107068 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126287 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_comparison_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-05-25 12:18:39.000000 apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_xml_helper.py
```

### Comparing `apimatic-core-0.2.2/LICENSE` & `apimatic-core-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/PKG-INFO` & `apimatic-core-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
 Home-page: https://github.com/apimatic/core-lib-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apimatic-core-0.2.2/README.md` & `apimatic-core-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/api_call.py` & `apimatic-core-0.2.3/apimatic_core/api_call.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/authentication/multiple/and_auth_group.py` & `apimatic-core-0.2.3/apimatic_core/authentication/multiple/and_auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/authentication/multiple/auth_group.py` & `apimatic-core-0.2.3/apimatic_core/authentication/multiple/auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/authentication/multiple/or_auth_group.py` & `apimatic-core-0.2.3/apimatic_core/authentication/multiple/or_auth_group.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/authentication/multiple/single_auth.py` & `apimatic-core-0.2.3/apimatic_core/authentication/multiple/single_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/configurations/endpoint_configuration.py` & `apimatic-core-0.2.3/apimatic_core/configurations/endpoint_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/configurations/global_configuration.py` & `apimatic-core-0.2.3/apimatic_core/configurations/global_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/http/configurations/http_client_configuration.py` & `apimatic-core-0.2.3/apimatic_core/http/configurations/http_client_configuration.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/http/http_callback.py` & `apimatic-core-0.2.3/apimatic_core/http/http_callback.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/http/request/http_request.py` & `apimatic-core-0.2.3/apimatic_core/http/request/http_request.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/http/response/api_response.py` & `apimatic-core-0.2.3/apimatic_core/http/response/api_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/http/response/http_response.py` & `apimatic-core-0.2.3/apimatic_core/http/response/http_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/request_builder.py` & `apimatic-core-0.2.3/apimatic_core/request_builder.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/response_handler.py` & `apimatic-core-0.2.3/apimatic_core/response_handler.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/types/array_serialization_format.py` & `apimatic-core-0.2.3/apimatic_core/types/array_serialization_format.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/types/error_case.py` & `apimatic-core-0.2.3/apimatic_core/types/error_case.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/types/parameter.py` & `apimatic-core-0.2.3/apimatic_core/types/parameter.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/types/xml_attributes.py` & `apimatic-core-0.2.3/apimatic_core/types/xml_attributes.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/utilities/api_helper.py` & `apimatic-core-0.2.3/apimatic_core/utilities/api_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/utilities/auth_helper.py` & `apimatic-core-0.2.3/apimatic_core/utilities/auth_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/utilities/comparison_helper.py` & `apimatic-core-0.2.3/apimatic_core/utilities/comparison_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/utilities/file_helper.py` & `apimatic-core-0.2.3/apimatic_core/utilities/file_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core/utilities/xml_helper.py` & `apimatic-core-0.2.3/apimatic_core/utilities/xml_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/apimatic_core.egg-info/PKG-INFO` & `apimatic-core-0.2.3/apimatic_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library that contains core logic and utilities for consuming REST APIs using Python SDKs generated by APIMatic.
 Home-page: https://github.com/apimatic/core-lib-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apimatic-core-0.2.2/apimatic_core.egg-info/SOURCES.txt` & `apimatic-core-0.2.3/apimatic_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/setup.py` & `apimatic-core-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='apimatic-core',
-    version='0.2.2',
+    version='0.2.3',
     description='A library that contains core logic and utilities for '
                 'consuming REST APIs using Python SDKs generated by APIMatic.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic',
     author_email='support@apimatic.io',
     license='MIT',
     url='https://github.com/apimatic/core-lib-python',
     packages=find_packages(),
     install_requires=[
         'apimatic-core-interfaces~=0.1.0',
         'jsonpickle~=3.0.1, >= 3.0.1',
         'python-dateutil~=2.8.1',
-        'requests~=2.28.1',
+        'requests~=2.31',
         'enum34~=1.1, >=1.1.10',
         'setuptools~=66.0.0',
         'jsonpointer~=2.3'
     ],
     tests_require=[
         'pytest~=7.2.2',
         'pytest-cov~=4.0.0'
```

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/api_call_tests/test_api_call.py` & `apimatic-core-0.2.3/tests/apimatic_core/api_call_tests/test_api_call.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/api_logger_tests/test_api_logger.py` & `apimatic-core-0.2.3/tests/apimatic_core/api_logger_tests/test_api_logger.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/base.py` & `apimatic-core-0.2.3/tests/apimatic_core/base.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/basic_auth.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/basic_auth.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/authentications/custom_query_authentication.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/authentications/custom_query_authentication.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/callables/base_uri_callable.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/callables/base_uri_callable.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/api_exception.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/global_test_exception.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/global_test_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/local_test_exception.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/local_test_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/exceptions/nested_model_exception.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/exceptions/nested_model_exception.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/http/http_client.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/http/http_client.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/api_response.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/api_response.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/cat_model.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/cat_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/days.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/days.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/dog_model.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/dog_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/grand_parent_class_model.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/grand_parent_class_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/one_of_xml.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/one_of_xml.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/person.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/person.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/validate.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/validate.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/wolf_model.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/wolf_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/mocks/models/xml_model.py` & `apimatic-core-0.2.3/tests/apimatic_core/mocks/models/xml_model.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/request_builder_tests/test_request_builder.py` & `apimatic-core-0.2.3/tests/apimatic_core/request_builder_tests/test_request_builder.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/response_handler_tests/test_response_handler.py` & `apimatic-core-0.2.3/tests/apimatic_core/response_handler_tests/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_api_helper.py` & `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_api_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_auth_helper.py` & `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_auth_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_comparison_helper.py` & `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_comparison_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_file_helper.py` & `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_file_helper.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-0.2.2/tests/apimatic_core/utility_tests/test_xml_helper.py` & `apimatic-core-0.2.3/tests/apimatic_core/utility_tests/test_xml_helper.py`

 * *Files identical despite different names*

