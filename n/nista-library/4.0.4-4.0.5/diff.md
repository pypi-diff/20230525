# Comparing `tmp/nista_library-4.0.4.tar.gz` & `tmp/nista_library-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.0.4.tar", max compression
+gzip compressed data, was "nista_library-4.0.5.tar", max compression
```

## Comparing `nista_library-4.0.4.tar` & `nista_library-4.0.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1117 2023-05-24 16:12:00.355567 nista_library-4.0.4/LICENSE.md
--rw-r--r--   0        0        0     6428 2023-05-24 16:12:00.355567 nista_library-4.0.4/README.md
--rw-r--r--   0        0        0      153 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     5482 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5376 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5768 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area.py
--rw-r--r--   0        0        0     6225 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area_message.py
--rw-r--r--   0        0        0     5323 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_chiller_samples.py
--rw-r--r--   0        0        0     5441 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4789 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_area.py
--rw-r--r--   0        0        0     4473 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4478 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5168 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_message.py
--rw-r--r--   0        0        0     5472 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5005 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5326 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     8928 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     7699 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags.py
--rw-r--r--   0        0        0     4805 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags_2.py
--rw-r--r--   0        0        0     5296 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_list_areas.py
--rw-r--r--   0        0        0     5769 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_area.py
--rw-r--r--   0        0        0     5397 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5369 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     6226 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_message.py
--rw-r--r--   0        0        0     5381 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5381 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0     2817 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/client.py
--rw-r--r--   0        0        0      470 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/errors.py
--rw-r--r--   0        0        0     4795 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1965 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     1906 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     7547 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     5874 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0      779 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     3212 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0     7362 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     7281 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     7564 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      181 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2579 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     3472 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     2529 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2045 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/rule.py
--rw-r--r--   0        0        0     9273 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3058 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     2675 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     3346 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     7576 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/py.typed
--rw-r--r--   0        0        0      993 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/types.py
--rw-r--r--   0        0        0     1007 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/__init__.py
--rw-r--r--   0        0        0    11406 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_connetion.py
--rw-r--r--   0        0        0     1049 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    17582 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1970 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_data_points.py
--rw-r--r--   0        0        0     1383 2023-05-24 16:12:00.362567 nista_library-4.0.4/pyproject.toml
--rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-25 12:03:49.719800 nista_library-4.0.5/LICENSE.md
+-rw-r--r--   0        0        0     6428 2023-05-25 12:03:49.719800 nista_library-4.0.5/README.md
+-rw-r--r--   0        0        0      153 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     5482 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5376 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5768 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area.py
+-rw-r--r--   0        0        0     6225 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area_message.py
+-rw-r--r--   0        0        0     5323 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_chiller_samples.py
+-rw-r--r--   0        0        0     5441 2023-05-25 12:03:49.720800 nista_library-4.0.5/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4789 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_area.py
+-rw-r--r--   0        0        0     4473 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4478 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5168 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_message.py
+-rw-r--r--   0        0        0     5472 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5005 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5326 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0     8928 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     7699 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags.py
+-rw-r--r--   0        0        0     4805 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags_2.py
+-rw-r--r--   0        0        0     5296 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_list_areas.py
+-rw-r--r--   0        0        0     5769 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_area.py
+-rw-r--r--   0        0        0     5397 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5369 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     6226 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_message.py
+-rw-r--r--   0        0        0     5381 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5381 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0     2817 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/errors.py
+-rw-r--r--   0        0        0     4795 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1965 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     1906 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     7547 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2023-05-25 12:03:49.721800 nista_library-4.0.5/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     5874 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0      779 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     3212 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0     7362 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     7281 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     7564 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      181 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2579 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     3472 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     2529 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2045 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2023-05-25 12:03:49.722800 nista_library-4.0.5/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/rule.py
+-rw-r--r--   0        0        0     9273 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3058 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     2675 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     3346 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     7576 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/py.typed
+-rw-r--r--   0        0        0      993 2023-05-25 12:03:49.723800 nista_library-4.0.5/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    18118 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1970 2023-05-25 12:03:49.724800 nista_library-4.0.5/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0     1383 2023-05-25 12:03:49.725800 nista_library-4.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.5/PKG-INFO
```

### Comparing `nista_library-4.0.4/LICENSE.md` & `nista_library-4.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/README.md` & `nista_library-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-4.0.5/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area_message.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_chiller_samples.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_chiller_samples.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_area.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_message.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags_2.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_list_areas.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_area.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_message.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-4.0.5/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/client.py` & `nista_library-4.0.5/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/__init__.py` & `nista_library-4.0.5/data_point_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.0.5/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/append_time_series_request.py` & `nista_library-4.0.5/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/area_of_interest_response.py` & `nista_library-4.0.5/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/calculation_origin.py` & `nista_library-4.0.5/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/constant_data_bucket.py` & `nista_library-4.0.5/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/constant_data_point_data.py` & `nista_library-4.0.5/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/continuous_location_rest.py` & `nista_library-4.0.5/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/create_area_message_request.py` & `nista_library-4.0.5/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/create_area_request.py` & `nista_library-4.0.5/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_bucket_base.py` & `nista_library-4.0.5/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_export_request.py` & `nista_library-4.0.5/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_point_comment_message_response.py` & `nista_library-4.0.5/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_point_data_base.py` & `nista_library-4.0.5/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_point_data_response.py` & `nista_library-4.0.5/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_point_origin.py` & `nista_library-4.0.5/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_point_request.py` & `nista_library-4.0.5/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/data_point_response_base.py` & `nista_library-4.0.5/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.0.5/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.0.5/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.0.5/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/file_origin.py` & `nista_library-4.0.5/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/get_constant_response.py` & `nista_library-4.0.5/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/get_data_request.py` & `nista_library-4.0.5/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/get_data_response.py` & `nista_library-4.0.5/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/get_day_period_response.py` & `nista_library-4.0.5/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/get_series_response.py` & `nista_library-4.0.5/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/get_week_period_response.py` & `nista_library-4.0.5/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/gnista_unit_response.py` & `nista_library-4.0.5/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/live_data_origin.py` & `nista_library-4.0.5/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/location_rest.py` & `nista_library-4.0.5/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/point_location_rest.py` & `nista_library-4.0.5/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/problem_details.py` & `nista_library-4.0.5/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/problem_details_extensions.py` & `nista_library-4.0.5/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/remote_origin.py` & `nista_library-4.0.5/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/rule.py` & `nista_library-4.0.5/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/series_data_bucket.py` & `nista_library-4.0.5/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/series_data_point_data.py` & `nista_library-4.0.5/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/sub_series_request.py` & `nista_library-4.0.5/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/sub_series_request_values.py` & `nista_library-4.0.5/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/time_series_period.py` & `nista_library-4.0.5/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/time_series_response.py` & `nista_library-4.0.5/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/time_series_response_curve.py` & `nista_library-4.0.5/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/update_area_message_request.py` & `nista_library-4.0.5/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/update_area_request.py` & `nista_library-4.0.5/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/update_constant_data_request.py` & `nista_library-4.0.5/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/update_day_period_request.py` & `nista_library-4.0.5/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/update_time_series_request.py` & `nista_library-4.0.5/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/update_week_period_request.py` & `nista_library-4.0.5/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/week_data_transfere.py` & `nista_library-4.0.5/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.0.5/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.0.5/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/data_point_client/types.py` & `nista_library-4.0.5/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/nista_library/__init__.py` & `nista_library-4.0.5/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/nista_library/nista_connetion.py` & `nista_library-4.0.5/nista_library/nista_connetion.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/nista_library/nista_credential_manager.py` & `nista_library-4.0.5/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/nista_library/nista_data_point.py` & `nista_library-4.0.5/nista_library/nista_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 from typing import Any, List, Optional, Type, TypeVar, Union
 
 import pandas as pd
 from pandas import DataFrame
 from structlog import get_logger
 from zoneinfo import ZoneInfo
+from http import HTTPStatus
 
 from data_point_client import AuthenticatedClient
 from data_point_client.api.data_point import (
     data_point_append_execution_result_data,
     data_point_append_time_series_data,
     data_point_create_data_point,
     data_point_get_data,
@@ -61,15 +62,17 @@
     """
 
     DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
     DATE_NAME = "Date"
     VALUE_NAME = "Value"
 
     _data_point_response: Optional[DataPointResponseBase] = None
-    _store: Union[SeriesDataBucket, ConstantDataBucket, WeekPeriodDataBucket, DayPeriodDataBucket, None]
+    _store: Union[SeriesDataBucket, ConstantDataBucket, WeekPeriodDataBucket, DayPeriodDataBucket, None] = None
+
+    loaded = False
 
     @property
     def data_point_response(self) -> Optional[DataPointResponseBase]:
         """Loads and interprets the DataPoint if it has not bee loaded.
         :returns: The DataPoint Details from nista.io
         """
         if self._data_point_response is None:
@@ -157,40 +160,53 @@
             client=client,
             data_point_id=self.data_point_id,
             workspace_id=self.connection.workspace_id,
         )
 
         content_text = response_content.content.decode("utf-8")
 
+        if (
+            response_content.parsed is None
+            or response_content.status_code == HTTPStatus.NOT_FOUND
+            or response_content.status_code == HTTPStatus.FORBIDDEN
+        ):
+            self._data_point_response = None
+            self.name = None
+            self.loaded = False
+            return
+
         if isinstance(response_content.parsed, ProblemDetails):
             log.error(content_text)
             raise ValueError("Cannot load Datapoint")
 
         jscon_content = json.loads(content_text)
         data_point = DataPointResponseBase.from_dict(jscon_content)
 
         if data_point is None:
             raise ValueError("Cannot load Datapoint")
 
-        discriminator = data_point.store.discriminator
-
-        if discriminator == "ConstantDataBucket":
-            self._store = ConstantDataBucket.from_dict(jscon_content.store)
-        elif discriminator == "SeriesDataBucket":
-            self._store = SeriesDataBucket.from_dict(jscon_content.store)
-        elif discriminator == "DayPeriodDataBucket":
-            self._store = DayPeriodDataBucket.from_dict(jscon_content.store)
-        elif discriminator == "WeekPeriodDataBucket":
-            self._store = WeekPeriodDataBucket.from_dict(jscon_content.store)
+        self._store = None
+        if data_point.store is not None:
+            discriminator = data_point.store.discriminator
+
+            if discriminator == "ConstantDataBucket":
+                self._store = ConstantDataBucket.from_dict(jscon_content["store"])
+            elif discriminator == "SeriesDataBucket":
+                self._store = SeriesDataBucket.from_dict(jscon_content["store"])
+            elif discriminator == "DayPeriodDataBucket":
+                self._store = DayPeriodDataBucket.from_dict(jscon_content["store"])
+            elif discriminator == "WeekPeriodDataBucket":
+                self._store = WeekPeriodDataBucket.from_dict(jscon_content["store"])
 
-        if self._store is not None:
-            data_point.store = self._store
+            if self._store is not None:
+                data_point.store = self._store
 
         self._data_point_response = data_point
         self.name = self.data_point_response.name
+        self.loaded = True
 
     # pylint: disable=too-many-arguments
     def get_data_point_data(
         self,
         request: GetDataRequest,
         post_fix: bool = False,
         timeout: float = 30,
```

### Comparing `nista_library-4.0.4/nista_library/nista_data_points.py` & `nista_library-4.0.5/nista_library/nista_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.4/pyproject.toml` & `nista_library-4.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.0.4"
+version = "4.0.5"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
```

### Comparing `nista_library-4.0.4/PKG-INFO` & `nista_library-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nista-library
-Version: 4.0.4
+Version: 4.0.5
 Summary: A client library for accessing nista.io
 Home-page: https://nista.io
 License: MIT
 Author: Markus Hoffmann
 Author-email: markus.hoffmann@nista.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

