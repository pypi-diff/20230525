# Comparing `tmp/ydb-3.3.3.tar.gz` & `tmp/ydb-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydb-3.3.3.tar", last modified: Fri May 19 15:22:00 2023, max compression
+gzip compressed data, was "ydb-3.3.4.tar", last modified: Thu May 25 14:36:51 2023, max compression
```

## Comparing `ydb-3.3.3.tar` & `ydb-3.3.4.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.013723 ydb-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-19 15:21:46.000000 ydb-3.3.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-19 15:21:46.000000 ydb-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 15:21:46.000000 ydb-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-19 15:22:00.013723 ydb-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-19 15:21:46.000000 ydb-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 15:21:46.000000 ydb-3.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 15:21:46.000000 ydb-3.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:22:00.013723 ydb-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-19 15:21:51.000000 ydb-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.969716 ydb-3.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_async_iter_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_session_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/aio/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/session_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/ssl/test_ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/table/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/table/test_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.973717 ydb-3.3.3/tests/topics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/test_control_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/test_topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-19 15:21:46.000000 ydb-3.3.3/tests/topics/test_topic_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.977717 ydb-3.3.3/ydb/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.977717 ydb-3.3.3/ydb/_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.977717 ydb-3.3.3/ydb/_grpc/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.981718 ydb-3.3.3/ydb/_grpc/grpcwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    42486 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.985719 ydb-3.3.3/ydb/_grpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.993720 ydb-3.3.3/ydb/_grpc/v3/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.993720 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:59.997721 ydb-3.3.3/ydb/_grpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.005722 ydb-3.3.3/ydb/_grpc/v4/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.005722 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/validation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_cms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_export_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_formats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_session_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_sp_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.005722 ydb-3.3.3/ydb/_topic_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_common/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/_topic_reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/datatypes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_reader/topic_reader_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/_topic_writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_topic_writer/topic_writer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_tx_ctx_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/_utilities_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/aio/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/auth_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/dbapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/default_pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.009723 ydb-3.3.3/ydb/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/iam/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/import_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/scheme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.013723 ydb-3.3.3/ydb/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/sqlalchemy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13414 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-19 15:21:46.000000 ydb-3.3.3/ydb/types.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 15:21:51.000000 ydb-3.3.3/ydb/ydb_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:22:00.013723 ydb-3.3.3/ydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 15:21:59.000000 ydb-3.3.3/ydb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 14:36:37.000000 ydb-3.3.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-25 14:36:37.000000 ydb-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 14:36:37.000000 ydb-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 14:36:51.173507 ydb-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 14:36:37.000000 ydb-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 14:36:37.000000 ydb-3.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 14:36:37.000000 ydb-3.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:36:51.173507 ydb-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 14:36:42.000000 ydb-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.129507 ydb-3.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.133507 ydb-3.3.4/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_async_iter_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_session_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/aio/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/session_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.133507 ydb-3.3.4/tests/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/ssl/test_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.137507 ydb-3.3.4/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/table/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/table/test_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.141507 ydb-3.3.4/tests/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/test_control_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/test_topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-05-25 14:36:37.000000 ydb-3.3.4/tests/topics/test_topic_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/_grpc/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.145507 ydb-3.3.4/ydb/_grpc/grpcwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45284 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.149507 ydb-3.3.4/ydb/_grpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.157507 ydb-3.3.4/ydb/_grpc/v3/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.157507 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83179 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121326 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41176 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72285 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29771 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40278 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332647 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234296 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.161507 ydb-3.3.4/ydb/_grpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.165507 ydb-3.3.4/ydb/_grpc/v4/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/validation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/annotations/validation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_cms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_cms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15716 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_coordination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_coordination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_export_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_export_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_formats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_formats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_issue_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_query_stats_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scheme_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scheme_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scripting_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scripting_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_status_codes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46408 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/protos/ydb_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16278 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_session_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_sp_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_topic_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_common/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_topic_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/datatypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23087 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47528 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_reader/topic_reader_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/_topic_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_topic_writer/topic_writer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_tx_ctx_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/_utilities_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.169507 ydb-3.3.4/ydb/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/aio/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/auth_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/dbapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   285865 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/default_pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/iam/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/import_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/scheme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/sqlalchemy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82321 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-25 14:36:37.000000 ydb-3.3.4/ydb/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 14:36:42.000000 ydb-3.3.4/ydb/ydb_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:51.173507 ydb-3.3.4/ydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 14:36:51.000000 ydb-3.3.4/ydb.egg-info/top_level.txt
```

### Comparing `ydb-3.3.3/LICENSE` & `ydb-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/PKG-INFO` & `ydb-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.3
+Version: 3.3.4
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.3/README.md` & `ydb-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/setup.py` & `ydb-3.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for line in r.readlines():
         line = line.strip()
         if line != "":
             requirements.append(line)
 
 setuptools.setup(
     name="ydb",
-    version="3.3.3",  # AUTOVERSION
+    version="3.3.4",  # AUTOVERSION
     description="YDB Python SDK",
     author="Yandex LLC",
     author_email="ydb@yandex-team.ru",
     url="http://github.com/ydb-platform/ydb-python-sdk",
     license="Apache 2.0",
     package_dir={"": "."},
     long_description=long_description,
```

### Comparing `ydb-3.3.3/tests/aio/test_async_iter_stream.py` & `ydb-3.3.4/tests/aio/test_async_iter_stream.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/aio/test_connection.py` & `ydb-3.3.4/tests/aio/test_connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/aio/test_connection_pool.py` & `ydb-3.3.4/tests/aio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/aio/test_session_pool.py` & `ydb-3.3.4/tests/aio/test_session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/aio/test_tx.py` & `ydb-3.3.4/tests/aio/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/aio/test_types.py` & `ydb-3.3.4/tests/aio/test_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/conftest.py` & `ydb-3.3.4/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,14 +174,34 @@
     )
 
     return topic_path
 
 
 @pytest.fixture()
 @pytest.mark.asyncio()
+async def topic_with_two_partitions_path(driver, topic_consumer, database) -> str:
+    topic_path = database + "/test-topic-two-partitions"
+
+    try:
+        await driver.topic_client.drop_topic(topic_path)
+    except issues.SchemeError:
+        pass
+
+    await driver.topic_client.create_topic(
+        path=topic_path,
+        consumers=[topic_consumer],
+        min_active_partitions=2,
+        partition_count_limit=2,
+    )
+
+    return topic_path
+
+
+@pytest.fixture()
+@pytest.mark.asyncio()
 async def topic_with_messages(driver, topic_consumer, database):
     topic_path = database + "/test-topic-with-messages"
     try:
         await driver.topic_client.drop_topic(topic_path)
     except issues.SchemeError:
         pass
```

### Comparing `ydb-3.3.3/tests/session_pool.py` & `ydb-3.3.4/tests/session_pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/table/table_test.py` & `ydb-3.3.4/tests/table/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/table/test_tx.py` & `ydb-3.3.4/tests/table/test_tx.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/test_errors.py` & `ydb-3.3.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/topics/test_control_plane.py` & `ydb-3.3.4/tests/topics/test_control_plane.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/tests/topics/test_topic_reader.py` & `ydb-3.3.4/tests/topics/test_topic_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import asyncio
+
 import pytest
 
 import ydb
 
 
 @pytest.mark.asyncio
 class TestTopicReaderAsyncIO:
@@ -157,7 +159,49 @@
 
         with driver_sync.topic_client.writer(topic_path, codec=codec, encoders={codec: encode}) as writer:
             writer.write("123")
 
         with driver_sync.topic_client.reader(topic_path, topic_consumer, decoders={codec: decode}) as reader:
             batch = reader.receive_batch()
             assert batch.messages[0].data.decode() == "123"
+
+
+@pytest.mark.asyncio
+class TestBugFixesAsync:
+    async def test_issue_297_bad_handle_stop_partition(
+        self, driver, topic_consumer, topic_with_two_partitions_path: str
+    ):
+        async def wait(fut):
+            return await asyncio.wait_for(fut, timeout=10)
+
+        topic = topic_with_two_partitions_path  # type: str
+
+        async with driver.topic_client.writer(topic, partition_id=0) as writer:
+            await writer.write_with_ack("00")
+
+        async with driver.topic_client.writer(topic, partition_id=1) as writer:
+            await writer.write_with_ack("01")
+
+        # Start first reader and receive messages from both partitions
+        reader0 = driver.topic_client.reader(topic, consumer=topic_consumer)
+        await wait(reader0.receive_message())
+        await wait(reader0.receive_message())
+
+        # Start second reader for same topic, same consumer, partition 1
+        reader1 = driver.topic_client.reader(topic, consumer=topic_consumer)
+
+        # receive uncommited message
+        await reader1.receive_message()
+
+        # write one message for every partition
+        async with driver.topic_client.writer(topic, partition_id=0) as writer:
+            await writer.write_with_ack("10")
+        async with driver.topic_client.writer(topic, partition_id=1) as writer:
+            await writer.write_with_ack("11")
+
+        msg0 = await wait(reader0.receive_message())
+        msg1 = await wait(reader1.receive_message())
+
+        datas = [msg0.data.decode(), msg1.data.decode()]
+        datas.sort()
+
+        assert datas == ["10", "11"]
```

### Comparing `ydb-3.3.3/tests/topics/test_topic_writer.py` & `ydb-3.3.4/tests/topics/test_topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/__init__.py` & `ydb-3.3.4/ydb/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_apis.py` & `ydb-3.3.4/ydb/_apis.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_errors.py` & `ydb-3.3.4/ydb/_errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/common/__init__.py` & `ydb-3.3.4/ydb/_grpc/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/grpcwrapper/common_utils.py` & `ydb-3.3.4/ydb/_grpc/grpcwrapper/common_utils.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_scheme.py` & `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic.py` & `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 import datetime
 import enum
 import typing
 from dataclasses import dataclass, field
 from typing import List, Union, Dict, Optional
 
 from google.protobuf.message import Message
 
 from . import ydb_topic_public_types
 from ... import scheme
+from ... import issues
 
 # Workaround for good IDE and universal for runtime
 if typing.TYPE_CHECKING:
     from ..v4.protos import ydb_scheme_pb2, ydb_topic_pb2
 else:
     from ..common.protos import ydb_scheme_pb2, ydb_topic_pb2
 
@@ -584,24 +587,40 @@
             ) -> "StreamReadMessage.CommitOffsetResponse.PartitionCommittedOffset":
                 return StreamReadMessage.CommitOffsetResponse.PartitionCommittedOffset(
                     partition_session_id=msg.partition_session_id,
                     committed_offset=msg.committed_offset,
                 )
 
     @dataclass
-    class PartitionSessionStatusRequest:
+    class PartitionSessionStatusRequest(IToProto):
         partition_session_id: int
 
+        def to_proto(self) -> ydb_topic_pb2.StreamReadMessage.PartitionSessionStatusRequest:
+            return ydb_topic_pb2.StreamReadMessage.PartitionSessionStatusRequest(
+                partition_session_id=self.partition_session_id
+            )
+
     @dataclass
-    class PartitionSessionStatusResponse:
+    class PartitionSessionStatusResponse(IFromProto):
         partition_session_id: int
         partition_offsets: "OffsetsRange"
         committed_offset: int
         write_time_high_watermark: float
 
+        @staticmethod
+        def from_proto(
+            msg: ydb_topic_pb2.StreamReadMessage.PartitionSessionStatusResponse,
+        ) -> "StreamReadMessage.PartitionSessionStatusResponse":
+            return StreamReadMessage.PartitionSessionStatusResponse(
+                partition_session_id=msg.partition_session_id,
+                partition_offsets=OffsetsRange.from_proto(msg.partition_offsets),
+                committed_offset=msg.committed_offset,
+                write_time_high_watermark=msg.write_time_high_watermark,
+            )
+
     @dataclass
     class StartPartitionSessionRequest(IFromProto):
         partition_session: "StreamReadMessage.PartitionSession"
         committed_offset: int
         partition_offsets: "OffsetsRange"
 
         @staticmethod
@@ -628,23 +647,38 @@
             if self.read_offset is not None:
                 res.read_offset = self.read_offset
             if self.commit_offset is not None:
                 res.commit_offset = self.commit_offset
             return res
 
     @dataclass
-    class StopPartitionSessionRequest:
+    class StopPartitionSessionRequest(IFromProto):
         partition_session_id: int
         graceful: bool
         committed_offset: int
 
+        @staticmethod
+        def from_proto(
+            msg: ydb_topic_pb2.StreamReadMessage.StopPartitionSessionRequest,
+        ) -> StreamReadMessage.StopPartitionSessionRequest:
+            return StreamReadMessage.StopPartitionSessionRequest(
+                partition_session_id=msg.partition_session_id,
+                graceful=msg.graceful,
+                committed_offset=msg.committed_offset,
+            )
+
     @dataclass
-    class StopPartitionSessionResponse:
+    class StopPartitionSessionResponse(IToProto):
         partition_session_id: int
 
+        def to_proto(self) -> ydb_topic_pb2.StreamReadMessage.StopPartitionSessionResponse:
+            return ydb_topic_pb2.StreamReadMessage.StopPartitionSessionResponse(
+                partition_session_id=self.partition_session_id,
+            )
+
     @dataclass
     class FromClient(IToProto):
         client_message: "ReaderMessagesFromClientToServer"
 
         def __init__(self, client_message: "ReaderMessagesFromClientToServer"):
             self.client_message = client_message
 
@@ -656,14 +690,18 @@
                 res.commit_offset_request.CopyFrom(self.client_message.to_proto())
             elif isinstance(self.client_message, StreamReadMessage.InitRequest):
                 res.init_request.CopyFrom(self.client_message.to_proto())
             elif isinstance(self.client_message, UpdateTokenRequest):
                 res.update_token_request.CopyFrom(self.client_message.to_proto())
             elif isinstance(self.client_message, StreamReadMessage.StartPartitionSessionResponse):
                 res.start_partition_session_response.CopyFrom(self.client_message.to_proto())
+            elif isinstance(self.client_message, StreamReadMessage.StopPartitionSessionResponse):
+                res.stop_partition_session_response.CopyFrom(self.client_message.to_proto())
+            elif isinstance(self.client_message, StreamReadMessage.PartitionSessionStatusRequest):
+                res.start_partition_session_response.CopyFrom(self.client_message.to_proto())
             else:
                 raise NotImplementedError("Unknown message type: %s" % type(self.client_message))
             return res
 
     @dataclass
     class FromServer(IFromProto):
         server_message: "ReaderMessagesFromServerToClient"
@@ -690,25 +728,40 @@
                     server_status=server_status,
                     server_message=StreamReadMessage.InitResponse.from_proto(msg.init_response),
                 )
             elif mess_type == "start_partition_session_request":
                 return StreamReadMessage.FromServer(
                     server_status=server_status,
                     server_message=StreamReadMessage.StartPartitionSessionRequest.from_proto(
-                        msg.start_partition_session_request
+                        msg.start_partition_session_request,
+                    ),
+                )
+            elif mess_type == "stop_partition_session_request":
+                return StreamReadMessage.FromServer(
+                    server_status=server_status,
+                    server_message=StreamReadMessage.StopPartitionSessionRequest.from_proto(
+                        msg.stop_partition_session_request
                     ),
                 )
             elif mess_type == "update_token_response":
                 return StreamReadMessage.FromServer(
                     server_status=server_status,
                     server_message=UpdateTokenResponse.from_proto(msg.update_token_response),
                 )
-
-            # todo replace exception to log
-            raise NotImplementedError()
+            elif mess_type == "partition_session_status_response":
+                return StreamReadMessage.FromServer(
+                    server_status=server_status,
+                    server_message=StreamReadMessage.PartitionSessionStatusResponse.from_proto(
+                        msg.partition_session_status_response
+                    ),
+                )
+            else:
+                raise issues.UnexpectedGrpcMessage(
+                    "Unexpected message while parse ReaderMessagesFromServerToClient: '%s'" % mess_type
+                )
 
 
 ReaderMessagesFromClientToServer = Union[
     StreamReadMessage.InitRequest,
     StreamReadMessage.ReadRequest,
     StreamReadMessage.CommitOffsetRequest,
     StreamReadMessage.PartitionSessionStatusRequest,
```

### Comparing `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py` & `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_public_types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/grpcwrapper/ydb_topic_test.py` & `ydb-3.3.4/ydb/_grpc/grpcwrapper/ydb_topic_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/annotations/validation_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_auth_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_cms_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_common_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_coordination_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_discovery_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_export_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_formats_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_import_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_operation_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scheme_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_scripting_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_table_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_topic_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/protos/ydb_value_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v3/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/annotations/validation_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/annotations/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_auth_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_auth_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_cms_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_cms_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_common_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_common_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_coordination_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_coordination_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_discovery_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_export_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_export_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_formats_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_formats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_import_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_import_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_issue_message_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_operation_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_query_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_rate_limiter_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scheme_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scheme_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_scripting_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_scripting_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_status_codes_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_table_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_topic_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/protos/ydb_value_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/protos/ydb_value_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_auth_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_cms_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_coordination_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_discovery_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_export_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_import_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_monitoring_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_operation_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_rate_limiter_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_scheme_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_scripting_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_table_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py` & `ydb-3.3.4/ydb/_grpc/v4/ydb_topic_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_session_impl.py` & `ydb-3.3.4/ydb/_session_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_sp_impl.py` & `ydb-3.3.4/ydb/_sp_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_common/common.py` & `ydb-3.3.4/ydb/_topic_common/common.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_common/common_test.py` & `ydb-3.3.4/ydb/_topic_common/common_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_common/test_helpers.py` & `ydb-3.3.4/ydb/_topic_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_reader/datatypes.py` & `ydb-3.3.4/ydb/_topic_reader/datatypes.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_reader/datatypes_test.py` & `ydb-3.3.4/ydb/_topic_reader/datatypes_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_reader/topic_reader.py` & `ydb-3.3.4/ydb/_topic_reader/topic_reader.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio.py` & `ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from .._grpc.grpcwrapper.ydb_topic import (
     StreamReadMessage,
     UpdateTokenRequest,
     UpdateTokenResponse,
     Codec,
 )
 from .._errors import check_retriable_error
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class TopicReaderError(YdbError):
     pass
 
 
 class TopicReaderUnexpectedCodec(YdbError):
@@ -142,15 +145,14 @@
 
     _state_changed: asyncio.Event
     _stream_reader: Optional["ReaderStream"]
     _first_error: asyncio.Future[YdbError]
 
     def __init__(self, driver: Driver, settings: topic_reader.PublicReaderSettings):
         self._id = self._static_reader_reconnector_counter.inc_and_get()
-
         self._settings = settings
         self._driver = driver
         self._background_tasks = set()
 
         self._state_changed = asyncio.Event()
         self._stream_reader = None
         self._background_tasks.add(asyncio.create_task(self._connection_loop()))
@@ -391,47 +393,50 @@
                 StreamReadMessage.FromClient(
                     client_message=StreamReadMessage.ReadRequest(
                         bytes_size=self._buffer_size_bytes,
                     ),
                 )
             )
             while True:
-                message = await self._stream.receive()  # type: StreamReadMessage.FromServer
-                _process_response(message.server_status)
+                try:
+                    message = await self._stream.receive()  # type: StreamReadMessage.FromServer
+                    _process_response(message.server_status)
 
-                if isinstance(message.server_message, StreamReadMessage.ReadResponse):
-                    self._on_read_response(message.server_message)
+                    if isinstance(message.server_message, StreamReadMessage.ReadResponse):
+                        self._on_read_response(message.server_message)
 
-                elif isinstance(message.server_message, StreamReadMessage.CommitOffsetResponse):
-                    self._on_commit_response(message.server_message)
+                    elif isinstance(message.server_message, StreamReadMessage.CommitOffsetResponse):
+                        self._on_commit_response(message.server_message)
 
-                elif isinstance(
-                    message.server_message,
-                    StreamReadMessage.StartPartitionSessionRequest,
-                ):
-                    self._on_start_partition_session(message.server_message)
-
-                elif isinstance(
-                    message.server_message,
-                    StreamReadMessage.StopPartitionSessionRequest,
-                ):
-                    self._on_partition_session_stop(message.server_message)
-
-                elif isinstance(message.server_message, UpdateTokenResponse):
-                    self._update_token_event.set()
-
-                else:
-                    raise NotImplementedError(
-                        "Unexpected type of StreamReadMessage.FromServer message: %s" % message.server_message
-                    )
+                    elif isinstance(
+                        message.server_message,
+                        StreamReadMessage.StartPartitionSessionRequest,
+                    ):
+                        self._on_start_partition_session(message.server_message)
+
+                    elif isinstance(
+                        message.server_message,
+                        StreamReadMessage.StopPartitionSessionRequest,
+                    ):
+                        self._on_partition_session_stop(message.server_message)
+
+                    elif isinstance(message.server_message, UpdateTokenResponse):
+                        self._update_token_event.set()
+
+                    else:
+                        raise issues.UnexpectedGrpcMessage(
+                            "Unexpected message in _read_messages_loop: %s" % type(message.server_message)
+                        )
+                except issues.UnexpectedGrpcMessage as e:
+                    logger.exception("unexpected message in stream reader: %s" % e)
 
                 self._state_changed.set()
         except Exception as e:
             self._set_first_error(e)
-            raise
+            return
 
     async def _update_token_loop(self):
         while True:
             await asyncio.sleep(self._update_token_interval)
             await self._update_token(token=self._get_token_function())
 
     async def _update_token(self, token: str):
```

### Comparing `ydb-3.3.3/ydb/_topic_reader/topic_reader_asyncio_test.py` & `ydb-3.3.4/ydb/_topic_reader/topic_reader_asyncio_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1123,14 +1123,37 @@
         )
 
         got = await wait_for_fast(stream.from_client.get())
         assert expected == got
 
         await reader.close()
 
+    async def test_read_unknown_message(self, stream, stream_reader, caplog):
+        class TestMessage:
+            pass
+
+        # noinspection PyTypeChecker
+        stream.from_server.put_nowait(
+            StreamReadMessage.FromServer(
+                server_status=ServerStatus(
+                    status=issues.StatusCode.SUCCESS,
+                    issues=[],
+                ),
+                server_message=TestMessage(),
+            )
+        )
+
+        def logged():
+            for rec in caplog.records:
+                if TestMessage.__name__ in rec.message:
+                    return True
+            return False
+
+        await wait_condition(logged)
+
 
 @pytest.mark.asyncio
 class TestReaderReconnector:
     async def test_reconnect_on_repeatable_error(self, monkeypatch):
         test_error = issues.Overloaded("test error")
 
         async def wait_error():
```

### Comparing `ydb-3.3.3/ydb/_topic_reader/topic_reader_sync.py` & `ydb-3.3.4/ydb/_topic_reader/topic_reader_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_writer/topic_writer.py` & `ydb-3.3.4/ydb/_topic_writer/topic_writer.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio.py` & `ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_writer/topic_writer_asyncio_test.py` & `ydb-3.3.4/ydb/_topic_writer/topic_writer_asyncio_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_writer/topic_writer_sync.py` & `ydb-3.3.4/ydb/_topic_writer/topic_writer_sync.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_topic_writer/topic_writer_test.py` & `ydb-3.3.4/ydb/_topic_writer/topic_writer_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_tx_ctx_impl.py` & `ydb-3.3.4/ydb/_tx_ctx_impl.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/_utilities.py` & `ydb-3.3.4/ydb/_utilities.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/connection.py` & `ydb-3.3.4/ydb/aio/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/credentials.py` & `ydb-3.3.4/ydb/aio/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/driver.py` & `ydb-3.3.4/ydb/aio/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/iam.py` & `ydb-3.3.4/ydb/aio/iam.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 except ImportError:
     aiohttp = None
 
 
 class TokenServiceCredentials(AbstractExpiringTokenCredentials):
     def __init__(self, iam_endpoint=None, iam_channel_credentials=None):
         super(TokenServiceCredentials, self).__init__()
-        assert iam_token_service_pb2_grpc is not None, "run pip install==ydb[yc] to use service account credentials"
+        assert iam_token_service_pb2_grpc is not None, 'run pip install "ydb[yc]" to use service account credentials'
         self._get_token_request_timeout = 10
         self._iam_endpoint = "iam.api.cloud.yandex.net:443" if iam_endpoint is None else iam_endpoint
         self._iam_channel_credentials = {} if iam_channel_credentials is None else iam_channel_credentials
 
     def _channel_factory(self):
         return grpc.aio.secure_channel(
             self._iam_endpoint,
```

### Comparing `ydb-3.3.3/ydb/aio/pool.py` & `ydb-3.3.4/ydb/aio/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/resolver.py` & `ydb-3.3.4/ydb/aio/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/scheme.py` & `ydb-3.3.4/ydb/aio/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/aio/table.py` & `ydb-3.3.4/ydb/aio/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/connection.py` & `ydb-3.3.4/ydb/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/convert.py` & `ydb-3.3.4/ydb/convert.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/credentials.py` & `ydb-3.3.4/ydb/credentials.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/dbapi/__init__.py` & `ydb-3.3.4/ydb/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/dbapi/connection.py` & `ydb-3.3.4/ydb/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/dbapi/cursor.py` & `ydb-3.3.4/ydb/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/dbapi/errors.py` & `ydb-3.3.4/ydb/dbapi/errors.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/default_pem.py` & `ydb-3.3.4/ydb/default_pem.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/driver.py` & `ydb-3.3.4/ydb/driver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/export.py` & `ydb-3.3.4/ydb/export.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/global_settings.py` & `ydb-3.3.4/ydb/global_settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/iam/auth.py` & `ydb-3.3.4/ydb/iam/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         },
     )
 
 
 class TokenServiceCredentials(credentials.AbstractExpiringTokenCredentials):
     def __init__(self, iam_endpoint=None, iam_channel_credentials=None, tracer=None):
         super(TokenServiceCredentials, self).__init__(tracer)
-        assert iam_token_service_pb2_grpc is not None, "run pip install==ydb[yc] to use service account credentials"
+        assert iam_token_service_pb2_grpc is not None, 'run pip install "ydb[yc]" to use service account credentials'
         self._get_token_request_timeout = 10
         self._iam_token_service_pb2 = iam_token_service_pb2
         self._iam_token_service_pb2_grpc = iam_token_service_pb2_grpc
         self._iam_endpoint = "iam.api.cloud.yandex.net:443" if iam_endpoint is None else iam_endpoint
         self._iam_channel_credentials = {} if iam_channel_credentials is None else iam_channel_credentials
 
     def _channel_factory(self):
```

### Comparing `ydb-3.3.3/ydb/import_client.py` & `ydb-3.3.4/ydb/import_client.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/interceptor.py` & `ydb-3.3.4/ydb/interceptor.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/issues.py` & `ydb-3.3.4/ydb/issues.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,19 @@
     status = StatusCode.SESSION_BUSY
 
 
 class SessionPoolEmpty(Error, queue.Empty):
     status = StatusCode.SESSION_POOL_EMPTY
 
 
+class UnexpectedGrpcMessage(Error):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
 def _format_issues(issues):
     if not issues:
         return ""
 
     return " ,".join(text_format.MessageToString(issue, as_utf8=False, as_one_line=True) for issue in issues)
```

### Comparing `ydb-3.3.3/ydb/operation.py` & `ydb-3.3.4/ydb/operation.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/pool.py` & `ydb-3.3.4/ydb/pool.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/resolver.py` & `ydb-3.3.4/ydb/resolver.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/scheme.py` & `ydb-3.3.4/ydb/scheme.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/scheme_test.py` & `ydb-3.3.4/ydb/scheme_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/scripting.py` & `ydb-3.3.4/ydb/scripting.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/settings.py` & `ydb-3.3.4/ydb/settings.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/sqlalchemy/__init__.py` & `ydb-3.3.4/ydb/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/sqlalchemy/types.py` & `ydb-3.3.4/ydb/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/table.py` & `ydb-3.3.4/ydb/table.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/table_test.py` & `ydb-3.3.4/ydb/table_test.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/topic.py` & `ydb-3.3.4/ydb/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         decoders: Union[Mapping[int, Callable[[bytes], bytes]], None] = None,
         decoder_executor: Optional[concurrent.futures.Executor] = None,  # default shared client executor pool
     ) -> TopicReaderAsyncIO:
 
         if not decoder_executor:
             decoder_executor = self._executor
 
-        args = locals()
+        args = locals().copy()
         del args["self"]
 
         settings = TopicReaderSettings(**args)
 
         return TopicReaderAsyncIO(self._driver, settings, _parent=self)
 
     def writer(
@@ -184,15 +184,15 @@
         partition_id: Union[int, None] = None,
         auto_seqno: bool = True,
         auto_created_at: bool = True,
         codec: Optional[TopicCodec] = None,  # default mean auto-select
         encoders: Optional[Mapping[_ydb_topic_public_types.PublicCodec, Callable[[bytes], bytes]]] = None,
         encoder_executor: Optional[concurrent.futures.Executor] = None,  # default shared client executor pool
     ) -> TopicWriterAsyncIO:
-        args = locals()
+        args = locals().copy()
         del args["self"]
 
         settings = TopicWriterSettings(**args)
 
         if not settings.encoder_executor:
             settings.encoder_executor = self._executor
```

### Comparing `ydb-3.3.3/ydb/tracing.py` & `ydb-3.3.4/ydb/tracing.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb/types.py` & `ydb-3.3.4/ydb/types.py`

 * *Files identical despite different names*

### Comparing `ydb-3.3.3/ydb.egg-info/PKG-INFO` & `ydb-3.3.4/ydb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydb
-Version: 3.3.3
+Version: 3.3.4
 Summary: YDB Python SDK
 Home-page: http://github.com/ydb-platform/ydb-python-sdk
 Author: Yandex LLC
 Author-email: ydb@yandex-team.ru
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ydb-3.3.3/ydb.egg-info/SOURCES.txt` & `ydb-3.3.4/ydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

