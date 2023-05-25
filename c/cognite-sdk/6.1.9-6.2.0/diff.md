# Comparing `tmp/cognite_sdk-6.1.9.tar.gz` & `tmp/cognite_sdk-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.1.9.tar", max compression
+gzip compressed data, was "cognite_sdk-6.2.0.tar", max compression
```

## Comparing `cognite_sdk-6.1.9.tar` & `cognite_sdk-6.2.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
--rw-r--r--   0        0        0    11349 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/LICENSE
--rw-r--r--   0        0        0     3945 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/README.md
--rw-r--r--   0        0        0      503 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48450 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    11025 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20644 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17419 2023-05-16 04:59:05.651029 cognite_sdk-6.1.9/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44308 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49922 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9297 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32132 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27928 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21039 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4638 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9570 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    36997 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5245 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      140 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-05-16 04:59:05.655029 cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/config.py
--rw-r--r--   0        0        0    18062 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14299 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    11319 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/py.typed
--rw-r--r--   0        0        0     8194 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7894 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5919 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-05-16 04:59:05.659030 cognite_sdk-6.1.9/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2001 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2132 2023-05-16 04:59:05.663030 cognite_sdk-6.1.9/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-25 11:10:55.565276 cognite_sdk-6.2.0/LICENSE
+-rw-r--r--   0        0        0     3945 2023-05-25 11:10:55.565276 cognite_sdk-6.2.0/README.md
+-rw-r--r--   0        0        0      503 2023-05-25 11:10:55.565276 cognite_sdk-6.2.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 11:10:55.565276 cognite_sdk-6.2.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-05-25 11:10:55.565276 cognite_sdk-6.2.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48450 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0      573 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/data_modeling.py
+-rw-r--r--   0        0        0    11025 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20644 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17419 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44319 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49915 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9297 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     6483 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/spaces.py
+-rw-r--r--   0        0        0     7909 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32111 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27928 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21012 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4638 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9570 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-05-25 11:10:55.569276 cognite_sdk-6.2.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    37531 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      140 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6501 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/config.py
+-rw-r--r--   0        0        0    18062 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8901 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14299 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0     1753 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/spaces.py
+-rw-r--r--   0        0        0    16814 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    10445 2023-05-25 11:10:55.573276 cognite_sdk-6.2.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/py.typed
+-rw-r--r--   0        0        0     8434 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7894 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7277 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2001 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2132 2023-05-25 11:10:55.577277 cognite_sdk-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.2.0/PKG-INFO
```

### Comparing `cognite_sdk-6.1.9/LICENSE` & `cognite_sdk-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/README.md` & `cognite_sdk-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/annotations.py` & `cognite_sdk-6.2.0/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/assets.py` & `cognite_sdk-6.2.0/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/data_sets.py` & `cognite_sdk-6.2.0/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.2.0/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/datapoints.py` & `cognite_sdk-6.2.0/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/diagrams.py` & `cognite_sdk-6.2.0/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.2.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/events.py` & `cognite_sdk-6.2.0/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.2.0/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/files.py` & `cognite_sdk-6.2.0/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/functions.py` & `cognite_sdk-6.2.0/cognite/client/_api/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             external_id (str, optional):             External id of the function.
             description (str, optional):             Description of the function.
             owner (str, optional):                   Owner of this function. Typically used to know who created it.
             secrets (Dict[str, str]):                Additional secrets as key/value pairs. These can e.g. password to simulators or other data sources. Keys must be lowercase characters, numbers or dashes (-) and at most 15 characters. You can create at most 30 secrets, all keys must be unique.
             env_vars (Dict[str, str]):               Environment variables as key/value pairs. Keys can contain only letters, numbers or the underscore character. You can create at most 100 environment variables.
             cpu (Number, optional):                  Number of CPU cores per function. Allowed values are in the range [0.1, 0.6], and None translates to the API default which is 0.25 in GCP. The argument is unavailable in Azure.
             memory (Number, optional):               Memory per function measured in GB. Allowed values are in the range [0.1, 2.5], and None translates to the API default which is 1 GB in GCP. The argument is unavailable in Azure.
-            runtime (str, optional):                 The function runtime. Valid values are ["py37", "py38", "py39", `None`], and `None` translates to the API default which currently is "py38". The runtime "py38" resolves to the latest version of the Python 3.8 series.
+            runtime (str, optional):                 The function runtime. Valid values are ["py37", "py38", "py39", "py310", `None`], and `None` translates to the API default which will change over time. The runtime "py38" resolves to the latest version of the Python 3.8 series.
             metadata (Dict[str, str], optional):     Metadata for the function as key/value pairs. Key & values can be at most 32, 512 characters long respectively. You can have at the most 16 key-value pairs, with a maximum size of 512 bytes.
             index_url (str, optional):               Index URL for Python Package Manager to use. Be aware of the intrinsic security implications of using the `index_url` option. `More information can be found on official docs, <https://docs.cognite.com/cdf/functions/#additional-arguments>`_
             extra_index_urls (List[str], optional):  Extra Index URLs for Python Package Manager to use. Be aware of the intrinsic security implications of using the `extra_index_urls` option. `More information can be found on official docs, <https://docs.cognite.com/cdf/functions/#additional-arguments>`_
         Returns:
             Function: The created function.
 
         Examples:
```

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/geospatial.py` & `cognite_sdk-6.2.0/cognite/client/_api/geospatial.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             Delete feature type definitions external id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.geospatial.delete_feature_types(external_id=["wells", "cities"])
         """
         extra_body_fields = {"recursive": True} if recursive else {}
-        return self._delete_multiple(
+        self._delete_multiple(
             identifiers=IdentifierSequence.load(external_ids=external_id),
             wrap_ids=True,
             resource_path=f"{self._RESOURCE_PATH}/featuretypes",
             extra_body_fields=extra_body_fields,
         )
 
     def list_feature_types(self) -> FeatureTypeList:
```

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/iam.py` & `cognite_sdk-6.2.0/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/labels.py` & `cognite_sdk-6.2.0/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/raw.py` & `cognite_sdk-6.2.0/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/relationships.py` & `cognite_sdk-6.2.0/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/sequences.py` & `cognite_sdk-6.2.0/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.2.0/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/templates.py` & `cognite_sdk-6.2.0/cognite/client/_api/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         Examples:
             Delete template groups by external id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.templates.groups.delete(external_ids=["a", "b"])
         """
-        return self._delete_multiple(
+        self._delete_multiple(
             wrap_ids=True,
             identifiers=IdentifierSequence.load(external_ids=external_ids),
             extra_body_fields={"ignoreUnknownIds": ignore_unknown_ids},
         )
 
 
 class TemplateGroupVersionsAPI(APIClient):
@@ -548,15 +548,15 @@
             Delete template groups by external id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.templates.instances.delete("sdk-test-group", 1, external_ids=["a", "b"])
         """
         resource_path = utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, external_id, version)
-        return self._delete_multiple(
+        self._delete_multiple(
             resource_path=resource_path,
             identifiers=IdentifierSequence.load(external_ids=external_ids),
             wrap_ids=True,
             extra_body_fields={"ignoreUnknownIds": ignore_unknown_ids},
         )
 
 
@@ -726,13 +726,13 @@
             Delete views by external id:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.templates.views.delete("sdk-test-group", 1, external_id=["a", "b"])
         """
         resource_path = utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, external_id, version)
-        return self._delete_multiple(
+        self._delete_multiple(
             resource_path=resource_path,
             identifiers=IdentifierSequence.load(external_ids=view_external_id),
             wrap_ids=True,
             extra_body_fields={"ignoreUnknownIds": ignore_unknown_ids},
         )
```

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/three_d.py` & `cognite_sdk-6.2.0/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/time_series.py` & `cognite_sdk-6.2.0/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.2.0/cognite/client/_api/transformations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,25 +70,25 @@
                 >>>     Transformation(
                 >>>         name="transformation2",
                 >>>         destination=TransformationDestination.raw("myDatabase", "myTable")
                 >>>     ),
                 >>>      Transformation(
                 >>>      name="transformation3",
                 >>>      view = ViewInfo(space="TypeSpace", external_id="TypeExtId", version="version"),
-                >>>      destination=TransformationDestination.instance_nodes(view, "InstanceSpace")
+                >>>      destination=TransformationDestination.nodes(view, "InstanceSpace")
                 >>>      ),
                 >>>      Transformation(
                 >>>      name="transformation4",
                 >>>      view = ViewInfo(space="TypeSpace", external_id="TypeExtId", version="version"),
-                >>>      destination=TransformationDestination.instance_edges(view, "InstanceSpace")
+                >>>      destination=TransformationDestination.edges(view, "InstanceSpace")
                 >>>      ),
                 >>>      Transformation(
                 >>>      name="transformation5",
                 >>>      edge_type = EdgeType(space="TypeSpace", external_id="TypeExtId"),
-                >>>      destination=TransformationDestination.instance_edges(edge_type,"InstanceSpace")
+                >>>      destination=TransformationDestination.edges(edge_type,"InstanceSpace")
                 >>>      ),
                 >>> ]
                 >>> res = c.transformations.create(transformations)
 
         """
         if isinstance(transformation, Sequence):
             sessions: Dict[str, NonceCredentials] = {}
```

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.2.0/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.2.0/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.2.0/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.2.0/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api/vision.py` & `cognite_sdk-6.2.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_api_client.py` & `cognite_sdk-6.2.0/cognite/client/_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     CogniteResource,
     CogniteUpdate,
     T_CogniteResource,
     T_CogniteResourceList,
 )
 from cognite.client.exceptions import CogniteAPIError, CogniteNotFoundError
 from cognite.client.utils._auxiliary import is_unlimited, split_into_chunks
-from cognite.client.utils._identifier import Identifier, IdentifierSequence, SingletonIdentifierSequence
+from cognite.client.utils._identifier import IdentifierCore, IdentifierSequenceCore, SingletonIdentifierSequence
 from cognite.client.utils._text import convert_all_keys_to_camel_case, shorten, to_snake_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
     from cognite.client.config import ClientConfig
 
 log = logging.getLogger("cognite-sdk")
@@ -239,15 +239,15 @@
         for pattern in cls._RETRYABLE_POST_ENDPOINT_REGEX_PATTERNS:
             if re.match(pattern, path):
                 return True
         return False
 
     def _retrieve(
         self,
-        identifier: Identifier,
+        identifier: IdentifierCore,
         cls: Type[T_CogniteResource],
         resource_path: str = None,
         params: Dict = None,
         headers: Dict = None,
     ) -> Optional[T_CogniteResource]:
         resource_path = resource_path or self._RESOURCE_PATH
         try:
@@ -278,27 +278,27 @@
         ...
 
     @overload
     def _retrieve_multiple(
         self,
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
-        identifiers: IdentifierSequence,
+        identifiers: IdentifierSequenceCore,
         resource_path: Optional[str] = None,
         ignore_unknown_ids: Optional[bool] = None,
         headers: Optional[Dict[str, Any]] = None,
         other_params: Optional[Dict[str, Any]] = None,
     ) -> T_CogniteResourceList:
         ...
 
     def _retrieve_multiple(
         self,
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
-        identifiers: Union[SingletonIdentifierSequence, IdentifierSequence],
+        identifiers: Union[SingletonIdentifierSequence, IdentifierSequenceCore],
         resource_path: Optional[str] = None,
         ignore_unknown_ids: Optional[bool] = None,
         headers: Optional[Dict[str, Any]] = None,
         other_params: Optional[Dict[str, Any]] = None,
     ) -> Union[T_CogniteResourceList, Optional[T_CogniteResource]]:
         resource_path = resource_path or self._RESOURCE_PATH
 
@@ -324,15 +324,20 @@
                 if identifiers.is_singleton():
                     return None
                 raise
 
         retrieved_items = tasks_summary.joined_results(lambda res: res.json()["items"])
 
         if identifiers.is_singleton():
-            return resource_cls._load(retrieved_items[0], cognite_client=self._cognite_client)
+            if retrieved_items:
+                return resource_cls._load(retrieved_items[0], cognite_client=self._cognite_client)
+            else:
+                # Not all APIs (such as the Data Modeling API) return an error when unknown ids are provided,
+                # so we need to handle the unknown singleton identifier case here as well.
+                return None
         return list_cls._load(retrieved_items, cognite_client=self._cognite_client)
 
     def _list_generator(
         self,
         method: str,
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
@@ -655,21 +660,22 @@
 
         if single_item:
             return resource_cls._load(created_resources[0], cognite_client=self._cognite_client)
         return list_cls._load(created_resources, cognite_client=self._cognite_client)
 
     def _delete_multiple(
         self,
-        identifiers: IdentifierSequence,
+        identifiers: IdentifierSequenceCore,
         wrap_ids: bool,
         resource_path: Optional[str] = None,
         params: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, Any]] = None,
         extra_body_fields: Optional[Dict[str, Any]] = None,
-    ) -> None:
+        returns_items: bool = False,
+    ) -> list | None:
         resource_path = resource_path or self._RESOURCE_PATH
         tasks = [
             {
                 "url_path": resource_path + "/delete",
                 "json": {
                     "items": chunk.as_dicts() if wrap_ids else chunk.as_primitives(),
                     **(extra_body_fields or {}),
@@ -680,14 +686,19 @@
             for chunk in identifiers.chunked(self._DELETE_LIMIT)
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"],
             task_list_element_unwrap_fn=utils._auxiliary.unwrap_identifer,
         )
+        if returns_items:
+            deleted_spaces = summary.joined_results(lambda res: res.json()["items"])
+            return deleted_spaces
+        else:
+            return None
 
     @overload
     def _update_multiple(
         self,
         items: Union[CogniteResource, CogniteUpdate],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
```

### Comparing `cognite_sdk-6.1.9/cognite/client/_cognite_client.py` & `cognite_sdk-6.2.0/cognite/client/_cognite_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict, Optional
 
 from requests import Response
 
 from cognite.client import utils
 from cognite.client._api.annotations import AnnotationsAPI
 from cognite.client._api.assets import AssetsAPI
+from cognite.client._api.data_modeling import DataModelingAPI
 from cognite.client._api.data_sets import DataSetsAPI
 from cognite.client._api.diagrams import DiagramsAPI
 from cognite.client._api.entity_matching import EntityMatchingAPI
 from cognite.client._api.events import EventsAPI
 from cognite.client._api.extractionpipelines import ExtractionPipelinesAPI
 from cognite.client._api.files import FilesAPI
 from cognite.client._api.functions import FunctionsAPI
@@ -66,14 +67,15 @@
         self.templates = TemplatesAPI(self._config, self._API_VERSION, self)
         self.vision = VisionAPI(self._config, self._API_VERSION, self)
         self.extraction_pipelines = ExtractionPipelinesAPI(self._config, self._API_VERSION, self)
         self.transformations = TransformationsAPI(self._config, self._API_VERSION, self)
         self.diagrams = DiagramsAPI(self._config, self._API_VERSION, self)
         self.annotations = AnnotationsAPI(self._config, self._API_VERSION, self)
         self.functions = FunctionsAPI(self._config, self._API_VERSION, self)
+        self.data_modeling = DataModelingAPI(self._config, self._API_VERSION, self)
 
         # APIs just using base_url:
         self._api_client = APIClient(self._config, api_version=None, cognite_client=self)
 
     def get(self, url: str, params: Dict[str, Any] = None, headers: Dict[str, Any] = None) -> Response:
         """Perform a GET request to an arbitrary path in the API."""
         return self._api_client._get(url, params=params, headers=headers)
```

### Comparing `cognite_sdk-6.1.9/cognite/client/_http_client.py` & `cognite_sdk-6.2.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.2.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.2.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.2.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.2.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.2.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.2.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.2.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/config.py` & `cognite_sdk-6.2.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/credentials.py` & `cognite_sdk-6.2.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,18 @@
     AggregateUniqueValuesResult,
     GeoLocation,
     GeoLocationFilter,
     Geometry,
     GeometryFilter,
     TimestampRange,
 )
+from cognite.client.data_classes.spaces import (
+    Space,
+    SpaceList,
+)
 from cognite.client.data_classes.templates import (
     ConstantResolver,
     Source,
     TemplateGroup,
     TemplateGroupList,
     TemplateGroupVersion,
     TemplateGroupVersionList,
@@ -349,8 +353,10 @@
     "FeatureTypePatch",
     "FeatureAggregate",
     "FeatureTypeUpdate",
     "FeatureAggregateList",
     "FeatureTypeUpdateList",
     "CoordinateReferenceSystemList",
     "CoordinateReferenceSystem",
+    "Space",
+    "SpaceList",
 ]
```

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/_base.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/assets.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/events.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/files.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/functions.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/iam.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/labels.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/raw.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/shared.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/templates.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/transformations/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import warnings
 from typing import Any, Dict, Optional, Union
 
 from cognite.client.utils._auxiliary import basic_obj_dump
 from cognite.client.utils._text import convert_all_keys_to_snake_case, iterable_to_case
 
 
 class TransformationDestination:
@@ -109,43 +108,41 @@
 
         Returns:
             TransformationDestination pointing to the target sequence rows
         """
         return SequenceRows(external_id=external_id)
 
     @staticmethod
-    def instance_nodes(view: Optional[ViewInfo] = None, instance_space: Optional[str] = None) -> InstanceNodes:
-        """To be used when the transformation is meant to produce node's instances.
-            Flexible Data Models resource type is on `beta` version currently.
+    def nodes(view: Optional[ViewInfo] = None, instance_space: Optional[str] = None) -> Nodes:
+        """
 
         Args:
             view (ViewInfo): information of the view.
             instance_space (str): space id of the instance.
         Returns:
-            InstanceNodes: pointing to the target flexible data model.
+            Nodes: pointing to the target flexible data model.
         """
-        return InstanceNodes(view=view, instance_space=instance_space)
+        return Nodes(view=view, instance_space=instance_space)
 
     @staticmethod
-    def instance_edges(
+    def edges(
         view: Optional[ViewInfo] = None,
         instance_space: Optional[str] = None,
         edge_type: Optional[EdgeType] = None,
-    ) -> InstanceEdges:
-        """To be used when the transformation is meant to produce edge's instances.
-            Flexible Data Models resource type is on `beta` version currently.
+    ) -> Edges:
+        """
 
         Args:
             view (ViewInfo): information of the view.
             instance_space (str): space id of the instance.
             edge_type (EdgeType): information about the type of the edge
         Returns:
-            InstanceEdges: pointing to the target flexible data model.
+            Edges: pointing to the target flexible data model.
         """
-        return InstanceEdges(view=view, instance_space=instance_space, edge_type=edge_type)
+        return Edges(view=view, instance_space=instance_space, edge_type=edge_type)
 
 
 class RawTable(TransformationDestination):
     def __init__(self, database: str = None, table: str = None):
         super().__init__(type="raw")
         self.database = database
         self.table = table
@@ -184,56 +181,48 @@
     def __hash__(self) -> int:
         return hash((self.space, self.external_id))
 
     def dump(self, camel_case: bool = False) -> Dict[str, Any]:
         return basic_obj_dump(self, camel_case)
 
 
-class InstanceNodes(TransformationDestination):
+class Nodes(TransformationDestination):
     def __init__(
         self,
         view: Optional[ViewInfo] = None,
         instance_space: Optional[str] = None,
     ):
-        warnings.warn(
-            "Feature DataModelStorage is in beta and still in development. "
-            "Breaking changes can happen in between patch versions.",
-            stacklevel=2,
-        )
+
         super().__init__(type="nodes")
         self.view = view
         self.instance_space = instance_space
 
     @classmethod
-    def _load(cls, resource: Dict[str, Any]) -> InstanceNodes:
+    def _load(cls, resource: Dict[str, Any]) -> Nodes:
         inst = cls(**resource)
         if isinstance(inst.view, dict):
             inst.view = ViewInfo(**convert_all_keys_to_snake_case(inst.view))
         return inst
 
 
-class InstanceEdges(TransformationDestination):
+class Edges(TransformationDestination):
     def __init__(
         self,
         view: Optional[ViewInfo] = None,
         instance_space: Optional[str] = None,
         edge_type: Optional[EdgeType] = None,
     ):
-        warnings.warn(
-            "Feature DataModelStorage is in beta and still in development. "
-            "Breaking changes can happen in between patch versions.",
-            stacklevel=2,
-        )
+
         super().__init__(type="edges")
         self.view = view
         self.instance_space = instance_space
         self.edge_type = edge_type
 
     @classmethod
-    def _load(cls, resource: Dict[str, Any]) -> InstanceEdges:
+    def _load(cls, resource: Dict[str, Any]) -> Edges:
         inst = cls(**resource)
         if isinstance(inst.view, dict):
             inst.view = ViewInfo(**convert_all_keys_to_snake_case(inst.view))
         if isinstance(inst.edge_type, dict):
             inst.edge_type = EdgeType(**convert_all_keys_to_snake_case(inst.edge_type))
         return inst
 
@@ -302,26 +291,26 @@
     def __init__(self, reason: str = None, created_time: Optional[int] = None):
         self.reason = reason
         self.created_time = created_time
 
 
 def _load_destination_dct(
     dct: Dict[str, Any]
-) -> Union[RawTable, InstanceNodes, InstanceEdges, SequenceRows, TransformationDestination]:
+) -> Union[RawTable, Nodes, Edges, SequenceRows, TransformationDestination]:
     """Helper function to load destination from dictionary"""
     snake_dict = convert_all_keys_to_snake_case(dct)
     destination_type = snake_dict.pop("type")
     simple = {
         "raw": RawTable,
         "sequence_rows": SequenceRows,
     }
     if destination_type in simple:
         return simple[destination_type](**snake_dict)
 
-    nested: Dict[str, Union[type[InstanceNodes], type[InstanceEdges]]] = {
-        "nodes": InstanceNodes,
-        "edges": InstanceEdges,
+    nested: Dict[str, Union[type[Nodes], type[Edges]]] = {
+        "nodes": Nodes,
+        "edges": Edges,
     }
     if destination_type in nested:
         return nested[destination_type]._load(snake_dict)
 
     return TransformationDestination(destination_type)
```

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.2.0/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/exceptions.py` & `cognite_sdk-6.2.0/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/testing.py` & `cognite_sdk-6.2.0/cognite/client/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from contextlib import contextmanager
 from typing import Any, Iterator
 from unittest.mock import MagicMock
 
 from cognite.client import CogniteClient
 from cognite.client._api.annotations import AnnotationsAPI
 from cognite.client._api.assets import AssetsAPI
+from cognite.client._api.data_modeling import DataModelingAPI
 from cognite.client._api.data_sets import DataSetsAPI
 from cognite.client._api.datapoints import DatapointsAPI
 from cognite.client._api.diagrams import DiagramsAPI
 from cognite.client._api.entity_matching import EntityMatchingAPI
 from cognite.client._api.events import EventsAPI
 from cognite.client._api.extractionpipelines import (
     ExtractionPipelineConfigsAPI,
@@ -21,14 +22,15 @@
 from cognite.client._api.functions import FunctionCallsAPI, FunctionsAPI, FunctionSchedulesAPI
 from cognite.client._api.geospatial import GeospatialAPI
 from cognite.client._api.iam import IAMAPI, GroupsAPI, SecurityCategoriesAPI, SessionsAPI, TokenAPI
 from cognite.client._api.labels import LabelsAPI
 from cognite.client._api.raw import RawAPI, RawDatabasesAPI, RawRowsAPI, RawTablesAPI
 from cognite.client._api.relationships import RelationshipsAPI
 from cognite.client._api.sequences import SequencesAPI, SequencesDataAPI
+from cognite.client._api.spaces import SpacesAPI
 from cognite.client._api.synthetic_time_series import SyntheticDatapointsAPI
 from cognite.client._api.templates import (
     TemplateGroupsAPI,
     TemplateGroupVersionsAPI,
     TemplateInstancesAPI,
     TemplatesAPI,
     TemplateViewsAPI,
@@ -66,14 +68,18 @@
         # - Please add your mocked APIs in chronological order
         # - For nested APIs:
         #   - Add spacing above and below
         #   - Use `spec=MyAPI` only for "top level"
         #   - Use `spec_set=MyNestedAPI` for all nested APIs
         self.annotations = MagicMock(spec_set=AnnotationsAPI)
         self.assets = MagicMock(spec_set=AssetsAPI)
+
+        self.data_modeling = MagicMock(spec=DataModelingAPI)
+        self.data_modeling.spaces = MagicMock(spec_set=SpacesAPI)
+
         self.data_sets = MagicMock(spec_set=DataSetsAPI)
 
         self.diagrams = MagicMock(spec_set=DiagramsAPI)
         self.entity_matching = MagicMock(spec_set=EntityMatchingAPI)
         self.events = MagicMock(spec_set=EventsAPI)
 
         self.extraction_pipelines = MagicMock(spec=ExtractionPipelinesAPI)
```

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/__init__.py` & `cognite_sdk-6.2.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.2.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.2.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_graph.py` & `cognite_sdk-6.2.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_identifier.py` & `cognite_sdk-6.2.0/cognite/client/utils/_identifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,40 @@
 from __future__ import annotations
 
 import numbers
-from typing import Dict, Generic, Iterable, List, Optional, Sequence, Tuple, TypeVar, Union, cast, overload
+from typing import (
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    NoReturn,
+    Optional,
+    Protocol,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
 
 from cognite.client._constants import MAX_VALID_INTERNAL_ID
 from cognite.client.utils._auxiliary import split_into_chunks
 
 T_ID = TypeVar("T_ID", int, str)
 
 
+class IdentifierCore(Protocol):
+    def as_dict(self, camel_case: bool = True) -> dict:
+        ...
+
+    def as_primitive(self) -> str | int:
+        ...
+
+
 class Identifier(Generic[T_ID]):
     def __init__(self, value: T_ID) -> None:
         self.__value: T_ID = value
 
     @classmethod
     def of_either(cls, id: Optional[int], external_id: Optional[str]) -> Identifier:
         if id is external_id is None:
@@ -50,40 +72,55 @@
 
     def as_dict(self, camel_case: bool = True) -> Dict[str, T_ID]:
         return {self.name(camel_case): self.__value}
 
     def as_tuple(self, camel_case: bool = True) -> Tuple[str, T_ID]:
         return self.name(camel_case), self.__value
 
-    def __str__(self) -> str:
-        return repr(self)
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({self.__value!r})"
+class DataModelingIdentifier:
+    def __init__(self, space: str, external_id: str | None = None):
+        self.__space = space
+        self.__external_id = external_id
+
+    def as_dict(self, camel_case: bool = True) -> dict[str, str]:
+        output = {"space": self.__space}
+        if self.__external_id is None:
+            return output
+        key = "externalId" if camel_case else "external_id"
+        return {**output, key: self.__external_id}
+
+    def as_primitive(self) -> NoReturn:
+        raise AttributeError(f"Not supported for {type(self).__name__} implementation")
 
 
 class ExternalId(Identifier[str]):
     ...
 
 
 class InternalId(Identifier[int]):
     ...
 
 
-class IdentifierSequence:
-    def __init__(self, identifiers: List[Identifier], is_singleton: bool) -> None:
-        if len(identifiers) == 0:
-            raise ValueError("No ids or external_ids specified")
+T_Identifier = TypeVar("T_Identifier", bound=IdentifierCore)
+
+
+class IdentifierSequenceCore(Generic[T_Identifier]):
+    _no_identifiers_error_message: str = ""
+
+    def __init__(self, identifiers: List[T_Identifier], is_singleton: bool) -> None:
+        if not identifiers:
+            raise ValueError(self._no_identifiers_error_message)
         self._identifiers = identifiers
         self.__is_singleton = is_singleton
 
     def __len__(self) -> int:
         return len(self._identifiers)
 
-    def __getitem__(self, item: int) -> Identifier:
+    def __getitem__(self, item: int) -> T_Identifier:
         return self._identifiers[item]
 
     def is_singleton(self) -> bool:
         return self.__is_singleton
 
     def assert_singleton(self) -> None:
         if not self.is_singleton():
@@ -95,35 +132,39 @@
 
     def chunked(self, chunk_size: int) -> Iterable[IdentifierSequence]:
         return [
             IdentifierSequence(chunk, is_singleton=self.is_singleton())
             for chunk in split_into_chunks(self._identifiers, chunk_size)
         ]
 
-    def as_dicts(self) -> List[Dict[str, Union[int, str]]]:
+    def as_dicts(self) -> list[dict[str, int | str]]:
         return [identifier.as_dict() for identifier in self._identifiers]
 
-    def as_primitives(self) -> List[Union[int, str]]:
+    def as_primitives(self) -> list[int | str]:
         return [identifier.as_primitive() for identifier in self._identifiers]
 
     def are_unique(self) -> bool:
         return len(self) == len(set(self.as_primitives()))
 
+
+class IdentifierSequence(IdentifierSequenceCore[Identifier]):
+    _no_identifiers_error_message = "No ids or external_ids specified"
+
     @overload
     @classmethod
     def of(cls, *ids: List[Union[int, str]]) -> IdentifierSequence:
         ...
 
     @overload
     @classmethod
     def of(cls, *ids: Union[int, str]) -> IdentifierSequence:
         ...
 
     @classmethod
-    def of(cls, *ids: Union[int, str, Sequence[Union[int, str]]]) -> IdentifierSequence:
+    def of(cls, *ids: Union[int, str, Sequence[int | str]]) -> IdentifierSequence:
         if len(ids) == 1 and isinstance(ids[0], Sequence) and not isinstance(ids[0], str):
             return cls([Identifier(val) for val in ids[0]], is_singleton=False)
         else:
             return cls([Identifier(val) for val in ids], is_singleton=len(ids) == 1)
 
     @classmethod
     def load(
@@ -158,9 +199,19 @@
                     f"{id_name}external_ids must be of type str or Sequence[str]. Found {type(external_ids)}"
                 )
 
         is_singleton = value_passed_as_primitive and len(all_identifiers) == 1
         return cls(identifiers=[Identifier(val) for val in all_identifiers], is_singleton=is_singleton)
 
 
-class SingletonIdentifierSequence(IdentifierSequence):
+class DataModelingIdentifierSequence(IdentifierSequenceCore[DataModelingIdentifier]):
+    _no_identifiers_error_message = "No spaces specified."
+
+    @classmethod
+    def load_spaces(cls, spaces: str | Sequence[str]) -> DataModelingIdentifierSequence:
+        spaces = [spaces] if isinstance(spaces, str) else spaces
+
+        return cls(identifiers=[DataModelingIdentifier(space) for space in spaces], is_singleton=len(spaces) == 1)
+
+
+class SingletonIdentifierSequence(IdentifierSequenceCore):
     ...
```

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_logging.py` & `cognite_sdk-6.2.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.2.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.2.0/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.2.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_text.py` & `cognite_sdk-6.2.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_time.py` & `cognite_sdk-6.2.0/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_validation.py` & `cognite_sdk-6.2.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.2.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.1.9/pyproject.toml` & `cognite_sdk-6.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.1.9"
+version = "6.2.0"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.1.9/PKG-INFO` & `cognite_sdk-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.1.9
+Version: 6.2.0
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.1.9 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.2.0 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

