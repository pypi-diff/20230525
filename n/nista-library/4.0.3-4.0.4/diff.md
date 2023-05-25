# Comparing `tmp/nista_library-4.0.3.tar.gz` & `tmp/nista_library-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-4.0.3.tar", max compression
+gzip compressed data, was "nista_library-4.0.4.tar", max compression
```

## Comparing `nista_library-4.0.3.tar` & `nista_library-4.0.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1117 2023-05-24 14:17:43.509786 nista_library-4.0.3/LICENSE.md
--rw-r--r--   0        0        0     6428 2023-05-24 14:17:43.510786 nista_library-4.0.3/README.md
--rw-r--r--   0        0        0      153 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     5482 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     5376 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     5768 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area.py
--rw-r--r--   0        0        0     6225 2023-05-24 14:17:43.511786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area_message.py
--rw-r--r--   0        0        0     5323 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_chiller_samples.py
--rw-r--r--   0        0        0     5441 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     4789 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_area.py
--rw-r--r--   0        0        0     4473 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     4478 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5168 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_message.py
--rw-r--r--   0        0        0     5472 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     5005 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     5326 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     8928 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     7699 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags.py
--rw-r--r--   0        0        0     4805 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags_2.py
--rw-r--r--   0        0        0     5296 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_list_areas.py
--rw-r--r--   0        0        0     5769 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_area.py
--rw-r--r--   0        0        0     5397 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     5442 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     5518 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     5262 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     5369 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     6226 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_message.py
--rw-r--r--   0        0        0     5381 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     5381 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0     2817 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/client.py
--rw-r--r--   0        0        0      470 2023-05-24 14:17:43.512786 nista_library-4.0.3/data_point_client/errors.py
--rw-r--r--   0        0        0     4795 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1965 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     1906 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     4359 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/area_of_interest_response.py
--rw-r--r--   0        0        0     1858 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     7547 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     2597 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/continuous_location_rest.py
--rw-r--r--   0        0        0      923 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/create_area_message_request.py
--rw-r--r--   0        0        0     2319 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/create_area_request.py
--rw-r--r--   0        0        0     5874 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2702 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_comment_message_response.py
--rw-r--r--   0        0        0     2016 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0      779 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     3212 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0     7362 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     7281 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     7564 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      191 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_area_type_rest.py
--rw-r--r--   0        0        0      192 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      181 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2579 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     3472 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     2529 2023-05-24 14:17:43.513786 nista_library-4.0.3/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     1810 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/live_data_origin.py
--rw-r--r--   0        0        0      765 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/location_rest.py
--rw-r--r--   0        0        0     2045 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/point_location_rest.py
--rw-r--r--   0        0        0     3377 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1215 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/rule.py
--rw-r--r--   0        0        0     9273 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3058 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1214 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     2675 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1219 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0      923 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_area_message_request.py
--rw-r--r--   0        0        0     2674 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_area_request.py
--rw-r--r--   0        0        0     1401 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     3346 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     7576 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/py.typed
--rw-r--r--   0        0        0      993 2023-05-24 14:17:43.514786 nista_library-4.0.3/data_point_client/types.py
--rw-r--r--   0        0        0     1007 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/__init__.py
--rw-r--r--   0        0        0    11406 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_connetion.py
--rw-r--r--   0        0        0     1049 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    15802 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1997 2023-05-24 14:17:43.515786 nista_library-4.0.3/nista_library/nista_data_points.py
--rw-r--r--   0        0        0     1383 2023-05-24 14:17:43.517786 nista_library-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-05-24 16:12:00.355567 nista_library-4.0.4/LICENSE.md
+-rw-r--r--   0        0        0     6428 2023-05-24 16:12:00.355567 nista_library-4.0.4/README.md
+-rw-r--r--   0        0        0      153 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:12:00.356567 nista_library-4.0.4/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     5482 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5376 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5768 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area.py
+-rw-r--r--   0        0        0     6225 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area_message.py
+-rw-r--r--   0        0        0     5323 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_chiller_samples.py
+-rw-r--r--   0        0        0     5441 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4789 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_area.py
+-rw-r--r--   0        0        0     4473 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4478 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5168 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_message.py
+-rw-r--r--   0        0        0     5472 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5005 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5326 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0     8928 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     7699 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags.py
+-rw-r--r--   0        0        0     4805 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags_2.py
+-rw-r--r--   0        0        0     5296 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_list_areas.py
+-rw-r--r--   0        0        0     5769 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_area.py
+-rw-r--r--   0        0        0     5397 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5369 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     6226 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_message.py
+-rw-r--r--   0        0        0     5381 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5381 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0     2817 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2023-05-24 16:12:00.357567 nista_library-4.0.4/data_point_client/errors.py
+-rw-r--r--   0        0        0     4795 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1965 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     1906 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     7547 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     5874 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0      779 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     3212 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0     7362 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     7281 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     7564 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      181 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2579 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     3472 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     2529 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2023-05-24 16:12:00.358567 nista_library-4.0.4/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2045 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/rule.py
+-rw-r--r--   0        0        0     9273 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3058 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     2675 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     3346 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     7576 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/py.typed
+-rw-r--r--   0        0        0      993 2023-05-24 16:12:00.359567 nista_library-4.0.4/data_point_client/types.py
+-rw-r--r--   0        0        0     1007 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/__init__.py
+-rw-r--r--   0        0        0    11406 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0     1049 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    17582 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1970 2023-05-24 16:12:00.360567 nista_library-4.0.4/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0     1383 2023-05-24 16:12:00.362567 nista_library-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7471 1970-01-01 00:00:00.000000 nista_library-4.0.4/PKG-INFO
```

### Comparing `nista_library-4.0.3/LICENSE.md` & `nista_library-4.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/README.md` & `nista_library-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_export/data_export_create_csv_export.py` & `nista_library-4.0.4/data_point_client/api/data_export/data_export_create_csv_export.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_append_execution_result_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_append_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_area_message.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_area_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_chiller_samples.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_chiller_samples.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_create_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_area.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_delete_message.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_delete_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_point_by_version.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_get_tags_2.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_get_tags_2.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_list_areas.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_list_areas.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_area.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_area.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_constant_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_constant_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_message.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_message.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_time_series_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/api/data_point/data_point_update_week_period_data.py` & `nista_library-4.0.4/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/client.py` & `nista_library-4.0.4/data_point_client/client.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/__init__.py` & `nista_library-4.0.4/data_point_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.0.4/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/append_time_series_request.py` & `nista_library-4.0.4/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/area_of_interest_response.py` & `nista_library-4.0.4/data_point_client/models/area_of_interest_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/calculation_origin.py` & `nista_library-4.0.4/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/constant_data_bucket.py` & `nista_library-4.0.4/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/constant_data_point_data.py` & `nista_library-4.0.4/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/continuous_location_rest.py` & `nista_library-4.0.4/data_point_client/models/continuous_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/create_area_message_request.py` & `nista_library-4.0.4/data_point_client/models/create_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/create_area_request.py` & `nista_library-4.0.4/data_point_client/models/create_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_bucket_base.py` & `nista_library-4.0.4/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_export_request.py` & `nista_library-4.0.4/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_point_comment_message_response.py` & `nista_library-4.0.4/data_point_client/models/data_point_comment_message_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_point_data_base.py` & `nista_library-4.0.4/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_point_data_response.py` & `nista_library-4.0.4/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_point_origin.py` & `nista_library-4.0.4/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_point_request.py` & `nista_library-4.0.4/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/data_point_response_base.py` & `nista_library-4.0.4/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.0.4/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.0.4/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.0.4/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/file_origin.py` & `nista_library-4.0.4/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/get_constant_response.py` & `nista_library-4.0.4/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/get_data_request.py` & `nista_library-4.0.4/data_point_client/models/get_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/get_data_response.py` & `nista_library-4.0.4/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/get_day_period_response.py` & `nista_library-4.0.4/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/get_series_response.py` & `nista_library-4.0.4/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/get_week_period_response.py` & `nista_library-4.0.4/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/gnista_unit_response.py` & `nista_library-4.0.4/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/live_data_origin.py` & `nista_library-4.0.4/data_point_client/models/live_data_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/location_rest.py` & `nista_library-4.0.4/data_point_client/models/location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/point_location_rest.py` & `nista_library-4.0.4/data_point_client/models/point_location_rest.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/problem_details.py` & `nista_library-4.0.4/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/problem_details_extensions.py` & `nista_library-4.0.4/data_point_client/models/problem_details_extensions.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/remote_origin.py` & `nista_library-4.0.4/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/rule.py` & `nista_library-4.0.4/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/series_data_bucket.py` & `nista_library-4.0.4/data_point_client/models/series_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/series_data_point_data.py` & `nista_library-4.0.4/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/sub_series_request.py` & `nista_library-4.0.4/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/sub_series_request_values.py` & `nista_library-4.0.4/data_point_client/models/sub_series_request_values.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/time_series_period.py` & `nista_library-4.0.4/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/time_series_response.py` & `nista_library-4.0.4/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/time_series_response_curve.py` & `nista_library-4.0.4/data_point_client/models/time_series_response_curve.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/update_area_message_request.py` & `nista_library-4.0.4/data_point_client/models/update_area_message_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/update_area_request.py` & `nista_library-4.0.4/data_point_client/models/update_area_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/update_constant_data_request.py` & `nista_library-4.0.4/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/update_day_period_request.py` & `nista_library-4.0.4/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/update_time_series_request.py` & `nista_library-4.0.4/data_point_client/models/update_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/update_week_period_request.py` & `nista_library-4.0.4/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/week_data_transfere.py` & `nista_library-4.0.4/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.0.4/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.0.4/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/data_point_client/types.py` & `nista_library-4.0.4/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/nista_library/__init__.py` & `nista_library-4.0.4/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/nista_library/nista_connetion.py` & `nista_library-4.0.4/nista_library/nista_connetion.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/nista_library/nista_credential_manager.py` & `nista_library-4.0.4/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-4.0.3/nista_library/nista_data_point.py` & `nista_library-4.0.4/nista_library/nista_data_point.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     data_point_update_week_period_data,
 )
 from data_point_client.models import GetConstantResponse, GetSeriesResponse
 from data_point_client.models.append_execution_result_data_request import (
     AppendExecutionResultDataRequest,
 )
 from data_point_client.models.data_point_response_base import DataPointResponseBase
+from data_point_client.models.series_data_bucket import SeriesDataBucket
+from data_point_client.models.constant_data_bucket import ConstantDataBucket
+from data_point_client.models.week_period_data_bucket import WeekPeriodDataBucket
+from data_point_client.models.day_period_data_bucket import DayPeriodDataBucket
 from data_point_client.models.append_time_series_request import AppendTimeSeriesRequest
 from data_point_client.models.data_point_request import DataPointRequest
 from data_point_client.models.day_data_by_hour_transfer import DayDataByHourTransfer
 from data_point_client.models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from data_point_client.models.get_data_request import GetDataRequest
 from data_point_client.models.get_day_period_response import GetDayPeriodResponse
 from data_point_client.models.get_week_period_response import GetWeekPeriodResponse
@@ -57,65 +61,76 @@
     """
 
     DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
     DATE_NAME = "Date"
     VALUE_NAME = "Value"
 
     _data_point_response: Optional[DataPointResponseBase] = None
+    _store: Union[SeriesDataBucket, ConstantDataBucket, WeekPeriodDataBucket, DayPeriodDataBucket, None]
 
     @property
     def data_point_response(self) -> Optional[DataPointResponseBase]:
         """Loads and interprets the DataPoint if it has not bee loaded.
         :returns: The DataPoint Details from nista.io
         """
         if self._data_point_response is None:
             self._load_details()
         return self._data_point_response
 
+    @property
+    def store(self) -> Union[SeriesDataBucket, ConstantDataBucket, WeekPeriodDataBucket, DayPeriodDataBucket, None]:
+        """Loads and interprets the DataPoint if it has not bee loaded.
+        :returns: The DataPoint Details from nista.io
+        """
+        if self._store is None:
+            self._load_details()
+        return self._store
+
     @classmethod
     def create_new(
-        cls: Type[T], connection: NistaConnection, name: str, tags: List[str]
+        cls: Type[T], connection: NistaConnection, name: str, tags: List[str], new_id: Optional[str] = None
     ) -> Optional[T]:
         """Creates a new DataPoint in nista.io
         :param connection: To be used to connecto to nista.io
         :param name: The new name of the DataPoint
         :param tags: List of Tags to add to the new DataPoint
+        :param new_id: The ID to use for the datapoint
         :returns: The created DataPoint
         """
 
         token = connection.get_access_token()
         client = AuthenticatedClient(
             base_url=connection.datapoint_base_url,
             token=token,
             verify_ssl=connection.verify_ssl,
         )
 
-        new_id = uuid.uuid4()
-        request = DataPointRequest(
-            name=name, description="", existence=EnDataPointExistenceDTO.FULL, tags=tags
-        )
+        if new_id is None:
+            new_id = str(uuid.uuid4())
+
+        request = DataPointRequest(name=name, description="", existence=EnDataPointExistenceDTO.FULL, tags=tags)
 
         response = data_point_create_data_point.sync(
             client=client,
-            data_point_id=str(new_id),
+            data_point_id=new_id,
             workspace_id=connection.workspace_id,
             json_body=request,
         )
 
         if isinstance(response, ProblemDetails):
             log.error(response)
             return None
 
         data_point = cls(connection=connection, data_point_id=new_id, name=name)
         return data_point
 
     def __init__(
         self,
         connection: NistaConnection,
-        data_point_id: uuid.UUID,
+        data_point_id: str,
         name: Optional[str] = None,
     ):
         """Load a DataPoint from nista.io
         :param connection: To be used to connecto to nista.io
         :param data_point_id: The Unique ID to load the DataPoint
         :param name: Optional Name to use for this DataPoint
         """
@@ -134,39 +149,56 @@
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
         )
 
-        data_point = data_point_get_data_point.sync(
+        response_content = data_point_get_data_point.sync_detailed(
             client=client,
             data_point_id=self.data_point_id,
             workspace_id=self.connection.workspace_id,
         )
 
-        if data_point is None:
+        content_text = response_content.content.decode("utf-8")
+
+        if isinstance(response_content.parsed, ProblemDetails):
+            log.error(content_text)
             raise ValueError("Cannot load Datapoint")
 
-        if isinstance(data_point, ProblemDetails):
-            log.error(data_point)
+        jscon_content = json.loads(content_text)
+        data_point = DataPointResponseBase.from_dict(jscon_content)
+
+        if data_point is None:
             raise ValueError("Cannot load Datapoint")
 
+        discriminator = data_point.store.discriminator
+
+        if discriminator == "ConstantDataBucket":
+            self._store = ConstantDataBucket.from_dict(jscon_content.store)
+        elif discriminator == "SeriesDataBucket":
+            self._store = SeriesDataBucket.from_dict(jscon_content.store)
+        elif discriminator == "DayPeriodDataBucket":
+            self._store = DayPeriodDataBucket.from_dict(jscon_content.store)
+        elif discriminator == "WeekPeriodDataBucket":
+            self._store = WeekPeriodDataBucket.from_dict(jscon_content.store)
+
+        if self._store is not None:
+            data_point.store = self._store
+
         self._data_point_response = data_point
         self.name = self.data_point_response.name
 
     # pylint: disable=too-many-arguments
     def get_data_point_data(
         self,
         request: GetDataRequest,
         post_fix: bool = False,
         timeout: float = 30,
-    ) -> Union[
-        List[DataFrame], float, Unset, WeekDataTransfere, DayDataByHourTransfer, None
-    ]:
+    ) -> Union[List[DataFrame], float, Unset, WeekDataTransfere, DayDataByHourTransfer, None]:
         """Retrieves the Data from a DataPoint
         :param request: Request details for retrieving Data
         :param post_fix: Append nista.io instance name after DataPoint Name
         :param timeout: How long to wait for response
         :return: The DataPoint Data
         """
 
@@ -174,42 +206,44 @@
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
 
-        byte_content = data_point_get_data.sync_detailed(
+        response_content = data_point_get_data.sync_detailed(
             client=client,
             data_point_id=str(self.data_point_id),
             workspace_id=self.connection.workspace_id,
             json_body=request,
-        ).content
+        )
 
-        log.debug("Received Response from nista.io", content=byte_content)
+        content_text = response_content.content.decode("utf-8")
 
-        content_text = byte_content.decode("utf-8")
-        jscon_content = json.loads(content_text)
+        if isinstance(response_content.parsed, ProblemDetails):
+            log.error(content_text)
+            raise ValueError("Cannot load Datapoint")
 
+        log.debug("Received Response from nista.io", content=content_text)
+
+        jscon_content = json.loads(content_text)
         content_type = jscon_content["discriminator"]
 
         if content_type == "GetSeriesResponse":
             series_response = GetSeriesResponse.from_dict(jscon_content)
             curves = series_response.curves
 
             if isinstance(curves, list):
                 data_frames = []
                 # pylint: disable=E1133
                 for curve in curves:
                     # pylint: enable=E1133
                     curve_dict = curve.curve
                     if isinstance(curve_dict, TimeSeriesResponseCurve):
-                        data_frame = self._from_time_frames(
-                            time_frames=curve_dict.to_dict(), post_fix=post_fix
-                        )
+                        data_frame = self._from_time_frames(time_frames=curve_dict.to_dict(), post_fix=post_fix)
                         data_frames.append(data_frame)
 
                 return data_frames
 
         if content_type == "GetConstantResponse":
             constant_response = GetConstantResponse.from_dict(jscon_content)
             if constant_response is not None:
@@ -228,19 +262,21 @@
         return None
 
     def append_data_point_data(
         self,
         data: Union[List[DataFrame], float],
         unit: Optional[str] = None,
         timeout: float = 5.0,
+        time_zone: ZoneInfo = ZoneInfo("UTC"),
     ) -> Optional[Response[Union[Any, ProblemDetails]]]:
         """Append data to an existing DataPoint
         :param data: To be added to a DataPoint
         :param unit: The Unit to set on the DataPoint Store
         :param timeout: How long to wait for response
+        :param time_zone: The Time Zone of the newly added Data, default is UTC
         """
 
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
@@ -251,15 +287,15 @@
             sub_series: List[SubSeriesRequest] = []
             for data_frame in data:
                 data_dict = self._to_dict(data_frame)
                 value = SubSeriesRequestValues.from_dict(src_dict=data_dict)
                 request = SubSeriesRequest(values=value)
                 sub_series.append(request)
 
-            append_request = AppendTimeSeriesRequest(sub_series=sub_series, unit=unit)
+            append_request = AppendTimeSeriesRequest(sub_series=sub_series, unit=unit, time_zone=time_zone.key)
 
             return data_point_append_time_series_data.sync_detailed(
                 workspace_id=self.connection.workspace_id,
                 client=client,
                 data_point_id=str(self.data_point_id),
                 json_body=append_request,
             )
@@ -309,15 +345,15 @@
         return None
 
     def set_data_point_data(
         self,
         data: Union[List[DataFrame], float, WeekDataTransfere],
         unit: Optional[str] = None,
         execution_id: Optional[str] = None,
-        time_zone: Optional[ZoneInfo] = None,
+        time_zone: ZoneInfo = ZoneInfo("UTC"),
     ) -> Optional[Response[Union[Any, ProblemDetails]]]:
         """Replace or Set DataPoint Data with new Data. This bumps the DataPoint Version
         :param data: To be added to a DataPoint
         :param unit: The Unit to set on the DataPoint Store
         :param execution_id: the execution ID that this data is assignable to
         :param time_zone: The Time Zone of the newly added Data
         """
@@ -325,28 +361,24 @@
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
         )
 
         if isinstance(data, WeekDataTransfere):
-            week_update_request = UpdateWeekPeriodRequest(
-                execution_id=execution_id, unit=unit, week_data=data
-            )
+            week_update_request = UpdateWeekPeriodRequest(execution_id=execution_id, unit=unit, week_data=data)
             return data_point_update_week_period_data.sync_detailed(
                 workspace_id=self.connection.workspace_id,
                 client=client,
                 data_point_id=str(self.data_point_id),
                 json_body=week_update_request,
             )
 
         if isinstance(data, list):
             sub_series: List[SubSeriesRequest] = []
-            if time_zone is None:
-                time_zone = ZoneInfo("UTC")
 
             for data_frame in data:
                 data_dict = self._to_dict(data_frame)
                 value = SubSeriesRequestValues.from_dict(src_dict=data_dict)
                 request = SubSeriesRequest(values=value)
                 sub_series.append(request)
 
@@ -385,44 +417,36 @@
         dct = data_frame.to_dict()[self.VALUE_NAME]
         for key in dct.keys():
             value = dct[key]
             key_string = key.strftime(self.DATE_FORMAT)
             result[key_string] = value
         return result
 
-    def _from_time_frames(
-        self, time_frames: dict, post_fix: bool, date_format: str = DATE_FORMAT
-    ) -> DataFrame:
+    def _from_time_frames(self, time_frames: dict, post_fix: bool, date_format: str = DATE_FORMAT) -> DataFrame:
         if not isinstance(time_frames, dict):
             raise TypeError
 
         value_column_name = self.name
 
         if value_column_name is None:
             value_column_name = self.VALUE_NAME
 
         if post_fix:
-            value_column_name = (
-                value_column_name + "_nista.io_" + str(self.data_point_id)
-            )
+            value_column_name = value_column_name + "_nista.io_" + str(self.data_point_id)
 
         log.debug("Reading data as Pandas DataFrame")
 
         data_record = []
         for date in time_frames:
             value = time_frames[date]
             data_record.append({self.DATE_NAME: date, value_column_name: value})
 
-        data_frame = pd.DataFrame.from_records(
-            data_record, columns=[self.DATE_NAME, value_column_name]
-        )
+        data_frame = pd.DataFrame.from_records(data_record, columns=[self.DATE_NAME, value_column_name])
 
-        data_frame[self.DATE_NAME] = pd.to_datetime(
-            data_frame[self.DATE_NAME], format=date_format
-        )
+        data_frame[self.DATE_NAME] = pd.to_datetime(data_frame[self.DATE_NAME], format=date_format)
 
         data_frame[value_column_name] = pd.to_numeric(data_frame[value_column_name])
 
         data_frame = data_frame.set_index(data_frame[self.DATE_NAME])
         data_frame = data_frame.drop([self.DATE_NAME], axis=1)
 
         return data_frame
```

### Comparing `nista_library-4.0.3/nista_library/nista_data_points.py` & `nista_library-4.0.4/nista_library/nista_data_points.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import uuid
 from typing import Generator, List, Optional
 
 from structlog import get_logger
 
 from data_point_client import AuthenticatedClient
 from data_point_client.api.data_point import data_point_get_data_points
 from data_point_client.models import DataPointResponseBase, EnDataPointExistenceDTO, ProblemDetails
 from nista_library.nista_connetion import NistaConnection
 from nista_library.nista_data_point import NistaDataPoint
 
 log = get_logger()
 
 
 class NistaDataPoints:
-    """Represents a DataPoint List from nista.io
-    """
+    """Represents a DataPoint List from nista.io"""
+
     def __init__(self, connection: NistaConnection):
         """Create a List of DataPoints
         :param connection: To be used to connecto to nista.io
         """
 
         self.connection = connection
 
@@ -44,10 +43,10 @@
 
         for data_point in list_of_data_points:
             name: Optional[str] = None
             if isinstance(data_point.name, str):
                 name = data_point.name
 
             nista_data_point = NistaDataPoint(
-                connection=self.connection, data_point_id=uuid.UUID(data_point.data_point_id), name=name
+                connection=self.connection, data_point_id=data_point.data_point_id, name=name
             )
             yield nista_data_point
```

### Comparing `nista_library-4.0.3/pyproject.toml` & `nista_library-4.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "4.0.3"
+version = "4.0.4"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
```

### Comparing `nista_library-4.0.3/PKG-INFO` & `nista_library-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nista-library
-Version: 4.0.3
+Version: 4.0.4
 Summary: A client library for accessing nista.io
 Home-page: https://nista.io
 License: MIT
 Author: Markus Hoffmann
 Author-email: markus.hoffmann@nista.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

