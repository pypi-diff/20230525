# Comparing `tmp/sparrow-order-lib-0.1.96.tar.gz` & `tmp/sparrow-order-lib-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/meng/git/sparrow-order-lib/dist/.tmp-t_489m7h/sparrow-order-lib-0.1.96.tar", last modified: Tue May 23 07:13:55 2023, max compression
+gzip compressed data, was "/Users/meng/git/sparrow-order-lib/dist/.tmp-y02u0foj/sparrow-order-lib-0.1.97.tar", last modified: Thu May 25 06:09:02 2023, max compression
```

## Comparing `sparrow-order-lib-0.1.96.tar` & `sparrow-order-lib-0.1.97.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/
--rw-r--r--   0 meng       (501) staff       (20)     1073 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/LICENSE
--rw-r--r--   0 meng       (501) staff       (20)     8898 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/PKG-INFO
--rw-r--r--   0 meng       (501) staff       (20)     8360 2023-05-23 07:13:46.000000 sparrow-order-lib-0.1.96/README.md
--rw-r--r--   0 meng       (501) staff       (20)      103 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/pyproject.toml
--rw-r--r--   0 meng       (501) staff       (20)      724 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/setup.cfg
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/
--rw-r--r--   0 meng       (501) staff       (20)       76 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/__init__.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/
--rw-r--r--   0 meng       (501) staff       (20)      912 2023-05-19 08:11:13.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     2014 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/base_models.py
--rw-r--r--   0 meng       (501) staff       (20)      704 2023-05-19 08:11:13.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/common_utils.py
--rw-r--r--   0 meng       (501) staff       (20)     5712 2023-04-21 07:43:37.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/constants.py
--rw-r--r--   0 meng       (501) staff       (20)     1592 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/datastructures.py
--rw-r--r--   0 meng       (501) staff       (20)     1353 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/decorators.py
--rw-r--r--   0 meng       (501) staff       (20)    12853 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/dt_utils.py
--rw-r--r--   0 meng       (501) staff       (20)       90 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/formats.py
--rw-r--r--   0 meng       (501) staff       (20)      714 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/model_function.py
--rw-r--r--   0 meng       (501) staff       (20)      251 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/numbers.py
--rw-r--r--   0 meng       (501) staff       (20)        0 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/text.py
--rw-r--r--   0 meng       (501) staff       (20)     1415 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/xls_util.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/db_tool/
--rw-r--r--   0 meng       (501) staff       (20)        0 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/db_tool/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)      848 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/db_tool/query.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/
--rw-r--r--   0 meng       (501) staff       (20)     1359 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)      422 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/constants.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/
--rw-r--r--   0 meng       (501) staff       (20)       56 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     7841 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/base.py
--rw-r--r--   0 meng       (501) staff       (20)     1092 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/client.py
--rw-r--r--   0 meng       (501) staff       (20)     1228 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/constants.py
--rw-r--r--   0 meng       (501) staff       (20)     3661 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_builder.py
--rw-r--r--   0 meng       (501) staff       (20)     3091 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_door.py
--rw-r--r--   0 meng       (501) staff       (20)     5145 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_param.py
--rw-r--r--   0 meng       (501) staff       (20)     3620 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_query_util.py
--rw-r--r--   0 meng       (501) staff       (20)     1223 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/exceptions.py
--rw-r--r--   0 meng       (501) staff       (20)     2207 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/field.py
--rw-r--r--   0 meng       (501) staff       (20)      381 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/in_query_param.py
--rw-r--r--   0 meng       (501) staff       (20)      163 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/index.py
--rw-r--r--   0 meng       (501) staff       (20)      241 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/mock.py
--rw-r--r--   0 meng       (501) staff       (20)     3137 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/operators.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/
--rw-r--r--   0 meng       (501) staff       (20)     1619 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     1782 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_base.py
--rw-r--r--   0 meng       (501) staff       (20)       64 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_client.py
--rw-r--r--   0 meng       (501) staff       (20)     2455 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
--rw-r--r--   0 meng       (501) staff       (20)     3294 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
--rw-r--r--   0 meng       (501) staff       (20)     3947 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
--rw-r--r--   0 meng       (501) staff       (20)     2500 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
--rw-r--r--   0 meng       (501) staff       (20)     2310 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_field.py
--rw-r--r--   0 meng       (501) staff       (20)      515 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
--rw-r--r--   0 meng       (501) staff       (20)      373 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_mock.py
--rw-r--r--   0 meng       (501) staff       (20)     2203 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_operators.py
--rw-r--r--   0 meng       (501) staff       (20)     7542 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/mapping_constants.py
--rw-r--r--   0 meng       (501) staff       (20)     3086 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/query_mapping_constants.py
--rw-r--r--   0 meng       (501) staff       (20)     3490 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/test_order_doc_type.py
--rw-r--r--   0 meng       (501) staff       (20)       42 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/example.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/
--rw-r--r--   0 meng       (501) staff       (20)        0 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     1406 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_api_path.py
--rw-r--r--   0 meng       (501) staff       (20)      815 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_core.py
--rw-r--r--   0 meng       (501) staff       (20)     5271 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_core_go.py
--rw-r--r--   0 meng       (501) staff       (20)     2778 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
--rw-r--r--   0 meng       (501) staff       (20)     4706 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_product.py
--rw-r--r--   0 meng       (501) staff       (20)      383 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/svc_config.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/
--rw-r--r--   0 meng       (501) staff       (20)       31 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     3239 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/constants.py
--rw-r--r--   0 meng       (501) staff       (20)     2974 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/models.py
--rw-r--r--   0 meng       (501) staff       (20)     1164 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py
--rw-r--r--   0 meng       (501) staff       (20)      539 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/utils.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/
--rw-r--r--   0 meng       (501) staff       (20)       33 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     8626 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py
--rw-r--r--   0 meng       (501) staff       (20)    31929 2023-05-23 07:13:15.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/constants.py
--rw-r--r--   0 meng       (501) staff       (20)    71783 2023-03-13 05:29:31.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/
--rw-r--r--   0 meng       (501) staff       (20)       34 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     7206 2023-02-14 04:38:57.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/constants.py
--rw-r--r--   0 meng       (501) staff       (20)     1892 2023-01-13 03:40:32.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/disstorage.py
--rw-r--r--   0 meng       (501) staff       (20)    15398 2023-02-20 01:41:50.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/models.py
--rw-r--r--   0 meng       (501) staff       (20)      550 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py
--rw-r--r--   0 meng       (501) staff       (20)      390 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/serializers.py
--rw-r--r--   0 meng       (501) staff       (20)      514 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/utils.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/
--rw-r--r--   0 meng       (501) staff       (20)       34 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)    57342 2023-05-11 03:49:32.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/constants.py
--rw-r--r--   0 meng       (501) staff       (20)    32810 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/models.py
--rw-r--r--   0 meng       (501) staff       (20)     7952 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/serializer_data.py
--rw-r--r--   0 meng       (501) staff       (20)     4095 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/serializers.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_exchange/
--rw-r--r--   0 meng       (501) staff       (20)      155 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_exchange/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)    15287 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_exchange/constants.py
--rw-r--r--   0 meng       (501) staff       (20)    17612 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_exchange/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_inparcel/
--rw-r--r--   0 meng       (501) staff       (20)       32 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_inparcel/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     8197 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_inparcel/constants.py
--rw-r--r--   0 meng       (501) staff       (20)    11201 2023-03-13 05:29:31.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_inparcel/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_orders/
--rw-r--r--   0 meng       (501) staff       (20)       68 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_orders/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)    10215 2022-12-30 05:46:03.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_orders/constants.py
--rw-r--r--   0 meng       (501) staff       (20)   108809 2022-12-30 05:46:03.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_orders/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/
--rw-r--r--   0 meng       (501) staff       (20)       30 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     4434 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/constants.py
--rw-r--r--   0 meng       (501) staff       (20)      455 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/exceptions.py
--rw-r--r--   0 meng       (501) staff       (20)     7599 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_promotions/
--rw-r--r--   0 meng       (501) staff       (20)       34 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_promotions/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     1979 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_promotions/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_shipping/
--rw-r--r--   0 meng       (501) staff       (20)       32 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_shipping/__init__.py
--rw-r--r--   0 meng       (501) staff       (20)     3236 2023-03-13 05:29:31.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_shipping/constants.py
--rw-r--r--   0 meng       (501) staff       (20)     9065 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_shipping/models.py
-drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/
--rw-r--r--   0 meng       (501) staff       (20)     8898 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/PKG-INFO
--rw-r--r--   0 meng       (501) staff       (20)     4741 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/SOURCES.txt
--rw-r--r--   0 meng       (501) staff       (20)        1 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/dependency_links.txt
--rw-r--r--   0 meng       (501) staff       (20)       39 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/requires.txt
--rw-r--r--   0 meng       (501) staff       (20)       18 2023-05-23 07:13:55.000000 sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/top_level.txt
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/
+-rw-r--r--   0 meng       (501) staff       (20)     1073 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/LICENSE
+-rw-r--r--   0 meng       (501) staff       (20)     8946 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/PKG-INFO
+-rw-r--r--   0 meng       (501) staff       (20)     8408 2023-05-25 06:03:45.000000 sparrow-order-lib-0.1.97/README.md
+-rw-r--r--   0 meng       (501) staff       (20)      103 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/pyproject.toml
+-rw-r--r--   0 meng       (501) staff       (20)      724 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/setup.cfg
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/
+-rw-r--r--   0 meng       (501) staff       (20)       76 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/__init__.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/
+-rw-r--r--   0 meng       (501) staff       (20)      912 2023-05-19 08:11:13.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     2014 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/base_models.py
+-rw-r--r--   0 meng       (501) staff       (20)      704 2023-05-19 08:11:13.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/common_utils.py
+-rw-r--r--   0 meng       (501) staff       (20)     5712 2023-04-21 07:43:37.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     1592 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/datastructures.py
+-rw-r--r--   0 meng       (501) staff       (20)     1353 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/decorators.py
+-rw-r--r--   0 meng       (501) staff       (20)    12853 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/dt_utils.py
+-rw-r--r--   0 meng       (501) staff       (20)       90 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/formats.py
+-rw-r--r--   0 meng       (501) staff       (20)      714 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/model_function.py
+-rw-r--r--   0 meng       (501) staff       (20)      251 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/numbers.py
+-rw-r--r--   0 meng       (501) staff       (20)        0 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/text.py
+-rw-r--r--   0 meng       (501) staff       (20)     1415 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/xls_util.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/db_tool/
+-rw-r--r--   0 meng       (501) staff       (20)        0 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/db_tool/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)      848 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/db_tool/query.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/
+-rw-r--r--   0 meng       (501) staff       (20)     1359 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)      422 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/constants.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/
+-rw-r--r--   0 meng       (501) staff       (20)       56 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     7841 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/base.py
+-rw-r--r--   0 meng       (501) staff       (20)     1092 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/client.py
+-rw-r--r--   0 meng       (501) staff       (20)     1228 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     3661 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_builder.py
+-rw-r--r--   0 meng       (501) staff       (20)     3091 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_door.py
+-rw-r--r--   0 meng       (501) staff       (20)     5145 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_param.py
+-rw-r--r--   0 meng       (501) staff       (20)     3620 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_query_util.py
+-rw-r--r--   0 meng       (501) staff       (20)     1223 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/exceptions.py
+-rw-r--r--   0 meng       (501) staff       (20)     2207 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/field.py
+-rw-r--r--   0 meng       (501) staff       (20)      381 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/in_query_param.py
+-rw-r--r--   0 meng       (501) staff       (20)      163 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/index.py
+-rw-r--r--   0 meng       (501) staff       (20)      241 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/mock.py
+-rw-r--r--   0 meng       (501) staff       (20)     3137 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/operators.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/
+-rw-r--r--   0 meng       (501) staff       (20)     1619 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     1782 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_base.py
+-rw-r--r--   0 meng       (501) staff       (20)       64 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_client.py
+-rw-r--r--   0 meng       (501) staff       (20)     2455 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py
+-rw-r--r--   0 meng       (501) staff       (20)     3294 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_door.py
+-rw-r--r--   0 meng       (501) staff       (20)     3947 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_param.py
+-rw-r--r--   0 meng       (501) staff       (20)     2500 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py
+-rw-r--r--   0 meng       (501) staff       (20)     2310 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_field.py
+-rw-r--r--   0 meng       (501) staff       (20)      515 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py
+-rw-r--r--   0 meng       (501) staff       (20)      373 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_mock.py
+-rw-r--r--   0 meng       (501) staff       (20)     2203 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_operators.py
+-rw-r--r--   0 meng       (501) staff       (20)     7542 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/mapping_constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     3086 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/query_mapping_constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     3490 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/test_order_doc_type.py
+-rw-r--r--   0 meng       (501) staff       (20)       42 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/example.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/
+-rw-r--r--   0 meng       (501) staff       (20)        0 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     1406 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_api_path.py
+-rw-r--r--   0 meng       (501) staff       (20)      815 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_core.py
+-rw-r--r--   0 meng       (501) staff       (20)     5271 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_core_go.py
+-rw-r--r--   0 meng       (501) staff       (20)     2778 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_lanyue.py
+-rw-r--r--   0 meng       (501) staff       (20)     4706 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_product.py
+-rw-r--r--   0 meng       (501) staff       (20)      383 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/svc_config.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/
+-rw-r--r--   0 meng       (501) staff       (20)       31 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     3239 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     2974 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/models.py
+-rw-r--r--   0 meng       (501) staff       (20)     1164 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py
+-rw-r--r--   0 meng       (501) staff       (20)      539 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/utils.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/
+-rw-r--r--   0 meng       (501) staff       (20)       33 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     8626 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py
+-rw-r--r--   0 meng       (501) staff       (20)    31929 2023-05-25 06:03:03.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)    71783 2023-03-13 05:29:31.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/
+-rw-r--r--   0 meng       (501) staff       (20)       34 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     7206 2023-02-14 04:38:57.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     1892 2023-01-13 03:40:32.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/disstorage.py
+-rw-r--r--   0 meng       (501) staff       (20)    15398 2023-02-20 01:41:50.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/models.py
+-rw-r--r--   0 meng       (501) staff       (20)      550 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py
+-rw-r--r--   0 meng       (501) staff       (20)      390 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/serializers.py
+-rw-r--r--   0 meng       (501) staff       (20)      514 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/utils.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/
+-rw-r--r--   0 meng       (501) staff       (20)       34 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)    57342 2023-05-11 03:49:32.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)    32810 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/models.py
+-rw-r--r--   0 meng       (501) staff       (20)     7952 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/serializer_data.py
+-rw-r--r--   0 meng       (501) staff       (20)     4095 2023-02-08 06:42:07.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/serializers.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_exchange/
+-rw-r--r--   0 meng       (501) staff       (20)      155 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_exchange/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)    15287 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_exchange/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)    17612 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_exchange/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_inparcel/
+-rw-r--r--   0 meng       (501) staff       (20)       32 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_inparcel/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     8197 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_inparcel/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)    11201 2023-03-13 05:29:31.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_inparcel/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_orders/
+-rw-r--r--   0 meng       (501) staff       (20)       68 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_orders/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)    10215 2022-12-30 05:46:03.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_orders/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)   108809 2022-12-30 05:46:03.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_orders/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/
+-rw-r--r--   0 meng       (501) staff       (20)       30 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     4434 2023-01-25 13:15:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)      455 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/exceptions.py
+-rw-r--r--   0 meng       (501) staff       (20)     7599 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_promotions/
+-rw-r--r--   0 meng       (501) staff       (20)       34 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_promotions/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     1979 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_promotions/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_shipping/
+-rw-r--r--   0 meng       (501) staff       (20)       32 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_shipping/__init__.py
+-rw-r--r--   0 meng       (501) staff       (20)     3236 2023-03-13 05:29:31.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_shipping/constants.py
+-rw-r--r--   0 meng       (501) staff       (20)     9065 2022-11-08 11:50:27.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_shipping/models.py
+drwxr-xr-x   0 meng       (501) staff       (20)        0 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/
+-rw-r--r--   0 meng       (501) staff       (20)     8946 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/PKG-INFO
+-rw-r--r--   0 meng       (501) staff       (20)     4741 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 meng       (501) staff       (20)        1 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 meng       (501) staff       (20)       39 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/requires.txt
+-rw-r--r--   0 meng       (501) staff       (20)       18 2023-05-25 06:09:02.000000 sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/top_level.txt
```

### Comparing `sparrow-order-lib-0.1.96/LICENSE` & `sparrow-order-lib-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/PKG-INFO` & `sparrow-order-lib-0.1.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-order-lib
-Version: 0.1.96
+Version: 0.1.97
 Summary: This is a lib for sparrow order projects.
 Home-page: https://gitee.com/sparrow614/sparrow-order-lib
 Author: Jessica Liao
 Author-email: 18610193367@sina.cn
 Project-URL: Bug Tracker, https://gitee.com/sparrow614/sparrow-order-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,17 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
 # Release History
+## version==0.1.97
+* SparrowAftersaleConstants
+
 ## version==0.1.96
 * SparrowAftersaleConstants
 
 ## version==0.1.95
 * SparrowAftersaleConstants
 
 ## version==0.1.93
```

### Comparing `sparrow-order-lib-0.1.96/README.md` & `sparrow-order-lib-0.1.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Project Description
 
 # Release History
+## version==0.1.97
+* SparrowAftersaleConstants
+
 ## version==0.1.96
 * SparrowAftersaleConstants
 
 ## version==0.1.95
 * SparrowAftersaleConstants
 
 ## version==0.1.93
```

### Comparing `sparrow-order-lib-0.1.96/setup.cfg` & `sparrow-order-lib-0.1.97/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-order-lib
-version = 0.1.96
+version = 0.1.97
 author = Jessica Liao
 author_email = 18610193367@sina.cn
 description = This is a lib for sparrow order projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/sparrow614/sparrow-order-lib
 project_urls =
```

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/__init__.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/base_models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/base_models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/common_utils.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/datastructures.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/decorators.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/dt_utils.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/dt_utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/model_function.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/model_function.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/core/xls_util.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/core/xls_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/db_tool/query.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/db_tool/query.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/__init__.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/base.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/client.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/client.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_builder.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_door.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_param.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/es_query_util.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/exceptions.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/field.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/operators.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/__init__.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_base.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_builder.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_door.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_door.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_param.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_es_query_util.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_field.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_in_query_param.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/es_util/tests/test_operators.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/es_util/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/mapping_constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/query_mapping_constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/query_mapping_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/es/test_order_doc_type.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/es/test_order_doc_type.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_api_path.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_api_path.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_core.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_core.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_core_go.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_core_go.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_lanyue.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_lanyue.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/remote_call/sparrow_product.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/remote_call/sparrow_product.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/serializer_data.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_afsplus/utils.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_afsplus/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/afsline_constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
     CLOSING = 'closing'  # 关闭中
     COMPLETING = 'completing'  # 完成中
     OPEN_FAILED = 'open_failed'  # 申请售后失败
     CLOSE_FAILED = 'close_failed'  # 关闭售后失败
     COMPLETE_FAILED = 'complete_failed'  # 完成售后失败
 
     ## 2023.05 货款分离退
-    # 未发货已退款
+    # 未退货已退款
     UNCONFIRM_REFUNDED = 'unconfirm_refunded'
 
     AFTERSALE_STATUS_CHOICES = (
         (OPEN, "待审核"),
         # (IN_FINANCE, "财务待审"),
         # (IN_FINANCE_2ND, "财务一审通过"),
         (REJECTED, "客服驳回"),
@@ -372,15 +372,15 @@
         (PENDING_REFUND, "待退款"),
         (INSTORE_APPROVED, "店内系统通过"),
         (INSTORE_REJECTED, "店内系统驳回"),
         (ALL_APPROVED, "店内系统通过"),
         (REFUND_FAILED, "退款失败"),
         (COMPLETED, "已完成"),
         (CLOSED, "已取消"),
-        (UNCONFIRM_REFUNDED, '未发货已退款'),
+        (UNCONFIRM_REFUNDED, '未退货已退款'),
     )
     AFTERSALE_STATUS_CHOICES_FOR_C = (
         (OPEN, "待审核"),
         (PENDING_RETURN_0, "待审核"), # 待客服退货
         (PENDING_RETURN_1, "待退货"), # 待客人退货
         (PENDING_RETURN_2, "待退货"), # 发货拦截中
         (PENDING_REFUND, "待退款"),
```

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_aftersale/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_aftersale/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/disstorage.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/disstorage.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/serializer_data.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_disstorage/utils.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_disstorage/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/serializer_data.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/serializer_data.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_distribute/serializers.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_distribute/serializers.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_exchange/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_exchange/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_exchange/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_exchange/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_inparcel/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_inparcel/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_inparcel/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_inparcel/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_orders/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_orders/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_orders/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_orders/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_parcel/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_parcel/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_promotions/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_promotions/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_shipping/constants.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_shipping/constants.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib/sparrow_shipping/models.py` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib/sparrow_shipping/models.py`

 * *Files identical despite different names*

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/PKG-INFO` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrow-order-lib
-Version: 0.1.96
+Version: 0.1.97
 Summary: This is a lib for sparrow order projects.
 Home-page: https://gitee.com/sparrow614/sparrow-order-lib
 Author: Jessica Liao
 Author-email: 18610193367@sina.cn
 Project-URL: Bug Tracker, https://gitee.com/sparrow614/sparrow-order-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,17 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
 # Release History
+## version==0.1.97
+* SparrowAftersaleConstants
+
 ## version==0.1.96
 * SparrowAftersaleConstants
 
 ## version==0.1.95
 * SparrowAftersaleConstants
 
 ## version==0.1.93
```

### Comparing `sparrow-order-lib-0.1.96/src/sparrow_order_lib.egg-info/SOURCES.txt` & `sparrow-order-lib-0.1.97/src/sparrow_order_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

