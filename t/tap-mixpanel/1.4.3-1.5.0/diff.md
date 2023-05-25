# Comparing `tmp/tap-mixpanel-1.4.3.tar.gz` & `tmp/tap-mixpanel-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-mixpanel-1.4.3.tar", last modified: Thu May 18 11:02:27 2023, max compression
+gzip compressed data, was "dist/tap-mixpanel-1.5.0.tar", last modified: Thu May 25 00:50:09 2023, max compression
```

## Comparing `tap-mixpanel-1.4.3.tar` & `tap-mixpanel-1.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tests/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tests/tap_tester/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7571 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2505 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7470 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_all_fields_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_bookmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tests/tap_tester/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15519 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/tap_tester/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tests/unittests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4296 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4819 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7646 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_support_eu_endpoints.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3438 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_request_timeout_param_value.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_transform_event_times.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5065 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tests/unittests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1717 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_attribution_window.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11184 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_error_handling.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3709 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tests/unittests/test_discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      727 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/LICENSE
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1400 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-05-18 11:02:26.000000 tap-mixpanel-1.4.3/tap_mixpanel.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12637 2023-05-03 05:08:09.000000 tap-mixpanel-1.4.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tap_mixpanel/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5161 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12294 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-18 11:02:27.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/export.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/cohort_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/funnels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/engage.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      510 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/cohorts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/revenue.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2022-10-10 07:35:16.000000 tap-mixpanel-1.4.3/tap_mixpanel/schemas/annotations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34143 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7134 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3548 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-05-18 11:02:07.000000 tap-mixpanel-1.4.3/tap_mixpanel/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tests/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tests/tap_tester/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8083 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2505 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8220 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7496 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_all_fields_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tests/tap_tester/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15708 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tests/tap_tester/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tests/unittests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4296 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4819 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7646 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_support_eu_endpoints.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3438 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_request_timeout_param_value.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_transform_event_times.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5065 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tests/unittests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1717 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_attribution_window.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11184 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_error_handling.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3709 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tests/unittests/test_discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      146 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      727 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/LICENSE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1400 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12936 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5161 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12294 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 00:50:09.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      603 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/export.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/cohort_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/funnels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      139 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/engage.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      510 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/cohorts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      449 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/revenue.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2022-10-10 07:35:16.000000 tap-mixpanel-1.5.0/tap_mixpanel/schemas/annotations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34637 2023-05-25 00:45:30.000000 tap-mixpanel-1.5.0/tap_mixpanel/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7134 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3548 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2023-05-18 11:02:07.000000 tap-mixpanel-1.5.0/tap_mixpanel/discover.py
```

### Comparing `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_start_date.py` & `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_start_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,65 +109,68 @@
 
                 primary_keys_sync_1 = set(primary_keys_list_1)
                 primary_keys_sync_2 = set(primary_keys_list_2)
 
                 if expected_metadata.get(self.OBEYS_START_DATE):
 
                     # Collect information specific to incremental streams from syncs 1 & 2
-                    expected_replication_key = next(
-                        iter(self.expected_replication_keys().get(stream, []))
-                    )
-                    replication_dates_1 = [
-                        row.get("data").get(expected_replication_key)
-                        for row in synced_records_1.get(stream, {"messages": []}).get(
-                            "messages", []
+                    if expected_metadata.get(self.REPLICATION_METHOD) == "INCREMENTAL":
+                        expected_replication_key = next(
+                            iter(self.expected_replication_keys().get(stream, []))
                         )
-                        if row.get("data")
-                    ]
-                    replication_dates_2 = [
-                        row.get("data").get(expected_replication_key)
-                        for row in synced_records_2.get(stream, {"messages": []}).get(
-                            "messages", []
-                        )
-                        if row.get("data")
-                    ]
-
-                    # Verify replication key is greater or equal to start_date for sync 1
-                    for replication_date in replication_dates_1:
-                        self.assertGreaterEqual(
-                            self.parse_date(replication_date),
-                            self.parse_date(expected_start_date_1),
-                            msg="Report pertains to a date prior to our start date.\n"
-                            + f"Sync start_date: {expected_start_date_1}\n"
-                            + f"Record date: {replication_date} ",
-                        )
-
-                    # Verify replication key is greater or equal to start_date for sync 2
-                    for replication_date in replication_dates_2:
-                        self.assertGreaterEqual(
-                            self.parse_date(replication_date),
-                            self.parse_date(expected_start_date_2),
-                            msg="Report pertains to a date prior to our start date.\n"
-                            + f"Sync start_date: {expected_start_date_2}\n"
-                            + f"Record date: {replication_date} ",
-                        )
-
-                    # Verify the number of records replicated in sync 1 is greater than the number
-                    # of records replicated in sync 2
-                    self.assertGreater(record_count_sync_1, record_count_sync_2)
-
-                    # Verify the records replicated in sync 2 were also replicated in sync 1
-                    self.assertTrue(primary_keys_sync_2.issubset(primary_keys_sync_1))
-
-                else:
-
-                    # Verify that the 2nd sync with a later start date replicates the same number of
-                    # records as the 1st sync.
-                    self.assertEqual(record_count_sync_2, record_count_sync_1)
+                        replication_dates_1 = [
+                            row.get("data").get(expected_replication_key)
+                            for row in synced_records_1.get(stream, {"messages": []}).get(
+                                "messages", []
+                            )
+                            if row.get("data")
+                        ]
+                        replication_dates_2 = [
+                            row.get("data").get(expected_replication_key)
+                            for row in synced_records_2.get(stream, {"messages": []}).get(
+                                "messages", []
+                            )
+                            if row.get("data")
+                        ]
+
+                        # Verify replication key is greater or equal to start_date for sync 1
+                        for replication_date in replication_dates_1:
+                            self.assertGreaterEqual(
+                                self.parse_date(replication_date),
+                                self.parse_date(expected_start_date_1),
+                                msg="Report pertains to a date prior to our start date.\n"
+                                + f"Sync start_date: {expected_start_date_1}\n"
+                                + f"Record date: {replication_date} ",
+                            )
+
+                        # Verify replication key is greater or equal to start_date for sync 2
+                        for replication_date in replication_dates_2:
+                            self.assertGreaterEqual(
+                                self.parse_date(replication_date),
+                                self.parse_date(expected_start_date_2),
+                                msg="Report pertains to a date prior to our start date.\n"
+                                + f"Sync start_date: {expected_start_date_2}\n"
+                                + f"Record date: {replication_date} ",
+                            )
+
+                        # Verify the number of records replicated in sync 1 is greater than
+                        # the number of records replicated in sync 2
+                        self.assertGreater(record_count_sync_1, record_count_sync_2)
+
+                        # Verify the records replicated in sync 2 were also replicated in sync 1
+                        self.assertTrue(primary_keys_sync_2.issubset(primary_keys_sync_1))
+
+                    else:
+                        # Verify that the 2nd sync with a later start date replicates the less or
+                        # same number of records as the 1st sync.
+                        # Since all the streams obey start_date it is expected that
+                        # second sync for full table streams
+                        # would have less or same number of records as the first sync.
+                        self.assertLessEqual(record_count_sync_2, record_count_sync_1)
 
-                    # Verify by primary key the same records are replicated in the 1st and 2nd syncs
-                    self.assertSetEqual(primary_keys_sync_1, primary_keys_sync_2)
+                        # Verify the records replicated in sync 2 were also replicated in sync 1
+                        self.assertTrue(primary_keys_sync_2.issubset(primary_keys_sync_1))
 
     def test_run(self):
         # Start date test for standard server
         self.eu_residency = False
         self.start_date_test_run()
```

### Comparing `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_automatic_fields.py` & `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_automatic_fields.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_discovery.py` & `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_all_fields_pagination.py` & `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_all_fields_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 self.assertTrue(expected_automatic_keys.issubset(
                     expected_all_keys), msg=f'{expected_automatic_keys-expected_all_keys} is not in "expected_all_keys"')
 
                 # As we can't find the below fields in the docs and also
                 # it won't be generated by mixpanel APIs now so expected.
                 if stream == "export":
                     expected_all_keys = expected_all_keys - {'labels', 'sampling_factor', 'dataset', 'mp_reserved_duration_s', 'mp_reserved_origin_end',
-                                                             'mp_reserved_origin_start', 'mp_reserved_event_count'}
+                                                             'mp_reserved_origin_start', 'mp_reserved_event_count', 'mp_reserved_event_name'}
 
                 # Verify all fields for each stream are replicated
                 # Skip engage as it return records in random manner with dynamic fields.
                 if not stream == "engage":
                     self.assertSetEqual(expected_all_keys, actual_all_keys)
 
         # Pagination Test
```

### Comparing `tap-mixpanel-1.4.3/tests/tap_tester/test_mixpanel_bookmark.py` & `tap-mixpanel-1.5.0/tests/tap_tester/test_mixpanel_bookmark.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/tap_tester/base.py` & `tap-mixpanel-1.5.0/tests/tap_tester/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     FULL_TABLE = "FULL_TABLE"
     API_LIMIT = 250
     TYPE = "platform.mixpanel"
     OBEYS_START_DATE = "obey-start-date"
     start_date = ""
     end_date = ""
     eu_residency = True
+    export_events = os.getenv("TAP_MIXPANEL_EXPORT_EVENTS")
 
     def tap_name(self):
         """The name of the tap."""
         return "tap-mixpanel"
 
     def expected_metadata(self):
         """The expected streams and metadata about the streams."""
@@ -42,42 +43,42 @@
                 self.REPLICATION_METHOD: self.INCREMENTAL,
                 self.REPLICATION_KEYS: {"time"},
                 self.OBEYS_START_DATE: True,
             },
             "engage": {
                 self.PRIMARY_KEYS: {"distinct_id"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
-                self.OBEYS_START_DATE: False,
+                self.OBEYS_START_DATE: True,
             },
             "funnels": {
                 self.PRIMARY_KEYS: {"funnel_id", "date"},
                 self.REPLICATION_METHOD: self.INCREMENTAL,
                 self.REPLICATION_KEYS: {"datetime"},
                 self.OBEYS_START_DATE: True,
             },
             "cohorts": {
                 self.PRIMARY_KEYS: {"id"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
-                self.OBEYS_START_DATE: False,
+                self.OBEYS_START_DATE: True,
             },
             "cohort_members": {
                 self.PRIMARY_KEYS: {"cohort_id", "distinct_id"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
-                self.OBEYS_START_DATE: False,
+                self.OBEYS_START_DATE: True,
             },
             "revenue": {
                 self.PRIMARY_KEYS: {"date"},
                 self.REPLICATION_METHOD: self.INCREMENTAL,
                 self.REPLICATION_KEYS: {"datetime"},
                 self.OBEYS_START_DATE: True,
             },
             "annotations": {
                 self.PRIMARY_KEYS: {"date"},
                 self.REPLICATION_METHOD: self.FULL_TABLE,
-                self.OBEYS_START_DATE: False,
+                self.OBEYS_START_DATE: True,
             },
         }
 
     def setUp(self):
         missing_envs = []
         if self.eu_residency:
             creds = {"api_secret": "TAP_MIXPANEL_EU_RESIDENCY_API_SECRET"}
@@ -97,27 +98,32 @@
         """The expected url route ending."""
         return "platform.mixpanel"
 
     def get_properties(self, original: bool = True):
         """Configuration properties required for the tap."""
 
         return_value = {
-            "start_date": "2020-02-01T00:00:00Z",
-            "end_date": "2020-03-01T00:00:00Z",
+            "start_date": "2023-04-18T00:00:00Z",
+            "end_date": "2023-05-23T00:00:00Z",
             "date_window_size": "30",
             "attribution_window": "5",
             "project_timezone": "US/Pacific",
             "eu_residency": "false",
             "select_properties_by_default": "false",
         }
         if self.eu_residency:
             return_value.update(
                 {"project_timezone": "Europe/Amsterdam", "eu_residency": "true"}
             )
 
+        if self.export_events:
+            return_value.update(
+                {"export_events": self.export_events}
+            )
+
         if original:
             return return_value
 
         return_value["start_date"] = self.start_date
         return return_value
 
     def get_start_date(self):
```

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_main.py` & `tap-mixpanel-1.5.0/tests/unittests/test_main.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_sync.py` & `tap-mixpanel-1.5.0/tests/unittests/test_sync.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_transform.py` & `tap-mixpanel-1.5.0/tests/unittests/test_transform.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_support_eu_endpoints.py` & `tap-mixpanel-1.5.0/tests/unittests/test_support_eu_endpoints.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_request_timeout_param_value.py` & `tap-mixpanel-1.5.0/tests/unittests/test_request_timeout_param_value.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_transform_event_times.py` & `tap-mixpanel-1.5.0/tests/unittests/test_transform_event_times.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_client.py` & `tap-mixpanel-1.5.0/tests/unittests/test_client.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_attribution_window.py` & `tap-mixpanel-1.5.0/tests/unittests/test_attribution_window.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_error_handling.py` & `tap-mixpanel-1.5.0/tests/unittests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tests/unittests/test_discover.py` & `tap-mixpanel-1.5.0/tests/unittests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/setup.py` & `tap-mixpanel-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-mixpanel',
-      version='1.4.3',
+      version='1.5.0',
       description='Singer.io tap for extracting data from the mixpanel API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mixpanel'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-mixpanel-1.4.3/LICENSE` & `tap-mixpanel-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel.egg-info/SOURCES.txt` & `tap-mixpanel-1.5.0/tap_mixpanel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/README.md` & `tap-mixpanel-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 - Standard Server endpoint: https://data.mixpanel.com/api/2.0/export
 - EU Residency Server endpoint: https://data-eu.mixpanel.com/api/2.0/export
 - Primary key fields: `event`, `time`, `distinct_id`
 - Replication strategy: INCREMENTAL (query filtered)
   - Bookmark: `time`
   - Bookmark query field: `from_date`, `to_date`
 - Transformations: De-nest `properties` to root-level, re-name properties with leading `$...` to `mp_reserved_...`, convert datetimes from project timezone to UTC.
+- Optional parameters
+  - `export_events` to export only certain events
 
 **[engage](https://developer.mixpanel.com/docs/data-export-api#section-engage)**
   - Standard Server endpoint: https://mixpanel.com/api/2.0/engage
   - EU Residency Server endpoint: https://eu.mixpanel.com/api/2.0/engage
 - Primary key fields:  `distinct_id`
 - Replication strategy: FULL_TABLE (all records, every load)
 - Transformations: De-nest `$properties` to root-level, re-name properties with leading `$...` to `mp_reserved_...`.
@@ -150,14 +152,20 @@
         "start_date": "2019-01-01T00:00:00Z",
         "user_agent": "tap-mixpanel <api_user_email@your_company.com>",
         "eu_residency_server": "true",
         "request_timeout": 300
     }
     ```
     
+      If you want to export only certain events from the [Raw export API](https://developer.mixpanel.com/reference/export)then provide the value of `export_events`
+
+    ```bash
+   "export_events": "event_one,event_two"
+   ```
+
     Optionally, also create a `state.json` file. `currently_syncing` is an optional attribute used for identifying the last object to be synced in case the job is interrupted mid-stream. The next run would begin where the last job left off.
 
     ```json
     {
         "currently_syncing": "engage",
         "bookmarks": {
             "export": "2019-09-27T22:34:39.000000Z",
```

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/transform.py` & `tap-mixpanel-1.5.0/tap_mixpanel/transform.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/client.py` & `tap-mixpanel-1.5.0/tap_mixpanel/client.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/schemas/export.json` & `tap-mixpanel-1.5.0/tap_mixpanel/schemas/export.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/schemas/funnels.json` & `tap-mixpanel-1.5.0/tap_mixpanel/schemas/funnels.json`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/streams.py` & `tap-mixpanel-1.5.0/tap_mixpanel/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module defines the stream classes and their individual sync logic."""
 
 import json
 import math
 from copy import deepcopy
 from datetime import datetime, timedelta
 
+import urllib
 import pytz
 import singer
 from singer import Transformer, metadata, metrics, utils
 from singer.utils import strptime_to_utc
 
 from tap_mixpanel.client import MixpanelClient
 from tap_mixpanel.transform import transform_datetime, transform_record
@@ -423,14 +424,15 @@
             int: Returns total number of records.
         """
 
         bookmark_field = next(iter(self.replication_keys), None)
         project_timezone = config.get("project_timezone", "UTC")
         days_interval = int(config.get("date_window_size", "30"))
         attribution_window = int(config.get("attribution_window", "5"))
+        export_events = config.get('export_events')
 
         # Update url if eu_residency is selected
         if str(config.get("eu_residency")).lower() == "true":
             if self.tap_stream_id == "export":
                 self.url = "https://data-eu.mixpanel.com/api/2.0"
             else:
                 self.url = "https://eu.mixpanel.com/api/2.0"
@@ -528,14 +530,22 @@
 
                     # querystring: Squash query params into string and replace [parent_id]
                     querystring = "&".join(
                         [f"{key}={value}" for (key, value) in params.items()]
                     )
                     querystring = querystring.replace("[parent_id]", str(parent_id))
 
+                    # To fetch specific event date add event from config if given
+                    if self.tap_stream_id == 'export' and export_events:
+                        event = json.dumps(
+                            list(map(str.strip, export_events.split(',')))
+                        )
+                        url_encoded = urllib.parse.quote(event)
+                        querystring += f'&event={url_encoded}'
+
                     full_url = f"{self.url}/{self.path}{f'?{querystring}' if querystring else ''}"
 
                     LOGGER.info("URL for Stream %s: %s", self.tap_stream_id, full_url)
 
                     (
                         parent_total,
                         date_total,
```

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/schema.py` & `tap-mixpanel-1.5.0/tap_mixpanel/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/__init__.py` & `tap-mixpanel-1.5.0/tap_mixpanel/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/sync.py` & `tap-mixpanel-1.5.0/tap_mixpanel/sync.py`

 * *Files identical despite different names*

### Comparing `tap-mixpanel-1.4.3/tap_mixpanel/discover.py` & `tap-mixpanel-1.5.0/tap_mixpanel/discover.py`

 * *Files identical despite different names*

