# Comparing `tmp/google-cloud-monitoring-2.9.1.tar.gz` & `tmp/google-cloud-monitoring-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-monitoring-2.9.1.tar", last modified: Mon Mar  7 16:02:21 2022, max compression
+gzip compressed data, was "google-cloud-monitoring-2.9.2.tar", last modified: Thu Jun  9 14:52:02 2022, max compression
```

## Comparing `google-cloud-monitoring-2.9.1.tar` & `google-cloud-monitoring-2.9.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.643210 google-cloud-monitoring-2.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3918 2022-03-07 16:02:21.643210 google-cloud-monitoring-2.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3071 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.619198 google-cloud-monitoring-2.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.619198 google-cloud-monitoring-2.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.619198 google-cloud-monitoring-2.9.1/google/cloud/monitoring/
--rw-rw-r--   0 root         (0)     1003    13787 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring/__init__.py
--rw-rw-r--   0 root         (0)     1003       84 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.623200 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/
--rw-rw-r--   0 root         (0)     1003    10409 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/__init__.py
--rw-rw-r--   0 root         (0)     1003     5568 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/_dataframe.py
--rw-rw-r--   0 root         (0)     1003    15390 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       84 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/py.typed
--rw-rw-r--   0 root         (0)     1003    22393 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/query.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.623200 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.623200 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/
--rw-rw-r--   0 root         (0)     1003      785 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    34200 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    43082 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     5976 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.623200 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8757 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16985 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17378 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.623200 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    39067 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    46961 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/client.py
--rw-rw-r--   0 root         (0)     1003    10914 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.627202 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9844 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17630 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18049 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.627202 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/
--rw-rw-r--   0 root         (0)     1003      765 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    51892 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    61387 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/client.py
--rw-rw-r--   0 root         (0)     1003    16999 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.627202 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12206 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    23055 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23544 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.627202 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/
--rw-rw-r--   0 root         (0)     1003      817 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    58175 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    67531 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/client.py
--rw-rw-r--   0 root         (0)     1003    12160 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.627202 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/
--rw-rw-r--   0 root         (0)     1003     1310 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13649 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26713 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    27211 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.631204 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    12391 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    20529 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/client.py
--rw-rw-r--   0 root         (0)     1003     5960 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.631204 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     5900 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11777 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12057 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.631204 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/
--rw-rw-r--   0 root         (0)     1003      809 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    52224 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    61313 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/client.py
--rw-rw-r--   0 root         (0)     1003    11329 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.631204 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/
--rw-rw-r--   0 root         (0)     1003     1292 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12340 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22884 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23411 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.631204 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/
--rw-rw-r--   0 root         (0)     1003      785 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    34404 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42856 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/client.py
--rw-rw-r--   0 root         (0)     1003    11361 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.635206 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/
--rw-rw-r--   0 root         (0)     1003     1238 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9883 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18941 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19369 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.635206 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/
--rw-rw-r--   0 root         (0)     1003     6743 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    29955 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/alert.py
--rw-rw-r--   0 root         (0)     1003     8586 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/alert_service.py
--rw-rw-r--   0 root         (0)     1003    14568 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/common.py
--rw-rw-r--   0 root         (0)     1003     2015 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/dropped_labels.py
--rw-rw-r--   0 root         (0)     1003     3827 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/group.py
--rw-rw-r--   0 root         (0)     1003    10015 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/group_service.py
--rw-rw-r--   0 root         (0)     1003    14245 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/metric.py
--rw-rw-r--   0 root         (0)     1003    20096 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/metric_service.py
--rw-rw-r--   0 root         (0)     1003     1296 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/mutation_record.py
--rw-rw-r--   0 root         (0)     1003     9994 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/notification.py
--rw-rw-r--   0 root         (0)     1003    14341 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/notification_service.py
--rw-rw-r--   0 root         (0)     1003      725 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/query_service.py
--rw-rw-r--   0 root         (0)     1003    30071 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/service.py
--rw-rw-r--   0 root         (0)     1003    12417 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/service_service.py
--rw-rw-r--   0 root         (0)     1003     1704 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/span_context.py
--rw-rw-r--   0 root         (0)     1003    20084 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/uptime.py
--rw-rw-r--   0 root         (0)     1003     8596 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/uptime_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/
--rw-r--r--   0 root         (0)     1003     3918 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     6368 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      116 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-03-07 16:02:21.000000 google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/scripts/
--rw-rw-r--   0 root         (0)     1003     9171 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/scripts/fixup_monitoring_v3_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-03-07 16:02:21.643210 google-cloud-monitoring-2.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2934 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/tests/system/
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.619198 google-cloud-monitoring-2.9.1/tests/system/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/tests/system/gapic/v3/
--rw-rw-r--   0 root         (0)     1003      974 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/system/gapic/v3/test_system_metric_service_v3.py
--rw-rw-r--   0 root         (0)     1003    27762 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/system/test_vpcsc_v3.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.639208 google-cloud-monitoring-2.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:02:21.643210 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/__init__.py
--rw-rw-r--   0 root         (0)     1003   100729 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_alert_policy_service.py
--rw-rw-r--   0 root         (0)     1003   108267 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_group_service.py
--rw-rw-r--   0 root         (0)     1003   153132 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_metric_service.py
--rw-rw-r--   0 root         (0)     1003   164318 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_notification_channel_service.py
--rw-rw-r--   0 root         (0)     1003    58346 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_query_service.py
--rw-rw-r--   0 root         (0)     1003   150772 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_service_monitoring_service.py
--rw-rw-r--   0 root         (0)     1003   111895 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_uptime_check_service.py
--rw-rw-r--   0 root         (0)     1003     8414 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/test__dataframe.py
--rw-rw-r--   0 root         (0)     1003    20466 2022-03-07 15:59:41.000000 google-cloud-monitoring-2.9.1/tests/unit/test_query.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.534159 google-cloud-monitoring-2.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3916 2022-06-09 14:52:02.534159 google-cloud-monitoring-2.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3071 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.510171 google-cloud-monitoring-2.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.510171 google-cloud-monitoring-2.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.514169 google-cloud-monitoring-2.9.2/google/cloud/monitoring/
+-rw-rw-r--   0 root         (0)     1003    13787 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring/__init__.py
+-rw-rw-r--   0 root         (0)     1003       84 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.514169 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/
+-rw-rw-r--   0 root         (0)     1003    10409 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5568 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/_dataframe.py
+-rw-rw-r--   0 root         (0)     1003    15390 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       84 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/py.typed
+-rw-rw-r--   0 root         (0)     1003    22393 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/query.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.514169 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.518167 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/
+-rw-rw-r--   0 root         (0)     1003      785 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34596 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43631 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5976 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.518167 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8903 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17040 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17378 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.518167 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39574 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    47600 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10914 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.518167 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9958 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17685 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18049 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.518167 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/
+-rw-rw-r--   0 root         (0)     1003      765 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    52609 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62171 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16999 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.518167 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12320 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23110 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23544 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.522165 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/
+-rw-rw-r--   0 root         (0)     1003      817 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58953 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    68437 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/client.py
+-rw-rw-r--   0 root         (0)     1003    12160 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.522165 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1310 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13731 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26768 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    27211 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.522165 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12510 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    20809 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5960 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.522165 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6014 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11832 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12057 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.522165 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/
+-rw-rw-r--   0 root         (0)     1003      809 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    53011 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62144 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11329 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.526163 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1292 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12486 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22939 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23411 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.526163 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/
+-rw-rw-r--   0 root         (0)     1003      785 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34909 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43457 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11361 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.526163 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1238 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9965 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18996 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19369 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/
+-rw-rw-r--   0 root         (0)     1003     6788 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    31161 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/alert.py
+-rw-rw-r--   0 root         (0)     1003     8898 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/alert_service.py
+-rw-rw-r--   0 root         (0)     1003    14870 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/common.py
+-rw-rw-r--   0 root         (0)     1003     2013 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/dropped_labels.py
+-rw-rw-r--   0 root         (0)     1003     3961 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/group.py
+-rw-rw-r--   0 root         (0)     1003    10593 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/group_service.py
+-rw-rw-r--   0 root         (0)     1003    15035 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/metric.py
+-rw-rw-r--   0 root         (0)     1003    21190 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/metric_service.py
+-rw-rw-r--   0 root         (0)     1003     1366 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/mutation_record.py
+-rw-rw-r--   0 root         (0)     1003    10288 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/notification.py
+-rw-rw-r--   0 root         (0)     1003    14943 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/notification_service.py
+-rw-rw-r--   0 root         (0)     1003      735 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/query_service.py
+-rw-rw-r--   0 root         (0)     1003    31574 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/service.py
+-rw-rw-r--   0 root         (0)     1003    13015 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/service_service.py
+-rw-rw-r--   0 root         (0)     1003     1750 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/span_context.py
+-rw-rw-r--   0 root         (0)     1003    21016 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/uptime.py
+-rw-rw-r--   0 root         (0)     1003     8918 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/uptime_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/
+-rw-r--r--   0 root         (0)     1003     3916 2022-06-09 14:52:01.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6368 2022-06-09 14:52:02.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-06-09 14:52:01.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-06-09 14:52:02.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-06-09 14:52:01.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      153 2022-06-09 14:52:02.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-06-09 14:52:02.000000 google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/scripts/
+-rw-rw-r--   0 root         (0)     1003     9171 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/scripts/fixup_monitoring_v3_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-06-09 14:52:02.534159 google-cloud-monitoring-2.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2982 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/tests/system/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.514169 google-cloud-monitoring-2.9.2/tests/system/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/tests/system/gapic/v3/
+-rw-rw-r--   0 root         (0)     1003      974 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/system/gapic/v3/test_system_metric_service_v3.py
+-rw-rw-r--   0 root         (0)     1003    27762 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/system/test_vpcsc_v3.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.530161 google-cloud-monitoring-2.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-09 14:52:02.534159 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103524 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_alert_policy_service.py
+-rw-rw-r--   0 root         (0)     1003   112942 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_group_service.py
+-rw-rw-r--   0 root         (0)     1003   157382 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_metric_service.py
+-rw-rw-r--   0 root         (0)     1003   167627 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_notification_channel_service.py
+-rw-rw-r--   0 root         (0)     1003    60609 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_query_service.py
+-rw-rw-r--   0 root         (0)     1003   155099 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_service_monitoring_service.py
+-rw-rw-r--   0 root         (0)     1003   114946 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_uptime_check_service.py
+-rw-rw-r--   0 root         (0)     1003     8414 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/test__dataframe.py
+-rw-rw-r--   0 root         (0)     1003    20465 2022-06-09 14:49:21.000000 google-cloud-monitoring-2.9.2/tests/unit/test_query.py
```

### Comparing `google-cloud-monitoring-2.9.1/LICENSE` & `google-cloud-monitoring-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/MANIFEST.in` & `google-cloud-monitoring-2.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/PKG-INFO` & `google-cloud-monitoring-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-monitoring
-Version: 2.9.1
+Version: 2.9.2
 Summary: Stackdriver Monitoring API client library
 Home-page: https://github.com/googleapis/python-monitoring
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -109,9 +109,7 @@
 ~~~~~~~~~~
 
 
 -  Read the `Client Library Documentation`_ for Cloud Monitoring API
    to see other available methods on the client.
 -  Read the `Product documentation`_ to learn more about the product and see
    How-to Guides.
-
-
```

### Comparing `google-cloud-monitoring-2.9.1/README.rst` & `google-cloud-monitoring-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/_dataframe.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/_dataframe.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/gapic_metadata.json` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/query.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/query.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -233,33 +233,32 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAlertPoliciesAsyncPager:
         r"""Lists the existing alerting policies for the
         workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_alert_policies():
+            async def sample_list_alert_policies():
                 # Create a client
-                client = monitoring_v3.AlertPolicyServiceClient()
+                client = monitoring_v3.AlertPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListAlertPoliciesRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_alert_policies(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListAlertPoliciesRequest, dict]):
                 The request object. The protocol for the
                 `ListAlertPolicies` request.
             name (:class:`str`):
@@ -331,20 +330,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListAlertPoliciesAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_alert_policy(
         self,
@@ -357,25 +364,25 @@
     ) -> alert.AlertPolicy:
         r"""Gets a single alerting policy.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_alert_policy():
+            async def sample_get_alert_policy():
                 # Create a client
-                client = monitoring_v3.AlertPolicyServiceClient()
+                client = monitoring_v3.AlertPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetAlertPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_alert_policy(request=request)
+                response = await client.get_alert_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetAlertPolicyRequest, dict]):
                 The request object. The protocol for the
@@ -443,15 +450,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def create_alert_policy(
         self,
         request: Union[alert_service.CreateAlertPolicyRequest, dict] = None,
@@ -464,25 +476,25 @@
     ) -> alert.AlertPolicy:
         r"""Creates a new alerting policy.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_alert_policy():
+            async def sample_create_alert_policy():
                 # Create a client
-                client = monitoring_v3.AlertPolicyServiceClient()
+                client = monitoring_v3.AlertPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateAlertPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.create_alert_policy(request=request)
+                response = await client.create_alert_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateAlertPolicyRequest, dict]):
                 The request object. The protocol for the
@@ -563,15 +575,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_alert_policy(
         self,
         request: Union[alert_service.DeleteAlertPolicyRequest, dict] = None,
@@ -583,25 +600,25 @@
     ) -> None:
         r"""Deletes an alerting policy.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_alert_policy():
+            async def sample_delete_alert_policy():
                 # Create a client
-                client = monitoring_v3.AlertPolicyServiceClient()
+                client = monitoring_v3.AlertPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteAlertPolicyRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_alert_policy(request=request)
+                await client.delete_alert_policy(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteAlertPolicyRequest, dict]):
                 The request object. The protocol for the
                 `DeleteAlertPolicy` request.
             name (:class:`str`):
                 Required. The alerting policy to delete. The format is:
@@ -660,15 +677,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def update_alert_policy(
         self,
         request: Union[alert_service.UpdateAlertPolicyRequest, dict] = None,
         *,
         update_mask: field_mask_pb2.FieldMask = None,
@@ -678,29 +698,28 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> alert.AlertPolicy:
         r"""Updates an alerting policy. You can either replace the entire
         policy with a new one or replace only certain fields in the
         current alerting policy by specifying the fields to be updated
         via ``updateMask``. Returns the updated alerting policy.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_update_alert_policy():
+            async def sample_update_alert_policy():
                 # Create a client
-                client = monitoring_v3.AlertPolicyServiceClient()
+                client = monitoring_v3.AlertPolicyServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.UpdateAlertPolicyRequest(
                 )
 
                 # Make the request
-                response = client.update_alert_policy(request=request)
+                response = await client.update_alert_policy(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.UpdateAlertPolicyRequest, dict]):
                 The request object. The protocol for the
@@ -794,15 +813,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("alert_policy.name", request.alert_policy.name),)
             ),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -57,15 +57,16 @@
     _transport_registry = (
         OrderedDict()
     )  # type: Dict[str, Type[AlertPolicyServiceTransport]]
     _transport_registry["grpc"] = AlertPolicyServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = AlertPolicyServiceGrpcAsyncIOTransport
 
     def get_transport_class(
-        cls, label: str = None,
+        cls,
+        label: str = None,
     ) -> Type[AlertPolicyServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -172,97 +173,123 @@
         Returns:
             AlertPolicyServiceTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def alert_policy_path(project: str, alert_policy: str,) -> str:
+    def alert_policy_path(
+        project: str,
+        alert_policy: str,
+    ) -> str:
         """Returns a fully-qualified alert_policy string."""
         return "projects/{project}/alertPolicies/{alert_policy}".format(
-            project=project, alert_policy=alert_policy,
+            project=project,
+            alert_policy=alert_policy,
         )
 
     @staticmethod
     def parse_alert_policy_path(path: str) -> Dict[str, str]:
         """Parses a alert_policy path into its component segments."""
         m = re.match(
             r"^projects/(?P<project>.+?)/alertPolicies/(?P<alert_policy>.+?)$", path
         )
         return m.groupdict() if m else {}
 
     @staticmethod
     def alert_policy_condition_path(
-        project: str, alert_policy: str, condition: str,
+        project: str,
+        alert_policy: str,
+        condition: str,
     ) -> str:
         """Returns a fully-qualified alert_policy_condition string."""
         return "projects/{project}/alertPolicies/{alert_policy}/conditions/{condition}".format(
-            project=project, alert_policy=alert_policy, condition=condition,
+            project=project,
+            alert_policy=alert_policy,
+            condition=condition,
         )
 
     @staticmethod
     def parse_alert_policy_condition_path(path: str) -> Dict[str, str]:
         """Parses a alert_policy_condition path into its component segments."""
         m = re.match(
             r"^projects/(?P<project>.+?)/alertPolicies/(?P<alert_policy>.+?)/conditions/(?P<condition>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -440,15 +467,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListAlertPoliciesPager:
         r"""Lists the existing alerting policies for the
         workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_alert_policies():
                 # Create a client
                 client = monitoring_v3.AlertPolicyServiceClient()
@@ -529,20 +555,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListAlertPoliciesPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_alert_policy(
         self,
@@ -632,15 +666,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def create_alert_policy(
         self,
         request: Union[alert_service.CreateAlertPolicyRequest, dict] = None,
@@ -752,15 +791,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_alert_policy(
         self,
         request: Union[alert_service.DeleteAlertPolicyRequest, dict] = None,
@@ -840,15 +884,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def update_alert_policy(
         self,
         request: Union[alert_service.UpdateAlertPolicyRequest, dict] = None,
         *,
         update_mask: field_mask_pb2.FieldMask = None,
@@ -858,15 +905,14 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> alert.AlertPolicy:
         r"""Updates an alerting policy. You can either replace the entire
         policy with a new one or replace only certain fields in the
         current alerting policy by specifying the fields to be updated
         via ``updateMask``. Returns the updated alerting policy.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_update_alert_policy():
                 # Create a client
                 client = monitoring_v3.AlertPolicyServiceClient()
@@ -974,15 +1020,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("alert_policy.name", request.alert_policy.name),)
             ),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def __enter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -151,15 +152,17 @@
                     ),
                     deadline=30.0,
                 ),
                 default_timeout=30.0,
                 client_info=client_info,
             ),
             self.create_alert_policy: gapic_v1.method.wrap_method(
-                self.create_alert_policy, default_timeout=30.0, client_info=client_info,
+                self.create_alert_policy,
+                default_timeout=30.0,
+                client_info=client_info,
             ),
             self.delete_alert_policy: gapic_v1.method.wrap_method(
                 self.delete_alert_policy,
                 default_retry=retries.Retry(
                     initial=0.1,
                     maximum=30.0,
                     multiplier=1.3,
@@ -168,24 +171,26 @@
                     ),
                     deadline=30.0,
                 ),
                 default_timeout=30.0,
                 client_info=client_info,
             ),
             self.update_alert_policy: gapic_v1.method.wrap_method(
-                self.update_alert_policy, default_timeout=30.0, client_info=client_info,
+                self.update_alert_policy,
+                default_timeout=30.0,
+                client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def list_alert_policies(
         self,
     ) -> Callable[
@@ -229,9 +234,13 @@
         self,
     ) -> Callable[
         [alert_service.UpdateAlertPolicyRequest],
         Union[alert.AlertPolicy, Awaitable[alert.AlertPolicy]],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("AlertPolicyServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,16 +230,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def list_alert_policies(
         self,
     ) -> Callable[
         [alert_service.ListAlertPoliciesRequest],
@@ -374,9 +373,13 @@
                 response_deserializer=alert.AlertPolicy.deserialize,
             )
         return self._stubs["update_alert_policy"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("AlertPolicyServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/alert_policy_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -224,29 +224,29 @@
     ) -> pagers.ListGroupsAsyncPager:
         r"""Lists the existing groups.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_groups():
+            async def sample_list_groups():
                 # Create a client
-                client = monitoring_v3.GroupServiceClient()
+                client = monitoring_v3.GroupServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListGroupsRequest(
                     children_of_group="children_of_group_value",
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_groups(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListGroupsRequest, dict]):
                 The request object. The `ListGroup` request.
             name (:class:`str`):
                 Required. The
@@ -311,20 +311,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListGroupsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_group(
         self,
@@ -337,25 +345,25 @@
     ) -> group.Group:
         r"""Gets a single group.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_group():
+            async def sample_get_group():
                 # Create a client
-                client = monitoring_v3.GroupServiceClient()
+                client = monitoring_v3.GroupServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetGroupRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_group(request=request)
+                response = await client.get_group(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetGroupRequest, dict]):
                 The request object. The `GetGroup` request.
@@ -449,15 +457,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def create_group(
         self,
         request: Union[group_service.CreateGroupRequest, dict] = None,
@@ -470,25 +483,25 @@
     ) -> gm_group.Group:
         r"""Creates a new group.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_group():
+            async def sample_create_group():
                 # Create a client
-                client = monitoring_v3.GroupServiceClient()
+                client = monitoring_v3.GroupServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateGroupRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.create_group(request=request)
+                response = await client.create_group(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateGroupRequest, dict]):
                 The request object. The `CreateGroup` request.
@@ -584,15 +597,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def update_group(
         self,
         request: Union[group_service.UpdateGroupRequest, dict] = None,
@@ -601,29 +619,28 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gm_group.Group:
         r"""Updates an existing group. You can change any group attributes
         except ``name``.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_update_group():
+            async def sample_update_group():
                 # Create a client
-                client = monitoring_v3.GroupServiceClient()
+                client = monitoring_v3.GroupServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.UpdateGroupRequest(
                 )
 
                 # Make the request
-                response = client.update_group(request=request)
+                response = await client.update_group(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.UpdateGroupRequest, dict]):
                 The request object. The `UpdateGroup` request.
@@ -717,15 +734,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("group.name", request.group.name),)
             ),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_group(
         self,
         request: Union[group_service.DeleteGroupRequest, dict] = None,
@@ -737,25 +759,25 @@
     ) -> None:
         r"""Deletes an existing group.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_group():
+            async def sample_delete_group():
                 # Create a client
-                client = monitoring_v3.GroupServiceClient()
+                client = monitoring_v3.GroupServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteGroupRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_group(request=request)
+                await client.delete_group(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteGroupRequest, dict]):
                 The request object. The `DeleteGroup` request. The
                 default behavior is to be able to delete a single group
                 without any descendants.
             name (:class:`str`):
@@ -812,48 +834,50 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def list_group_members(
         self,
         request: Union[group_service.ListGroupMembersRequest, dict] = None,
         *,
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListGroupMembersAsyncPager:
         r"""Lists the monitored resources that are members of a
         group.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_group_members():
+            async def sample_list_group_members():
                 # Create a client
-                client = monitoring_v3.GroupServiceClient()
+                client = monitoring_v3.GroupServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListGroupMembersRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_group_members(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListGroupMembersRequest, dict]):
                 The request object. The `ListGroupMembers` request.
             name (:class:`str`):
                 Required. The group whose members are listed. The format
@@ -917,20 +941,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListGroupMembersAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -52,15 +52,18 @@
     objects.
     """
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[GroupServiceTransport]]
     _transport_registry["grpc"] = GroupServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = GroupServiceGrpcAsyncIOTransport
 
-    def get_transport_class(cls, label: str = None,) -> Type[GroupServiceTransport]:
+    def get_transport_class(
+        cls,
+        label: str = None,
+    ) -> Type[GroupServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
         Returns:
@@ -169,75 +172,99 @@
         Returns:
             GroupServiceTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def group_path(project: str, group: str,) -> str:
+    def group_path(
+        project: str,
+        group: str,
+    ) -> str:
         """Returns a fully-qualified group string."""
-        return "projects/{project}/groups/{group}".format(project=project, group=group,)
+        return "projects/{project}/groups/{group}".format(
+            project=project,
+            group=group,
+        )
 
     @staticmethod
     def parse_group_path(path: str) -> Dict[str, str]:
         """Parses a group path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/groups/(?P<group>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -496,20 +523,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListGroupsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_group(
         self,
@@ -625,15 +660,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def create_group(
         self,
         request: Union[group_service.CreateGroupRequest, dict] = None,
@@ -760,15 +800,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def update_group(
         self,
         request: Union[group_service.UpdateGroupRequest, dict] = None,
@@ -777,15 +822,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gm_group.Group:
         r"""Updates an existing group. You can change any group attributes
         except ``name``.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_update_group():
                 # Create a client
                 client = monitoring_v3.GroupServiceClient()
@@ -884,15 +928,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("group.name", request.group.name),)
             ),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_group(
         self,
         request: Union[group_service.DeleteGroupRequest, dict] = None,
@@ -970,30 +1019,32 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def list_group_members(
         self,
         request: Union[group_service.ListGroupMembersRequest, dict] = None,
         *,
         name: str = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListGroupMembersPager:
         r"""Lists the monitored resources that are members of a
         group.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_group_members():
                 # Create a client
                 client = monitoring_v3.GroupServiceClient()
@@ -1066,20 +1117,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListGroupMembersPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def __enter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -152,15 +153,17 @@
                     ),
                     deadline=30.0,
                 ),
                 default_timeout=30.0,
                 client_info=client_info,
             ),
             self.create_group: gapic_v1.method.wrap_method(
-                self.create_group, default_timeout=30.0, client_info=client_info,
+                self.create_group,
+                default_timeout=30.0,
+                client_info=client_info,
             ),
             self.update_group: gapic_v1.method.wrap_method(
                 self.update_group,
                 default_retry=retries.Retry(
                     initial=0.1,
                     maximum=30.0,
                     multiplier=1.3,
@@ -201,17 +204,17 @@
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def list_groups(
         self,
     ) -> Callable[
@@ -266,9 +269,13 @@
         Union[
             group_service.ListGroupMembersResponse,
             Awaitable[group_service.ListGroupMembersResponse],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("GroupServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,16 +234,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def list_groups(
         self,
     ) -> Callable[[group_service.ListGroupsRequest], group_service.ListGroupsResponse]:
         r"""Return a callable for the list groups method over gRPC.
@@ -399,9 +398,13 @@
                 response_deserializer=group_service.ListGroupMembersResponse.deserialize,
             )
         return self._stubs["list_group_members"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("GroupServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/group_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/group_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/async_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -228,33 +228,32 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListMonitoredResourceDescriptorsAsyncPager:
         r"""Lists monitored resource descriptors that match a
         filter. This method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_monitored_resource_descriptors():
+            async def sample_list_monitored_resource_descriptors():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListMonitoredResourceDescriptorsRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_monitored_resource_descriptors(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListMonitoredResourceDescriptorsRequest, dict]):
                 The request object. The
                 `ListMonitoredResourceDescriptors` request.
             name (:class:`str`):
@@ -320,20 +319,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListMonitoredResourceDescriptorsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_monitored_resource_descriptor(
         self,
@@ -345,30 +352,29 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> monitored_resource_pb2.MonitoredResourceDescriptor:
         r"""Gets a single monitored resource descriptor. This
         method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_monitored_resource_descriptor():
+            async def sample_get_monitored_resource_descriptor():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetMonitoredResourceDescriptorRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_monitored_resource_descriptor(request=request)
+                response = await client.get_monitored_resource_descriptor(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetMonitoredResourceDescriptorRequest, dict]):
                 The request object. The `GetMonitoredResourceDescriptor`
@@ -445,15 +451,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def list_metric_descriptors(
         self,
         request: Union[metric_service.ListMetricDescriptorsRequest, dict] = None,
@@ -462,33 +473,32 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListMetricDescriptorsAsyncPager:
         r"""Lists metric descriptors that match a filter. This
         method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_metric_descriptors():
+            async def sample_list_metric_descriptors():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListMetricDescriptorsRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_metric_descriptors(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListMetricDescriptorsRequest, dict]):
                 The request object. The `ListMetricDescriptors` request.
             name (:class:`str`):
                 Required. The
@@ -553,20 +563,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListMetricDescriptorsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_metric_descriptor(
         self,
@@ -576,30 +594,29 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> metric_pb2.MetricDescriptor:
         r"""Gets a single metric descriptor. This method does not
         require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_metric_descriptor():
+            async def sample_get_metric_descriptor():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetMetricDescriptorRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_metric_descriptor(request=request)
+                response = await client.get_metric_descriptor(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetMetricDescriptorRequest, dict]):
                 The request object. The `GetMetricDescriptor` request.
@@ -669,15 +686,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def create_metric_descriptor(
         self,
         request: Union[metric_service.CreateMetricDescriptorRequest, dict] = None,
@@ -690,30 +712,29 @@
     ) -> metric_pb2.MetricDescriptor:
         r"""Creates a new metric descriptor. The creation is executed
         asynchronously and callers may check the returned operation to
         track its progress. User-created metric descriptors define
         `custom
         metrics <https://cloud.google.com/monitoring/custom-metrics>`__.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_metric_descriptor():
+            async def sample_create_metric_descriptor():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateMetricDescriptorRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.create_metric_descriptor(request=request)
+                response = await client.create_metric_descriptor(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateMetricDescriptorRequest, dict]):
                 The request object. The `CreateMetricDescriptor`
@@ -780,15 +801,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_metric_descriptor(
         self,
         request: Union[metric_service.DeleteMetricDescriptorRequest, dict] = None,
@@ -798,30 +824,29 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a metric descriptor. Only user-created `custom
         metrics <https://cloud.google.com/monitoring/custom-metrics>`__
         can be deleted.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_metric_descriptor():
+            async def sample_delete_metric_descriptor():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteMetricDescriptorRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_metric_descriptor(request=request)
+                await client.delete_metric_descriptor(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteMetricDescriptorRequest, dict]):
                 The request object. The `DeleteMetricDescriptor`
                 request.
             name (:class:`str`):
                 Required. The metric descriptor on which to execute the
@@ -881,15 +906,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def list_time_series(
         self,
         request: Union[metric_service.ListTimeSeriesRequest, dict] = None,
         *,
         name: str = None,
@@ -899,35 +927,34 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListTimeSeriesAsyncPager:
         r"""Lists time series that match a filter. This method
         does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_time_series():
+            async def sample_list_time_series():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListTimeSeriesRequest(
                     name="name_value",
                     filter="filter_value",
                     view="HEADERS",
                 )
 
                 # Make the request
                 page_result = client.list_time_series(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListTimeSeriesRequest, dict]):
                 The request object. The `ListTimeSeries` request.
             name (:class:`str`):
                 Required. The
@@ -1034,20 +1061,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListTimeSeriesAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def create_time_series(
         self,
@@ -1061,30 +1096,29 @@
     ) -> None:
         r"""Creates or adds data to one or more time series.
         The response is empty if all time series in the request
         were written. If any time series could not be written, a
         corresponding failure message is included in the error
         response.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_time_series():
+            async def sample_create_time_series():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateTimeSeriesRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.create_time_series(request=request)
+                await client.create_time_series(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateTimeSeriesRequest, dict]):
                 The request object. The `CreateTimeSeries` request.
             name (:class:`str`):
                 Required. The
                 `project <https://cloud.google.com/monitoring/api/v3#project_name>`__
@@ -1149,15 +1183,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def create_service_time_series(
         self,
         request: Union[metric_service.CreateTimeSeriesRequest, dict] = None,
         *,
         name: str = None,
@@ -1172,30 +1209,29 @@
         request were written. If any time series could not be written, a
         corresponding failure message is included in the error response.
         This endpoint rejects writes to user-defined metrics. This
         method is only for use by Google Cloud services. Use
         [projects.timeSeries.create][google.monitoring.v3.MetricService.CreateTimeSeries]
         instead.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_service_time_series():
+            async def sample_create_service_time_series():
                 # Create a client
-                client = monitoring_v3.MetricServiceClient()
+                client = monitoring_v3.MetricServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateTimeSeriesRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.create_service_time_series(request=request)
+                await client.create_service_time_series(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateTimeSeriesRequest, dict]):
                 The request object. The `CreateTimeSeries` request.
             name (:class:`str`):
                 Required. The
                 `project <https://cloud.google.com/monitoring/api/v3#project_name>`__
@@ -1260,15 +1296,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -55,15 +55,18 @@
     objects.
     """
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[MetricServiceTransport]]
     _transport_registry["grpc"] = MetricServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = MetricServiceGrpcAsyncIOTransport
 
-    def get_transport_class(cls, label: str = None,) -> Type[MetricServiceTransport]:
+    def get_transport_class(
+        cls,
+        label: str = None,
+    ) -> Type[MetricServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
         Returns:
@@ -174,15 +177,16 @@
     def parse_metric_descriptor_path(path: str) -> Dict[str,str]:
         """Parses a metric_descriptor path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/metricDescriptors/(?P<metric_descriptor>.+?)$", path)
         return m.groupdict() if m else {}'''
 
     @staticmethod
     def monitored_resource_descriptor_path(
-        project: str, monitored_resource_descriptor: str,
+        project: str,
+        monitored_resource_descriptor: str,
     ) -> str:
         """Returns a fully-qualified monitored_resource_descriptor string."""
         return "projects/{project}/monitoredResourceDescriptors/{monitored_resource_descriptor}".format(
             project=project,
             monitored_resource_descriptor=monitored_resource_descriptor,
         )
 
@@ -192,79 +196,101 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/monitoredResourceDescriptors/(?P<monitored_resource_descriptor>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def time_series_path(project: str, time_series: str,) -> str:
+    def time_series_path(
+        project: str,
+        time_series: str,
+    ) -> str:
         """Returns a fully-qualified time_series string."""
         return "projects/{project}/timeSeries/{time_series}".format(
-            project=project, time_series=time_series,
+            project=project,
+            time_series=time_series,
         )
 
     @staticmethod
     def parse_time_series_path(path: str) -> Dict[str, str]:
         """Parses a time_series path into its component segments."""
         m = re.match(
             r"^projects/(?P<project>.+?)/timeSeries/(?P<time_series>.+?)$", path
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -444,15 +470,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListMonitoredResourceDescriptorsPager:
         r"""Lists monitored resource descriptors that match a
         filter. This method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_monitored_resource_descriptors():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -531,20 +556,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListMonitoredResourceDescriptorsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_monitored_resource_descriptor(
         self,
@@ -556,15 +589,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> monitored_resource_pb2.MonitoredResourceDescriptor:
         r"""Gets a single monitored resource descriptor. This
         method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_get_monitored_resource_descriptor():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -651,15 +683,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def list_metric_descriptors(
         self,
         request: Union[metric_service.ListMetricDescriptorsRequest, dict] = None,
@@ -668,15 +705,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListMetricDescriptorsPager:
         r"""Lists metric descriptors that match a filter. This
         method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_metric_descriptors():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -750,20 +786,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListMetricDescriptorsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_metric_descriptor(
         self,
@@ -773,15 +817,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> metric_pb2.MetricDescriptor:
         r"""Gets a single metric descriptor. This method does not
         require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_get_metric_descriptor():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -857,15 +900,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def create_metric_descriptor(
         self,
         request: Union[metric_service.CreateMetricDescriptorRequest, dict] = None,
@@ -878,15 +926,14 @@
     ) -> metric_pb2.MetricDescriptor:
         r"""Creates a new metric descriptor. The creation is executed
         asynchronously and callers may check the returned operation to
         track its progress. User-created metric descriptors define
         `custom
         metrics <https://cloud.google.com/monitoring/custom-metrics>`__.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_create_metric_descriptor():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -968,15 +1015,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_metric_descriptor(
         self,
         request: Union[metric_service.DeleteMetricDescriptorRequest, dict] = None,
@@ -986,15 +1038,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes a metric descriptor. Only user-created `custom
         metrics <https://cloud.google.com/monitoring/custom-metrics>`__
         can be deleted.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_delete_metric_descriptor():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -1060,15 +1111,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def list_time_series(
         self,
         request: Union[metric_service.ListTimeSeriesRequest, dict] = None,
         *,
         name: str = None,
@@ -1078,15 +1132,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListTimeSeriesPager:
         r"""Lists time series that match a filter. This method
         does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_time_series():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -1204,20 +1257,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListTimeSeriesPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def create_time_series(
         self,
@@ -1231,15 +1292,14 @@
     ) -> None:
         r"""Creates or adds data to one or more time series.
         The response is empty if all time series in the request
         were written. If any time series could not be written, a
         corresponding failure message is included in the error
         response.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_create_time_series():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -1319,15 +1379,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def create_service_time_series(
         self,
         request: Union[metric_service.CreateTimeSeriesRequest, dict] = None,
         *,
         name: str = None,
@@ -1342,15 +1405,14 @@
         request were written. If any time series could not be written, a
         corresponding failure message is included in the error response.
         This endpoint rejects writes to user-defined metrics. This
         method is only for use by Google Cloud services. Use
         [projects.timeSeries.create][google.monitoring.v3.MetricService.CreateTimeSeries]
         instead.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_create_service_time_series():
                 # Create a client
                 client = monitoring_v3.MetricServiceClient()
@@ -1432,15 +1494,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -214,29 +215,31 @@
                     ),
                     deadline=90.0,
                 ),
                 default_timeout=90.0,
                 client_info=client_info,
             ),
             self.create_time_series: gapic_v1.method.wrap_method(
-                self.create_time_series, default_timeout=12.0, client_info=client_info,
+                self.create_time_series,
+                default_timeout=12.0,
+                client_info=client_info,
             ),
             self.create_service_time_series: gapic_v1.method.wrap_method(
                 self.create_service_time_series,
                 default_timeout=None,
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def list_monitored_resource_descriptors(
         self,
     ) -> Callable[
@@ -325,9 +328,13 @@
         self,
     ) -> Callable[
         [metric_service.CreateTimeSeriesRequest],
         Union[empty_pb2.Empty, Awaitable[empty_pb2.Empty]],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("MetricServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,16 +224,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def list_monitored_resource_descriptors(
         self,
     ) -> Callable[
         [metric_service.ListMonitoredResourceDescriptorsRequest],
@@ -509,9 +508,13 @@
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["create_service_time_series"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("MetricServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/metric_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/metric_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -240,33 +240,32 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationChannelDescriptorsAsyncPager:
         r"""Lists the descriptors for supported channel types.
         The use of descriptors makes it possible for new channel
         types to be dynamically added.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_notification_channel_descriptors():
+            async def sample_list_notification_channel_descriptors():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListNotificationChannelDescriptorsRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_notification_channel_descriptors(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListNotificationChannelDescriptorsRequest, dict]):
                 The request object. The
                 `ListNotificationChannelDescriptors` request.
             name (:class:`str`):
@@ -342,20 +341,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListNotificationChannelDescriptorsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_notification_channel_descriptor(
         self,
@@ -368,30 +375,29 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannelDescriptor:
         r"""Gets a single channel descriptor. The descriptor
         indicates which fields are expected / permitted for a
         notification channel of the given type.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_notification_channel_descriptor():
+            async def sample_get_notification_channel_descriptor():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetNotificationChannelDescriptorRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_notification_channel_descriptor(request=request)
+                response = await client.get_notification_channel_descriptor(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetNotificationChannelDescriptorRequest, dict]):
                 The request object. The
@@ -459,15 +465,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def list_notification_channels(
         self,
         request: Union[
@@ -478,33 +489,32 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationChannelsAsyncPager:
         r"""Lists the notification channels that have been
         created for the project.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_notification_channels():
+            async def sample_list_notification_channels():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListNotificationChannelsRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 page_result = client.list_notification_channels(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListNotificationChannelsRequest, dict]):
                 The request object. The `ListNotificationChannels`
                 request.
             name (:class:`str`):
@@ -577,20 +587,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListNotificationChannelsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_notification_channel(
         self,
@@ -605,30 +623,29 @@
         includes the relevant configuration details with which
         the channel was created. However, the response may
         truncate or omit passwords, API keys, or other private
         key matter and thus the response may not be 100%
         identical to the information that was supplied in the
         call to the create method.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_notification_channel():
+            async def sample_get_notification_channel():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetNotificationChannelRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_notification_channel(request=request)
+                response = await client.get_notification_channel(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetNotificationChannelRequest, dict]):
                 The request object. The `GetNotificationChannel`
@@ -698,15 +715,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def create_notification_channel(
         self,
         request: Union[
@@ -719,30 +741,29 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannel:
         r"""Creates a new notification channel, representing a
         single notification endpoint such as an email address,
         SMS number, or PagerDuty service.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_notification_channel():
+            async def sample_create_notification_channel():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateNotificationChannelRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.create_notification_channel(request=request)
+                response = await client.create_notification_channel(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateNotificationChannelRequest, dict]):
                 The request object. The `CreateNotificationChannel`
@@ -820,15 +841,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def update_notification_channel(
         self,
         request: Union[
@@ -840,29 +866,28 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannel:
         r"""Updates a notification channel. Fields not specified
         in the field mask remain unchanged.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_update_notification_channel():
+            async def sample_update_notification_channel():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.UpdateNotificationChannelRequest(
                 )
 
                 # Make the request
-                response = client.update_notification_channel(request=request)
+                response = await client.update_notification_channel(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.UpdateNotificationChannelRequest, dict]):
                 The request object. The `UpdateNotificationChannel`
@@ -931,15 +956,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("notification_channel.name", request.notification_channel.name),)
             ),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_notification_channel(
         self,
         request: Union[
@@ -954,25 +984,25 @@
     ) -> None:
         r"""Deletes a notification channel.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_notification_channel():
+            async def sample_delete_notification_channel():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteNotificationChannelRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_notification_channel(request=request)
+                await client.delete_notification_channel(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteNotificationChannelRequest, dict]):
                 The request object. The `DeleteNotificationChannel`
                 request.
             name (:class:`str`):
                 Required. The channel for which to execute the request.
@@ -1044,15 +1074,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def send_notification_channel_verification_code(
         self,
         request: Union[
             notification_service.SendNotificationChannelVerificationCodeRequest, dict
         ] = None,
@@ -1062,30 +1095,29 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Causes a verification code to be delivered to the channel. The
         code can then be supplied in ``VerifyNotificationChannel`` to
         verify the channel.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_send_notification_channel_verification_code():
+            async def sample_send_notification_channel_verification_code():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.SendNotificationChannelVerificationCodeRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.send_notification_channel_verification_code(request=request)
+                await client.send_notification_channel_verification_code(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.SendNotificationChannelVerificationCodeRequest, dict]):
                 The request object. The
                 `SendNotificationChannelVerificationCode` request.
             name (:class:`str`):
                 Required. The notification channel to
@@ -1131,15 +1163,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def get_notification_channel_verification_code(
         self,
         request: Union[
             notification_service.GetNotificationChannelVerificationCodeRequest, dict
         ] = None,
@@ -1174,30 +1209,29 @@
         via
         SendNotificationChannelVerificationCode() will be
         shorter and also have a shorter expiration (e.g. codes
         such as "G-123456") whereas GetVerificationCode() will
         typically return a much longer, websafe base 64 encoded
         string that has a longer expiration time.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_notification_channel_verification_code():
+            async def sample_get_notification_channel_verification_code():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetNotificationChannelVerificationCodeRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_notification_channel_verification_code(request=request)
+                response = await client.get_notification_channel_verification_code(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetNotificationChannelVerificationCodeRequest, dict]):
                 The request object. The
@@ -1262,15 +1296,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def verify_notification_channel(
         self,
         request: Union[
@@ -1283,31 +1322,30 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannel:
         r"""Verifies a ``NotificationChannel`` by proving receipt of the
         code delivered to the channel as a result of calling
         ``SendNotificationChannelVerificationCode``.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_verify_notification_channel():
+            async def sample_verify_notification_channel():
                 # Create a client
-                client = monitoring_v3.NotificationChannelServiceClient()
+                client = monitoring_v3.NotificationChannelServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.VerifyNotificationChannelRequest(
                     name="name_value",
                     code="code_value",
                 )
 
                 # Make the request
-                response = client.verify_notification_channel(request=request)
+                response = await client.verify_notification_channel(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.VerifyNotificationChannelRequest, dict]):
                 The request object. The `VerifyNotificationChannel`
@@ -1389,15 +1427,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -60,15 +60,16 @@
     _transport_registry = (
         OrderedDict()
     )  # type: Dict[str, Type[NotificationChannelServiceTransport]]
     _transport_registry["grpc"] = NotificationChannelServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = NotificationChannelServiceGrpcAsyncIOTransport
 
     def get_transport_class(
-        cls, label: str = None,
+        cls,
+        label: str = None,
     ) -> Type[NotificationChannelServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -168,98 +169,122 @@
         Returns:
             NotificationChannelServiceTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def notification_channel_path(project: str, notification_channel: str,) -> str:
+    def notification_channel_path(
+        project: str,
+        notification_channel: str,
+    ) -> str:
         """Returns a fully-qualified notification_channel string."""
         return "projects/{project}/notificationChannels/{notification_channel}".format(
-            project=project, notification_channel=notification_channel,
+            project=project,
+            notification_channel=notification_channel,
         )
 
     @staticmethod
     def parse_notification_channel_path(path: str) -> Dict[str, str]:
         """Parses a notification_channel path into its component segments."""
         m = re.match(
             r"^projects/(?P<project>.+?)/notificationChannels/(?P<notification_channel>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
     def notification_channel_descriptor_path(
-        project: str, channel_descriptor: str,
+        project: str,
+        channel_descriptor: str,
     ) -> str:
         """Returns a fully-qualified notification_channel_descriptor string."""
         return "projects/{project}/notificationChannelDescriptors/{channel_descriptor}".format(
-            project=project, channel_descriptor=channel_descriptor,
+            project=project,
+            channel_descriptor=channel_descriptor,
         )
 
     @staticmethod
     def parse_notification_channel_descriptor_path(path: str) -> Dict[str, str]:
         """Parses a notification_channel_descriptor path into its component segments."""
         m = re.match(
             r"^projects/(?P<project>.+?)/notificationChannelDescriptors/(?P<channel_descriptor>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -440,15 +465,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationChannelDescriptorsPager:
         r"""Lists the descriptors for supported channel types.
         The use of descriptors makes it possible for new channel
         types to be dynamically added.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_notification_channel_descriptors():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -537,20 +561,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListNotificationChannelDescriptorsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_notification_channel_descriptor(
         self,
@@ -563,15 +595,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannelDescriptor:
         r"""Gets a single channel descriptor. The descriptor
         indicates which fields are expected / permitted for a
         notification channel of the given type.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_get_notification_channel_descriptor():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -651,15 +682,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def list_notification_channels(
         self,
         request: Union[
@@ -670,15 +706,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListNotificationChannelsPager:
         r"""Lists the notification channels that have been
         created for the project.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_notification_channels():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -764,20 +799,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListNotificationChannelsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_notification_channel(
         self,
@@ -792,15 +835,14 @@
         includes the relevant configuration details with which
         the channel was created. However, the response may
         truncate or omit passwords, API keys, or other private
         key matter and thus the response may not be 100%
         identical to the information that was supplied in the
         call to the create method.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_get_notification_channel():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -876,15 +918,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def create_notification_channel(
         self,
         request: Union[
@@ -897,15 +944,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannel:
         r"""Creates a new notification channel, representing a
         single notification endpoint such as an email address,
         SMS number, or PagerDuty service.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_create_notification_channel():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -1002,15 +1048,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def update_notification_channel(
         self,
         request: Union[
@@ -1022,15 +1073,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannel:
         r"""Updates a notification channel. Fields not specified
         in the field mask remain unchanged.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_update_notification_channel():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -1117,15 +1167,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("notification_channel.name", request.notification_channel.name),)
             ),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_notification_channel(
         self,
         request: Union[
@@ -1225,15 +1280,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def send_notification_channel_verification_code(
         self,
         request: Union[
             notification_service.SendNotificationChannelVerificationCodeRequest, dict
         ] = None,
@@ -1243,15 +1301,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Causes a verification code to be delivered to the channel. The
         code can then be supplied in ``VerifyNotificationChannel`` to
         verify the channel.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_send_notification_channel_verification_code():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -1294,16 +1351,18 @@
         # Minor optimization to avoid making a copy if the user passes
         # in a notification_service.SendNotificationChannelVerificationCodeRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(
             request, notification_service.SendNotificationChannelVerificationCodeRequest
         ):
-            request = notification_service.SendNotificationChannelVerificationCodeRequest(
-                request
+            request = (
+                notification_service.SendNotificationChannelVerificationCodeRequest(
+                    request
+                )
             )
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
@@ -1316,15 +1375,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def get_notification_channel_verification_code(
         self,
         request: Union[
             notification_service.GetNotificationChannelVerificationCodeRequest, dict
         ] = None,
@@ -1359,15 +1421,14 @@
         via
         SendNotificationChannelVerificationCode() will be
         shorter and also have a shorter expiration (e.g. codes
         such as "G-123456") whereas GetVerificationCode() will
         typically return a much longer, websafe base 64 encoded
         string that has a longer expiration time.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_get_notification_channel_verification_code():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -1421,16 +1482,18 @@
         # Minor optimization to avoid making a copy if the user passes
         # in a notification_service.GetNotificationChannelVerificationCodeRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(
             request, notification_service.GetNotificationChannelVerificationCodeRequest
         ):
-            request = notification_service.GetNotificationChannelVerificationCodeRequest(
-                request
+            request = (
+                notification_service.GetNotificationChannelVerificationCodeRequest(
+                    request
+                )
             )
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
@@ -1442,15 +1505,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def verify_notification_channel(
         self,
         request: Union[
@@ -1463,15 +1531,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> notification.NotificationChannel:
         r"""Verifies a ``NotificationChannel`` by proving receipt of the
         code delivered to the channel as a result of calling
         ``SendNotificationChannelVerificationCode``.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_verify_notification_channel():
                 # Create a client
                 client = monitoring_v3.NotificationChannelServiceClient()
@@ -1564,15 +1631,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def __enter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -240,17 +241,17 @@
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def list_notification_channel_descriptors(
         self,
     ) -> Callable[
@@ -362,9 +363,13 @@
         Union[
             notification.NotificationChannel,
             Awaitable[notification.NotificationChannel],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("NotificationChannelServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,16 +223,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def list_notification_channel_descriptors(
         self,
     ) -> Callable[
         [notification_service.ListNotificationChannelDescriptorsRequest],
@@ -576,9 +575,13 @@
                 response_deserializer=notification.NotificationChannel.deserialize,
             )
         return self._stubs["verify_notification_channel"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("NotificationChannelServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/notification_channel_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -207,34 +207,33 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.QueryTimeSeriesAsyncPager:
         r"""Queries time series using Monitoring Query Language.
         This method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_query_time_series():
+            async def sample_query_time_series():
                 # Create a client
-                client = monitoring_v3.QueryServiceClient()
+                client = monitoring_v3.QueryServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.QueryTimeSeriesRequest(
                     name="name_value",
                     query="query_value",
                 )
 
                 # Make the request
                 page_result = client.query_time_series(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.QueryTimeSeriesRequest, dict]):
                 The request object. The `QueryTimeSeries` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -264,20 +263,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.QueryTimeSeriesAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -50,15 +50,18 @@
     objects.
     """
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[QueryServiceTransport]]
     _transport_registry["grpc"] = QueryServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = QueryServiceGrpcAsyncIOTransport
 
-    def get_transport_class(cls, label: str = None,) -> Type[QueryServiceTransport]:
+    def get_transport_class(
+        cls,
+        label: str = None,
+    ) -> Type[QueryServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
         Returns:
@@ -158,64 +161,82 @@
         Returns:
             QueryServiceTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -392,15 +413,14 @@
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.QueryTimeSeriesPager:
         r"""Queries time series using Monitoring Query Language.
         This method does not require a Workspace.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_query_time_series():
                 # Create a client
                 client = monitoring_v3.QueryServiceClient()
@@ -450,20 +470,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.QueryTimeSeriesPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def __enter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -121,24 +122,26 @@
         # Save the credentials.
         self._credentials = credentials
 
     def _prep_wrapped_messages(self, client_info):
         # Precompute the wrapped methods.
         self._wrapped_methods = {
             self.query_time_series: gapic_v1.method.wrap_method(
-                self.query_time_series, default_timeout=None, client_info=client_info,
+                self.query_time_series,
+                default_timeout=None,
+                client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def query_time_series(
         self,
     ) -> Callable[
@@ -146,9 +149,13 @@
         Union[
             metric_service.QueryTimeSeriesResponse,
             Awaitable[metric_service.QueryTimeSeriesResponse],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("QueryServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def query_time_series(
         self,
     ) -> Callable[
         [metric_service.QueryTimeSeriesRequest], metric_service.QueryTimeSeriesResponse
@@ -258,9 +257,13 @@
                 response_deserializer=metric_service.QueryTimeSeriesResponse.deserialize,
             )
         return self._stubs["query_time_series"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("QueryServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/query_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/query_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -233,25 +233,25 @@
     ) -> gm_service.Service:
         r"""Create a ``Service``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_service():
+            async def sample_create_service():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateServiceRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
-                response = client.create_service(request=request)
+                response = await client.create_service(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateServiceRequest, dict]):
                 The request object. The `CreateService` request.
@@ -318,15 +318,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def get_service(
         self,
         request: Union[service_service.GetServiceRequest, dict] = None,
@@ -338,25 +343,25 @@
     ) -> service.Service:
         r"""Get the named ``Service``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_service():
+            async def sample_get_service():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetServiceRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_service(request=request)
+                response = await client.get_service(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetServiceRequest, dict]):
                 The request object. The `GetService` request.
@@ -424,15 +429,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def list_services(
         self,
         request: Union[service_service.ListServicesRequest, dict] = None,
@@ -444,28 +454,28 @@
     ) -> pagers.ListServicesAsyncPager:
         r"""List ``Service``\ s for this workspace.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_services():
+            async def sample_list_services():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListServicesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_services(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListServicesRequest, dict]):
                 The request object. The `ListServices` request.
             parent (:class:`str`):
                 Required. Resource name of the parent containing the
@@ -532,20 +542,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListServicesAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def update_service(
         self,
@@ -558,24 +576,24 @@
     ) -> gm_service.Service:
         r"""Update this ``Service``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_update_service():
+            async def sample_update_service():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.UpdateServiceRequest(
                 )
 
                 # Make the request
-                response = client.update_service(request=request)
+                response = await client.update_service(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.UpdateServiceRequest, dict]):
                 The request object. The `UpdateService` request.
@@ -632,15 +650,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("service.name", request.service.name),)
             ),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_service(
         self,
         request: Union[service_service.DeleteServiceRequest, dict] = None,
@@ -652,25 +675,25 @@
     ) -> None:
         r"""Soft delete this ``Service``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_service():
+            async def sample_delete_service():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteServiceRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_service(request=request)
+                await client.delete_service(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteServiceRequest, dict]):
                 The request object. The `DeleteService` request.
             name (:class:`str`):
                 Required. Resource name of the ``Service`` to delete.
                 The format is:
@@ -726,15 +749,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def create_service_level_objective(
         self,
         request: Union[service_service.CreateServiceLevelObjectiveRequest, dict] = None,
         *,
         parent: str = None,
@@ -745,25 +771,25 @@
     ) -> service.ServiceLevelObjective:
         r"""Create a ``ServiceLevelObjective`` for the given ``Service``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_service_level_objective():
+            async def sample_create_service_level_objective():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateServiceLevelObjectiveRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
-                response = client.create_service_level_objective(request=request)
+                response = await client.create_service_level_objective(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateServiceLevelObjectiveRequest, dict]):
                 The request object. The `CreateServiceLevelObjective`
@@ -840,15 +866,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def get_service_level_objective(
         self,
         request: Union[service_service.GetServiceLevelObjectiveRequest, dict] = None,
@@ -860,25 +891,25 @@
     ) -> service.ServiceLevelObjective:
         r"""Get a ``ServiceLevelObjective`` by name.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_service_level_objective():
+            async def sample_get_service_level_objective():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetServiceLevelObjectiveRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_service_level_objective(request=request)
+                response = await client.get_service_level_objective(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetServiceLevelObjectiveRequest, dict]):
                 The request object. The `GetServiceLevelObjective`
@@ -954,15 +985,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def list_service_level_objectives(
         self,
         request: Union[service_service.ListServiceLevelObjectivesRequest, dict] = None,
@@ -974,28 +1010,28 @@
     ) -> pagers.ListServiceLevelObjectivesAsyncPager:
         r"""List the ``ServiceLevelObjective``\ s for the given ``Service``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_service_level_objectives():
+            async def sample_list_service_level_objectives():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListServiceLevelObjectivesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_service_level_objectives(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListServiceLevelObjectivesRequest, dict]):
                 The request object. The `ListServiceLevelObjectives`
                 request.
             parent (:class:`str`):
@@ -1062,20 +1098,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListServiceLevelObjectivesAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def update_service_level_objective(
         self,
@@ -1088,24 +1132,24 @@
     ) -> service.ServiceLevelObjective:
         r"""Update the given ``ServiceLevelObjective``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_update_service_level_objective():
+            async def sample_update_service_level_objective():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.UpdateServiceLevelObjectiveRequest(
                 )
 
                 # Make the request
-                response = client.update_service_level_objective(request=request)
+                response = await client.update_service_level_objective(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.UpdateServiceLevelObjectiveRequest, dict]):
                 The request object. The `UpdateServiceLevelObjective`
@@ -1176,15 +1220,20 @@
                         request.service_level_objective.name,
                     ),
                 )
             ),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_service_level_objective(
         self,
         request: Union[service_service.DeleteServiceLevelObjectiveRequest, dict] = None,
@@ -1196,25 +1245,25 @@
     ) -> None:
         r"""Delete the given ``ServiceLevelObjective``.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_service_level_objective():
+            async def sample_delete_service_level_objective():
                 # Create a client
-                client = monitoring_v3.ServiceMonitoringServiceClient()
+                client = monitoring_v3.ServiceMonitoringServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteServiceLevelObjectiveRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_service_level_objective(request=request)
+                await client.delete_service_level_objective(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteServiceLevelObjectiveRequest, dict]):
                 The request object. The `DeleteServiceLevelObjective`
                 request.
             name (:class:`str`):
                 Required. Resource name of the ``ServiceLevelObjective``
@@ -1271,15 +1320,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -56,15 +56,16 @@
     _transport_registry = (
         OrderedDict()
     )  # type: Dict[str, Type[ServiceMonitoringServiceTransport]]
     _transport_registry["grpc"] = ServiceMonitoringServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = ServiceMonitoringServiceGrpcAsyncIOTransport
 
     def get_transport_class(
-        cls, label: str = None,
+        cls,
+        label: str = None,
     ) -> Type[ServiceMonitoringServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -166,29 +167,35 @@
         Returns:
             ServiceMonitoringServiceTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def service_path(project: str, service: str,) -> str:
+    def service_path(
+        project: str,
+        service: str,
+    ) -> str:
         """Returns a fully-qualified service string."""
         return "projects/{project}/services/{service}".format(
-            project=project, service=service,
+            project=project,
+            service=service,
         )
 
     @staticmethod
     def parse_service_path(path: str) -> Dict[str, str]:
         """Parses a service path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/services/(?P<service>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
     def service_level_objective_path(
-        project: str, service: str, service_level_objective: str,
+        project: str,
+        service: str,
+        service_level_objective: str,
     ) -> str:
         """Returns a fully-qualified service_level_objective string."""
         return "projects/{project}/services/{service}/serviceLevelObjectives/{service_level_objective}".format(
             project=project,
             service=service,
             service_level_objective=service_level_objective,
         )
@@ -199,64 +206,82 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/services/(?P<service>.+?)/serviceLevelObjectives/(?P<service_level_objective>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -523,15 +548,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def get_service(
         self,
         request: Union[service_service.GetServiceRequest, dict] = None,
@@ -620,15 +650,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def list_services(
         self,
         request: Union[service_service.ListServicesRequest, dict] = None,
@@ -719,20 +754,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListServicesPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def update_service(
         self,
@@ -819,15 +862,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("service.name", request.service.name),)
             ),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_service(
         self,
         request: Union[service_service.DeleteServiceRequest, dict] = None,
@@ -904,15 +952,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def create_service_level_objective(
         self,
         request: Union[service_service.CreateServiceLevelObjectiveRequest, dict] = None,
         *,
         parent: str = None,
@@ -1020,15 +1071,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def get_service_level_objective(
         self,
         request: Union[service_service.GetServiceLevelObjectiveRequest, dict] = None,
@@ -1127,15 +1183,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def list_service_level_objectives(
         self,
         request: Union[service_service.ListServiceLevelObjectivesRequest, dict] = None,
@@ -1228,20 +1289,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListServiceLevelObjectivesPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def update_service_level_objective(
         self,
@@ -1344,15 +1413,20 @@
                         request.service_level_objective.name,
                     ),
                 )
             ),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_service_level_objective(
         self,
         request: Union[service_service.DeleteServiceLevelObjectiveRequest, dict] = None,
@@ -1432,15 +1506,18 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -124,15 +125,17 @@
         # Save the credentials.
         self._credentials = credentials
 
     def _prep_wrapped_messages(self, client_info):
         # Precompute the wrapped methods.
         self._wrapped_methods = {
             self.create_service: gapic_v1.method.wrap_method(
-                self.create_service, default_timeout=30.0, client_info=client_info,
+                self.create_service,
+                default_timeout=30.0,
+                client_info=client_info,
             ),
             self.get_service: gapic_v1.method.wrap_method(
                 self.get_service,
                 default_retry=retries.Retry(
                     initial=0.1,
                     maximum=30.0,
                     multiplier=1.3,
@@ -155,15 +158,17 @@
                     ),
                     deadline=30.0,
                 ),
                 default_timeout=30.0,
                 client_info=client_info,
             ),
             self.update_service: gapic_v1.method.wrap_method(
-                self.update_service, default_timeout=30.0, client_info=client_info,
+                self.update_service,
+                default_timeout=30.0,
+                client_info=client_info,
             ),
             self.delete_service: gapic_v1.method.wrap_method(
                 self.delete_service,
                 default_retry=retries.Retry(
                     initial=0.1,
                     maximum=30.0,
                     multiplier=1.3,
@@ -228,17 +233,17 @@
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def create_service(
         self,
     ) -> Callable[
@@ -330,9 +335,13 @@
         self,
     ) -> Callable[
         [service_service.DeleteServiceLevelObjectiveRequest],
         Union[empty_pb2.Empty, Awaitable[empty_pb2.Empty]],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("ServiceMonitoringServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def create_service(
         self,
     ) -> Callable[[service_service.CreateServiceRequest], gm_service.Service]:
         r"""Return a callable for the create service method over gRPC.
@@ -516,9 +515,13 @@
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["delete_service_level_objective"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("ServiceMonitoringServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/service_monitoring_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/async_client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -227,33 +227,32 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUptimeCheckConfigsAsyncPager:
         r"""Lists the existing valid Uptime check configurations
         for the project (leaving out any invalid
         configurations).
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_uptime_check_configs():
+            async def sample_list_uptime_check_configs():
                 # Create a client
-                client = monitoring_v3.UptimeCheckServiceClient()
+                client = monitoring_v3.UptimeCheckServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListUptimeCheckConfigsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_uptime_check_configs(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListUptimeCheckConfigsRequest, dict]):
                 The request object. The protocol for the
                 `ListUptimeCheckConfigs` request.
             parent (:class:`str`):
@@ -320,20 +319,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListUptimeCheckConfigsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def get_uptime_check_config(
         self,
@@ -346,25 +353,25 @@
     ) -> uptime.UptimeCheckConfig:
         r"""Gets a single Uptime check configuration.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_get_uptime_check_config():
+            async def sample_get_uptime_check_config():
                 # Create a client
-                client = monitoring_v3.UptimeCheckServiceClient()
+                client = monitoring_v3.UptimeCheckServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.GetUptimeCheckConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                response = client.get_uptime_check_config(request=request)
+                response = await client.get_uptime_check_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.GetUptimeCheckConfigRequest, dict]):
                 The request object. The protocol for the
@@ -430,15 +437,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def create_uptime_check_config(
         self,
         request: Union[uptime_service.CreateUptimeCheckConfigRequest, dict] = None,
@@ -451,25 +463,25 @@
     ) -> uptime.UptimeCheckConfig:
         r"""Creates a new Uptime check configuration.
 
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_create_uptime_check_config():
+            async def sample_create_uptime_check_config():
                 # Create a client
-                client = monitoring_v3.UptimeCheckServiceClient()
+                client = monitoring_v3.UptimeCheckServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.CreateUptimeCheckConfigRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
-                response = client.create_uptime_check_config(request=request)
+                response = await client.create_uptime_check_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.CreateUptimeCheckConfigRequest, dict]):
                 The request object. The protocol for the
@@ -536,15 +548,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def update_uptime_check_config(
         self,
         request: Union[uptime_service.UpdateUptimeCheckConfigRequest, dict] = None,
@@ -556,29 +573,28 @@
     ) -> uptime.UptimeCheckConfig:
         r"""Updates an Uptime check configuration. You can either replace
         the entire configuration with a new one or replace only certain
         fields in the current configuration by specifying the fields to
         be updated via ``updateMask``. Returns the updated
         configuration.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_update_uptime_check_config():
+            async def sample_update_uptime_check_config():
                 # Create a client
-                client = monitoring_v3.UptimeCheckServiceClient()
+                client = monitoring_v3.UptimeCheckServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.UpdateUptimeCheckConfigRequest(
                 )
 
                 # Make the request
-                response = client.update_uptime_check_config(request=request)
+                response = await client.update_uptime_check_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.UpdateUptimeCheckConfigRequest, dict]):
                 The request object. The protocol for the
@@ -644,15 +660,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("uptime_check_config.name", request.uptime_check_config.name),)
             ),
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     async def delete_uptime_check_config(
         self,
         request: Union[uptime_service.DeleteUptimeCheckConfigRequest, dict] = None,
@@ -663,30 +684,29 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes an Uptime check configuration. Note that this
         method will fail if the Uptime check configuration is
         referenced by an alert policy or other dependent configs
         that would be rendered invalid by the deletion.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_delete_uptime_check_config():
+            async def sample_delete_uptime_check_config():
                 # Create a client
-                client = monitoring_v3.UptimeCheckServiceClient()
+                client = monitoring_v3.UptimeCheckServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.DeleteUptimeCheckConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
-                client.delete_uptime_check_config(request=request)
+                await client.delete_uptime_check_config(request=request)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.DeleteUptimeCheckConfigRequest, dict]):
                 The request object. The protocol for the
                 `DeleteUptimeCheckConfig` request.
             name (:class:`str`):
                 Required. The Uptime check configuration to delete. The
@@ -743,46 +763,48 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         await rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     async def list_uptime_check_ips(
         self,
         request: Union[uptime_service.ListUptimeCheckIpsRequest, dict] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUptimeCheckIpsAsyncPager:
         r"""Returns the list of IP addresses that checkers run
         from
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
-            def sample_list_uptime_check_ips():
+            async def sample_list_uptime_check_ips():
                 # Create a client
-                client = monitoring_v3.UptimeCheckServiceClient()
+                client = monitoring_v3.UptimeCheckServiceAsyncClient()
 
                 # Initialize request argument(s)
                 request = monitoring_v3.ListUptimeCheckIpsRequest(
                 )
 
                 # Make the request
                 page_result = client.list_uptime_check_ips(request=request)
 
                 # Handle the response
-                for response in page_result:
+                async for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.monitoring_v3.types.ListUptimeCheckIpsRequest, dict]):
                 The request object. The protocol for the
                 `ListUptimeCheckIps` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -816,20 +838,28 @@
                 deadline=30.0,
             ),
             default_timeout=30.0,
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Send the request.
-        response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__aiter__` convenience method.
         response = pagers.ListUptimeCheckIpsAsyncPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     async def __aenter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/client.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Optional, Sequence, Tuple, Type, Union
+from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
 import pkg_resources
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
@@ -55,15 +55,16 @@
     _transport_registry = (
         OrderedDict()
     )  # type: Dict[str, Type[UptimeCheckServiceTransport]]
     _transport_registry["grpc"] = UptimeCheckServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = UptimeCheckServiceGrpcAsyncIOTransport
 
     def get_transport_class(
-        cls, label: str = None,
+        cls,
+        label: str = None,
     ) -> Type[UptimeCheckServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -169,80 +170,102 @@
         Returns:
             UptimeCheckServiceTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def uptime_check_config_path(project: str, uptime_check_config: str,) -> str:
+    def uptime_check_config_path(
+        project: str,
+        uptime_check_config: str,
+    ) -> str:
         """Returns a fully-qualified uptime_check_config string."""
         return "projects/{project}/uptimeCheckConfigs/{uptime_check_config}".format(
-            project=project, uptime_check_config=uptime_check_config,
+            project=project,
+            uptime_check_config=uptime_check_config,
         )
 
     @staticmethod
     def parse_uptime_check_config_path(path: str) -> Dict[str, str]:
         """Parses a uptime_check_config path into its component segments."""
         m = re.match(
             r"^projects/(?P<project>.+?)/uptimeCheckConfigs/(?P<uptime_check_config>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_billing_account_path(billing_account: str,) -> str:
+    def common_billing_account_path(
+        billing_account: str,
+    ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
 
     @staticmethod
     def parse_common_billing_account_path(path: str) -> Dict[str, str]:
         """Parse a billing_account path into its component segments."""
         m = re.match(r"^billingAccounts/(?P<billing_account>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_folder_path(folder: str,) -> str:
+    def common_folder_path(
+        folder: str,
+    ) -> str:
         """Returns a fully-qualified folder string."""
-        return "folders/{folder}".format(folder=folder,)
+        return "folders/{folder}".format(
+            folder=folder,
+        )
 
     @staticmethod
     def parse_common_folder_path(path: str) -> Dict[str, str]:
         """Parse a folder path into its component segments."""
         m = re.match(r"^folders/(?P<folder>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_organization_path(organization: str,) -> str:
+    def common_organization_path(
+        organization: str,
+    ) -> str:
         """Returns a fully-qualified organization string."""
-        return "organizations/{organization}".format(organization=organization,)
+        return "organizations/{organization}".format(
+            organization=organization,
+        )
 
     @staticmethod
     def parse_common_organization_path(path: str) -> Dict[str, str]:
         """Parse a organization path into its component segments."""
         m = re.match(r"^organizations/(?P<organization>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_project_path(project: str,) -> str:
+    def common_project_path(
+        project: str,
+    ) -> str:
         """Returns a fully-qualified project string."""
-        return "projects/{project}".format(project=project,)
+        return "projects/{project}".format(
+            project=project,
+        )
 
     @staticmethod
     def parse_common_project_path(path: str) -> Dict[str, str]:
         """Parse a project path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)$", path)
         return m.groupdict() if m else {}
 
     @staticmethod
-    def common_location_path(project: str, location: str,) -> str:
+    def common_location_path(
+        project: str,
+        location: str,
+    ) -> str:
         """Returns a fully-qualified location string."""
         return "projects/{project}/locations/{location}".format(
-            project=project, location=location,
+            project=project,
+            location=location,
         )
 
     @staticmethod
     def parse_common_location_path(path: str) -> Dict[str, str]:
         """Parse a location path into its component segments."""
         m = re.match(r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)$", path)
         return m.groupdict() if m else {}
@@ -421,15 +444,14 @@
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUptimeCheckConfigsPager:
         r"""Lists the existing valid Uptime check configurations
         for the project (leaving out any invalid
         configurations).
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_uptime_check_configs():
                 # Create a client
                 client = monitoring_v3.UptimeCheckServiceClient()
@@ -507,20 +529,28 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListUptimeCheckConfigsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def get_uptime_check_config(
         self,
@@ -608,15 +638,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def create_uptime_check_config(
         self,
         request: Union[uptime_service.CreateUptimeCheckConfigRequest, dict] = None,
@@ -716,15 +751,20 @@
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def update_uptime_check_config(
         self,
         request: Union[uptime_service.UpdateUptimeCheckConfigRequest, dict] = None,
@@ -736,15 +776,14 @@
     ) -> uptime.UptimeCheckConfig:
         r"""Updates an Uptime check configuration. You can either replace
         the entire configuration with a new one or replace only certain
         fields in the current configuration by specifying the fields to
         be updated via ``updateMask``. Returns the updated
         configuration.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_update_uptime_check_config():
                 # Create a client
                 client = monitoring_v3.UptimeCheckServiceClient()
@@ -826,15 +865,20 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("uptime_check_config.name", request.uptime_check_config.name),)
             ),
         )
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # Done; return the response.
         return response
 
     def delete_uptime_check_config(
         self,
         request: Union[uptime_service.DeleteUptimeCheckConfigRequest, dict] = None,
@@ -845,15 +889,14 @@
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes an Uptime check configuration. Note that this
         method will fail if the Uptime check configuration is
         referenced by an alert policy or other dependent configs
         that would be rendered invalid by the deletion.
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_delete_uptime_check_config():
                 # Create a client
                 client = monitoring_v3.UptimeCheckServiceClient()
@@ -918,29 +961,31 @@
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         rpc(
-            request, retry=retry, timeout=timeout, metadata=metadata,
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
         )
 
     def list_uptime_check_ips(
         self,
         request: Union[uptime_service.ListUptimeCheckIpsRequest, dict] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUptimeCheckIpsPager:
         r"""Returns the list of IP addresses that checkers run
         from
 
-
         .. code-block:: python
 
             from google.cloud import monitoring_v3
 
             def sample_list_uptime_check_ips():
                 # Create a client
                 client = monitoring_v3.UptimeCheckServiceClient()
@@ -983,20 +1028,28 @@
             request = uptime_service.ListUptimeCheckIpsRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
         rpc = self._transport._wrapped_methods[self._transport.list_uptime_check_ips]
 
         # Send the request.
-        response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
 
         # This method is paged; wrap the response in a pager, which provides
         # an `__iter__` convenience method.
         response = pagers.ListUptimeCheckIpsPager(
-            method=rpc, request=request, response=response, metadata=metadata,
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
     def __enter__(self):
         return self
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/pagers.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/base.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
+
         # Save the hostname. Default to port 443 (HTTPS) if none is specified.
         if ":" not in host:
             host += ":443"
         self._host = host
 
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
@@ -193,17 +194,17 @@
                 client_info=client_info,
             ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
-       .. warning::
-            Only call this method if the transport is NOT shared
-            with other clients - this may cause errors in other clients!
+        .. warning::
+             Only call this method if the transport is NOT shared
+             with other clients - this may cause errors in other clients!
         """
         raise NotImplementedError()
 
     @property
     def list_uptime_check_configs(
         self,
     ) -> Callable[
@@ -259,9 +260,13 @@
         Union[
             uptime_service.ListUptimeCheckIpsResponse,
             Awaitable[uptime_service.ListUptimeCheckIpsResponse],
         ],
     ]:
         raise NotImplementedError()
 
+    @property
+    def kind(self) -> str:
+        raise NotImplementedError()
+
 
 __all__ = ("UptimeCheckServiceTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,15 @@
             scopes=scopes,
             default_host=cls.DEFAULT_HOST,
             **kwargs,
         )
 
     @property
     def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service.
-        """
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
     def list_uptime_check_configs(
         self,
     ) -> Callable[
         [uptime_service.ListUptimeCheckConfigsRequest],
@@ -414,9 +413,13 @@
                 response_deserializer=uptime_service.ListUptimeCheckIpsResponse.deserialize,
             )
         return self._stubs["list_uptime_check_ips"]
 
     def close(self):
         self.grpc_channel.close()
 
+    @property
+    def kind(self) -> str:
+        return "grpc"
+
 
 __all__ = ("UptimeCheckServiceGrpcTransport",)
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/services/uptime_check_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/__init__.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .alert import AlertPolicy
+from .alert import (
+    AlertPolicy,
+)
 from .alert_service import (
     CreateAlertPolicyRequest,
     DeleteAlertPolicyRequest,
     GetAlertPolicyRequest,
     ListAlertPoliciesRequest,
     ListAlertPoliciesResponse,
     UpdateAlertPolicyRequest,
@@ -25,16 +27,20 @@
 from .common import (
     Aggregation,
     TimeInterval,
     TypedValue,
     ComparisonType,
     ServiceTier,
 )
-from .dropped_labels import DroppedLabels
-from .group import Group
+from .dropped_labels import (
+    DroppedLabels,
+)
+from .group import (
+    Group,
+)
 from .group_service import (
     CreateGroupRequest,
     DeleteGroupRequest,
     GetGroupRequest,
     ListGroupMembersRequest,
     ListGroupMembersResponse,
     ListGroupsRequest,
@@ -64,15 +70,17 @@
     ListMonitoredResourceDescriptorsResponse,
     ListTimeSeriesRequest,
     ListTimeSeriesResponse,
     QueryErrorList,
     QueryTimeSeriesRequest,
     QueryTimeSeriesResponse,
 )
-from .mutation_record import MutationRecord
+from .mutation_record import (
+    MutationRecord,
+)
 from .notification import (
     NotificationChannel,
     NotificationChannelDescriptor,
 )
 from .notification_service import (
     CreateNotificationChannelRequest,
     DeleteNotificationChannelRequest,
@@ -109,15 +117,17 @@
     ListServiceLevelObjectivesRequest,
     ListServiceLevelObjectivesResponse,
     ListServicesRequest,
     ListServicesResponse,
     UpdateServiceLevelObjectiveRequest,
     UpdateServiceRequest,
 )
-from .span_context import SpanContext
+from .span_context import (
+    SpanContext,
+)
 from .uptime import (
     InternalChecker,
     UptimeCheckConfig,
     UptimeCheckIp,
     GroupResourceType,
     UptimeCheckRegion,
 )
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/alert.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/alert.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 from google.cloud.monitoring_v3.types import common
 from google.cloud.monitoring_v3.types import mutation_record as gm_mutation_record
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 
 
-__protobuf__ = proto.module(package="google.monitoring.v3", manifest={"AlertPolicy",},)
+__protobuf__ = proto.module(
+    package="google.monitoring.v3",
+    manifest={
+        "AlertPolicy",
+    },
+)
 
 
 class AlertPolicy(proto.Message):
     r"""A description of the conditions under which some aspect of your
     system is considered to be "unhealthy" and the ways to notify people
     or services about this state. For an overview of alert policies, see
     `Introduction to
@@ -58,15 +63,15 @@
             notifications and incidents related to this
             policy. Best practice is for the documentation
             to include information to help responders
             understand, mitigate, escalate, and correct the
             underlying problems detected by the alerting
             policy. Notification channels that have limited
             capacity might not show this documentation.
-        user_labels (Sequence[google.cloud.monitoring_v3.types.AlertPolicy.UserLabelsEntry]):
+        user_labels (Mapping[str, str]):
             User-supplied key/value data to be used for organizing and
             identifying the ``AlertPolicy`` objects.
 
             The field can contain up to 64 entries. Each key and value
             is limited to 63 Unicode characters or 128 bytes, whichever
             is smaller. Labels and values can contain only lowercase
             letters, numerals, underscores, and dashes. Keys must begin
@@ -145,16 +150,22 @@
             mime_type (str):
                 The format of the ``content`` field. Presently, only the
                 value ``"text/markdown"`` is supported. See
                 `Markdown <https://en.wikipedia.org/wiki/Markdown>`__ for
                 more information.
         """
 
-        content = proto.Field(proto.STRING, number=1,)
-        mime_type = proto.Field(proto.STRING, number=2,)
+        content = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        mime_type = proto.Field(
+            proto.STRING,
+            number=2,
+        )
 
     class Condition(proto.Message):
         r"""A condition is a true/false test that determines when an
         alerting policy should open an incident. If a condition
         evaluates to true, it signifies that something is wrong.
 
         This message has `oneof`_ fields (mutually exclusive fields).
@@ -245,16 +256,24 @@
                 percent (float):
                     The percentage of time series that must fail
                     the predicate for the condition to be triggered.
 
                     This field is a member of `oneof`_ ``type``.
             """
 
-            count = proto.Field(proto.INT32, number=1, oneof="type",)
-            percent = proto.Field(proto.DOUBLE, number=2, oneof="type",)
+            count = proto.Field(
+                proto.INT32,
+                number=1,
+                oneof="type",
+            )
+            percent = proto.Field(
+                proto.DOUBLE,
+                number=2,
+                oneof="type",
+            )
 
         class MetricThreshold(proto.Message):
             r"""A condition type that compares a collection of time series
             against a threshold.
 
             Attributes:
                 filter (str):
@@ -339,29 +358,50 @@
                     unspecified, then the condition will trigger if the
                     comparison is true for any of the time series that have been
                     identified by ``filter`` and ``aggregations``, or by the
                     ratio, if ``denominator_filter`` and
                     ``denominator_aggregations`` are specified.
             """
 
-            filter = proto.Field(proto.STRING, number=2,)
+            filter = proto.Field(
+                proto.STRING,
+                number=2,
+            )
             aggregations = proto.RepeatedField(
-                proto.MESSAGE, number=8, message=common.Aggregation,
+                proto.MESSAGE,
+                number=8,
+                message=common.Aggregation,
+            )
+            denominator_filter = proto.Field(
+                proto.STRING,
+                number=9,
             )
-            denominator_filter = proto.Field(proto.STRING, number=9,)
             denominator_aggregations = proto.RepeatedField(
-                proto.MESSAGE, number=10, message=common.Aggregation,
+                proto.MESSAGE,
+                number=10,
+                message=common.Aggregation,
+            )
+            comparison = proto.Field(
+                proto.ENUM,
+                number=4,
+                enum=common.ComparisonType,
+            )
+            threshold_value = proto.Field(
+                proto.DOUBLE,
+                number=5,
             )
-            comparison = proto.Field(proto.ENUM, number=4, enum=common.ComparisonType,)
-            threshold_value = proto.Field(proto.DOUBLE, number=5,)
             duration = proto.Field(
-                proto.MESSAGE, number=6, message=duration_pb2.Duration,
+                proto.MESSAGE,
+                number=6,
+                message=duration_pb2.Duration,
             )
             trigger = proto.Field(
-                proto.MESSAGE, number=7, message="AlertPolicy.Condition.Trigger",
+                proto.MESSAGE,
+                number=7,
+                message="AlertPolicy.Condition.Trigger",
             )
 
         class MetricAbsence(proto.Message):
             r"""A condition type that checks that monitored resources are reporting
             data. The configuration defines a metric and a set of monitored
             resources. The predicate is considered in violation when a time
             series for the specified metric of a monitored resource does not
@@ -406,53 +446,69 @@
                     The number/percent of time series for which the comparison
                     must hold in order for the condition to trigger. If
                     unspecified, then the condition will trigger if the
                     comparison is true for any of the time series that have been
                     identified by ``filter`` and ``aggregations``.
             """
 
-            filter = proto.Field(proto.STRING, number=1,)
+            filter = proto.Field(
+                proto.STRING,
+                number=1,
+            )
             aggregations = proto.RepeatedField(
-                proto.MESSAGE, number=5, message=common.Aggregation,
+                proto.MESSAGE,
+                number=5,
+                message=common.Aggregation,
             )
             duration = proto.Field(
-                proto.MESSAGE, number=2, message=duration_pb2.Duration,
+                proto.MESSAGE,
+                number=2,
+                message=duration_pb2.Duration,
             )
             trigger = proto.Field(
-                proto.MESSAGE, number=3, message="AlertPolicy.Condition.Trigger",
+                proto.MESSAGE,
+                number=3,
+                message="AlertPolicy.Condition.Trigger",
             )
 
         class LogMatch(proto.Message):
             r"""A condition type that checks whether a log message in the `scoping
             project <https://cloud.google.com/monitoring/api/v3#project_name>`__
             satisfies the given filter. Logs from other projects in the metrics
             scope are not evaluated.
 
             Attributes:
                 filter (str):
                     Required. A logs-based filter. See `Advanced Logs
                     Queries <https://cloud.google.com/logging/docs/view/advanced-queries>`__
                     for how this filter should be constructed.
-                label_extractors (Sequence[google.cloud.monitoring_v3.types.AlertPolicy.Condition.LogMatch.LabelExtractorsEntry]):
+                label_extractors (Mapping[str, str]):
                     Optional. A map from a label key to an extractor expression,
                     which is used to extract the value for this label key. Each
                     entry in this map is a specification for how data should be
                     extracted from log entries that match ``filter``. Each
                     combination of extracted values is treated as a separate
                     rule for the purposes of triggering notifications. Label
                     keys and corresponding values can be used in notifications
                     generated by this condition.
 
                     Please see `the documentation on logs-based metric
                     ``valueExtractor``\ s <https://cloud.google.com/logging/docs/reference/v2/rest/v2/projects.metrics#LogMetric.FIELDS.value_extractor>`__
                     for syntax and examples.
             """
 
-            filter = proto.Field(proto.STRING, number=1,)
-            label_extractors = proto.MapField(proto.STRING, proto.STRING, number=2,)
+            filter = proto.Field(
+                proto.STRING,
+                number=1,
+            )
+            label_extractors = proto.MapField(
+                proto.STRING,
+                proto.STRING,
+                number=2,
+            )
 
         class MonitoringQueryLanguageCondition(proto.Message):
             r"""A condition type that allows alert policies to be defined using
             `Monitoring Query
             Language <https://cloud.google.com/monitoring/mql>`__.
 
             Attributes:
@@ -478,24 +534,37 @@
                     unspecified, then the condition will trigger if the
                     comparison is true for any of the time series that have been
                     identified by ``filter`` and ``aggregations``, or by the
                     ratio, if ``denominator_filter`` and
                     ``denominator_aggregations`` are specified.
             """
 
-            query = proto.Field(proto.STRING, number=1,)
+            query = proto.Field(
+                proto.STRING,
+                number=1,
+            )
             duration = proto.Field(
-                proto.MESSAGE, number=2, message=duration_pb2.Duration,
+                proto.MESSAGE,
+                number=2,
+                message=duration_pb2.Duration,
             )
             trigger = proto.Field(
-                proto.MESSAGE, number=3, message="AlertPolicy.Condition.Trigger",
+                proto.MESSAGE,
+                number=3,
+                message="AlertPolicy.Condition.Trigger",
             )
 
-        name = proto.Field(proto.STRING, number=12,)
-        display_name = proto.Field(proto.STRING, number=6,)
+        name = proto.Field(
+            proto.STRING,
+            number=12,
+        )
+        display_name = proto.Field(
+            proto.STRING,
+            number=6,
+        )
         condition_threshold = proto.Field(
             proto.MESSAGE,
             number=1,
             oneof="condition",
             message="AlertPolicy.Condition.MetricThreshold",
         )
         condition_absent = proto.Field(
@@ -539,38 +608,83 @@
 
             Attributes:
                 period (google.protobuf.duration_pb2.Duration):
                     Not more than one notification per ``period``.
             """
 
             period = proto.Field(
-                proto.MESSAGE, number=1, message=duration_pb2.Duration,
+                proto.MESSAGE,
+                number=1,
+                message=duration_pb2.Duration,
             )
 
         notification_rate_limit = proto.Field(
             proto.MESSAGE,
             number=1,
             message="AlertPolicy.AlertStrategy.NotificationRateLimit",
         )
         auto_close = proto.Field(
-            proto.MESSAGE, number=3, message=duration_pb2.Duration,
+            proto.MESSAGE,
+            number=3,
+            message=duration_pb2.Duration,
         )
 
-    name = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=2,)
-    documentation = proto.Field(proto.MESSAGE, number=13, message=Documentation,)
-    user_labels = proto.MapField(proto.STRING, proto.STRING, number=16,)
-    conditions = proto.RepeatedField(proto.MESSAGE, number=12, message=Condition,)
-    combiner = proto.Field(proto.ENUM, number=6, enum=ConditionCombinerType,)
-    enabled = proto.Field(proto.MESSAGE, number=17, message=wrappers_pb2.BoolValue,)
-    validity = proto.Field(proto.MESSAGE, number=18, message=status_pb2.Status,)
-    notification_channels = proto.RepeatedField(proto.STRING, number=14,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    documentation = proto.Field(
+        proto.MESSAGE,
+        number=13,
+        message=Documentation,
+    )
+    user_labels = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=16,
+    )
+    conditions = proto.RepeatedField(
+        proto.MESSAGE,
+        number=12,
+        message=Condition,
+    )
+    combiner = proto.Field(
+        proto.ENUM,
+        number=6,
+        enum=ConditionCombinerType,
+    )
+    enabled = proto.Field(
+        proto.MESSAGE,
+        number=17,
+        message=wrappers_pb2.BoolValue,
+    )
+    validity = proto.Field(
+        proto.MESSAGE,
+        number=18,
+        message=status_pb2.Status,
+    )
+    notification_channels = proto.RepeatedField(
+        proto.STRING,
+        number=14,
+    )
     creation_record = proto.Field(
-        proto.MESSAGE, number=10, message=gm_mutation_record.MutationRecord,
+        proto.MESSAGE,
+        number=10,
+        message=gm_mutation_record.MutationRecord,
     )
     mutation_record = proto.Field(
-        proto.MESSAGE, number=11, message=gm_mutation_record.MutationRecord,
+        proto.MESSAGE,
+        number=11,
+        message=gm_mutation_record.MutationRecord,
+    )
+    alert_strategy = proto.Field(
+        proto.MESSAGE,
+        number=21,
+        message=AlertStrategy,
     )
-    alert_strategy = proto.Field(proto.MESSAGE, number=21, message=AlertStrategy,)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/alert_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/alert_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,31 +55,41 @@
             identifying the policy in the container.
         alert_policy (google.cloud.monitoring_v3.types.AlertPolicy):
             Required. The requested alerting policy. You should omit the
             ``name`` field in this policy. The name will be returned in
             the new policy, including a new ``[ALERT_POLICY_ID]`` value.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
-    alert_policy = proto.Field(proto.MESSAGE, number=2, message=alert.AlertPolicy,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    alert_policy = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=alert.AlertPolicy,
+    )
 
 
 class GetAlertPolicyRequest(proto.Message):
     r"""The protocol for the ``GetAlertPolicy`` request.
 
     Attributes:
         name (str):
             Required. The alerting policy to retrieve. The format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/alertPolicies/[ALERT_POLICY_ID]
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class ListAlertPoliciesRequest(proto.Message):
     r"""The protocol for the ``ListAlertPolicies`` request.
 
     Attributes:
         name (str):
@@ -116,19 +126,34 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return more
             results from the previous method call.
     """
 
-    name = proto.Field(proto.STRING, number=4,)
-    filter = proto.Field(proto.STRING, number=5,)
-    order_by = proto.Field(proto.STRING, number=6,)
-    page_size = proto.Field(proto.INT32, number=2,)
-    page_token = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    order_by = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class ListAlertPoliciesResponse(proto.Message):
     r"""The protocol for the ``ListAlertPolicies`` response.
 
     Attributes:
         alert_policies (Sequence[google.cloud.monitoring_v3.types.AlertPolicy]):
@@ -145,18 +170,26 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     alert_policies = proto.RepeatedField(
-        proto.MESSAGE, number=3, message=alert.AlertPolicy,
+        proto.MESSAGE,
+        number=3,
+        message=alert.AlertPolicy,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    total_size = proto.Field(
+        proto.INT32,
+        number=4,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
-    total_size = proto.Field(proto.INT32, number=4,)
 
 
 class UpdateAlertPolicyRequest(proto.Message):
     r"""The protocol for the ``UpdateAlertPolicy`` request.
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
@@ -191,17 +224,23 @@
             Required. The updated alerting policy or the updated values
             for the fields listed in ``update_mask``. If ``update_mask``
             is not empty, any fields in this policy that are not in
             ``update_mask`` are ignored.
     """
 
     update_mask = proto.Field(
-        proto.MESSAGE, number=2, message=field_mask_pb2.FieldMask,
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
+    )
+    alert_policy = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=alert.AlertPolicy,
     )
-    alert_policy = proto.Field(proto.MESSAGE, number=3, message=alert.AlertPolicy,)
 
 
 class DeleteAlertPolicyRequest(proto.Message):
     r"""The protocol for the ``DeleteAlertPolicy`` request.
 
     Attributes:
         name (str):
@@ -211,11 +250,14 @@
 
                 projects/[PROJECT_ID_OR_NUMBER]/alertPolicies/[ALERT_POLICY_ID]
 
             For more information, see
             [AlertPolicy][google.monitoring.v3.AlertPolicy].
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/common.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,20 +89,39 @@
             This field is a member of `oneof`_ ``value``.
         distribution_value (google.api.distribution_pb2.Distribution):
             A distribution value.
 
             This field is a member of `oneof`_ ``value``.
     """
 
-    bool_value = proto.Field(proto.BOOL, number=1, oneof="value",)
-    int64_value = proto.Field(proto.INT64, number=2, oneof="value",)
-    double_value = proto.Field(proto.DOUBLE, number=3, oneof="value",)
-    string_value = proto.Field(proto.STRING, number=4, oneof="value",)
+    bool_value = proto.Field(
+        proto.BOOL,
+        number=1,
+        oneof="value",
+    )
+    int64_value = proto.Field(
+        proto.INT64,
+        number=2,
+        oneof="value",
+    )
+    double_value = proto.Field(
+        proto.DOUBLE,
+        number=3,
+        oneof="value",
+    )
+    string_value = proto.Field(
+        proto.STRING,
+        number=4,
+        oneof="value",
+    )
     distribution_value = proto.Field(
-        proto.MESSAGE, number=5, oneof="value", message=distribution_pb2.Distribution,
+        proto.MESSAGE,
+        number=5,
+        oneof="value",
+        message=distribution_pb2.Distribution,
     )
 
 
 class TimeInterval(proto.Message):
     r"""A closed time interval. It extends from the start time to the end
     time, and includes both: ``[startTime, endTime]``. Valid time
     intervals depend on the
@@ -146,16 +165,24 @@
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Optional. The beginning of the time interval.
             The default value for the start time is the end
             time. The start time must not be later than the
             end time.
     """
 
-    end_time = proto.Field(proto.MESSAGE, number=2, message=timestamp_pb2.Timestamp,)
-    start_time = proto.Field(proto.MESSAGE, number=1, message=timestamp_pb2.Timestamp,)
+    end_time = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
+    start_time = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=timestamp_pb2.Timestamp,
+    )
 
 
 class Aggregation(proto.Message):
     r"""Describes how to combine multiple time series to provide a different
     view of the data. Aggregation of time series is done in two steps.
     First, each time series in the set is *aligned* to the same time
     interval boundaries, then the set of time series is optionally
@@ -310,15 +337,28 @@
         REDUCE_FRACTION_TRUE = 8
         REDUCE_PERCENTILE_99 = 9
         REDUCE_PERCENTILE_95 = 10
         REDUCE_PERCENTILE_50 = 11
         REDUCE_PERCENTILE_05 = 12
 
     alignment_period = proto.Field(
-        proto.MESSAGE, number=1, message=duration_pb2.Duration,
+        proto.MESSAGE,
+        number=1,
+        message=duration_pb2.Duration,
+    )
+    per_series_aligner = proto.Field(
+        proto.ENUM,
+        number=2,
+        enum=Aligner,
+    )
+    cross_series_reducer = proto.Field(
+        proto.ENUM,
+        number=4,
+        enum=Reducer,
+    )
+    group_by_fields = proto.RepeatedField(
+        proto.STRING,
+        number=5,
     )
-    per_series_aligner = proto.Field(proto.ENUM, number=2, enum=Aligner,)
-    cross_series_reducer = proto.Field(proto.ENUM, number=4, enum=Reducer,)
-    group_by_fields = proto.RepeatedField(proto.STRING, number=5,)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/dropped_labels.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/dropped_labels.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
-    package="google.monitoring.v3", manifest={"DroppedLabels",},
+    package="google.monitoring.v3",
+    manifest={
+        "DroppedLabels",
+    },
 )
 
 
 class DroppedLabels(proto.Message):
     r"""A set of (label, value) pairs that were removed from a
     Distribution time series during aggregation and then added as an
     attachment to a Distribution.Exemplar.
@@ -37,16 +40,20 @@
 
     Note that there are no guarantees on ordering of the labels from
     exemplar-to-exemplar and from distribution-to-distribution in
     the same stream, and there may be duplicates.  It is up to
     clients to resolve any ambiguities.
 
     Attributes:
-        label (Sequence[google.cloud.monitoring_v3.types.DroppedLabels.LabelEntry]):
+        label (Mapping[str, str]):
             Map from label to its value, for all labels
             dropped in any aggregation.
     """
 
-    label = proto.MapField(proto.STRING, proto.STRING, number=1,)
+    label = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=1,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/group.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/group.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import proto  # type: ignore
 
 
-__protobuf__ = proto.module(package="google.monitoring.v3", manifest={"Group",},)
+__protobuf__ = proto.module(
+    package="google.monitoring.v3",
+    manifest={
+        "Group",
+    },
+)
 
 
 class Group(proto.Message):
     r"""The description of a dynamic collection of monitored resources. Each
     group has a filter that is matched against monitored resources and
     their associated metadata. If a group's filter matches an available
     monitored resource, then that resource is a member of that group.
@@ -78,15 +83,30 @@
         is_cluster (bool):
             If true, the members of this group are
             considered to be a cluster. The system can
             perform additional analysis on groups that are
             clusters.
     """
 
-    name = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=2,)
-    parent_name = proto.Field(proto.STRING, number=3,)
-    filter = proto.Field(proto.STRING, number=5,)
-    is_cluster = proto.Field(proto.BOOL, number=6,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    parent_name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    is_cluster = proto.Field(
+        proto.BOOL,
+        number=6,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/group_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/group_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -99,20 +99,41 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``next_page_token`` value returned by a previous call to
             this method. Using this field causes the method to return
             additional results from the previous method call.
     """
 
-    name = proto.Field(proto.STRING, number=7,)
-    children_of_group = proto.Field(proto.STRING, number=2, oneof="filter",)
-    ancestors_of_group = proto.Field(proto.STRING, number=3, oneof="filter",)
-    descendants_of_group = proto.Field(proto.STRING, number=4, oneof="filter",)
-    page_size = proto.Field(proto.INT32, number=5,)
-    page_token = proto.Field(proto.STRING, number=6,)
+    name = proto.Field(
+        proto.STRING,
+        number=7,
+    )
+    children_of_group = proto.Field(
+        proto.STRING,
+        number=2,
+        oneof="filter",
+    )
+    ancestors_of_group = proto.Field(
+        proto.STRING,
+        number=3,
+        oneof="filter",
+    )
+    descendants_of_group = proto.Field(
+        proto.STRING,
+        number=4,
+        oneof="filter",
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=5,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=6,
+    )
 
 
 class ListGroupsResponse(proto.Message):
     r"""The ``ListGroups`` response.
 
     Attributes:
         group (Sequence[google.cloud.monitoring_v3.types.Group]):
@@ -124,31 +145,41 @@
             to this method.
     """
 
     @property
     def raw_page(self):
         return self
 
-    group = proto.RepeatedField(proto.MESSAGE, number=1, message=gm_group.Group,)
-    next_page_token = proto.Field(proto.STRING, number=2,)
+    group = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message=gm_group.Group,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 class GetGroupRequest(proto.Message):
     r"""The ``GetGroup`` request.
 
     Attributes:
         name (str):
             Required. The group to retrieve. The format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/groups/[GROUP_ID]
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class CreateGroupRequest(proto.Message):
     r"""The ``CreateGroup`` request.
 
     Attributes:
         name (str):
@@ -163,17 +194,27 @@
             Required. A group definition. It is an error to define the
             ``name`` field because the system assigns the name.
         validate_only (bool):
             If true, validate this request but do not
             create the group.
     """
 
-    name = proto.Field(proto.STRING, number=4,)
-    group = proto.Field(proto.MESSAGE, number=2, message=gm_group.Group,)
-    validate_only = proto.Field(proto.BOOL, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    group = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=gm_group.Group,
+    )
+    validate_only = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
 
 
 class UpdateGroupRequest(proto.Message):
     r"""The ``UpdateGroup`` request.
 
     Attributes:
         group (google.cloud.monitoring_v3.types.Group):
@@ -181,16 +222,23 @@
             existing group, excepting ``name``, are replaced with the
             corresponding fields of this group.
         validate_only (bool):
             If true, validate this request but do not
             update the existing group.
     """
 
-    group = proto.Field(proto.MESSAGE, number=2, message=gm_group.Group,)
-    validate_only = proto.Field(proto.BOOL, number=3,)
+    group = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=gm_group.Group,
+    )
+    validate_only = proto.Field(
+        proto.BOOL,
+        number=3,
+    )
 
 
 class DeleteGroupRequest(proto.Message):
     r"""The ``DeleteGroup`` request. The default behavior is to be able to
     delete a single group without any descendants.
 
     Attributes:
@@ -204,16 +252,22 @@
             If this field is true, then the request means
             to delete a group with all its descendants.
             Otherwise, the request means to delete a group
             only when it has no descendants. The default
             value is false.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
-    recursive = proto.Field(proto.BOOL, number=4,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    recursive = proto.Field(
+        proto.BOOL,
+        number=4,
+    )
 
 
 class ListGroupMembersRequest(proto.Message):
     r"""The ``ListGroupMembers`` request.
 
     Attributes:
         name (str):
@@ -247,19 +301,35 @@
             should be returned. Only members that were part
             of the group during the specified interval are
             included in the response.  If no interval is
             provided then the group membership over the last
             minute is returned.
     """
 
-    name = proto.Field(proto.STRING, number=7,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
-    filter = proto.Field(proto.STRING, number=5,)
-    interval = proto.Field(proto.MESSAGE, number=6, message=common.TimeInterval,)
+    name = proto.Field(
+        proto.STRING,
+        number=7,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    interval = proto.Field(
+        proto.MESSAGE,
+        number=6,
+        message=common.TimeInterval,
+    )
 
 
 class ListGroupMembersResponse(proto.Message):
     r"""The ``ListGroupMembers`` response.
 
     Attributes:
         members (Sequence[google.api.monitored_resource_pb2.MonitoredResource]):
@@ -275,14 +345,22 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     members = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=monitored_resource_pb2.MonitoredResource,
+        proto.MESSAGE,
+        number=1,
+        message=monitored_resource_pb2.MonitoredResource,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    total_size = proto.Field(
+        proto.INT32,
+        number=3,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
-    total_size = proto.Field(proto.INT32, number=3,)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/metric.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,16 +51,24 @@
             increasing end times, until an event resets the cumulative
             value to zero and sets a new start time for the following
             points.
         value (google.cloud.monitoring_v3.types.TypedValue):
             The value of the data point.
     """
 
-    interval = proto.Field(proto.MESSAGE, number=1, message=common.TimeInterval,)
-    value = proto.Field(proto.MESSAGE, number=2, message=common.TypedValue,)
+    interval = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=common.TimeInterval,
+    )
+    value = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=common.TypedValue,
+    )
 
 
 class TimeSeries(proto.Message):
     r"""A collection of data points that describes the time-varying
     values of a metric. A time series is identified by a combination
     of a fully-specified monitored resource and a fully-specified
     metric. This type is used for both listing and creating time
@@ -116,31 +124,48 @@
         unit (str):
             The units in which the metric value is reported. It is only
             applicable if the ``value_type`` is ``INT64``, ``DOUBLE``,
             or ``DISTRIBUTION``. The ``unit`` defines the representation
             of the stored metric values.
     """
 
-    metric = proto.Field(proto.MESSAGE, number=1, message=metric_pb2.Metric,)
+    metric = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=metric_pb2.Metric,
+    )
     resource = proto.Field(
-        proto.MESSAGE, number=2, message=monitored_resource_pb2.MonitoredResource,
+        proto.MESSAGE,
+        number=2,
+        message=monitored_resource_pb2.MonitoredResource,
     )
     metadata = proto.Field(
         proto.MESSAGE,
         number=7,
         message=monitored_resource_pb2.MonitoredResourceMetadata,
     )
     metric_kind = proto.Field(
-        proto.ENUM, number=3, enum=metric_pb2.MetricDescriptor.MetricKind,
+        proto.ENUM,
+        number=3,
+        enum=metric_pb2.MetricDescriptor.MetricKind,
     )
     value_type = proto.Field(
-        proto.ENUM, number=4, enum=metric_pb2.MetricDescriptor.ValueType,
+        proto.ENUM,
+        number=4,
+        enum=metric_pb2.MetricDescriptor.ValueType,
+    )
+    points = proto.RepeatedField(
+        proto.MESSAGE,
+        number=5,
+        message="Point",
+    )
+    unit = proto.Field(
+        proto.STRING,
+        number=8,
     )
-    points = proto.RepeatedField(proto.MESSAGE, number=5, message="Point",)
-    unit = proto.Field(proto.STRING, number=8,)
 
 
 class TimeSeriesDescriptor(proto.Message):
     r"""A descriptor for the labels and points in a time series.
 
     Attributes:
         label_descriptors (Sequence[google.api.label_pb2.LabelDescriptor]):
@@ -162,28 +187,42 @@
             unit (str):
                 The unit in which ``time_series`` point values are reported.
                 ``unit`` follows the UCUM format for units as seen in
                 https://unitsofmeasure.org/ucum.html. ``unit`` is only valid
                 if ``value_type`` is INTEGER, DOUBLE, DISTRIBUTION.
         """
 
-        key = proto.Field(proto.STRING, number=1,)
+        key = proto.Field(
+            proto.STRING,
+            number=1,
+        )
         value_type = proto.Field(
-            proto.ENUM, number=2, enum=metric_pb2.MetricDescriptor.ValueType,
+            proto.ENUM,
+            number=2,
+            enum=metric_pb2.MetricDescriptor.ValueType,
         )
         metric_kind = proto.Field(
-            proto.ENUM, number=3, enum=metric_pb2.MetricDescriptor.MetricKind,
+            proto.ENUM,
+            number=3,
+            enum=metric_pb2.MetricDescriptor.MetricKind,
+        )
+        unit = proto.Field(
+            proto.STRING,
+            number=4,
         )
-        unit = proto.Field(proto.STRING, number=4,)
 
     label_descriptors = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=label_pb2.LabelDescriptor,
+        proto.MESSAGE,
+        number=1,
+        message=label_pb2.LabelDescriptor,
     )
     point_descriptors = proto.RepeatedField(
-        proto.MESSAGE, number=5, message=ValueDescriptor,
+        proto.MESSAGE,
+        number=5,
+        message=ValueDescriptor,
     )
 
 
 class TimeSeriesData(proto.Message):
     r"""Represents the values of a time series associated with a
     TimeSeriesDescriptor.
 
@@ -208,22 +247,34 @@
             values (Sequence[google.cloud.monitoring_v3.types.TypedValue]):
                 The values that make up the point.
             time_interval (google.cloud.monitoring_v3.types.TimeInterval):
                 The time interval associated with the point.
         """
 
         values = proto.RepeatedField(
-            proto.MESSAGE, number=1, message=common.TypedValue,
+            proto.MESSAGE,
+            number=1,
+            message=common.TypedValue,
         )
         time_interval = proto.Field(
-            proto.MESSAGE, number=2, message=common.TimeInterval,
+            proto.MESSAGE,
+            number=2,
+            message=common.TimeInterval,
         )
 
-    label_values = proto.RepeatedField(proto.MESSAGE, number=1, message="LabelValue",)
-    point_data = proto.RepeatedField(proto.MESSAGE, number=2, message=PointData,)
+    label_values = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message="LabelValue",
+    )
+    point_data = proto.RepeatedField(
+        proto.MESSAGE,
+        number=2,
+        message=PointData,
+    )
 
 
 class LabelValue(proto.Message):
     r"""A label value.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
@@ -243,33 +294,52 @@
             This field is a member of `oneof`_ ``value``.
         string_value (str):
             A string label value.
 
             This field is a member of `oneof`_ ``value``.
     """
 
-    bool_value = proto.Field(proto.BOOL, number=1, oneof="value",)
-    int64_value = proto.Field(proto.INT64, number=2, oneof="value",)
-    string_value = proto.Field(proto.STRING, number=3, oneof="value",)
+    bool_value = proto.Field(
+        proto.BOOL,
+        number=1,
+        oneof="value",
+    )
+    int64_value = proto.Field(
+        proto.INT64,
+        number=2,
+        oneof="value",
+    )
+    string_value = proto.Field(
+        proto.STRING,
+        number=3,
+        oneof="value",
+    )
 
 
 class QueryError(proto.Message):
     r"""An error associated with a query in the time series query
     language format.
 
     Attributes:
         locator (google.cloud.monitoring_v3.types.TextLocator):
             The location of the time series query
             language text that this error applies to.
         message (str):
             The error message.
     """
 
-    locator = proto.Field(proto.MESSAGE, number=1, message="TextLocator",)
-    message = proto.Field(proto.STRING, number=2,)
+    locator = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message="TextLocator",
+    )
+    message = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 class TextLocator(proto.Message):
     r"""A locator for text. Indicates a particular part of the text of a
     request or of an object referenced in the request.
 
     For example, suppose the request field ``text`` contains:
@@ -324,18 +394,42 @@
                 positioned.
             column (int):
                 The column within the line, starting with 1,
                 where the byte is positioned. This is a byte
                 index even though the text is UTF-8.
         """
 
-        line = proto.Field(proto.INT32, number=1,)
-        column = proto.Field(proto.INT32, number=2,)
+        line = proto.Field(
+            proto.INT32,
+            number=1,
+        )
+        column = proto.Field(
+            proto.INT32,
+            number=2,
+        )
 
-    source = proto.Field(proto.STRING, number=1,)
-    start_position = proto.Field(proto.MESSAGE, number=2, message=Position,)
-    end_position = proto.Field(proto.MESSAGE, number=3, message=Position,)
-    nested_locator = proto.Field(proto.MESSAGE, number=4, message="TextLocator",)
-    nesting_reason = proto.Field(proto.STRING, number=5,)
+    source = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    start_position = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=Position,
+    )
+    end_position = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=Position,
+    )
+    nested_locator = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        message="TextLocator",
+    )
+    nesting_reason = proto.Field(
+        proto.STRING,
+        number=5,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/metric_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/metric_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,18 +74,30 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return
             additional results from the previous method call.
     """
 
-    name = proto.Field(proto.STRING, number=5,)
-    filter = proto.Field(proto.STRING, number=2,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
+    name = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListMonitoredResourceDescriptorsResponse(proto.Message):
     r"""The ``ListMonitoredResourceDescriptors`` response.
 
     Attributes:
         resource_descriptors (Sequence[google.api.monitored_resource_pb2.MonitoredResourceDescriptor]):
@@ -103,15 +115,18 @@
         return self
 
     resource_descriptors = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=monitored_resource_pb2.MonitoredResourceDescriptor,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 class GetMonitoredResourceDescriptorRequest(proto.Message):
     r"""The ``GetMonitoredResourceDescriptor`` request.
 
     Attributes:
         name (str):
@@ -122,15 +137,18 @@
 
                 projects/[PROJECT_ID_OR_NUMBER]/monitoredResourceDescriptors/[RESOURCE_TYPE]
 
             The ``[RESOURCE_TYPE]`` is a predefined type, such as
             ``cloudsql_database``.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class ListMetricDescriptorsRequest(proto.Message):
     r"""The ``ListMetricDescriptors`` request.
 
     Attributes:
         name (str):
@@ -158,18 +176,30 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return
             additional results from the previous method call.
     """
 
-    name = proto.Field(proto.STRING, number=5,)
-    filter = proto.Field(proto.STRING, number=2,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
+    name = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListMetricDescriptorsResponse(proto.Message):
     r"""The ``ListMetricDescriptors`` response.
 
     Attributes:
         metric_descriptors (Sequence[google.api.metric_pb2.MetricDescriptor]):
@@ -183,17 +213,22 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     metric_descriptors = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=metric_pb2.MetricDescriptor,
+        proto.MESSAGE,
+        number=1,
+        message=metric_pb2.MetricDescriptor,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
 
 
 class GetMetricDescriptorRequest(proto.Message):
     r"""The ``GetMetricDescriptor`` request.
 
     Attributes:
         name (str):
@@ -204,15 +239,18 @@
 
                 projects/[PROJECT_ID_OR_NUMBER]/metricDescriptors/[METRIC_ID]
 
             An example value of ``[METRIC_ID]`` is
             ``"compute.googleapis.com/instance/disk/read_bytes_count"``.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class CreateMetricDescriptorRequest(proto.Message):
     r"""The ``CreateMetricDescriptor`` request.
 
     Attributes:
         name (str):
@@ -222,17 +260,22 @@
             projects/[PROJECT_ID_OR_NUMBER]
         metric_descriptor (google.api.metric_pb2.MetricDescriptor):
             Required. The new `custom
             metric <https://cloud.google.com/monitoring/custom-metrics>`__
             descriptor.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
     metric_descriptor = proto.Field(
-        proto.MESSAGE, number=2, message=metric_pb2.MetricDescriptor,
+        proto.MESSAGE,
+        number=2,
+        message=metric_pb2.MetricDescriptor,
     )
 
 
 class DeleteMetricDescriptorRequest(proto.Message):
     r"""The ``DeleteMetricDescriptor`` request.
 
     Attributes:
@@ -244,15 +287,18 @@
 
                 projects/[PROJECT_ID_OR_NUMBER]/metricDescriptors/[METRIC_ID]
 
             An example of ``[METRIC_ID]`` is:
             ``"custom.googleapis.com/my_test_metric"``.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class ListTimeSeriesRequest(proto.Message):
     r"""The ``ListTimeSeries`` request.
 
     Attributes:
         name (str):
@@ -315,25 +361,54 @@
     """
 
     class TimeSeriesView(proto.Enum):
         r"""Controls which fields are returned by ``ListTimeSeries``."""
         FULL = 0
         HEADERS = 1
 
-    name = proto.Field(proto.STRING, number=10,)
-    filter = proto.Field(proto.STRING, number=2,)
-    interval = proto.Field(proto.MESSAGE, number=4, message=common.TimeInterval,)
-    aggregation = proto.Field(proto.MESSAGE, number=5, message=common.Aggregation,)
+    name = proto.Field(
+        proto.STRING,
+        number=10,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    interval = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        message=common.TimeInterval,
+    )
+    aggregation = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message=common.Aggregation,
+    )
     secondary_aggregation = proto.Field(
-        proto.MESSAGE, number=11, message=common.Aggregation,
+        proto.MESSAGE,
+        number=11,
+        message=common.Aggregation,
+    )
+    order_by = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    view = proto.Field(
+        proto.ENUM,
+        number=7,
+        enum=TimeSeriesView,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=8,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=9,
     )
-    order_by = proto.Field(proto.STRING, number=6,)
-    view = proto.Field(proto.ENUM, number=7, enum=TimeSeriesView,)
-    page_size = proto.Field(proto.INT32, number=8,)
-    page_token = proto.Field(proto.STRING, number=9,)
 
 
 class ListTimeSeriesResponse(proto.Message):
     r"""The ``ListTimeSeries`` response.
 
     Attributes:
         time_series (Sequence[google.cloud.monitoring_v3.types.TimeSeries]):
@@ -357,21 +432,31 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     time_series = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=gm_metric.TimeSeries,
+        proto.MESSAGE,
+        number=1,
+        message=gm_metric.TimeSeries,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
     execution_errors = proto.RepeatedField(
-        proto.MESSAGE, number=3, message=status_pb2.Status,
+        proto.MESSAGE,
+        number=3,
+        message=status_pb2.Status,
+    )
+    unit = proto.Field(
+        proto.STRING,
+        number=5,
     )
-    unit = proto.Field(proto.STRING, number=5,)
 
 
 class CreateTimeSeriesRequest(proto.Message):
     r"""The ``CreateTimeSeries`` request.
 
     Attributes:
         name (str):
@@ -390,17 +475,22 @@
             specify a unique time series by supplying all label values
             for the metric and the monitored resource.
 
             The maximum number of ``TimeSeries`` objects per ``Create``
             request is 200.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
     time_series = proto.RepeatedField(
-        proto.MESSAGE, number=2, message=gm_metric.TimeSeries,
+        proto.MESSAGE,
+        number=2,
+        message=gm_metric.TimeSeries,
     )
 
 
 class CreateTimeSeriesError(proto.Message):
     r"""DEPRECATED. Used to hold per-time-series error status.
 
     Attributes:
@@ -408,16 +498,24 @@
             DEPRECATED. Time series ID that resulted in the ``status``
             error.
         status (google.rpc.status_pb2.Status):
             DEPRECATED. The status of the requested write operation for
             ``time_series``.
     """
 
-    time_series = proto.Field(proto.MESSAGE, number=1, message=gm_metric.TimeSeries,)
-    status = proto.Field(proto.MESSAGE, number=2, message=status_pb2.Status,)
+    time_series = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=gm_metric.TimeSeries,
+    )
+    status = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=status_pb2.Status,
+    )
 
 
 class CreateTimeSeriesSummary(proto.Message):
     r"""Summary of the result of a failed request to write data to a
     time series.
 
     Attributes:
@@ -438,20 +536,37 @@
             status (google.rpc.status_pb2.Status):
                 The status of the requested write operation.
             point_count (int):
                 The number of points that couldn't be written because of
                 ``status``.
         """
 
-        status = proto.Field(proto.MESSAGE, number=1, message=status_pb2.Status,)
-        point_count = proto.Field(proto.INT32, number=2,)
+        status = proto.Field(
+            proto.MESSAGE,
+            number=1,
+            message=status_pb2.Status,
+        )
+        point_count = proto.Field(
+            proto.INT32,
+            number=2,
+        )
 
-    total_point_count = proto.Field(proto.INT32, number=1,)
-    success_point_count = proto.Field(proto.INT32, number=2,)
-    errors = proto.RepeatedField(proto.MESSAGE, number=3, message=Error,)
+    total_point_count = proto.Field(
+        proto.INT32,
+        number=1,
+    )
+    success_point_count = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    errors = proto.RepeatedField(
+        proto.MESSAGE,
+        number=3,
+        message=Error,
+    )
 
 
 class QueryTimeSeriesRequest(proto.Message):
     r"""The ``QueryTimeSeries`` request.
 
     Attributes:
         name (str):
@@ -472,18 +587,30 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return
             additional results from the previous method call.
     """
 
-    name = proto.Field(proto.STRING, number=1,)
-    query = proto.Field(proto.STRING, number=7,)
-    page_size = proto.Field(proto.INT32, number=9,)
-    page_token = proto.Field(proto.STRING, number=10,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    query = proto.Field(
+        proto.STRING,
+        number=7,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=9,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=10,
+    )
 
 
 class QueryTimeSeriesResponse(proto.Message):
     r"""The ``QueryTimeSeries`` response.
 
     Attributes:
         time_series_descriptor (google.cloud.monitoring_v3.types.TimeSeriesDescriptor):
@@ -503,22 +630,31 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     time_series_descriptor = proto.Field(
-        proto.MESSAGE, number=8, message=gm_metric.TimeSeriesDescriptor,
+        proto.MESSAGE,
+        number=8,
+        message=gm_metric.TimeSeriesDescriptor,
     )
     time_series_data = proto.RepeatedField(
-        proto.MESSAGE, number=9, message=gm_metric.TimeSeriesData,
+        proto.MESSAGE,
+        number=9,
+        message=gm_metric.TimeSeriesData,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=10,
     )
-    next_page_token = proto.Field(proto.STRING, number=10,)
     partial_errors = proto.RepeatedField(
-        proto.MESSAGE, number=11, message=status_pb2.Status,
+        proto.MESSAGE,
+        number=11,
+        message=status_pb2.Status,
     )
 
 
 class QueryErrorList(proto.Message):
     r"""This is an error detail intended to be used with INVALID_ARGUMENT
     errors.
 
@@ -527,12 +663,19 @@
             Errors in parsing the time series query
             language text. The number of errors in the
             response may be limited.
         error_summary (str):
             A summary of all the errors.
     """
 
-    errors = proto.RepeatedField(proto.MESSAGE, number=1, message=gm_metric.QueryError,)
-    error_summary = proto.Field(proto.STRING, number=2,)
+    errors = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message=gm_metric.QueryError,
+    )
+    error_summary = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/mutation_record.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/mutation_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,27 +15,37 @@
 #
 import proto  # type: ignore
 
 from google.protobuf import timestamp_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
-    package="google.monitoring.v3", manifest={"MutationRecord",},
+    package="google.monitoring.v3",
+    manifest={
+        "MutationRecord",
+    },
 )
 
 
 class MutationRecord(proto.Message):
     r"""Describes a change made to a configuration.
 
     Attributes:
         mutate_time (google.protobuf.timestamp_pb2.Timestamp):
             When the change occurred.
         mutated_by (str):
             The email address of the user making the
             change.
     """
 
-    mutate_time = proto.Field(proto.MESSAGE, number=1, message=timestamp_pb2.Timestamp,)
-    mutated_by = proto.Field(proto.STRING, number=2,)
+    mutate_time = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=timestamp_pb2.Timestamp,
+    )
+    mutated_by = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/notification.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 from google.cloud.monitoring_v3.types import common
 from google.cloud.monitoring_v3.types import mutation_record
 from google.protobuf import wrappers_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.v3",
-    manifest={"NotificationChannelDescriptor", "NotificationChannel",},
+    manifest={
+        "NotificationChannelDescriptor",
+        "NotificationChannel",
+    },
 )
 
 
 class NotificationChannelDescriptor(proto.Message):
     r"""A description of a notification channel. The descriptor
     includes the properties of the channel and the set of labels or
     fields that must be specified to configure channels of a given
@@ -68,25 +71,45 @@
             The tiers that support this notification channel; the
             project service tier must be one of the supported_tiers.
         launch_stage (google.api.launch_stage_pb2.LaunchStage):
             The product launch stage for channels of this
             type.
     """
 
-    name = proto.Field(proto.STRING, number=6,)
-    type_ = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=2,)
-    description = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    type_ = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    description = proto.Field(
+        proto.STRING,
+        number=3,
+    )
     labels = proto.RepeatedField(
-        proto.MESSAGE, number=4, message=label_pb2.LabelDescriptor,
+        proto.MESSAGE,
+        number=4,
+        message=label_pb2.LabelDescriptor,
     )
     supported_tiers = proto.RepeatedField(
-        proto.ENUM, number=5, enum=common.ServiceTier,
+        proto.ENUM,
+        number=5,
+        enum=common.ServiceTier,
+    )
+    launch_stage = proto.Field(
+        proto.ENUM,
+        number=7,
+        enum=launch_stage_pb2.LaunchStage,
     )
-    launch_stage = proto.Field(proto.ENUM, number=7, enum=launch_stage_pb2.LaunchStage,)
 
 
 class NotificationChannel(proto.Message):
     r"""A ``NotificationChannel`` is a medium through which an alert is
     delivered when a policy violation is detected. Examples of channels
     include email, SMS, and third-party messaging applications. Fields
     containing sensitive information like authentication tokens or
@@ -117,22 +140,22 @@
             characters.
         description (str):
             An optional human-readable description of
             this notification channel. This description may
             provide additional details, beyond the display
             name, for the channel. This may not exceed 1024
             Unicode characters.
-        labels (Sequence[google.cloud.monitoring_v3.types.NotificationChannel.LabelsEntry]):
+        labels (Mapping[str, str]):
             Configuration fields that define the channel and its
             behavior. The permissible and required labels are specified
             in the
             [NotificationChannelDescriptor.labels][google.monitoring.v3.NotificationChannelDescriptor.labels]
             of the ``NotificationChannelDescriptor`` corresponding to
             the ``type`` field.
-        user_labels (Sequence[google.cloud.monitoring_v3.types.NotificationChannel.UserLabelsEntry]):
+        user_labels (Mapping[str, str]):
             User-supplied key/value data that does not need to conform
             to the corresponding ``NotificationChannelDescriptor``'s
             schema, unlike the ``labels`` field. This field is intended
             to be used for organizing and identifying the
             ``NotificationChannel`` objects.
 
             The field can contain up to 64 entries. Each key and value
@@ -188,24 +211,56 @@
         [``UpdateNotificationChannel``][google.monitoring.v3.NotificationChannelService.UpdateNotificationChannel]
         operation.
         """
         VERIFICATION_STATUS_UNSPECIFIED = 0
         UNVERIFIED = 1
         VERIFIED = 2
 
-    type_ = proto.Field(proto.STRING, number=1,)
-    name = proto.Field(proto.STRING, number=6,)
-    display_name = proto.Field(proto.STRING, number=3,)
-    description = proto.Field(proto.STRING, number=4,)
-    labels = proto.MapField(proto.STRING, proto.STRING, number=5,)
-    user_labels = proto.MapField(proto.STRING, proto.STRING, number=8,)
-    verification_status = proto.Field(proto.ENUM, number=9, enum=VerificationStatus,)
-    enabled = proto.Field(proto.MESSAGE, number=11, message=wrappers_pb2.BoolValue,)
+    type_ = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    name = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    description = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    labels = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=5,
+    )
+    user_labels = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=8,
+    )
+    verification_status = proto.Field(
+        proto.ENUM,
+        number=9,
+        enum=VerificationStatus,
+    )
+    enabled = proto.Field(
+        proto.MESSAGE,
+        number=11,
+        message=wrappers_pb2.BoolValue,
+    )
     creation_record = proto.Field(
-        proto.MESSAGE, number=12, message=mutation_record.MutationRecord,
+        proto.MESSAGE,
+        number=12,
+        message=mutation_record.MutationRecord,
     )
     mutation_records = proto.RepeatedField(
-        proto.MESSAGE, number=13, message=mutation_record.MutationRecord,
+        proto.MESSAGE,
+        number=13,
+        message=mutation_record.MutationRecord,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/notification_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/notification_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,17 +66,26 @@
             service.
         page_token (str):
             If non-empty, ``page_token`` must contain a value returned
             as the ``next_page_token`` in a previous response to request
             the next set of results.
     """
 
-    name = proto.Field(proto.STRING, number=4,)
-    page_size = proto.Field(proto.INT32, number=2,)
-    page_token = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class ListNotificationChannelDescriptorsResponse(proto.Message):
     r"""The ``ListNotificationChannelDescriptors`` response.
 
     Attributes:
         channel_descriptors (Sequence[google.cloud.monitoring_v3.types.NotificationChannelDescriptor]):
@@ -90,17 +99,22 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     channel_descriptors = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=notification.NotificationChannelDescriptor,
+        proto.MESSAGE,
+        number=1,
+        message=notification.NotificationChannelDescriptor,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
 
 
 class GetNotificationChannelDescriptorRequest(proto.Message):
     r"""The ``GetNotificationChannelDescriptor`` response.
 
     Attributes:
         name (str):
@@ -108,15 +122,18 @@
             The format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/notificationChannelDescriptors/[CHANNEL_TYPE]
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class CreateNotificationChannelRequest(proto.Message):
     r"""The ``CreateNotificationChannel`` request.
 
     Attributes:
         name (str):
@@ -135,17 +152,22 @@
             ``/notificationChannels/[CHANNEL_ID]`` to identify the
             channel.
         notification_channel (google.cloud.monitoring_v3.types.NotificationChannel):
             Required. The definition of the ``NotificationChannel`` to
             create.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
     notification_channel = proto.Field(
-        proto.MESSAGE, number=2, message=notification.NotificationChannel,
+        proto.MESSAGE,
+        number=2,
+        message=notification.NotificationChannel,
     )
 
 
 class ListNotificationChannelsRequest(proto.Message):
     r"""The ``ListNotificationChannels`` request.
 
     Attributes:
@@ -184,19 +206,34 @@
             service.
         page_token (str):
             If non-empty, ``page_token`` must contain a value returned
             as the ``next_page_token`` in a previous response to request
             the next set of results.
     """
 
-    name = proto.Field(proto.STRING, number=5,)
-    filter = proto.Field(proto.STRING, number=6,)
-    order_by = proto.Field(proto.STRING, number=7,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
+    name = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    order_by = proto.Field(
+        proto.STRING,
+        number=7,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListNotificationChannelsResponse(proto.Message):
     r"""The ``ListNotificationChannels`` response.
 
     Attributes:
         notification_channels (Sequence[google.cloud.monitoring_v3.types.NotificationChannel]):
@@ -215,18 +252,26 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     notification_channels = proto.RepeatedField(
-        proto.MESSAGE, number=3, message=notification.NotificationChannel,
+        proto.MESSAGE,
+        number=3,
+        message=notification.NotificationChannel,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    total_size = proto.Field(
+        proto.INT32,
+        number=4,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
-    total_size = proto.Field(proto.INT32, number=4,)
 
 
 class GetNotificationChannelRequest(proto.Message):
     r"""The ``GetNotificationChannel`` request.
 
     Attributes:
         name (str):
@@ -234,15 +279,18 @@
             format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/notificationChannels/[CHANNEL_ID]
     """
 
-    name = proto.Field(proto.STRING, number=3,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class UpdateNotificationChannelRequest(proto.Message):
     r"""The ``UpdateNotificationChannel`` request.
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
@@ -251,18 +299,22 @@
             Required. A description of the changes to be applied to the
             specified notification channel. The description must provide
             a definition for fields to be updated; the names of these
             fields should also be included in the ``update_mask``.
     """
 
     update_mask = proto.Field(
-        proto.MESSAGE, number=2, message=field_mask_pb2.FieldMask,
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
     )
     notification_channel = proto.Field(
-        proto.MESSAGE, number=3, message=notification.NotificationChannel,
+        proto.MESSAGE,
+        number=3,
+        message=notification.NotificationChannel,
     )
 
 
 class DeleteNotificationChannelRequest(proto.Message):
     r"""The ``DeleteNotificationChannel`` request.
 
     Attributes:
@@ -278,28 +330,37 @@
             deleted regardless of its use in alert policies
             (the policies will be updated to remove the
             channel). If false, channels that are still
             referenced by an existing alerting policy will
             fail to be deleted in a delete operation.
     """
 
-    name = proto.Field(proto.STRING, number=3,)
-    force = proto.Field(proto.BOOL, number=5,)
+    name = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    force = proto.Field(
+        proto.BOOL,
+        number=5,
+    )
 
 
 class SendNotificationChannelVerificationCodeRequest(proto.Message):
     r"""The ``SendNotificationChannelVerificationCode`` request.
 
     Attributes:
         name (str):
             Required. The notification channel to which
             to send a verification code.
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 class GetNotificationChannelVerificationCodeRequest(proto.Message):
     r"""The ``GetNotificationChannelVerificationCode`` request.
 
     Attributes:
         name (str):
@@ -321,16 +382,23 @@
             permissible expiration (so specifying an
             expiration may extend the code's lifetime over
             omitting an expiration, even though the API does
             impose an upper limit on the maximum expiration
             that is permitted).
     """
 
-    name = proto.Field(proto.STRING, number=1,)
-    expire_time = proto.Field(proto.MESSAGE, number=2, message=timestamp_pb2.Timestamp,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    expire_time = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
 
 
 class GetNotificationChannelVerificationCodeResponse(proto.Message):
     r"""The ``GetNotificationChannelVerificationCode`` request.
 
     Attributes:
         code (str):
@@ -344,16 +412,23 @@
             The expiration time associated with the code
             that was returned. If an expiration was provided
             in the request, this is the minimum of the
             requested expiration in the request and the max
             permitted expiration.
     """
 
-    code = proto.Field(proto.STRING, number=1,)
-    expire_time = proto.Field(proto.MESSAGE, number=2, message=timestamp_pb2.Timestamp,)
+    code = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    expire_time = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
 
 
 class VerifyNotificationChannelRequest(proto.Message):
     r"""The ``VerifyNotificationChannel`` request.
 
     Attributes:
         name (str):
@@ -366,12 +441,18 @@
             ``GetNotificationChannelVerificationCode``. For example, one
             might have "G-123456" or "TKNZGhhd2EyN3I1MnRnMjRv" (in
             general, one is only guaranteed that the code is valid
             UTF-8; one should not make any assumptions regarding the
             structure or format of the code).
     """
 
-    name = proto.Field(proto.STRING, number=1,)
-    code = proto.Field(proto.STRING, number=2,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    code = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/query_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/query_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,11 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
-__protobuf__ = proto.module(package="google.monitoring.v3", manifest={},)
+__protobuf__ = proto.module(
+    package="google.monitoring.v3",
+    manifest={},
+)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             Metrics for Istio are `documented
             here <https://istio.io/latest/docs/reference/config/metrics/>`__
 
             This field is a member of `oneof`_ ``identifier``.
         telemetry (google.cloud.monitoring_v3.types.Service.Telemetry):
             Configuration for how to query telemetry on a
             Service.
-        user_labels (Sequence[google.cloud.monitoring_v3.types.Service.UserLabelsEntry]):
+        user_labels (Mapping[str, str]):
             Labels which have been used to annotate the
             service. Label keys must start with a letter.
             Label keys and values may contain lowercase
             letters, numbers, underscores, and dashes. Label
             keys and values have a maximum length of 63
             characters, and must be less than 128 bytes in
             size. Up to 64 label entries may be stored. For
@@ -117,29 +117,35 @@
             module_id (str):
                 The ID of the App Engine module underlying this service.
                 Corresponds to the ``module_id`` resource label in the
                 ``gae_app`` monitored resource:
                 https://cloud.google.com/monitoring/api/resources#tag_gae_app
         """
 
-        module_id = proto.Field(proto.STRING, number=1,)
+        module_id = proto.Field(
+            proto.STRING,
+            number=1,
+        )
 
     class CloudEndpoints(proto.Message):
         r"""Cloud Endpoints service. Learn more at
         https://cloud.google.com/endpoints.
 
         Attributes:
             service (str):
                 The name of the Cloud Endpoints service underlying this
                 service. Corresponds to the ``service`` resource label in
                 the ``api`` monitored resource:
                 https://cloud.google.com/monitoring/api/resources#tag_api
         """
 
-        service = proto.Field(proto.STRING, number=1,)
+        service = proto.Field(
+            proto.STRING,
+            number=1,
+        )
 
     class ClusterIstio(proto.Message):
         r"""Istio service scoped to a single Kubernetes cluster. Learn
         more at https://istio.io. Clusters running OSS Istio will have
         their services ingested as this type.
 
         Attributes:
@@ -157,18 +163,30 @@
                 label in Istio metrics.
             service_name (str):
                 The name of the Istio service underlying this service.
                 Corresponds to the ``destination_service_name`` metric label
                 in Istio metrics.
         """
 
-        location = proto.Field(proto.STRING, number=1,)
-        cluster_name = proto.Field(proto.STRING, number=2,)
-        service_namespace = proto.Field(proto.STRING, number=3,)
-        service_name = proto.Field(proto.STRING, number=4,)
+        location = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        cluster_name = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+        service_namespace = proto.Field(
+            proto.STRING,
+            number=3,
+        )
+        service_name = proto.Field(
+            proto.STRING,
+            number=4,
+        )
 
     class MeshIstio(proto.Message):
         r"""Istio service scoped to an Istio mesh. Anthos clusters
         running ASM < 1.6.8 will have their services ingested as this
         type.
 
         Attributes:
@@ -182,17 +200,26 @@
                 label in Istio metrics.
             service_name (str):
                 The name of the Istio service underlying this service.
                 Corresponds to the ``destination_service_name`` metric label
                 in Istio metrics.
         """
 
-        mesh_uid = proto.Field(proto.STRING, number=1,)
-        service_namespace = proto.Field(proto.STRING, number=3,)
-        service_name = proto.Field(proto.STRING, number=4,)
+        mesh_uid = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        service_namespace = proto.Field(
+            proto.STRING,
+            number=3,
+        )
+        service_name = proto.Field(
+            proto.STRING,
+            number=4,
+        )
 
     class IstioCanonicalService(proto.Message):
         r"""Canonical service scoped to an Istio mesh. Anthos clusters
         running ASM >= 1.6.8 will have their services ingested as this
         type.
 
         Attributes:
@@ -210,50 +237,96 @@
             canonical_service (str):
                 The name of the canonical service underlying this service.
                 Corresponds to the ``destination_canonical_service_name``
                 metric label in label in `Istio
                 metrics <https://cloud.google.com/monitoring/api/metrics_istio>`__.
         """
 
-        mesh_uid = proto.Field(proto.STRING, number=1,)
-        canonical_service_namespace = proto.Field(proto.STRING, number=3,)
-        canonical_service = proto.Field(proto.STRING, number=4,)
+        mesh_uid = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        canonical_service_namespace = proto.Field(
+            proto.STRING,
+            number=3,
+        )
+        canonical_service = proto.Field(
+            proto.STRING,
+            number=4,
+        )
 
     class Telemetry(proto.Message):
         r"""Configuration for how to query telemetry on a Service.
 
         Attributes:
             resource_name (str):
                 The full name of the resource that defines this service.
                 Formatted as described in
                 https://cloud.google.com/apis/design/resource_names.
         """
 
-        resource_name = proto.Field(proto.STRING, number=1,)
+        resource_name = proto.Field(
+            proto.STRING,
+            number=1,
+        )
 
-    name = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=2,)
-    custom = proto.Field(proto.MESSAGE, number=6, oneof="identifier", message=Custom,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    custom = proto.Field(
+        proto.MESSAGE,
+        number=6,
+        oneof="identifier",
+        message=Custom,
+    )
     app_engine = proto.Field(
-        proto.MESSAGE, number=7, oneof="identifier", message=AppEngine,
+        proto.MESSAGE,
+        number=7,
+        oneof="identifier",
+        message=AppEngine,
     )
     cloud_endpoints = proto.Field(
-        proto.MESSAGE, number=8, oneof="identifier", message=CloudEndpoints,
+        proto.MESSAGE,
+        number=8,
+        oneof="identifier",
+        message=CloudEndpoints,
     )
     cluster_istio = proto.Field(
-        proto.MESSAGE, number=9, oneof="identifier", message=ClusterIstio,
+        proto.MESSAGE,
+        number=9,
+        oneof="identifier",
+        message=ClusterIstio,
     )
     mesh_istio = proto.Field(
-        proto.MESSAGE, number=10, oneof="identifier", message=MeshIstio,
+        proto.MESSAGE,
+        number=10,
+        oneof="identifier",
+        message=MeshIstio,
     )
     istio_canonical_service = proto.Field(
-        proto.MESSAGE, number=11, oneof="identifier", message=IstioCanonicalService,
+        proto.MESSAGE,
+        number=11,
+        oneof="identifier",
+        message=IstioCanonicalService,
+    )
+    telemetry = proto.Field(
+        proto.MESSAGE,
+        number=13,
+        message=Telemetry,
+    )
+    user_labels = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=14,
     )
-    telemetry = proto.Field(proto.MESSAGE, number=13, message=Telemetry,)
-    user_labels = proto.MapField(proto.STRING, proto.STRING, number=14,)
 
 
 class ServiceLevelObjective(proto.Message):
     r"""A Service-Level Objective (SLO) describes a level of desired
     good service. It consists of a service-level indicator (SLI), a
     performance goal, and a period over which the objective is to be
     evaluated against that goal. The SLO can use SLIs defined in a
@@ -294,15 +367,15 @@
             This field is a member of `oneof`_ ``period``.
         calendar_period (google.type.calendar_period_pb2.CalendarPeriod):
             A calendar period, semantically "since the start of the
             current ``<calendar_period>``". At this time, only ``DAY``,
             ``WEEK``, ``FORTNIGHT``, and ``MONTH`` are supported.
 
             This field is a member of `oneof`_ ``period``.
-        user_labels (Sequence[google.cloud.monitoring_v3.types.ServiceLevelObjective.UserLabelsEntry]):
+        user_labels (Mapping[str, str]):
             Labels which have been used to annotate the
             service-level objective. Label keys must start
             with a letter. Label keys and values may contain
             lowercase letters, numbers, underscores, and
             dashes. Label keys and values have a maximum
             length of 63 characters, and must be less than
             128 bytes in size. Up to 64 label entries may be
@@ -317,27 +390,48 @@
         ``GetServiceLevelObjective``, ``ListServiceLevelObjectives``, and
         ``ListServiceLevelObjectiveVersions`` RPCs.
         """
         VIEW_UNSPECIFIED = 0
         FULL = 2
         EXPLICIT = 1
 
-    name = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=11,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=11,
+    )
     service_level_indicator = proto.Field(
-        proto.MESSAGE, number=3, message="ServiceLevelIndicator",
+        proto.MESSAGE,
+        number=3,
+        message="ServiceLevelIndicator",
+    )
+    goal = proto.Field(
+        proto.DOUBLE,
+        number=4,
     )
-    goal = proto.Field(proto.DOUBLE, number=4,)
     rolling_period = proto.Field(
-        proto.MESSAGE, number=5, oneof="period", message=duration_pb2.Duration,
+        proto.MESSAGE,
+        number=5,
+        oneof="period",
+        message=duration_pb2.Duration,
     )
     calendar_period = proto.Field(
-        proto.ENUM, number=6, oneof="period", enum=calendar_period_pb2.CalendarPeriod,
+        proto.ENUM,
+        number=6,
+        oneof="period",
+        enum=calendar_period_pb2.CalendarPeriod,
+    )
+    user_labels = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=12,
     )
-    user_labels = proto.MapField(proto.STRING, proto.STRING, number=12,)
 
 
 class ServiceLevelIndicator(proto.Message):
     r"""A Service-Level Indicator (SLI) describes the "performance" of a
     service. For some services, the SLI is well-defined. In such cases,
     the SLI can be described easily by referencing the well-known SLI
     and providing the needed parameters. Alternatively, a "custom" SLI
@@ -371,20 +465,31 @@
             This field is a member of `oneof`_ ``type``.
         windows_based (google.cloud.monitoring_v3.types.WindowsBasedSli):
             Windows-based SLIs
 
             This field is a member of `oneof`_ ``type``.
     """
 
-    basic_sli = proto.Field(proto.MESSAGE, number=4, oneof="type", message="BasicSli",)
+    basic_sli = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        oneof="type",
+        message="BasicSli",
+    )
     request_based = proto.Field(
-        proto.MESSAGE, number=1, oneof="type", message="RequestBasedSli",
+        proto.MESSAGE,
+        number=1,
+        oneof="type",
+        message="RequestBasedSli",
     )
     windows_based = proto.Field(
-        proto.MESSAGE, number=2, oneof="type", message="WindowsBasedSli",
+        proto.MESSAGE,
+        number=2,
+        oneof="type",
+        message="WindowsBasedSli",
     )
 
 
 class BasicSli(proto.Message):
     r"""An SLI measuring performance on a well-known service type.
     Performance will be computed on the basis of pre-defined metrics.
     The type of the ``service_resource`` determines the metrics to use
@@ -436,51 +541,75 @@
             this service that are fast enough with respect to
             ``latency.threshold``.
 
             This field is a member of `oneof`_ ``sli_criteria``.
     """
 
     class AvailabilityCriteria(proto.Message):
-        r"""Future parameters for the availability SLI.
-        """
+        r"""Future parameters for the availability SLI."""
 
     class LatencyCriteria(proto.Message):
         r"""Parameters for a latency threshold SLI.
 
         Attributes:
             threshold (google.protobuf.duration_pb2.Duration):
                 Good service is defined to be the count of requests made to
                 this service that return in no more than ``threshold``.
         """
 
-        threshold = proto.Field(proto.MESSAGE, number=3, message=duration_pb2.Duration,)
+        threshold = proto.Field(
+            proto.MESSAGE,
+            number=3,
+            message=duration_pb2.Duration,
+        )
 
-    method = proto.RepeatedField(proto.STRING, number=7,)
-    location = proto.RepeatedField(proto.STRING, number=8,)
-    version = proto.RepeatedField(proto.STRING, number=9,)
+    method = proto.RepeatedField(
+        proto.STRING,
+        number=7,
+    )
+    location = proto.RepeatedField(
+        proto.STRING,
+        number=8,
+    )
+    version = proto.RepeatedField(
+        proto.STRING,
+        number=9,
+    )
     availability = proto.Field(
-        proto.MESSAGE, number=2, oneof="sli_criteria", message=AvailabilityCriteria,
+        proto.MESSAGE,
+        number=2,
+        oneof="sli_criteria",
+        message=AvailabilityCriteria,
     )
     latency = proto.Field(
-        proto.MESSAGE, number=3, oneof="sli_criteria", message=LatencyCriteria,
+        proto.MESSAGE,
+        number=3,
+        oneof="sli_criteria",
+        message=LatencyCriteria,
     )
 
 
 class Range(proto.Message):
     r"""Range of numerical values within ``min`` and ``max``.
 
     Attributes:
         min_ (float):
             Range minimum.
         max_ (float):
             Range maximum.
     """
 
-    min_ = proto.Field(proto.DOUBLE, number=1,)
-    max_ = proto.Field(proto.DOUBLE, number=2,)
+    min_ = proto.Field(
+        proto.DOUBLE,
+        number=1,
+    )
+    max_ = proto.Field(
+        proto.DOUBLE,
+        number=2,
+    )
 
 
 class RequestBasedSli(proto.Message):
     r"""Service Level Indicators for which atomic units of service
     are counted directly.
 
     This message has `oneof`_ fields (mutually exclusive fields).
@@ -503,18 +632,24 @@
             into a good range. The ``total_service`` is the total count
             of all values aggregated in the ``Distribution``.
 
             This field is a member of `oneof`_ ``method``.
     """
 
     good_total_ratio = proto.Field(
-        proto.MESSAGE, number=1, oneof="method", message="TimeSeriesRatio",
+        proto.MESSAGE,
+        number=1,
+        oneof="method",
+        message="TimeSeriesRatio",
     )
     distribution_cut = proto.Field(
-        proto.MESSAGE, number=3, oneof="method", message="DistributionCut",
+        proto.MESSAGE,
+        number=3,
+        oneof="method",
+        message="DistributionCut",
     )
 
 
 class TimeSeriesRatio(proto.Message):
     r"""A ``TimeSeriesRatio`` specifies two ``TimeSeries`` to use for
     computing the ``good_service / total_service`` ratio. The specified
     ``TimeSeries`` must have ``ValueType = DOUBLE`` or
@@ -544,17 +679,26 @@
             filter <https://cloud.google.com/monitoring/api/v3/filters>`__
             specifying a ``TimeSeries`` quantifying total demanded
             service. Must have ``ValueType = DOUBLE`` or
             ``ValueType = INT64`` and must have ``MetricKind = DELTA``
             or ``MetricKind = CUMULATIVE``.
     """
 
-    good_service_filter = proto.Field(proto.STRING, number=4,)
-    bad_service_filter = proto.Field(proto.STRING, number=5,)
-    total_service_filter = proto.Field(proto.STRING, number=6,)
+    good_service_filter = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    bad_service_filter = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+    total_service_filter = proto.Field(
+        proto.STRING,
+        number=6,
+    )
 
 
 class DistributionCut(proto.Message):
     r"""A ``DistributionCut`` defines a ``TimeSeries`` and thresholds used
     for measuring good service and total service. The ``TimeSeries``
     must have ``ValueType = DISTRIBUTION`` and ``MetricKind = DELTA`` or
     ``MetricKind = CUMULATIVE``. The computed ``good_service`` will be
@@ -570,16 +714,23 @@
             ``MetricKind = CUMULATIVE``.
         range_ (google.cloud.monitoring_v3.types.Range):
             Range of values considered "good." For a
             one-sided range, set one bound to an infinite
             value.
     """
 
-    distribution_filter = proto.Field(proto.STRING, number=4,)
-    range_ = proto.Field(proto.MESSAGE, number=5, message="Range",)
+    distribution_filter = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    range_ = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message="Range",
+    )
 
 
 class WindowsBasedSli(proto.Message):
     r"""A ``WindowsBasedSli`` defines ``good_service`` as the count of time
     windows for which the provided service was of good quality. Criteria
     for determining if service was good are embedded in the
     ``window_criterion``.
@@ -640,20 +791,29 @@
                 This field is a member of `oneof`_ ``type``.
             threshold (float):
                 If window ``performance >= threshold``, the window is
                 counted as good.
         """
 
         performance = proto.Field(
-            proto.MESSAGE, number=1, oneof="type", message="RequestBasedSli",
+            proto.MESSAGE,
+            number=1,
+            oneof="type",
+            message="RequestBasedSli",
         )
         basic_sli_performance = proto.Field(
-            proto.MESSAGE, number=3, oneof="type", message="BasicSli",
+            proto.MESSAGE,
+            number=3,
+            oneof="type",
+            message="BasicSli",
+        )
+        threshold = proto.Field(
+            proto.DOUBLE,
+            number=2,
         )
-        threshold = proto.Field(proto.DOUBLE, number=2,)
 
     class MetricRange(proto.Message):
         r"""A ``MetricRange`` is used when each window is good when the value x
         of a single ``TimeSeries`` satisfies
         ``range.min <= x <= range.max``. The provided ``TimeSeries`` must
         have ``ValueType = INT64`` or ``ValueType = DOUBLE`` and
         ``MetricKind = GAUGE``.
@@ -666,26 +826,48 @@
                 quality.
             range_ (google.cloud.monitoring_v3.types.Range):
                 Range of values considered "good." For a
                 one-sided range, set one bound to an infinite
                 value.
         """
 
-        time_series = proto.Field(proto.STRING, number=1,)
-        range_ = proto.Field(proto.MESSAGE, number=4, message="Range",)
+        time_series = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        range_ = proto.Field(
+            proto.MESSAGE,
+            number=4,
+            message="Range",
+        )
 
     good_bad_metric_filter = proto.Field(
-        proto.STRING, number=5, oneof="window_criterion",
+        proto.STRING,
+        number=5,
+        oneof="window_criterion",
     )
     good_total_ratio_threshold = proto.Field(
-        proto.MESSAGE, number=2, oneof="window_criterion", message=PerformanceThreshold,
+        proto.MESSAGE,
+        number=2,
+        oneof="window_criterion",
+        message=PerformanceThreshold,
     )
     metric_mean_in_range = proto.Field(
-        proto.MESSAGE, number=6, oneof="window_criterion", message=MetricRange,
+        proto.MESSAGE,
+        number=6,
+        oneof="window_criterion",
+        message=MetricRange,
     )
     metric_sum_in_range = proto.Field(
-        proto.MESSAGE, number=7, oneof="window_criterion", message=MetricRange,
+        proto.MESSAGE,
+        number=7,
+        oneof="window_criterion",
+        message=MetricRange,
+    )
+    window_period = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        message=duration_pb2.Duration,
     )
-    window_period = proto.Field(proto.MESSAGE, number=4, message=duration_pb2.Duration,)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/service_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/service_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,32 +54,45 @@
             Optional. The Service id to use for this Service. If
             omitted, an id will be generated instead. Must match the
             pattern ``[a-z0-9\-]+``
         service (google.cloud.monitoring_v3.types.Service):
             Required. The ``Service`` to create.
     """
 
-    parent = proto.Field(proto.STRING, number=1,)
-    service_id = proto.Field(proto.STRING, number=3,)
-    service = proto.Field(proto.MESSAGE, number=2, message=gm_service.Service,)
+    parent = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    service_id = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    service = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=gm_service.Service,
+    )
 
 
 class GetServiceRequest(proto.Message):
     r"""The ``GetService`` request.
 
     Attributes:
         name (str):
             Required. Resource name of the ``Service``. The format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/services/[SERVICE_ID]
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 class ListServicesRequest(proto.Message):
     r"""The ``ListServices`` request.
 
     Attributes:
         parent (str):
@@ -123,18 +136,30 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return
             additional results from the previous method call.
     """
 
-    parent = proto.Field(proto.STRING, number=1,)
-    filter = proto.Field(proto.STRING, number=2,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
+    parent = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListServicesResponse(proto.Message):
     r"""The ``ListServices`` response.
 
     Attributes:
         services (Sequence[google.cloud.monitoring_v3.types.Service]):
@@ -146,33 +171,46 @@
             to this method.
     """
 
     @property
     def raw_page(self):
         return self
 
-    services = proto.RepeatedField(proto.MESSAGE, number=1, message=gm_service.Service,)
-    next_page_token = proto.Field(proto.STRING, number=2,)
+    services = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message=gm_service.Service,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
 
 
 class UpdateServiceRequest(proto.Message):
     r"""The ``UpdateService`` request.
 
     Attributes:
         service (google.cloud.monitoring_v3.types.Service):
             Required. The ``Service`` to draw updates from. The given
             ``name`` specifies the resource to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             A set of field paths defining which fields to
             use for the update.
     """
 
-    service = proto.Field(proto.MESSAGE, number=1, message=gm_service.Service,)
+    service = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=gm_service.Service,
+    )
     update_mask = proto.Field(
-        proto.MESSAGE, number=2, message=field_mask_pb2.FieldMask,
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
     )
 
 
 class DeleteServiceRequest(proto.Message):
     r"""The ``DeleteService`` request.
 
     Attributes:
@@ -181,15 +219,18 @@
             format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/services/[SERVICE_ID]
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 class CreateServiceLevelObjectiveRequest(proto.Message):
     r"""The ``CreateServiceLevelObjective`` request.
 
     Attributes:
         parent (str):
@@ -205,18 +246,26 @@
             instead. Must match the pattern ``[a-z0-9\-]+``
         service_level_objective (google.cloud.monitoring_v3.types.ServiceLevelObjective):
             Required. The ``ServiceLevelObjective`` to create. The
             provided ``name`` will be respected if no
             ``ServiceLevelObjective`` exists with this name.
     """
 
-    parent = proto.Field(proto.STRING, number=1,)
-    service_level_objective_id = proto.Field(proto.STRING, number=3,)
+    parent = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    service_level_objective_id = proto.Field(
+        proto.STRING,
+        number=3,
+    )
     service_level_objective = proto.Field(
-        proto.MESSAGE, number=2, message=gm_service.ServiceLevelObjective,
+        proto.MESSAGE,
+        number=2,
+        message=gm_service.ServiceLevelObjective,
     )
 
 
 class GetServiceLevelObjectiveRequest(proto.Message):
     r"""The ``GetServiceLevelObjective`` request.
 
     Attributes:
@@ -232,17 +281,22 @@
             ``DEFAULT``, return the ``ServiceLevelObjective`` as
             originally defined. If ``EXPLICIT`` and the
             ``ServiceLevelObjective`` is defined in terms of a
             ``BasicSli``, replace the ``BasicSli`` with a
             ``RequestBasedSli`` spelling out how the SLI is computed.
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
     view = proto.Field(
-        proto.ENUM, number=2, enum=gm_service.ServiceLevelObjective.View,
+        proto.ENUM,
+        number=2,
+        enum=gm_service.ServiceLevelObjective.View,
     )
 
 
 class ListServiceLevelObjectivesRequest(proto.Message):
     r"""The ``ListServiceLevelObjectives`` request.
 
     Attributes:
@@ -272,20 +326,34 @@
             ``DEFAULT``, return each ``ServiceLevelObjective`` as
             originally defined. If ``EXPLICIT`` and the
             ``ServiceLevelObjective`` is defined in terms of a
             ``BasicSli``, replace the ``BasicSli`` with a
             ``RequestBasedSli`` spelling out how the SLI is computed.
     """
 
-    parent = proto.Field(proto.STRING, number=1,)
-    filter = proto.Field(proto.STRING, number=2,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
+    parent = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    filter = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
     view = proto.Field(
-        proto.ENUM, number=5, enum=gm_service.ServiceLevelObjective.View,
+        proto.ENUM,
+        number=5,
+        enum=gm_service.ServiceLevelObjective.View,
     )
 
 
 class ListServiceLevelObjectivesResponse(proto.Message):
     r"""The ``ListServiceLevelObjectives`` response.
 
     Attributes:
@@ -300,17 +368,22 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     service_level_objectives = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=gm_service.ServiceLevelObjective,
+        proto.MESSAGE,
+        number=1,
+        message=gm_service.ServiceLevelObjective,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
 
 
 class UpdateServiceLevelObjectiveRequest(proto.Message):
     r"""The ``UpdateServiceLevelObjective`` request.
 
     Attributes:
         service_level_objective (google.cloud.monitoring_v3.types.ServiceLevelObjective):
@@ -318,18 +391,22 @@
             from. The given ``name`` specifies the resource to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             A set of field paths defining which fields to
             use for the update.
     """
 
     service_level_objective = proto.Field(
-        proto.MESSAGE, number=1, message=gm_service.ServiceLevelObjective,
+        proto.MESSAGE,
+        number=1,
+        message=gm_service.ServiceLevelObjective,
     )
     update_mask = proto.Field(
-        proto.MESSAGE, number=2, message=field_mask_pb2.FieldMask,
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
     )
 
 
 class DeleteServiceLevelObjectiveRequest(proto.Message):
     r"""The ``DeleteServiceLevelObjective`` request.
 
     Attributes:
@@ -338,11 +415,14 @@
             delete. The format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/services/[SERVICE_ID]/serviceLevelObjectives/[SLO_NAME]
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/span_context.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/span_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import proto  # type: ignore
 
 
-__protobuf__ = proto.module(package="google.monitoring.v3", manifest={"SpanContext",},)
+__protobuf__ = proto.module(
+    package="google.monitoring.v3",
+    manifest={
+        "SpanContext",
+    },
+)
 
 
 class SpanContext(proto.Message):
     r"""The context of a span. This is attached to an
     [Exemplar][google.api.Distribution.Exemplar] in
     [Distribution][google.api.Distribution] values during aggregation.
 
@@ -43,11 +48,14 @@
             16-byte array.
 
             ``[SPAN_ID]`` is a unique identifier for a span within a
             trace; it is a 16-character hexadecimal encoding of an
             8-byte array.
     """
 
-    span_name = proto.Field(proto.STRING, number=1,)
+    span_name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/uptime.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/uptime.py`

 * *Files 11% similar despite different names*

```diff
@@ -93,20 +93,39 @@
 
     class State(proto.Enum):
         r"""Operational states for an internal checker."""
         UNSPECIFIED = 0
         CREATING = 1
         RUNNING = 2
 
-    name = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=2,)
-    network = proto.Field(proto.STRING, number=3,)
-    gcp_zone = proto.Field(proto.STRING, number=4,)
-    peer_project_id = proto.Field(proto.STRING, number=6,)
-    state = proto.Field(proto.ENUM, number=7, enum=State,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    network = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    gcp_zone = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    peer_project_id = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    state = proto.Field(
+        proto.ENUM,
+        number=7,
+        enum=State,
+    )
 
 
 class UptimeCheckConfig(proto.Message):
     r"""This message configures which resources and services to
     monitor for availability.
 
     This message has `oneof`_ fields (mutually exclusive fields).
@@ -209,16 +228,23 @@
                 The group of resources being monitored. Should be only the
                 ``[GROUP_ID]``, and not the full-path
                 ``projects/[PROJECT_ID_OR_NUMBER]/groups/[GROUP_ID]``.
             resource_type (google.cloud.monitoring_v3.types.GroupResourceType):
                 The resource type of the group members.
         """
 
-        group_id = proto.Field(proto.STRING, number=1,)
-        resource_type = proto.Field(proto.ENUM, number=2, enum="GroupResourceType",)
+        group_id = proto.Field(
+            proto.STRING,
+            number=1,
+        )
+        resource_type = proto.Field(
+            proto.ENUM,
+            number=2,
+            enum="GroupResourceType",
+        )
 
     class HttpCheck(proto.Message):
         r"""Information involved in an HTTP/HTTPS Uptime check request.
 
         Attributes:
             request_method (google.cloud.monitoring_v3.types.UptimeCheckConfig.HttpCheck.RequestMethod):
                 The HTTP request method to use for the check. If set to
@@ -245,15 +271,15 @@
                 Boolean specifying whether to encrypt the header
                 information. Encryption should be specified for any headers
                 related to authentication that you do not wish to be seen
                 when retrieving the configuration. The server will be
                 responsible for encrypting the headers. On Get/List calls,
                 if ``mask_headers`` is set to ``true`` then the headers will
                 be obscured with ``******.``
-            headers (Sequence[google.cloud.monitoring_v3.types.UptimeCheckConfig.HttpCheck.HeadersEntry]):
+            headers (Mapping[str, str]):
                 The list of headers to send as part of the
                 Uptime check request. If two headers have the
                 same key and different values, they should be
                 entered as a single header, with the value being
                 a comma-separated list of all the desired values
                 as described at
                 https://www.w3.org/Protocols/rfc2616/rfc2616.txt
@@ -317,47 +343,82 @@
                     The username to use when authenticating with
                     the HTTP server.
                 password (str):
                     The password to use when authenticating with
                     the HTTP server.
             """
 
-            username = proto.Field(proto.STRING, number=1,)
-            password = proto.Field(proto.STRING, number=2,)
+            username = proto.Field(
+                proto.STRING,
+                number=1,
+            )
+            password = proto.Field(
+                proto.STRING,
+                number=2,
+            )
 
         request_method = proto.Field(
-            proto.ENUM, number=8, enum="UptimeCheckConfig.HttpCheck.RequestMethod",
+            proto.ENUM,
+            number=8,
+            enum="UptimeCheckConfig.HttpCheck.RequestMethod",
+        )
+        use_ssl = proto.Field(
+            proto.BOOL,
+            number=1,
+        )
+        path = proto.Field(
+            proto.STRING,
+            number=2,
+        )
+        port = proto.Field(
+            proto.INT32,
+            number=3,
         )
-        use_ssl = proto.Field(proto.BOOL, number=1,)
-        path = proto.Field(proto.STRING, number=2,)
-        port = proto.Field(proto.INT32, number=3,)
         auth_info = proto.Field(
             proto.MESSAGE,
             number=4,
             message="UptimeCheckConfig.HttpCheck.BasicAuthentication",
         )
-        mask_headers = proto.Field(proto.BOOL, number=5,)
-        headers = proto.MapField(proto.STRING, proto.STRING, number=6,)
+        mask_headers = proto.Field(
+            proto.BOOL,
+            number=5,
+        )
+        headers = proto.MapField(
+            proto.STRING,
+            proto.STRING,
+            number=6,
+        )
         content_type = proto.Field(
-            proto.ENUM, number=9, enum="UptimeCheckConfig.HttpCheck.ContentType",
+            proto.ENUM,
+            number=9,
+            enum="UptimeCheckConfig.HttpCheck.ContentType",
+        )
+        validate_ssl = proto.Field(
+            proto.BOOL,
+            number=7,
+        )
+        body = proto.Field(
+            proto.BYTES,
+            number=10,
         )
-        validate_ssl = proto.Field(proto.BOOL, number=7,)
-        body = proto.Field(proto.BYTES, number=10,)
 
     class TcpCheck(proto.Message):
         r"""Information required for a TCP Uptime check request.
 
         Attributes:
             port (int):
                 The TCP port on the server against which to run the check.
                 Will be combined with host (specified within the
                 ``monitored_resource``) to construct the full URL. Required.
         """
 
-        port = proto.Field(proto.INT32, number=1,)
+        port = proto.Field(
+            proto.INT32,
+            number=1,
+        )
 
     class ContentMatcher(proto.Message):
         r"""Optional. Used to perform content matching. This allows
         matching based on substrings and regular expressions, together
         with their negations. Only the first 4&nbsp;MB of an HTTP or
         HTTPS check's response (and the first 1&nbsp;MB of a TCP check's
         response) are examined for purposes of content matching.
@@ -377,49 +438,84 @@
             r"""Options to perform content matching."""
             CONTENT_MATCHER_OPTION_UNSPECIFIED = 0
             CONTAINS_STRING = 1
             NOT_CONTAINS_STRING = 2
             MATCHES_REGEX = 3
             NOT_MATCHES_REGEX = 4
 
-        content = proto.Field(proto.STRING, number=1,)
+        content = proto.Field(
+            proto.STRING,
+            number=1,
+        )
         matcher = proto.Field(
             proto.ENUM,
             number=2,
             enum="UptimeCheckConfig.ContentMatcher.ContentMatcherOption",
         )
 
-    name = proto.Field(proto.STRING, number=1,)
-    display_name = proto.Field(proto.STRING, number=2,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    display_name = proto.Field(
+        proto.STRING,
+        number=2,
+    )
     monitored_resource = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="resource",
         message=monitored_resource_pb2.MonitoredResource,
     )
     resource_group = proto.Field(
-        proto.MESSAGE, number=4, oneof="resource", message=ResourceGroup,
+        proto.MESSAGE,
+        number=4,
+        oneof="resource",
+        message=ResourceGroup,
     )
     http_check = proto.Field(
-        proto.MESSAGE, number=5, oneof="check_request_type", message=HttpCheck,
+        proto.MESSAGE,
+        number=5,
+        oneof="check_request_type",
+        message=HttpCheck,
     )
     tcp_check = proto.Field(
-        proto.MESSAGE, number=6, oneof="check_request_type", message=TcpCheck,
+        proto.MESSAGE,
+        number=6,
+        oneof="check_request_type",
+        message=TcpCheck,
+    )
+    period = proto.Field(
+        proto.MESSAGE,
+        number=7,
+        message=duration_pb2.Duration,
+    )
+    timeout = proto.Field(
+        proto.MESSAGE,
+        number=8,
+        message=duration_pb2.Duration,
     )
-    period = proto.Field(proto.MESSAGE, number=7, message=duration_pb2.Duration,)
-    timeout = proto.Field(proto.MESSAGE, number=8, message=duration_pb2.Duration,)
     content_matchers = proto.RepeatedField(
-        proto.MESSAGE, number=9, message=ContentMatcher,
+        proto.MESSAGE,
+        number=9,
+        message=ContentMatcher,
     )
     selected_regions = proto.RepeatedField(
-        proto.ENUM, number=10, enum="UptimeCheckRegion",
+        proto.ENUM,
+        number=10,
+        enum="UptimeCheckRegion",
+    )
+    is_internal = proto.Field(
+        proto.BOOL,
+        number=15,
     )
-    is_internal = proto.Field(proto.BOOL, number=15,)
     internal_checkers = proto.RepeatedField(
-        proto.MESSAGE, number=14, message="InternalChecker",
+        proto.MESSAGE,
+        number=14,
+        message="InternalChecker",
     )
 
 
 class UptimeCheckIp(proto.Message):
     r"""Contains the region, location, and list of IP
     addresses where checkers in the location run from.
 
@@ -440,13 +536,23 @@
             of this publication, are in IPv4 format;
             however, one should not rely on the IP addresses
             being in IPv4 format indefinitely, and should
             support interpreting this field in either IPv4
             or IPv6 format.
     """
 
-    region = proto.Field(proto.ENUM, number=1, enum="UptimeCheckRegion",)
-    location = proto.Field(proto.STRING, number=2,)
-    ip_address = proto.Field(proto.STRING, number=3,)
+    region = proto.Field(
+        proto.ENUM,
+        number=1,
+        enum="UptimeCheckRegion",
+    )
+    location = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    ip_address = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google/cloud/monitoring_v3/types/uptime_service.py` & `google-cloud-monitoring-2.9.2/google/cloud/monitoring_v3/types/uptime_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,17 +55,26 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return more
             results from the previous method call.
     """
 
-    parent = proto.Field(proto.STRING, number=1,)
-    page_size = proto.Field(proto.INT32, number=3,)
-    page_token = proto.Field(proto.STRING, number=4,)
+    parent = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    page_size = proto.Field(
+        proto.INT32,
+        number=3,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListUptimeCheckConfigsResponse(proto.Message):
     r"""The protocol for the ``ListUptimeCheckConfigs`` response.
 
     Attributes:
         uptime_check_configs (Sequence[google.cloud.monitoring_v3.types.UptimeCheckConfig]):
@@ -84,18 +93,26 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     uptime_check_configs = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=uptime.UptimeCheckConfig,
+        proto.MESSAGE,
+        number=1,
+        message=uptime.UptimeCheckConfig,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    total_size = proto.Field(
+        proto.INT32,
+        number=3,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
-    total_size = proto.Field(proto.INT32, number=3,)
 
 
 class GetUptimeCheckConfigRequest(proto.Message):
     r"""The protocol for the ``GetUptimeCheckConfig`` request.
 
     Attributes:
         name (str):
@@ -103,15 +120,18 @@
             format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/uptimeCheckConfigs/[UPTIME_CHECK_ID]
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 class CreateUptimeCheckConfigRequest(proto.Message):
     r"""The protocol for the ``CreateUptimeCheckConfig`` request.
 
     Attributes:
         parent (str):
@@ -122,17 +142,22 @@
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]
         uptime_check_config (google.cloud.monitoring_v3.types.UptimeCheckConfig):
             Required. The new Uptime check configuration.
     """
 
-    parent = proto.Field(proto.STRING, number=1,)
+    parent = proto.Field(
+        proto.STRING,
+        number=1,
+    )
     uptime_check_config = proto.Field(
-        proto.MESSAGE, number=2, message=uptime.UptimeCheckConfig,
+        proto.MESSAGE,
+        number=2,
+        message=uptime.UptimeCheckConfig,
     )
 
 
 class UpdateUptimeCheckConfigRequest(proto.Message):
     r"""The protocol for the ``UpdateUptimeCheckConfig`` request.
 
     Attributes:
@@ -155,18 +180,22 @@
 
             The following fields can be updated: ``display_name``,
             ``http_check``, ``tcp_check``, ``timeout``,
             ``content_matchers``, and ``selected_regions``.
     """
 
     update_mask = proto.Field(
-        proto.MESSAGE, number=2, message=field_mask_pb2.FieldMask,
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
     )
     uptime_check_config = proto.Field(
-        proto.MESSAGE, number=3, message=uptime.UptimeCheckConfig,
+        proto.MESSAGE,
+        number=3,
+        message=uptime.UptimeCheckConfig,
     )
 
 
 class DeleteUptimeCheckConfigRequest(proto.Message):
     r"""The protocol for the ``DeleteUptimeCheckConfig`` request.
 
     Attributes:
@@ -175,15 +204,18 @@
             format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/uptimeCheckConfigs/[UPTIME_CHECK_ID]
     """
 
-    name = proto.Field(proto.STRING, number=1,)
+    name = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 class ListUptimeCheckIpsRequest(proto.Message):
     r"""The protocol for the ``ListUptimeCheckIps`` request.
 
     Attributes:
         page_size (int):
@@ -197,16 +229,22 @@
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return more
             results from the previous method call. NOTE: this field is
             not yet implemented
     """
 
-    page_size = proto.Field(proto.INT32, number=2,)
-    page_token = proto.Field(proto.STRING, number=3,)
+    page_size = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token = proto.Field(
+        proto.STRING,
+        number=3,
+    )
 
 
 class ListUptimeCheckIpsResponse(proto.Message):
     r"""The protocol for the ``ListUptimeCheckIps`` response.
 
     Attributes:
         uptime_check_ips (Sequence[google.cloud.monitoring_v3.types.UptimeCheckIp]):
@@ -222,13 +260,18 @@
     """
 
     @property
     def raw_page(self):
         return self
 
     uptime_check_ips = proto.RepeatedField(
-        proto.MESSAGE, number=1, message=uptime.UptimeCheckIp,
+        proto.MESSAGE,
+        number=1,
+        message=uptime.UptimeCheckIp,
+    )
+    next_page_token = proto.Field(
+        proto.STRING,
+        number=2,
     )
-    next_page_token = proto.Field(proto.STRING, number=2,)
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/PKG-INFO` & `google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-monitoring
-Version: 2.9.1
+Version: 2.9.2
 Summary: Stackdriver Monitoring API client library
 Home-page: https://github.com/googleapis/python-monitoring
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -109,9 +109,7 @@
 ~~~~~~~~~~
 
 
 -  Read the `Client Library Documentation`_ for Cloud Monitoring API
    to see other available methods on the client.
 -  Read the `Product documentation`_ to learn more about the product and see
    How-to Guides.
-
-
```

### Comparing `google-cloud-monitoring-2.9.1/google_cloud_monitoring.egg-info/SOURCES.txt` & `google-cloud-monitoring-2.9.2/google_cloud_monitoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/scripts/fixup_monitoring_v3_keywords.py` & `google-cloud-monitoring-2.9.2/scripts/fixup_monitoring_v3_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/setup.py` & `google-cloud-monitoring-2.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,27 @@
 import setuptools
 
 
 # Package metadata.
 
 name = "google-cloud-monitoring"
 description = "Stackdriver Monitoring API client library"
-version = "2.9.1"
+version = "2.9.2"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
-    "proto-plus >= 1.15.0",
+    "proto-plus >= 1.15.0, <2.0.0dev",
+    "protobuf >= 3.19.0, <4.0.0dev",
 ]
 extras = {"pandas": "pandas >= 0.17.1"}
 
 
 # Setup boilerplate below this line.
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-monitoring-2.9.1/tests/__init__.py` & `google-cloud-monitoring-2.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/system/gapic/v3/test_system_metric_service_v3.py` & `google-cloud-monitoring-2.9.2/tests/system/gapic/v3/test_system_metric_service_v3.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/system/test_vpcsc_v3.py` & `google-cloud-monitoring-2.9.2/tests/system/test_vpcsc_v3.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/__init__.py` & `google-cloud-monitoring-2.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/__init__.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/__init__.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_alert_policy_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_alert_policy_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -95,28 +101,34 @@
     assert (
         AlertPolicyServiceClient._get_default_mtls_endpoint(non_googleapi)
         == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class", [AlertPolicyServiceClient, AlertPolicyServiceAsyncClient,]
+    "client_class,transport_name",
+    [
+        (AlertPolicyServiceClient, "grpc"),
+        (AlertPolicyServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_alert_policy_service_client_from_service_account_info(client_class):
+def test_alert_policy_service_client_from_service_account_info(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.AlertPolicyServiceGrpcTransport, "grpc"),
         (transports.AlertPolicyServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -137,31 +149,41 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class", [AlertPolicyServiceClient, AlertPolicyServiceAsyncClient,]
+    "client_class,transport_name",
+    [
+        (AlertPolicyServiceClient, "grpc"),
+        (AlertPolicyServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_alert_policy_service_client_from_service_account_file(client_class):
+def test_alert_policy_service_client_from_service_account_file(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_alert_policy_service_client_get_transport_class():
     transport = AlertPolicyServiceClient.get_transport_class()
     available_transports = [
         transports.AlertPolicyServiceGrpcTransport,
     ]
@@ -511,15 +533,17 @@
         ),
     ],
 )
 def test_alert_policy_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -656,32 +680,38 @@
                 ("grpc.max_send_message_length", -1),
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [alert_service.ListAlertPoliciesRequest, dict,]
+    "request_type",
+    [
+        alert_service.ListAlertPoliciesRequest,
+        dict,
+    ],
 )
 def test_list_alert_policies(request_type, transport: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = alert_service.ListAlertPoliciesResponse(
-            next_page_token="next_page_token_value", total_size=1086,
+            next_page_token="next_page_token_value",
+            total_size=1086,
         )
         response = client.list_alert_policies(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == alert_service.ListAlertPoliciesRequest()
@@ -692,15 +722,16 @@
     assert response.total_size == 1086
 
 
 def test_list_alert_policies_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         client.list_alert_policies()
@@ -710,29 +741,31 @@
 
 
 @pytest.mark.asyncio
 async def test_list_alert_policies_async(
     transport: str = "grpc_asyncio", request_type=alert_service.ListAlertPoliciesRequest
 ):
     client = AlertPolicyServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             alert_service.ListAlertPoliciesResponse(
-                next_page_token="next_page_token_value", total_size=1086,
+                next_page_token="next_page_token_value",
+                total_size=1086,
             )
         )
         response = await client.list_alert_policies(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -754,15 +787,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.ListAlertPoliciesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         call.return_value = alert_service.ListAlertPoliciesResponse()
         client.list_alert_policies(request)
@@ -770,28 +803,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_alert_policies_field_headers_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.ListAlertPoliciesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             alert_service.ListAlertPoliciesResponse()
@@ -801,15 +837,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_alert_policies_flattened():
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -817,15 +856,17 @@
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = alert_service.ListAlertPoliciesResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_alert_policies(name="name_value",)
+        client.list_alert_policies(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -837,15 +878,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_alert_policies(
-            alert_service.ListAlertPoliciesRequest(), name="name_value",
+            alert_service.ListAlertPoliciesRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_alert_policies_flattened_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -859,15 +901,17 @@
         call.return_value = alert_service.ListAlertPoliciesResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             alert_service.ListAlertPoliciesResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_alert_policies(name="name_value",)
+        response = await client.list_alert_policies(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -880,21 +924,23 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_alert_policies(
-            alert_service.ListAlertPoliciesRequest(), name="name_value",
+            alert_service.ListAlertPoliciesRequest(),
+            name="name_value",
         )
 
 
 def test_list_alert_policies_pager(transport_name: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -904,41 +950,49 @@
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                 ],
                 next_page_token="abc",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[], next_page_token="def",
+                alert_policies=[],
+                next_page_token="def",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(),], next_page_token="ghi",
+                alert_policies=[
+                    alert.AlertPolicy(),
+                ],
+                next_page_token="ghi",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(), alert.AlertPolicy(),],
+                alert_policies=[
+                    alert.AlertPolicy(),
+                    alert.AlertPolicy(),
+                ],
             ),
             RuntimeError,
         )
 
         metadata = ()
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_alert_policies(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, alert.AlertPolicy) for i in results)
 
 
 def test_list_alert_policies_pages(transport_name: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_alert_policies), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -948,21 +1002,28 @@
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                 ],
                 next_page_token="abc",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[], next_page_token="def",
+                alert_policies=[],
+                next_page_token="def",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(),], next_page_token="ghi",
+                alert_policies=[
+                    alert.AlertPolicy(),
+                ],
+                next_page_token="ghi",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(), alert.AlertPolicy(),],
+                alert_policies=[
+                    alert.AlertPolicy(),
+                    alert.AlertPolicy(),
+                ],
             ),
             RuntimeError,
         )
         pages = list(client.list_alert_policies(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
@@ -986,28 +1047,37 @@
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                 ],
                 next_page_token="abc",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[], next_page_token="def",
+                alert_policies=[],
+                next_page_token="def",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(),], next_page_token="ghi",
+                alert_policies=[
+                    alert.AlertPolicy(),
+                ],
+                next_page_token="ghi",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(), alert.AlertPolicy(),],
+                alert_policies=[
+                    alert.AlertPolicy(),
+                    alert.AlertPolicy(),
+                ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_alert_policies(request={},)
+        async_pager = await client.list_alert_policies(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, alert.AlertPolicy) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -1029,35 +1099,51 @@
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                     alert.AlertPolicy(),
                 ],
                 next_page_token="abc",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[], next_page_token="def",
+                alert_policies=[],
+                next_page_token="def",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(),], next_page_token="ghi",
+                alert_policies=[
+                    alert.AlertPolicy(),
+                ],
+                next_page_token="ghi",
             ),
             alert_service.ListAlertPoliciesResponse(
-                alert_policies=[alert.AlertPolicy(), alert.AlertPolicy(),],
+                alert_policies=[
+                    alert.AlertPolicy(),
+                    alert.AlertPolicy(),
+                ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_alert_policies(request={})).pages:
+        async for page_ in (
+            await client.list_alert_policies(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
-@pytest.mark.parametrize("request_type", [alert_service.GetAlertPolicyRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        alert_service.GetAlertPolicyRequest,
+        dict,
+    ],
+)
 def test_get_alert_policy(request_type, transport: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1084,15 +1170,16 @@
     assert response.notification_channels == ["notification_channels_value"]
 
 
 def test_get_alert_policy_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_alert_policy), "__call__") as call:
         client.get_alert_policy()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1100,15 +1187,16 @@
 
 
 @pytest.mark.asyncio
 async def test_get_alert_policy_async(
     transport: str = "grpc_asyncio", request_type=alert_service.GetAlertPolicyRequest
 ):
     client = AlertPolicyServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1147,70 +1235,78 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.GetAlertPolicyRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_alert_policy), "__call__") as call:
         call.return_value = alert.AlertPolicy()
         client.get_alert_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_alert_policy_field_headers_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.GetAlertPolicyRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_alert_policy), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(alert.AlertPolicy())
         await client.get_alert_policy(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_alert_policy_flattened():
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_alert_policy), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = alert.AlertPolicy()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_alert_policy(name="name_value",)
+        client.get_alert_policy(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1222,15 +1318,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_alert_policy(
-            alert_service.GetAlertPolicyRequest(), name="name_value",
+            alert_service.GetAlertPolicyRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_alert_policy_flattened_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1240,15 +1337,17 @@
     with mock.patch.object(type(client.transport.get_alert_policy), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = alert.AlertPolicy()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(alert.AlertPolicy())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_alert_policy(name="name_value",)
+        response = await client.get_alert_policy(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1261,24 +1360,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_alert_policy(
-            alert_service.GetAlertPolicyRequest(), name="name_value",
+            alert_service.GetAlertPolicyRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [alert_service.CreateAlertPolicyRequest, dict,]
+    "request_type",
+    [
+        alert_service.CreateAlertPolicyRequest,
+        dict,
+    ],
 )
 def test_create_alert_policy(request_type, transport: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1307,15 +1412,16 @@
     assert response.notification_channels == ["notification_channels_value"]
 
 
 def test_create_alert_policy_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_alert_policy), "__call__"
     ) as call:
         client.create_alert_policy()
@@ -1325,15 +1431,16 @@
 
 
 @pytest.mark.asyncio
 async def test_create_alert_policy_async(
     transport: str = "grpc_asyncio", request_type=alert_service.CreateAlertPolicyRequest
 ):
     client = AlertPolicyServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1374,15 +1481,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.CreateAlertPolicyRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_alert_policy), "__call__"
     ) as call:
         call.return_value = alert.AlertPolicy()
         client.create_alert_policy(request)
@@ -1390,28 +1497,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_alert_policy_field_headers_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.CreateAlertPolicyRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_alert_policy), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(alert.AlertPolicy())
         await client.create_alert_policy(request)
@@ -1419,15 +1529,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_create_alert_policy_flattened():
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1436,15 +1549,16 @@
         type(client.transport.create_alert_policy), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = alert.AlertPolicy()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         client.create_alert_policy(
-            name="name_value", alert_policy=alert.AlertPolicy(name="name_value"),
+            name="name_value",
+            alert_policy=alert.AlertPolicy(name="name_value"),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -1483,15 +1597,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = alert.AlertPolicy()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(alert.AlertPolicy())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         response = await client.create_alert_policy(
-            name="name_value", alert_policy=alert.AlertPolicy(name="name_value"),
+            name="name_value",
+            alert_policy=alert.AlertPolicy(name="name_value"),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -1515,19 +1630,24 @@
             alert_service.CreateAlertPolicyRequest(),
             name="name_value",
             alert_policy=alert.AlertPolicy(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [alert_service.DeleteAlertPolicyRequest, dict,]
+    "request_type",
+    [
+        alert_service.DeleteAlertPolicyRequest,
+        dict,
+    ],
 )
 def test_delete_alert_policy(request_type, transport: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1547,15 +1667,16 @@
     assert response is None
 
 
 def test_delete_alert_policy_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_alert_policy), "__call__"
     ) as call:
         client.delete_alert_policy()
@@ -1565,15 +1686,16 @@
 
 
 @pytest.mark.asyncio
 async def test_delete_alert_policy_async(
     transport: str = "grpc_asyncio", request_type=alert_service.DeleteAlertPolicyRequest
 ):
     client = AlertPolicyServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1603,15 +1725,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.DeleteAlertPolicyRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_alert_policy), "__call__"
     ) as call:
         call.return_value = None
         client.delete_alert_policy(request)
@@ -1619,28 +1741,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_alert_policy_field_headers_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.DeleteAlertPolicyRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_alert_policy), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_alert_policy(request)
@@ -1648,15 +1773,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_alert_policy_flattened():
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1664,15 +1792,17 @@
     with mock.patch.object(
         type(client.transport.delete_alert_policy), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.delete_alert_policy(name="name_value",)
+        client.delete_alert_policy(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1684,15 +1814,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.delete_alert_policy(
-            alert_service.DeleteAlertPolicyRequest(), name="name_value",
+            alert_service.DeleteAlertPolicyRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_delete_alert_policy_flattened_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1704,15 +1835,17 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.delete_alert_policy(name="name_value",)
+        response = await client.delete_alert_policy(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1725,24 +1858,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.delete_alert_policy(
-            alert_service.DeleteAlertPolicyRequest(), name="name_value",
+            alert_service.DeleteAlertPolicyRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [alert_service.UpdateAlertPolicyRequest, dict,]
+    "request_type",
+    [
+        alert_service.UpdateAlertPolicyRequest,
+        dict,
+    ],
 )
 def test_update_alert_policy(request_type, transport: str = "grpc"):
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1771,15 +1910,16 @@
     assert response.notification_channels == ["notification_channels_value"]
 
 
 def test_update_alert_policy_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = AlertPolicyServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_alert_policy), "__call__"
     ) as call:
         client.update_alert_policy()
@@ -1789,15 +1929,16 @@
 
 
 @pytest.mark.asyncio
 async def test_update_alert_policy_async(
     transport: str = "grpc_asyncio", request_type=alert_service.UpdateAlertPolicyRequest
 ):
     client = AlertPolicyServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1838,15 +1979,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.UpdateAlertPolicyRequest()
 
-    request.alert_policy.name = "alert_policy.name/value"
+    request.alert_policy.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_alert_policy), "__call__"
     ) as call:
         call.return_value = alert.AlertPolicy()
         client.update_alert_policy(request)
@@ -1856,29 +1997,29 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "alert_policy.name=alert_policy.name/value",
+        "alert_policy.name=name_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_update_alert_policy_field_headers_async():
     client = AlertPolicyServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = alert_service.UpdateAlertPolicyRequest()
 
-    request.alert_policy.name = "alert_policy.name/value"
+    request.alert_policy.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_alert_policy), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(alert.AlertPolicy())
         await client.update_alert_policy(request)
@@ -1888,15 +2029,15 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "alert_policy.name=alert_policy.name/value",
+        "alert_policy.name=name_value",
     ) in kw["metadata"]
 
 
 def test_update_alert_policy_flattened():
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1993,15 +2134,16 @@
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.AlertPolicyServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = AlertPolicyServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.AlertPolicyServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -2013,15 +2155,18 @@
     # It is an error to provide an api_key and a transport instance.
     transport = transports.AlertPolicyServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
-        client = AlertPolicyServiceClient(client_options=options, transport=transport,)
+        client = AlertPolicyServiceClient(
+            client_options=options,
+            transport=transport,
+        )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = AlertPolicyServiceClient(
             client_options=options, credentials=ga_credentials.AnonymousCredentials()
@@ -2029,15 +2174,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.AlertPolicyServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = AlertPolicyServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.AlertPolicyServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2072,20 +2218,36 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = AlertPolicyServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
-    assert isinstance(client.transport, transports.AlertPolicyServiceGrpcTransport,)
+    assert isinstance(
+        client.transport,
+        transports.AlertPolicyServiceGrpcTransport,
+    )
 
 
 def test_alert_policy_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.AlertPolicyServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
@@ -2115,26 +2277,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_alert_policy_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.alert_policy_service.transports.AlertPolicyServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.AlertPolicyServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -2277,52 +2448,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_alert_policy_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_alert_policy_service_host_no_port(transport_name):
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_alert_policy_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_alert_policy_service_host_with_port(transport_name):
     client = AlertPolicyServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_alert_policy_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.AlertPolicyServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_alert_policy_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.AlertPolicyServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -2425,15 +2614,16 @@
             assert transport.grpc_channel == mock_grpc_channel
 
 
 def test_alert_policy_path():
     project = "squid"
     alert_policy = "clam"
     expected = "projects/{project}/alertPolicies/{alert_policy}".format(
-        project=project, alert_policy=alert_policy,
+        project=project,
+        alert_policy=alert_policy,
     )
     actual = AlertPolicyServiceClient.alert_policy_path(project, alert_policy)
     assert expected == actual
 
 
 def test_parse_alert_policy_path():
     expected = {
@@ -2447,16 +2637,20 @@
     assert expected == actual
 
 
 def test_alert_policy_condition_path():
     project = "oyster"
     alert_policy = "nudibranch"
     condition = "cuttlefish"
-    expected = "projects/{project}/alertPolicies/{alert_policy}/conditions/{condition}".format(
-        project=project, alert_policy=alert_policy, condition=condition,
+    expected = (
+        "projects/{project}/alertPolicies/{alert_policy}/conditions/{condition}".format(
+            project=project,
+            alert_policy=alert_policy,
+            condition=condition,
+        )
     )
     actual = AlertPolicyServiceClient.alert_policy_condition_path(
         project, alert_policy, condition
     )
     assert expected == actual
 
 
@@ -2491,15 +2685,17 @@
     # Check that the path construction is reversible.
     actual = AlertPolicyServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "squid"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = AlertPolicyServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "clam",
@@ -2509,15 +2705,17 @@
     # Check that the path construction is reversible.
     actual = AlertPolicyServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "whelk"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = AlertPolicyServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "octopus",
@@ -2527,15 +2725,17 @@
     # Check that the path construction is reversible.
     actual = AlertPolicyServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "oyster"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = AlertPolicyServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "nudibranch",
@@ -2547,15 +2747,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "cuttlefish"
     location = "mussel"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = AlertPolicyServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -2572,32 +2773,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.AlertPolicyServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = AlertPolicyServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.AlertPolicyServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = AlertPolicyServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = AlertPolicyServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_group_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_group_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -82,27 +88,33 @@
     assert (
         GroupServiceClient._get_default_mtls_endpoint(sandbox_mtls_endpoint)
         == sandbox_mtls_endpoint
     )
     assert GroupServiceClient._get_default_mtls_endpoint(non_googleapi) == non_googleapi
 
 
-@pytest.mark.parametrize("client_class", [GroupServiceClient, GroupServiceAsyncClient,])
-def test_group_service_client_from_service_account_info(client_class):
+@pytest.mark.parametrize(
+    "client_class,transport_name",
+    [
+        (GroupServiceClient, "grpc"),
+        (GroupServiceAsyncClient, "grpc_asyncio"),
+    ],
+)
+def test_group_service_client_from_service_account_info(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.GroupServiceGrpcTransport, "grpc"),
         (transports.GroupServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -122,30 +134,40 @@
         service_account.Credentials, "with_always_use_jwt_access", create=True
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
-@pytest.mark.parametrize("client_class", [GroupServiceClient, GroupServiceAsyncClient,])
-def test_group_service_client_from_service_account_file(client_class):
+@pytest.mark.parametrize(
+    "client_class,transport_name",
+    [
+        (GroupServiceClient, "grpc"),
+        (GroupServiceAsyncClient, "grpc_asyncio"),
+    ],
+)
+def test_group_service_client_from_service_account_file(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_group_service_client_get_transport_class():
     transport = GroupServiceClient.get_transport_class()
     available_transports = [
         transports.GroupServiceGrpcTransport,
     ]
@@ -477,15 +499,17 @@
         ),
     ],
 )
 def test_group_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -619,18 +643,25 @@
             options=[
                 ("grpc.max_send_message_length", -1),
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
-@pytest.mark.parametrize("request_type", [group_service.ListGroupsRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        group_service.ListGroupsRequest,
+        dict,
+    ],
+)
 def test_list_groups(request_type, transport: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -651,15 +682,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_groups_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         client.list_groups()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -667,26 +699,29 @@
 
 
 @pytest.mark.asyncio
 async def test_list_groups_async(
     transport: str = "grpc_asyncio", request_type=group_service.ListGroupsRequest
 ):
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            group_service.ListGroupsResponse(next_page_token="next_page_token_value",)
+            group_service.ListGroupsResponse(
+                next_page_token="next_page_token_value",
+            )
         )
         response = await client.list_groups(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == group_service.ListGroupsRequest()
@@ -698,46 +733,53 @@
 
 @pytest.mark.asyncio
 async def test_list_groups_async_from_dict():
     await test_list_groups_async(request_type=dict)
 
 
 def test_list_groups_field_headers():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.ListGroupsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         call.return_value = group_service.ListGroupsResponse()
         client.list_groups(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_groups_field_headers_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.ListGroupsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             group_service.ListGroupsResponse()
         )
         await client.list_groups(request)
@@ -745,207 +787,301 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_groups_flattened():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = group_service.ListGroupsResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_groups(name="name_value",)
+        client.list_groups(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_list_groups_flattened_error():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_groups(
-            group_service.ListGroupsRequest(), name="name_value",
+            group_service.ListGroupsRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_groups_flattened_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = group_service.ListGroupsResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             group_service.ListGroupsResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_groups(name="name_value",)
+        response = await client.list_groups(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_groups_flattened_error_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_groups(
-            group_service.ListGroupsRequest(), name="name_value",
+            group_service.ListGroupsRequest(),
+            name="name_value",
         )
 
 
 def test_list_groups_pager(transport_name: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         # Set the response to a series of pages.
         call.side_effect = (
             group_service.ListGroupsResponse(
-                group=[group.Group(), group.Group(), group.Group(),],
+                group=[
+                    group.Group(),
+                    group.Group(),
+                    group.Group(),
+                ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupsResponse(group=[], next_page_token="def",),
             group_service.ListGroupsResponse(
-                group=[group.Group(),], next_page_token="ghi",
+                group=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                ],
+                next_page_token="ghi",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                    group.Group(),
+                ],
             ),
-            group_service.ListGroupsResponse(group=[group.Group(), group.Group(),],),
             RuntimeError,
         )
 
         metadata = ()
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_groups(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, group.Group) for i in results)
 
 
 def test_list_groups_pages(transport_name: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_groups), "__call__") as call:
         # Set the response to a series of pages.
         call.side_effect = (
             group_service.ListGroupsResponse(
-                group=[group.Group(), group.Group(), group.Group(),],
+                group=[
+                    group.Group(),
+                    group.Group(),
+                    group.Group(),
+                ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupsResponse(group=[], next_page_token="def",),
             group_service.ListGroupsResponse(
-                group=[group.Group(),], next_page_token="ghi",
+                group=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                ],
+                next_page_token="ghi",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                    group.Group(),
+                ],
             ),
-            group_service.ListGroupsResponse(group=[group.Group(), group.Group(),],),
             RuntimeError,
         )
         pages = list(client.list_groups(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.asyncio
 async def test_list_groups_async_pager():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_groups), "__call__", new_callable=mock.AsyncMock
     ) as call:
         # Set the response to a series of pages.
         call.side_effect = (
             group_service.ListGroupsResponse(
-                group=[group.Group(), group.Group(), group.Group(),],
+                group=[
+                    group.Group(),
+                    group.Group(),
+                    group.Group(),
+                ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupsResponse(group=[], next_page_token="def",),
             group_service.ListGroupsResponse(
-                group=[group.Group(),], next_page_token="ghi",
+                group=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                ],
+                next_page_token="ghi",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                    group.Group(),
+                ],
             ),
-            group_service.ListGroupsResponse(group=[group.Group(), group.Group(),],),
             RuntimeError,
         )
-        async_pager = await client.list_groups(request={},)
+        async_pager = await client.list_groups(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, group.Group) for i in responses)
 
 
 @pytest.mark.asyncio
 async def test_list_groups_async_pages():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_groups), "__call__", new_callable=mock.AsyncMock
     ) as call:
         # Set the response to a series of pages.
         call.side_effect = (
             group_service.ListGroupsResponse(
-                group=[group.Group(), group.Group(), group.Group(),],
+                group=[
+                    group.Group(),
+                    group.Group(),
+                    group.Group(),
+                ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupsResponse(group=[], next_page_token="def",),
             group_service.ListGroupsResponse(
-                group=[group.Group(),], next_page_token="ghi",
+                group=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                ],
+                next_page_token="ghi",
+            ),
+            group_service.ListGroupsResponse(
+                group=[
+                    group.Group(),
+                    group.Group(),
+                ],
             ),
-            group_service.ListGroupsResponse(group=[group.Group(), group.Group(),],),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_groups(request={})).pages:
+        async for page_ in (
+            await client.list_groups(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
-@pytest.mark.parametrize("request_type", [group_service.GetGroupRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        group_service.GetGroupRequest,
+        dict,
+    ],
+)
 def test_get_group(request_type, transport: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -974,15 +1110,16 @@
     assert response.is_cluster is True
 
 
 def test_get_group_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_group), "__call__") as call:
         client.get_group()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -990,15 +1127,16 @@
 
 
 @pytest.mark.asyncio
 async def test_get_group_async(
     transport: str = "grpc_asyncio", request_type=group_service.GetGroupRequest
 ):
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1031,132 +1169,163 @@
 
 @pytest.mark.asyncio
 async def test_get_group_async_from_dict():
     await test_get_group_async(request_type=dict)
 
 
 def test_get_group_field_headers():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.GetGroupRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_group), "__call__") as call:
         call.return_value = group.Group()
         client.get_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_group_field_headers_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.GetGroupRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_group), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(group.Group())
         await client.get_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_group_flattened():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = group.Group()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_group(name="name_value",)
+        client.get_group(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_get_group_flattened_error():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_group(
-            group_service.GetGroupRequest(), name="name_value",
+            group_service.GetGroupRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_group_flattened_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = group.Group()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(group.Group())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_group(name="name_value",)
+        response = await client.get_group(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_get_group_flattened_error_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_group(
-            group_service.GetGroupRequest(), name="name_value",
+            group_service.GetGroupRequest(),
+            name="name_value",
         )
 
 
-@pytest.mark.parametrize("request_type", [group_service.CreateGroupRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        group_service.CreateGroupRequest,
+        dict,
+    ],
+)
 def test_create_group(request_type, transport: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1185,15 +1354,16 @@
     assert response.is_cluster is True
 
 
 def test_create_group_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_group), "__call__") as call:
         client.create_group()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1201,15 +1371,16 @@
 
 
 @pytest.mark.asyncio
 async def test_create_group_async(
     transport: str = "grpc_asyncio", request_type=group_service.CreateGroupRequest
 ):
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1242,73 +1413,86 @@
 
 @pytest.mark.asyncio
 async def test_create_group_async_from_dict():
     await test_create_group_async(request_type=dict)
 
 
 def test_create_group_field_headers():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.CreateGroupRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_group), "__call__") as call:
         call.return_value = gm_group.Group()
         client.create_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_group_field_headers_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.CreateGroupRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_group), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_group.Group())
         await client.create_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_create_group_flattened():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_group.Group()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         client.create_group(
-            name="name_value", group=gm_group.Group(name="name_value"),
+            name="name_value",
+            group=gm_group.Group(name="name_value"),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -1316,40 +1500,45 @@
         assert arg == mock_val
         arg = args[0].group
         mock_val = gm_group.Group(name="name_value")
         assert arg == mock_val
 
 
 def test_create_group_flattened_error():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.create_group(
             group_service.CreateGroupRequest(),
             name="name_value",
             group=gm_group.Group(name="name_value"),
         )
 
 
 @pytest.mark.asyncio
 async def test_create_group_flattened_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_group.Group()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_group.Group())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         response = await client.create_group(
-            name="name_value", group=gm_group.Group(name="name_value"),
+            name="name_value",
+            group=gm_group.Group(name="name_value"),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -1358,30 +1547,39 @@
         arg = args[0].group
         mock_val = gm_group.Group(name="name_value")
         assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_create_group_flattened_error_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.create_group(
             group_service.CreateGroupRequest(),
             name="name_value",
             group=gm_group.Group(name="name_value"),
         )
 
 
-@pytest.mark.parametrize("request_type", [group_service.UpdateGroupRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        group_service.UpdateGroupRequest,
+        dict,
+    ],
+)
 def test_update_group(request_type, transport: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1410,15 +1608,16 @@
     assert response.is_cluster is True
 
 
 def test_update_group_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_group), "__call__") as call:
         client.update_group()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1426,15 +1625,16 @@
 
 
 @pytest.mark.asyncio
 async def test_update_group_async(
     transport: str = "grpc_asyncio", request_type=group_service.UpdateGroupRequest
 ):
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1467,132 +1667,163 @@
 
 @pytest.mark.asyncio
 async def test_update_group_async_from_dict():
     await test_update_group_async(request_type=dict)
 
 
 def test_update_group_field_headers():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.UpdateGroupRequest()
 
-    request.group.name = "group.name/value"
+    request.group.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_group), "__call__") as call:
         call.return_value = gm_group.Group()
         client.update_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "group.name=group.name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "group.name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_update_group_field_headers_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.UpdateGroupRequest()
 
-    request.group.name = "group.name/value"
+    request.group.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_group), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_group.Group())
         await client.update_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "group.name=group.name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "group.name=name_value",
+    ) in kw["metadata"]
 
 
 def test_update_group_flattened():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_group.Group()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.update_group(group=gm_group.Group(name="name_value"),)
+        client.update_group(
+            group=gm_group.Group(name="name_value"),
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].group
         mock_val = gm_group.Group(name="name_value")
         assert arg == mock_val
 
 
 def test_update_group_flattened_error():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.update_group(
-            group_service.UpdateGroupRequest(), group=gm_group.Group(name="name_value"),
+            group_service.UpdateGroupRequest(),
+            group=gm_group.Group(name="name_value"),
         )
 
 
 @pytest.mark.asyncio
 async def test_update_group_flattened_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_group.Group()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_group.Group())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.update_group(group=gm_group.Group(name="name_value"),)
+        response = await client.update_group(
+            group=gm_group.Group(name="name_value"),
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].group
         mock_val = gm_group.Group(name="name_value")
         assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_update_group_flattened_error_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.update_group(
-            group_service.UpdateGroupRequest(), group=gm_group.Group(name="name_value"),
+            group_service.UpdateGroupRequest(),
+            group=gm_group.Group(name="name_value"),
         )
 
 
-@pytest.mark.parametrize("request_type", [group_service.DeleteGroupRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        group_service.DeleteGroupRequest,
+        dict,
+    ],
+)
 def test_delete_group(request_type, transport: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1610,15 +1841,16 @@
     assert response is None
 
 
 def test_delete_group_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_group), "__call__") as call:
         client.delete_group()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1626,15 +1858,16 @@
 
 
 @pytest.mark.asyncio
 async def test_delete_group_async(
     transport: str = "grpc_asyncio", request_type=group_service.DeleteGroupRequest
 ):
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1654,145 +1887,177 @@
 
 @pytest.mark.asyncio
 async def test_delete_group_async_from_dict():
     await test_delete_group_async(request_type=dict)
 
 
 def test_delete_group_field_headers():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.DeleteGroupRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_group), "__call__") as call:
         call.return_value = None
         client.delete_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_group_field_headers_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.DeleteGroupRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_group), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_group(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_group_flattened():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.delete_group(name="name_value",)
+        client.delete_group(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_delete_group_flattened_error():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.delete_group(
-            group_service.DeleteGroupRequest(), name="name_value",
+            group_service.DeleteGroupRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_delete_group_flattened_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_group), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.delete_group(name="name_value",)
+        response = await client.delete_group(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_delete_group_flattened_error_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.delete_group(
-            group_service.DeleteGroupRequest(), name="name_value",
+            group_service.DeleteGroupRequest(),
+            name="name_value",
         )
 
 
-@pytest.mark.parametrize("request_type", [group_service.ListGroupMembersRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        group_service.ListGroupMembersRequest,
+        dict,
+    ],
+)
 def test_list_group_members(request_type, transport: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = group_service.ListGroupMembersResponse(
-            next_page_token="next_page_token_value", total_size=1086,
+            next_page_token="next_page_token_value",
+            total_size=1086,
         )
         response = client.list_group_members(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == group_service.ListGroupMembersRequest()
@@ -1803,15 +2068,16 @@
     assert response.total_size == 1086
 
 
 def test_list_group_members_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         client.list_group_members()
@@ -1821,29 +2087,31 @@
 
 
 @pytest.mark.asyncio
 async def test_list_group_members_async(
     transport: str = "grpc_asyncio", request_type=group_service.ListGroupMembersRequest
 ):
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             group_service.ListGroupMembersResponse(
-                next_page_token="next_page_token_value", total_size=1086,
+                next_page_token="next_page_token_value",
+                total_size=1086,
             )
         )
         response = await client.list_group_members(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1857,21 +2125,23 @@
 
 @pytest.mark.asyncio
 async def test_list_group_members_async_from_dict():
     await test_list_group_members_async(request_type=dict)
 
 
 def test_list_group_members_field_headers():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.ListGroupMembersRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         call.return_value = group_service.ListGroupMembersResponse()
         client.list_group_members(request)
@@ -1879,26 +2149,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_group_members_field_headers_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = group_service.ListGroupMembersRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             group_service.ListGroupMembersResponse()
@@ -1908,92 +2183,110 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_group_members_flattened():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = group_service.ListGroupMembersResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_group_members(name="name_value",)
+        client.list_group_members(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_list_group_members_flattened_error():
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_group_members(
-            group_service.ListGroupMembersRequest(), name="name_value",
+            group_service.ListGroupMembersRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_group_members_flattened_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = group_service.ListGroupMembersResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             group_service.ListGroupMembersResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_group_members(name="name_value",)
+        response = await client.list_group_members(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 @pytest.mark.asyncio
 async def test_list_group_members_flattened_error_async():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_group_members(
-            group_service.ListGroupMembersRequest(), name="name_value",
+            group_service.ListGroupMembersRequest(),
+            name="name_value",
         )
 
 
 def test_list_group_members_pager(transport_name: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -2002,17 +2295,22 @@
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupMembersResponse(members=[], next_page_token="def",),
             group_service.ListGroupMembersResponse(
-                members=[monitored_resource_pb2.MonitoredResource(),],
+                members=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupMembersResponse(
+                members=[
+                    monitored_resource_pb2.MonitoredResource(),
+                ],
                 next_page_token="ghi",
             ),
             group_service.ListGroupMembersResponse(
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
@@ -2024,24 +2322,25 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_group_members(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(
             isinstance(i, monitored_resource_pb2.MonitoredResource) for i in results
         )
 
 
 def test_list_group_members_pages(transport_name: str = "grpc"):
     client = GroupServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -2050,17 +2349,22 @@
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupMembersResponse(members=[], next_page_token="def",),
             group_service.ListGroupMembersResponse(
-                members=[monitored_resource_pb2.MonitoredResource(),],
+                members=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupMembersResponse(
+                members=[
+                    monitored_resource_pb2.MonitoredResource(),
+                ],
                 next_page_token="ghi",
             ),
             group_service.ListGroupMembersResponse(
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
@@ -2070,15 +2374,17 @@
         pages = list(client.list_group_members(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.asyncio
 async def test_list_group_members_async_pager():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -2088,42 +2394,51 @@
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupMembersResponse(members=[], next_page_token="def",),
             group_service.ListGroupMembersResponse(
-                members=[monitored_resource_pb2.MonitoredResource(),],
+                members=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupMembersResponse(
+                members=[
+                    monitored_resource_pb2.MonitoredResource(),
+                ],
                 next_page_token="ghi",
             ),
             group_service.ListGroupMembersResponse(
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_group_members(request={},)
+        async_pager = await client.list_group_members(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(
             isinstance(i, monitored_resource_pb2.MonitoredResource) for i in responses
         )
 
 
 @pytest.mark.asyncio
 async def test_list_group_members_async_pages():
-    client = GroupServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = GroupServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_group_members),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -2133,42 +2448,50 @@
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
                 next_page_token="abc",
             ),
-            group_service.ListGroupMembersResponse(members=[], next_page_token="def",),
             group_service.ListGroupMembersResponse(
-                members=[monitored_resource_pb2.MonitoredResource(),],
+                members=[],
+                next_page_token="def",
+            ),
+            group_service.ListGroupMembersResponse(
+                members=[
+                    monitored_resource_pb2.MonitoredResource(),
+                ],
                 next_page_token="ghi",
             ),
             group_service.ListGroupMembersResponse(
                 members=[
                     monitored_resource_pb2.MonitoredResource(),
                     monitored_resource_pb2.MonitoredResource(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_group_members(request={})).pages:
+        async for page_ in (
+            await client.list_group_members(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.GroupServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = GroupServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.GroupServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -2180,15 +2503,18 @@
     # It is an error to provide an api_key and a transport instance.
     transport = transports.GroupServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
-        client = GroupServiceClient(client_options=options, transport=transport,)
+        client = GroupServiceClient(
+            client_options=options,
+            transport=transport,
+        )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = GroupServiceClient(
             client_options=options, credentials=ga_credentials.AnonymousCredentials()
@@ -2196,15 +2522,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.GroupServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = GroupServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.GroupServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2239,18 +2566,36 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = GroupServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
-    client = GroupServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
-    assert isinstance(client.transport, transports.GroupServiceGrpcTransport,)
+    client = GroupServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert isinstance(
+        client.transport,
+        transports.GroupServiceGrpcTransport,
+    )
 
 
 def test_group_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.GroupServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
@@ -2281,26 +2626,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_group_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.group_service.transports.GroupServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.GroupServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -2438,52 +2792,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_group_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_group_service_host_no_port(transport_name):
     client = GroupServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_group_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_group_service_host_with_port(transport_name):
     client = GroupServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_group_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.GroupServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_group_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.GroupServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -2577,15 +2949,18 @@
             )
             assert transport.grpc_channel == mock_grpc_channel
 
 
 def test_group_path():
     project = "squid"
     group = "clam"
-    expected = "projects/{project}/groups/{group}".format(project=project, group=group,)
+    expected = "projects/{project}/groups/{group}".format(
+        project=project,
+        group=group,
+    )
     actual = GroupServiceClient.group_path(project, group)
     assert expected == actual
 
 
 def test_parse_group_path():
     expected = {
         "project": "whelk",
@@ -2616,15 +2991,17 @@
     # Check that the path construction is reversible.
     actual = GroupServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "cuttlefish"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = GroupServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "mussel",
@@ -2634,15 +3011,17 @@
     # Check that the path construction is reversible.
     actual = GroupServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "winkle"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = GroupServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "nautilus",
@@ -2652,15 +3031,17 @@
     # Check that the path construction is reversible.
     actual = GroupServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "scallop"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = GroupServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "abalone",
@@ -2672,15 +3053,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "squid"
     location = "clam"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = GroupServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -2697,32 +3079,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.GroupServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = GroupServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.GroupServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = GroupServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = GroupServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_metric_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_metric_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -92,28 +98,32 @@
     )
     assert (
         MetricServiceClient._get_default_mtls_endpoint(non_googleapi) == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class", [MetricServiceClient, MetricServiceAsyncClient,]
+    "client_class,transport_name",
+    [
+        (MetricServiceClient, "grpc"),
+        (MetricServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_metric_service_client_from_service_account_info(client_class):
+def test_metric_service_client_from_service_account_info(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.MetricServiceGrpcTransport, "grpc"),
         (transports.MetricServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -134,31 +144,39 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class", [MetricServiceClient, MetricServiceAsyncClient,]
+    "client_class,transport_name",
+    [
+        (MetricServiceClient, "grpc"),
+        (MetricServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_metric_service_client_from_service_account_file(client_class):
+def test_metric_service_client_from_service_account_file(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_metric_service_client_get_transport_class():
     transport = MetricServiceClient.get_transport_class()
     available_transports = [
         transports.MetricServiceGrpcTransport,
     ]
@@ -498,15 +516,17 @@
         ),
     ],
 )
 def test_metric_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -644,19 +664,24 @@
                 ("grpc.max_send_message_length", -1),
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.ListMonitoredResourceDescriptorsRequest, dict,]
+    "request_type",
+    [
+        metric_service.ListMonitoredResourceDescriptorsRequest,
+        dict,
+    ],
 )
 def test_list_monitored_resource_descriptors(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -679,15 +704,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_monitored_resource_descriptors_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors), "__call__"
     ) as call:
         client.list_monitored_resource_descriptors()
@@ -698,15 +724,16 @@
 
 @pytest.mark.asyncio
 async def test_list_monitored_resource_descriptors_async(
     transport: str = "grpc_asyncio",
     request_type=metric_service.ListMonitoredResourceDescriptorsRequest,
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -733,21 +760,23 @@
 
 @pytest.mark.asyncio
 async def test_list_monitored_resource_descriptors_async_from_dict():
     await test_list_monitored_resource_descriptors_async(request_type=dict)
 
 
 def test_list_monitored_resource_descriptors_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.ListMonitoredResourceDescriptorsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors), "__call__"
     ) as call:
         call.return_value = metric_service.ListMonitoredResourceDescriptorsResponse()
         client.list_monitored_resource_descriptors(request)
@@ -755,28 +784,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_monitored_resource_descriptors_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.ListMonitoredResourceDescriptorsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.ListMonitoredResourceDescriptorsResponse()
@@ -786,47 +818,57 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_monitored_resource_descriptors_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = metric_service.ListMonitoredResourceDescriptorsResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_monitored_resource_descriptors(name="name_value",)
+        client.list_monitored_resource_descriptors(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_list_monitored_resource_descriptors_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_monitored_resource_descriptors(
-            metric_service.ListMonitoredResourceDescriptorsRequest(), name="name_value",
+            metric_service.ListMonitoredResourceDescriptorsRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_monitored_resource_descriptors_flattened_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -840,15 +882,17 @@
         call.return_value = metric_service.ListMonitoredResourceDescriptorsResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.ListMonitoredResourceDescriptorsResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_monitored_resource_descriptors(name="name_value",)
+        response = await client.list_monitored_resource_descriptors(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -861,21 +905,23 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_monitored_resource_descriptors(
-            metric_service.ListMonitoredResourceDescriptorsRequest(), name="name_value",
+            metric_service.ListMonitoredResourceDescriptorsRequest(),
+            name="name_value",
         )
 
 
 def test_list_monitored_resource_descriptors_pager(transport_name: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -885,15 +931,16 @@
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
-                resource_descriptors=[], next_page_token="def",
+                resource_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
                 resource_descriptors=[
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="ghi",
             ),
@@ -910,25 +957,26 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_monitored_resource_descriptors(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(
             isinstance(i, monitored_resource_pb2.MonitoredResourceDescriptor)
             for i in results
         )
 
 
 def test_list_monitored_resource_descriptors_pages(transport_name: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -938,15 +986,16 @@
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
-                resource_descriptors=[], next_page_token="def",
+                resource_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
                 resource_descriptors=[
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="ghi",
             ),
@@ -961,15 +1010,17 @@
         pages = list(client.list_monitored_resource_descriptors(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.asyncio
 async def test_list_monitored_resource_descriptors_async_pager():
-    client = MetricServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = MetricServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -980,15 +1031,16 @@
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
-                resource_descriptors=[], next_page_token="def",
+                resource_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
                 resource_descriptors=[
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="ghi",
             ),
@@ -996,30 +1048,34 @@
                 resource_descriptors=[
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_monitored_resource_descriptors(request={},)
+        async_pager = await client.list_monitored_resource_descriptors(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(
             isinstance(i, monitored_resource_pb2.MonitoredResourceDescriptor)
             for i in responses
         )
 
 
 @pytest.mark.asyncio
 async def test_list_monitored_resource_descriptors_async_pages():
-    client = MetricServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = MetricServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_monitored_resource_descriptors),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -1030,15 +1086,16 @@
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
-                resource_descriptors=[], next_page_token="def",
+                resource_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMonitoredResourceDescriptorsResponse(
                 resource_descriptors=[
                     monitored_resource_pb2.MonitoredResourceDescriptor(),
                 ],
                 next_page_token="ghi",
             ),
@@ -1049,26 +1106,31 @@
                 ],
             ),
             RuntimeError,
         )
         pages = []
         async for page_ in (
             await client.list_monitored_resource_descriptors(request={})
-        ).pages:
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.GetMonitoredResourceDescriptorRequest, dict,]
+    "request_type",
+    [
+        metric_service.GetMonitoredResourceDescriptorRequest,
+        dict,
+    ],
 )
 def test_get_monitored_resource_descriptor(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1097,15 +1159,16 @@
     assert response.description == "description_value"
 
 
 def test_get_monitored_resource_descriptor_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_monitored_resource_descriptor), "__call__"
     ) as call:
         client.get_monitored_resource_descriptor()
@@ -1116,15 +1179,16 @@
 
 @pytest.mark.asyncio
 async def test_get_monitored_resource_descriptor_async(
     transport: str = "grpc_asyncio",
     request_type=metric_service.GetMonitoredResourceDescriptorRequest,
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1157,21 +1221,23 @@
 
 @pytest.mark.asyncio
 async def test_get_monitored_resource_descriptor_async_from_dict():
     await test_get_monitored_resource_descriptor_async(request_type=dict)
 
 
 def test_get_monitored_resource_descriptor_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.GetMonitoredResourceDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_monitored_resource_descriptor), "__call__"
     ) as call:
         call.return_value = monitored_resource_pb2.MonitoredResourceDescriptor()
         client.get_monitored_resource_descriptor(request)
@@ -1179,28 +1245,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_monitored_resource_descriptor_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.GetMonitoredResourceDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_monitored_resource_descriptor), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             monitored_resource_pb2.MonitoredResourceDescriptor()
@@ -1210,47 +1279,57 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_monitored_resource_descriptor_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_monitored_resource_descriptor), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = monitored_resource_pb2.MonitoredResourceDescriptor()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_monitored_resource_descriptor(name="name_value",)
+        client.get_monitored_resource_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_get_monitored_resource_descriptor_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_monitored_resource_descriptor(
-            metric_service.GetMonitoredResourceDescriptorRequest(), name="name_value",
+            metric_service.GetMonitoredResourceDescriptorRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_monitored_resource_descriptor_flattened_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1264,15 +1343,17 @@
         call.return_value = monitored_resource_pb2.MonitoredResourceDescriptor()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             monitored_resource_pb2.MonitoredResourceDescriptor()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_monitored_resource_descriptor(name="name_value",)
+        response = await client.get_monitored_resource_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1285,24 +1366,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_monitored_resource_descriptor(
-            metric_service.GetMonitoredResourceDescriptorRequest(), name="name_value",
+            metric_service.GetMonitoredResourceDescriptorRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.ListMetricDescriptorsRequest, dict,]
+    "request_type",
+    [
+        metric_service.ListMetricDescriptorsRequest,
+        dict,
+    ],
 )
 def test_list_metric_descriptors(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1325,15 +1412,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_metric_descriptors_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors), "__call__"
     ) as call:
         client.list_metric_descriptors()
@@ -1344,15 +1432,16 @@
 
 @pytest.mark.asyncio
 async def test_list_metric_descriptors_async(
     transport: str = "grpc_asyncio",
     request_type=metric_service.ListMetricDescriptorsRequest,
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1379,21 +1468,23 @@
 
 @pytest.mark.asyncio
 async def test_list_metric_descriptors_async_from_dict():
     await test_list_metric_descriptors_async(request_type=dict)
 
 
 def test_list_metric_descriptors_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.ListMetricDescriptorsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors), "__call__"
     ) as call:
         call.return_value = metric_service.ListMetricDescriptorsResponse()
         client.list_metric_descriptors(request)
@@ -1401,28 +1492,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_metric_descriptors_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.ListMetricDescriptorsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.ListMetricDescriptorsResponse()
@@ -1432,47 +1526,57 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_metric_descriptors_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = metric_service.ListMetricDescriptorsResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_metric_descriptors(name="name_value",)
+        client.list_metric_descriptors(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_list_metric_descriptors_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_metric_descriptors(
-            metric_service.ListMetricDescriptorsRequest(), name="name_value",
+            metric_service.ListMetricDescriptorsRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_metric_descriptors_flattened_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1486,15 +1590,17 @@
         call.return_value = metric_service.ListMetricDescriptorsResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.ListMetricDescriptorsResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_metric_descriptors(name="name_value",)
+        response = await client.list_metric_descriptors(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1507,21 +1613,23 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_metric_descriptors(
-            metric_service.ListMetricDescriptorsRequest(), name="name_value",
+            metric_service.ListMetricDescriptorsRequest(),
+            name="name_value",
         )
 
 
 def test_list_metric_descriptors_pager(transport_name: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -1531,18 +1639,21 @@
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[], next_page_token="def",
+                metric_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[metric_pb2.MetricDescriptor(),],
+                metric_descriptors=[
+                    metric_pb2.MetricDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             metric_service.ListMetricDescriptorsResponse(
                 metric_descriptors=[
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
@@ -1554,22 +1665,23 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_metric_descriptors(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, metric_pb2.MetricDescriptor) for i in results)
 
 
 def test_list_metric_descriptors_pages(transport_name: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -1579,18 +1691,21 @@
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[], next_page_token="def",
+                metric_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[metric_pb2.MetricDescriptor(),],
+                metric_descriptors=[
+                    metric_pb2.MetricDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             metric_service.ListMetricDescriptorsResponse(
                 metric_descriptors=[
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
@@ -1600,15 +1715,17 @@
         pages = list(client.list_metric_descriptors(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.asyncio
 async def test_list_metric_descriptors_async_pager():
-    client = MetricServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = MetricServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -1619,41 +1736,48 @@
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[], next_page_token="def",
+                metric_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[metric_pb2.MetricDescriptor(),],
+                metric_descriptors=[
+                    metric_pb2.MetricDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             metric_service.ListMetricDescriptorsResponse(
                 metric_descriptors=[
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_metric_descriptors(request={},)
+        async_pager = await client.list_metric_descriptors(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, metric_pb2.MetricDescriptor) for i in responses)
 
 
 @pytest.mark.asyncio
 async def test_list_metric_descriptors_async_pages():
-    client = MetricServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = MetricServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_metric_descriptors),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -1664,41 +1788,51 @@
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[], next_page_token="def",
+                metric_descriptors=[],
+                next_page_token="def",
             ),
             metric_service.ListMetricDescriptorsResponse(
-                metric_descriptors=[metric_pb2.MetricDescriptor(),],
+                metric_descriptors=[
+                    metric_pb2.MetricDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             metric_service.ListMetricDescriptorsResponse(
                 metric_descriptors=[
                     metric_pb2.MetricDescriptor(),
                     metric_pb2.MetricDescriptor(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_metric_descriptors(request={})).pages:
+        async for page_ in (
+            await client.list_metric_descriptors(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.GetMetricDescriptorRequest, dict,]
+    "request_type",
+    [
+        metric_service.GetMetricDescriptorRequest,
+        dict,
+    ],
 )
 def test_get_metric_descriptor(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1733,15 +1867,16 @@
     assert response.display_name == "display_name_value"
 
 
 def test_get_metric_descriptor_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_metric_descriptor), "__call__"
     ) as call:
         client.get_metric_descriptor()
@@ -1752,15 +1887,16 @@
 
 @pytest.mark.asyncio
 async def test_get_metric_descriptor_async(
     transport: str = "grpc_asyncio",
     request_type=metric_service.GetMetricDescriptorRequest,
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1799,21 +1935,23 @@
 
 @pytest.mark.asyncio
 async def test_get_metric_descriptor_async_from_dict():
     await test_get_metric_descriptor_async(request_type=dict)
 
 
 def test_get_metric_descriptor_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.GetMetricDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_metric_descriptor), "__call__"
     ) as call:
         call.return_value = metric_pb2.MetricDescriptor()
         client.get_metric_descriptor(request)
@@ -1821,28 +1959,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_metric_descriptor_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.GetMetricDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_metric_descriptor), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_pb2.MetricDescriptor()
@@ -1852,47 +1993,57 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_metric_descriptor_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_metric_descriptor), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = metric_pb2.MetricDescriptor()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_metric_descriptor(name="name_value",)
+        client.get_metric_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_get_metric_descriptor_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_metric_descriptor(
-            metric_service.GetMetricDescriptorRequest(), name="name_value",
+            metric_service.GetMetricDescriptorRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_metric_descriptor_flattened_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1906,15 +2057,17 @@
         call.return_value = metric_pb2.MetricDescriptor()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_pb2.MetricDescriptor()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_metric_descriptor(name="name_value",)
+        response = await client.get_metric_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1927,24 +2080,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_metric_descriptor(
-            metric_service.GetMetricDescriptorRequest(), name="name_value",
+            metric_service.GetMetricDescriptorRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.CreateMetricDescriptorRequest, dict,]
+    "request_type",
+    [
+        metric_service.CreateMetricDescriptorRequest,
+        dict,
+    ],
 )
 def test_create_metric_descriptor(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1979,15 +2138,16 @@
     assert response.display_name == "display_name_value"
 
 
 def test_create_metric_descriptor_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_metric_descriptor), "__call__"
     ) as call:
         client.create_metric_descriptor()
@@ -1998,15 +2158,16 @@
 
 @pytest.mark.asyncio
 async def test_create_metric_descriptor_async(
     transport: str = "grpc_asyncio",
     request_type=metric_service.CreateMetricDescriptorRequest,
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2045,21 +2206,23 @@
 
 @pytest.mark.asyncio
 async def test_create_metric_descriptor_async_from_dict():
     await test_create_metric_descriptor_async(request_type=dict)
 
 
 def test_create_metric_descriptor_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.CreateMetricDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_metric_descriptor), "__call__"
     ) as call:
         call.return_value = metric_pb2.MetricDescriptor()
         client.create_metric_descriptor(request)
@@ -2067,28 +2230,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_metric_descriptor_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.CreateMetricDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_metric_descriptor), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_pb2.MetricDescriptor()
@@ -2098,19 +2264,24 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_create_metric_descriptor_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_metric_descriptor), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = metric_pb2.MetricDescriptor()
@@ -2130,15 +2301,17 @@
         assert arg == mock_val
         arg = args[0].metric_descriptor
         mock_val = metric_pb2.MetricDescriptor(name="name_value")
         assert arg == mock_val
 
 
 def test_create_metric_descriptor_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.create_metric_descriptor(
             metric_service.CreateMetricDescriptorRequest(),
             name="name_value",
@@ -2194,19 +2367,24 @@
             metric_service.CreateMetricDescriptorRequest(),
             name="name_value",
             metric_descriptor=metric_pb2.MetricDescriptor(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.DeleteMetricDescriptorRequest, dict,]
+    "request_type",
+    [
+        metric_service.DeleteMetricDescriptorRequest,
+        dict,
+    ],
 )
 def test_delete_metric_descriptor(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2226,15 +2404,16 @@
     assert response is None
 
 
 def test_delete_metric_descriptor_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_metric_descriptor), "__call__"
     ) as call:
         client.delete_metric_descriptor()
@@ -2245,15 +2424,16 @@
 
 @pytest.mark.asyncio
 async def test_delete_metric_descriptor_async(
     transport: str = "grpc_asyncio",
     request_type=metric_service.DeleteMetricDescriptorRequest,
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2275,21 +2455,23 @@
 
 @pytest.mark.asyncio
 async def test_delete_metric_descriptor_async_from_dict():
     await test_delete_metric_descriptor_async(request_type=dict)
 
 
 def test_delete_metric_descriptor_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.DeleteMetricDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_metric_descriptor), "__call__"
     ) as call:
         call.return_value = None
         client.delete_metric_descriptor(request)
@@ -2297,28 +2479,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_metric_descriptor_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.DeleteMetricDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_metric_descriptor), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_metric_descriptor(request)
@@ -2326,47 +2511,57 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_metric_descriptor_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_metric_descriptor), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.delete_metric_descriptor(name="name_value",)
+        client.delete_metric_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
         assert arg == mock_val
 
 
 def test_delete_metric_descriptor_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.delete_metric_descriptor(
-            metric_service.DeleteMetricDescriptorRequest(), name="name_value",
+            metric_service.DeleteMetricDescriptorRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_delete_metric_descriptor_flattened_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2378,15 +2573,17 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.delete_metric_descriptor(name="name_value",)
+        response = await client.delete_metric_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -2399,33 +2596,42 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.delete_metric_descriptor(
-            metric_service.DeleteMetricDescriptorRequest(), name="name_value",
+            metric_service.DeleteMetricDescriptorRequest(),
+            name="name_value",
         )
 
 
-@pytest.mark.parametrize("request_type", [metric_service.ListTimeSeriesRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        metric_service.ListTimeSeriesRequest,
+        dict,
+    ],
+)
 def test_list_time_series(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metric_service.ListTimeSeriesResponse(
-            next_page_token="next_page_token_value", unit="unit_value",
+            next_page_token="next_page_token_value",
+            unit="unit_value",
         )
         response = client.list_time_series(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == metric_service.ListTimeSeriesRequest()
@@ -2436,15 +2642,16 @@
     assert response.unit == "unit_value"
 
 
 def test_list_time_series_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         client.list_time_series()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -2452,27 +2659,29 @@
 
 
 @pytest.mark.asyncio
 async def test_list_time_series_async(
     transport: str = "grpc_asyncio", request_type=metric_service.ListTimeSeriesRequest
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.ListTimeSeriesResponse(
-                next_page_token="next_page_token_value", unit="unit_value",
+                next_page_token="next_page_token_value",
+                unit="unit_value",
             )
         )
         response = await client.list_time_series(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -2486,48 +2695,53 @@
 
 @pytest.mark.asyncio
 async def test_list_time_series_async_from_dict():
     await test_list_time_series_async(request_type=dict)
 
 
 def test_list_time_series_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.ListTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         call.return_value = metric_service.ListTimeSeriesResponse()
         client.list_time_series(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_time_series_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.ListTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.ListTimeSeriesResponse()
         )
         await client.list_time_series(request)
@@ -2535,19 +2749,24 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_time_series_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = metric_service.ListTimeSeriesResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
@@ -2573,15 +2792,17 @@
         assert arg == mock_val
         arg = args[0].view
         mock_val = metric_service.ListTimeSeriesRequest.TimeSeriesView.HEADERS
         assert arg == mock_val
 
 
 def test_list_time_series_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_time_series(
             metric_service.ListTimeSeriesRequest(),
             name="name_value",
@@ -2648,15 +2869,16 @@
             interval=common.TimeInterval(end_time=timestamp_pb2.Timestamp(seconds=751)),
             view=metric_service.ListTimeSeriesRequest.TimeSeriesView.HEADERS,
         )
 
 
 def test_list_time_series_pager(transport_name: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         # Set the response to a series of pages.
         call.side_effect = (
             metric_service.ListTimeSeriesResponse(
@@ -2664,41 +2886,49 @@
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[], next_page_token="def",
+                time_series=[],
+                next_page_token="def",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(),], next_page_token="ghi",
+                time_series=[
+                    gm_metric.TimeSeries(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(), gm_metric.TimeSeries(),],
+                time_series=[
+                    gm_metric.TimeSeries(),
+                    gm_metric.TimeSeries(),
+                ],
             ),
             RuntimeError,
         )
 
         metadata = ()
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_time_series(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, gm_metric.TimeSeries) for i in results)
 
 
 def test_list_time_series_pages(transport_name: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_time_series), "__call__") as call:
         # Set the response to a series of pages.
         call.side_effect = (
             metric_service.ListTimeSeriesResponse(
@@ -2706,32 +2936,41 @@
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[], next_page_token="def",
+                time_series=[],
+                next_page_token="def",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(),], next_page_token="ghi",
+                time_series=[
+                    gm_metric.TimeSeries(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(), gm_metric.TimeSeries(),],
+                time_series=[
+                    gm_metric.TimeSeries(),
+                    gm_metric.TimeSeries(),
+                ],
             ),
             RuntimeError,
         )
         pages = list(client.list_time_series(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.asyncio
 async def test_list_time_series_async_pager():
-    client = MetricServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = MetricServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_time_series), "__call__", new_callable=mock.AsyncMock
     ) as call:
         # Set the response to a series of pages.
         call.side_effect = (
@@ -2740,37 +2979,48 @@
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[], next_page_token="def",
+                time_series=[],
+                next_page_token="def",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(),], next_page_token="ghi",
+                time_series=[
+                    gm_metric.TimeSeries(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(), gm_metric.TimeSeries(),],
+                time_series=[
+                    gm_metric.TimeSeries(),
+                    gm_metric.TimeSeries(),
+                ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_time_series(request={},)
+        async_pager = await client.list_time_series(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, gm_metric.TimeSeries) for i in responses)
 
 
 @pytest.mark.asyncio
 async def test_list_time_series_async_pages():
-    client = MetricServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = MetricServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_time_series), "__call__", new_callable=mock.AsyncMock
     ) as call:
         # Set the response to a series of pages.
         call.side_effect = (
@@ -2779,37 +3029,51 @@
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                     gm_metric.TimeSeries(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[], next_page_token="def",
+                time_series=[],
+                next_page_token="def",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(),], next_page_token="ghi",
+                time_series=[
+                    gm_metric.TimeSeries(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.ListTimeSeriesResponse(
-                time_series=[gm_metric.TimeSeries(), gm_metric.TimeSeries(),],
+                time_series=[
+                    gm_metric.TimeSeries(),
+                    gm_metric.TimeSeries(),
+                ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_time_series(request={})).pages:
+        async for page_ in (
+            await client.list_time_series(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.CreateTimeSeriesRequest, dict,]
+    "request_type",
+    [
+        metric_service.CreateTimeSeriesRequest,
+        dict,
+    ],
 )
 def test_create_time_series(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2829,15 +3093,16 @@
     assert response is None
 
 
 def test_create_time_series_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_time_series), "__call__"
     ) as call:
         client.create_time_series()
@@ -2847,15 +3112,16 @@
 
 
 @pytest.mark.asyncio
 async def test_create_time_series_async(
     transport: str = "grpc_asyncio", request_type=metric_service.CreateTimeSeriesRequest
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2877,21 +3143,23 @@
 
 @pytest.mark.asyncio
 async def test_create_time_series_async_from_dict():
     await test_create_time_series_async(request_type=dict)
 
 
 def test_create_time_series_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.CreateTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_time_series), "__call__"
     ) as call:
         call.return_value = None
         client.create_time_series(request)
@@ -2899,28 +3167,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_time_series_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.CreateTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_time_series), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.create_time_series(request)
@@ -2928,19 +3199,24 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_create_time_series_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_time_series), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
@@ -2962,15 +3238,17 @@
         assert arg == mock_val
         arg = args[0].time_series
         mock_val = [gm_metric.TimeSeries(metric=metric_pb2.Metric(type="type_value"))]
         assert arg == mock_val
 
 
 def test_create_time_series_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.create_time_series(
             metric_service.CreateTimeSeriesRequest(),
             name="name_value",
@@ -3030,19 +3308,24 @@
             time_series=[
                 gm_metric.TimeSeries(metric=metric_pb2.Metric(type="type_value"))
             ],
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [metric_service.CreateTimeSeriesRequest, dict,]
+    "request_type",
+    [
+        metric_service.CreateTimeSeriesRequest,
+        dict,
+    ],
 )
 def test_create_service_time_series(request_type, transport: str = "grpc"):
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3062,15 +3345,16 @@
     assert response is None
 
 
 def test_create_service_time_series_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = MetricServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_time_series), "__call__"
     ) as call:
         client.create_service_time_series()
@@ -3080,15 +3364,16 @@
 
 
 @pytest.mark.asyncio
 async def test_create_service_time_series_async(
     transport: str = "grpc_asyncio", request_type=metric_service.CreateTimeSeriesRequest
 ):
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3110,21 +3395,23 @@
 
 @pytest.mark.asyncio
 async def test_create_service_time_series_async_from_dict():
     await test_create_service_time_series_async(request_type=dict)
 
 
 def test_create_service_time_series_field_headers():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.CreateTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_time_series), "__call__"
     ) as call:
         call.return_value = None
         client.create_service_time_series(request)
@@ -3132,28 +3419,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_service_time_series_field_headers_async():
     client = MetricServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.CreateTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_time_series), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.create_service_time_series(request)
@@ -3161,19 +3451,24 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_create_service_time_series_flattened():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_time_series), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
@@ -3195,15 +3490,17 @@
         assert arg == mock_val
         arg = args[0].time_series
         mock_val = [gm_metric.TimeSeries(metric=metric_pb2.Metric(type="type_value"))]
         assert arg == mock_val
 
 
 def test_create_service_time_series_flattened_error():
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.create_service_time_series(
             metric_service.CreateTimeSeriesRequest(),
             name="name_value",
@@ -3269,15 +3566,16 @@
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.MetricServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = MetricServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.MetricServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -3289,15 +3587,18 @@
     # It is an error to provide an api_key and a transport instance.
     transport = transports.MetricServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
-        client = MetricServiceClient(client_options=options, transport=transport,)
+        client = MetricServiceClient(
+            client_options=options,
+            transport=transport,
+        )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = MetricServiceClient(
             client_options=options, credentials=ga_credentials.AnonymousCredentials()
@@ -3305,15 +3606,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.MetricServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = MetricServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.MetricServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3348,18 +3650,36 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = MetricServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
-    client = MetricServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
-    assert isinstance(client.transport, transports.MetricServiceGrpcTransport,)
+    client = MetricServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert isinstance(
+        client.transport,
+        transports.MetricServiceGrpcTransport,
+    )
 
 
 def test_metric_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.MetricServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
@@ -3393,26 +3713,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_metric_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.metric_service.transports.MetricServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.MetricServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -3557,52 +3886,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_metric_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_metric_service_host_no_port(transport_name):
     client = MetricServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_metric_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_metric_service_host_with_port(transport_name):
     client = MetricServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_metric_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.MetricServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_metric_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.MetricServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -3725,15 +4072,16 @@
 """
 
 
 def test_monitored_resource_descriptor_path():
     project = "oyster"
     monitored_resource_descriptor = "nudibranch"
     expected = "projects/{project}/monitoredResourceDescriptors/{monitored_resource_descriptor}".format(
-        project=project, monitored_resource_descriptor=monitored_resource_descriptor,
+        project=project,
+        monitored_resource_descriptor=monitored_resource_descriptor,
     )
     actual = MetricServiceClient.monitored_resource_descriptor_path(
         project, monitored_resource_descriptor
     )
     assert expected == actual
 
 
@@ -3749,15 +4097,16 @@
     assert expected == actual
 
 
 def test_time_series_path():
     project = "winkle"
     time_series = "nautilus"
     expected = "projects/{project}/timeSeries/{time_series}".format(
-        project=project, time_series=time_series,
+        project=project,
+        time_series=time_series,
     )
     actual = MetricServiceClient.time_series_path(project, time_series)
     assert expected == actual
 
 
 def test_parse_time_series_path():
     expected = {
@@ -3789,15 +4138,17 @@
     # Check that the path construction is reversible.
     actual = MetricServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "whelk"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = MetricServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "octopus",
@@ -3807,15 +4158,17 @@
     # Check that the path construction is reversible.
     actual = MetricServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "oyster"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = MetricServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "nudibranch",
@@ -3825,15 +4178,17 @@
     # Check that the path construction is reversible.
     actual = MetricServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "cuttlefish"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = MetricServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "mussel",
@@ -3845,15 +4200,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "winkle"
     location = "nautilus"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = MetricServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -3870,32 +4226,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.MetricServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = MetricServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.MetricServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = MetricServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = MetricServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_notification_channel_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_notification_channel_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -96,29 +102,34 @@
     assert (
         NotificationChannelServiceClient._get_default_mtls_endpoint(non_googleapi)
         == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class",
-    [NotificationChannelServiceClient, NotificationChannelServiceAsyncClient,],
+    "client_class,transport_name",
+    [
+        (NotificationChannelServiceClient, "grpc"),
+        (NotificationChannelServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_notification_channel_service_client_from_service_account_info(client_class):
+def test_notification_channel_service_client_from_service_account_info(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.NotificationChannelServiceGrpcTransport, "grpc"),
         (transports.NotificationChannelServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -139,32 +150,41 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class",
-    [NotificationChannelServiceClient, NotificationChannelServiceAsyncClient,],
+    "client_class,transport_name",
+    [
+        (NotificationChannelServiceClient, "grpc"),
+        (NotificationChannelServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_notification_channel_service_client_from_service_account_file(client_class):
+def test_notification_channel_service_client_from_service_account_file(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_notification_channel_service_client_get_transport_class():
     transport = NotificationChannelServiceClient.get_transport_class()
     available_transports = [
         transports.NotificationChannelServiceGrpcTransport,
     ]
@@ -529,15 +549,17 @@
         ),
     ],
 )
 def test_notification_channel_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -675,32 +697,38 @@
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
-    [notification_service.ListNotificationChannelDescriptorsRequest, dict,],
+    [
+        notification_service.ListNotificationChannelDescriptorsRequest,
+        dict,
+    ],
 )
 def test_list_notification_channel_descriptors(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channel_descriptors), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
-        call.return_value = notification_service.ListNotificationChannelDescriptorsResponse(
-            next_page_token="next_page_token_value",
+        call.return_value = (
+            notification_service.ListNotificationChannelDescriptorsResponse(
+                next_page_token="next_page_token_value",
+            )
         )
         response = client.list_notification_channel_descriptors(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert (
@@ -712,15 +740,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_notification_channel_descriptors_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channel_descriptors), "__call__"
     ) as call:
         client.list_notification_channel_descriptors()
@@ -733,15 +762,16 @@
 
 @pytest.mark.asyncio
 async def test_list_notification_channel_descriptors_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.ListNotificationChannelDescriptorsRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -778,15 +808,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.ListNotificationChannelDescriptorsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channel_descriptors), "__call__"
     ) as call:
         call.return_value = (
             notification_service.ListNotificationChannelDescriptorsResponse()
@@ -796,28 +826,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_notification_channel_descriptors_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.ListNotificationChannelDescriptorsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channel_descriptors), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification_service.ListNotificationChannelDescriptorsResponse()
@@ -827,15 +860,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_notification_channel_descriptors_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -845,15 +881,17 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = (
             notification_service.ListNotificationChannelDescriptorsResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_notification_channel_descriptors(name="name_value",)
+        client.list_notification_channel_descriptors(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -920,15 +958,16 @@
             notification_service.ListNotificationChannelDescriptorsRequest(),
             name="name_value",
         )
 
 
 def test_list_notification_channel_descriptors_pager(transport_name: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channel_descriptors), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -938,18 +977,21 @@
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[], next_page_token="def",
+                channel_descriptors=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[notification.NotificationChannelDescriptor(),],
+                channel_descriptors=[
+                    notification.NotificationChannelDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
                 channel_descriptors=[
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
@@ -961,24 +1003,25 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_notification_channel_descriptors(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(
             isinstance(i, notification.NotificationChannelDescriptor) for i in results
         )
 
 
 def test_list_notification_channel_descriptors_pages(transport_name: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channel_descriptors), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -988,18 +1031,21 @@
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[], next_page_token="def",
+                channel_descriptors=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[notification.NotificationChannelDescriptor(),],
+                channel_descriptors=[
+                    notification.NotificationChannelDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
                 channel_descriptors=[
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
@@ -1030,32 +1076,37 @@
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[], next_page_token="def",
+                channel_descriptors=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[notification.NotificationChannelDescriptor(),],
+                channel_descriptors=[
+                    notification.NotificationChannelDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
                 channel_descriptors=[
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_notification_channel_descriptors(request={},)
+        async_pager = await client.list_notification_channel_descriptors(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(
             isinstance(i, notification.NotificationChannelDescriptor) for i in responses
         )
 
@@ -1079,44 +1130,51 @@
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[], next_page_token="def",
+                channel_descriptors=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
-                channel_descriptors=[notification.NotificationChannelDescriptor(),],
+                channel_descriptors=[
+                    notification.NotificationChannelDescriptor(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelDescriptorsResponse(
                 channel_descriptors=[
                     notification.NotificationChannelDescriptor(),
                     notification.NotificationChannelDescriptor(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
         async for page_ in (
             await client.list_notification_channel_descriptors(request={})
-        ).pages:
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
-    [notification_service.GetNotificationChannelDescriptorRequest, dict,],
+    [
+        notification_service.GetNotificationChannelDescriptorRequest,
+        dict,
+    ],
 )
 def test_get_notification_channel_descriptor(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1147,15 +1205,16 @@
     assert response.supported_tiers == [common.ServiceTier.SERVICE_TIER_BASIC]
 
 
 def test_get_notification_channel_descriptor_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_descriptor), "__call__"
     ) as call:
         client.get_notification_channel_descriptor()
@@ -1166,15 +1225,16 @@
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_descriptor_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.GetNotificationChannelDescriptorRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1217,15 +1277,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.GetNotificationChannelDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_descriptor), "__call__"
     ) as call:
         call.return_value = notification.NotificationChannelDescriptor()
         client.get_notification_channel_descriptor(request)
@@ -1233,28 +1293,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_descriptor_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.GetNotificationChannelDescriptorRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_descriptor), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannelDescriptor()
@@ -1264,15 +1327,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_notification_channel_descriptor_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1280,15 +1346,17 @@
     with mock.patch.object(
         type(client.transport.get_notification_channel_descriptor), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = notification.NotificationChannelDescriptor()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_notification_channel_descriptor(name="name_value",)
+        client.get_notification_channel_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1323,15 +1391,17 @@
         call.return_value = notification.NotificationChannelDescriptor()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannelDescriptor()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_notification_channel_descriptor(name="name_value",)
+        response = await client.get_notification_channel_descriptor(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1350,32 +1420,38 @@
         await client.get_notification_channel_descriptor(
             notification_service.GetNotificationChannelDescriptorRequest(),
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [notification_service.ListNotificationChannelsRequest, dict,]
+    "request_type",
+    [
+        notification_service.ListNotificationChannelsRequest,
+        dict,
+    ],
 )
 def test_list_notification_channels(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = notification_service.ListNotificationChannelsResponse(
-            next_page_token="next_page_token_value", total_size=1086,
+            next_page_token="next_page_token_value",
+            total_size=1086,
         )
         response = client.list_notification_channels(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == notification_service.ListNotificationChannelsRequest()
@@ -1386,15 +1462,16 @@
     assert response.total_size == 1086
 
 
 def test_list_notification_channels_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         client.list_notification_channels()
@@ -1405,29 +1482,31 @@
 
 @pytest.mark.asyncio
 async def test_list_notification_channels_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.ListNotificationChannelsRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification_service.ListNotificationChannelsResponse(
-                next_page_token="next_page_token_value", total_size=1086,
+                next_page_token="next_page_token_value",
+                total_size=1086,
             )
         )
         response = await client.list_notification_channels(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1449,15 +1528,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.ListNotificationChannelsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         call.return_value = notification_service.ListNotificationChannelsResponse()
         client.list_notification_channels(request)
@@ -1465,28 +1544,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_notification_channels_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.ListNotificationChannelsRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification_service.ListNotificationChannelsResponse()
@@ -1496,15 +1578,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_list_notification_channels_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1512,15 +1597,17 @@
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = notification_service.ListNotificationChannelsResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_notification_channels(name="name_value",)
+        client.list_notification_channels(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1532,15 +1619,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_notification_channels(
-            notification_service.ListNotificationChannelsRequest(), name="name_value",
+            notification_service.ListNotificationChannelsRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_notification_channels_flattened_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1554,15 +1642,17 @@
         call.return_value = notification_service.ListNotificationChannelsResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification_service.ListNotificationChannelsResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_notification_channels(name="name_value",)
+        response = await client.list_notification_channels(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1575,21 +1665,23 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_notification_channels(
-            notification_service.ListNotificationChannelsRequest(), name="name_value",
+            notification_service.ListNotificationChannelsRequest(),
+            name="name_value",
         )
 
 
 def test_list_notification_channels_pager(transport_name: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -1599,18 +1691,21 @@
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[], next_page_token="def",
+                notification_channels=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[notification.NotificationChannel(),],
+                notification_channels=[
+                    notification.NotificationChannel(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelsResponse(
                 notification_channels=[
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
@@ -1622,22 +1717,23 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.list_notification_channels(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, notification.NotificationChannel) for i in results)
 
 
 def test_list_notification_channels_pages(transport_name: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_notification_channels), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -1647,18 +1743,21 @@
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[], next_page_token="def",
+                notification_channels=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[notification.NotificationChannel(),],
+                notification_channels=[
+                    notification.NotificationChannel(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelsResponse(
                 notification_channels=[
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
@@ -1689,32 +1788,37 @@
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[], next_page_token="def",
+                notification_channels=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[notification.NotificationChannel(),],
+                notification_channels=[
+                    notification.NotificationChannel(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelsResponse(
                 notification_channels=[
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_notification_channels(request={},)
+        async_pager = await client.list_notification_channels(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, notification.NotificationChannel) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -1736,41 +1840,51 @@
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
                 next_page_token="abc",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[], next_page_token="def",
+                notification_channels=[],
+                next_page_token="def",
             ),
             notification_service.ListNotificationChannelsResponse(
-                notification_channels=[notification.NotificationChannel(),],
+                notification_channels=[
+                    notification.NotificationChannel(),
+                ],
                 next_page_token="ghi",
             ),
             notification_service.ListNotificationChannelsResponse(
                 notification_channels=[
                     notification.NotificationChannel(),
                     notification.NotificationChannel(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_notification_channels(request={})).pages:
+        async for page_ in (
+            await client.list_notification_channels(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
-    "request_type", [notification_service.GetNotificationChannelRequest, dict,]
+    "request_type",
+    [
+        notification_service.GetNotificationChannelRequest,
+        dict,
+    ],
 )
 def test_get_notification_channel(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1804,15 +1918,16 @@
     )
 
 
 def test_get_notification_channel_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel), "__call__"
     ) as call:
         client.get_notification_channel()
@@ -1823,15 +1938,16 @@
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.GetNotificationChannelRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1877,15 +1993,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.GetNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel), "__call__"
     ) as call:
         call.return_value = notification.NotificationChannel()
         client.get_notification_channel(request)
@@ -1893,28 +2009,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.GetNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannel()
@@ -1924,15 +2043,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_notification_channel_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1940,15 +2062,17 @@
     with mock.patch.object(
         type(client.transport.get_notification_channel), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = notification.NotificationChannel()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_notification_channel(name="name_value",)
+        client.get_notification_channel(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1960,15 +2084,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_notification_channel(
-            notification_service.GetNotificationChannelRequest(), name="name_value",
+            notification_service.GetNotificationChannelRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_flattened_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1982,15 +2107,17 @@
         call.return_value = notification.NotificationChannel()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannel()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_notification_channel(name="name_value",)
+        response = await client.get_notification_channel(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -2003,24 +2130,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_notification_channel(
-            notification_service.GetNotificationChannelRequest(), name="name_value",
+            notification_service.GetNotificationChannelRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [notification_service.CreateNotificationChannelRequest, dict,]
+    "request_type",
+    [
+        notification_service.CreateNotificationChannelRequest,
+        dict,
+    ],
 )
 def test_create_notification_channel(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2054,15 +2187,16 @@
     )
 
 
 def test_create_notification_channel_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_notification_channel), "__call__"
     ) as call:
         client.create_notification_channel()
@@ -2073,15 +2207,16 @@
 
 @pytest.mark.asyncio
 async def test_create_notification_channel_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.CreateNotificationChannelRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2127,15 +2262,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.CreateNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_notification_channel), "__call__"
     ) as call:
         call.return_value = notification.NotificationChannel()
         client.create_notification_channel(request)
@@ -2143,28 +2278,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_notification_channel_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.CreateNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_notification_channel), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannel()
@@ -2174,15 +2312,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_create_notification_channel_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2274,19 +2415,24 @@
             notification_service.CreateNotificationChannelRequest(),
             name="name_value",
             notification_channel=notification.NotificationChannel(type_="type__value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [notification_service.UpdateNotificationChannelRequest, dict,]
+    "request_type",
+    [
+        notification_service.UpdateNotificationChannelRequest,
+        dict,
+    ],
 )
 def test_update_notification_channel(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2320,15 +2466,16 @@
     )
 
 
 def test_update_notification_channel_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_notification_channel), "__call__"
     ) as call:
         client.update_notification_channel()
@@ -2339,15 +2486,16 @@
 
 @pytest.mark.asyncio
 async def test_update_notification_channel_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.UpdateNotificationChannelRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2393,15 +2541,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.UpdateNotificationChannelRequest()
 
-    request.notification_channel.name = "notification_channel.name/value"
+    request.notification_channel.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_notification_channel), "__call__"
     ) as call:
         call.return_value = notification.NotificationChannel()
         client.update_notification_channel(request)
@@ -2411,29 +2559,29 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "notification_channel.name=notification_channel.name/value",
+        "notification_channel.name=name_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_update_notification_channel_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.UpdateNotificationChannelRequest()
 
-    request.notification_channel.name = "notification_channel.name/value"
+    request.notification_channel.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_notification_channel), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannel()
@@ -2445,15 +2593,15 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "notification_channel.name=notification_channel.name/value",
+        "notification_channel.name=name_value",
     ) in kw["metadata"]
 
 
 def test_update_notification_channel_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2546,19 +2694,24 @@
             notification_service.UpdateNotificationChannelRequest(),
             update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
             notification_channel=notification.NotificationChannel(type_="type__value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [notification_service.DeleteNotificationChannelRequest, dict,]
+    "request_type",
+    [
+        notification_service.DeleteNotificationChannelRequest,
+        dict,
+    ],
 )
 def test_delete_notification_channel(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2578,15 +2731,16 @@
     assert response is None
 
 
 def test_delete_notification_channel_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_notification_channel), "__call__"
     ) as call:
         client.delete_notification_channel()
@@ -2597,15 +2751,16 @@
 
 @pytest.mark.asyncio
 async def test_delete_notification_channel_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.DeleteNotificationChannelRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2635,15 +2790,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.DeleteNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_notification_channel), "__call__"
     ) as call:
         call.return_value = None
         client.delete_notification_channel(request)
@@ -2651,28 +2806,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_notification_channel_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.DeleteNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_notification_channel), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_notification_channel(request)
@@ -2680,15 +2838,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_notification_channel_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2697,15 +2858,16 @@
         type(client.transport.delete_notification_channel), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         client.delete_notification_channel(
-            name="name_value", force=True,
+            name="name_value",
+            force=True,
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -2744,15 +2906,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         response = await client.delete_notification_channel(
-            name="name_value", force=True,
+            name="name_value",
+            force=True,
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -2777,21 +2940,25 @@
             name="name_value",
             force=True,
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
-    [notification_service.SendNotificationChannelVerificationCodeRequest, dict,],
+    [
+        notification_service.SendNotificationChannelVerificationCodeRequest,
+        dict,
+    ],
 )
 def test_send_notification_channel_verification_code(
     request_type, transport: str = "grpc"
 ):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2814,15 +2981,16 @@
     assert response is None
 
 
 def test_send_notification_channel_verification_code_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.send_notification_channel_verification_code), "__call__"
     ) as call:
         client.send_notification_channel_verification_code()
@@ -2836,15 +3004,16 @@
 
 @pytest.mark.asyncio
 async def test_send_notification_channel_verification_code_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.SendNotificationChannelVerificationCodeRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2877,15 +3046,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.SendNotificationChannelVerificationCodeRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.send_notification_channel_verification_code), "__call__"
     ) as call:
         call.return_value = None
         client.send_notification_channel_verification_code(request)
@@ -2893,28 +3062,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_send_notification_channel_verification_code_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.SendNotificationChannelVerificationCodeRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.send_notification_channel_verification_code), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.send_notification_channel_verification_code(request)
@@ -2922,15 +3094,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_send_notification_channel_verification_code_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2938,15 +3113,17 @@
     with mock.patch.object(
         type(client.transport.send_notification_channel_verification_code), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.send_notification_channel_verification_code(name="name_value",)
+        client.send_notification_channel_verification_code(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -3009,34 +3186,40 @@
             notification_service.SendNotificationChannelVerificationCodeRequest(),
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
     "request_type",
-    [notification_service.GetNotificationChannelVerificationCodeRequest, dict,],
+    [
+        notification_service.GetNotificationChannelVerificationCodeRequest,
+        dict,
+    ],
 )
 def test_get_notification_channel_verification_code(
     request_type, transport: str = "grpc"
 ):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_verification_code), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
-        call.return_value = notification_service.GetNotificationChannelVerificationCodeResponse(
-            code="code_value",
+        call.return_value = (
+            notification_service.GetNotificationChannelVerificationCodeResponse(
+                code="code_value",
+            )
         )
         response = client.get_notification_channel_verification_code(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert (
@@ -3051,15 +3234,16 @@
     assert response.code == "code_value"
 
 
 def test_get_notification_channel_verification_code_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_verification_code), "__call__"
     ) as call:
         client.get_notification_channel_verification_code()
@@ -3073,15 +3257,16 @@
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_verification_code_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.GetNotificationChannelVerificationCodeRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3121,15 +3306,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.GetNotificationChannelVerificationCodeRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_verification_code), "__call__"
     ) as call:
         call.return_value = (
             notification_service.GetNotificationChannelVerificationCodeResponse()
@@ -3139,28 +3324,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_notification_channel_verification_code_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.GetNotificationChannelVerificationCodeRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_notification_channel_verification_code), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification_service.GetNotificationChannelVerificationCodeResponse()
@@ -3170,15 +3358,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_notification_channel_verification_code_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3188,15 +3379,17 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = (
             notification_service.GetNotificationChannelVerificationCodeResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_notification_channel_verification_code(name="name_value",)
+        client.get_notification_channel_verification_code(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -3262,19 +3455,24 @@
         await client.get_notification_channel_verification_code(
             notification_service.GetNotificationChannelVerificationCodeRequest(),
             name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [notification_service.VerifyNotificationChannelRequest, dict,]
+    "request_type",
+    [
+        notification_service.VerifyNotificationChannelRequest,
+        dict,
+    ],
 )
 def test_verify_notification_channel(request_type, transport: str = "grpc"):
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3308,15 +3506,16 @@
     )
 
 
 def test_verify_notification_channel_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = NotificationChannelServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.verify_notification_channel), "__call__"
     ) as call:
         client.verify_notification_channel()
@@ -3327,15 +3526,16 @@
 
 @pytest.mark.asyncio
 async def test_verify_notification_channel_async(
     transport: str = "grpc_asyncio",
     request_type=notification_service.VerifyNotificationChannelRequest,
 ):
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3381,15 +3581,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.VerifyNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.verify_notification_channel), "__call__"
     ) as call:
         call.return_value = notification.NotificationChannel()
         client.verify_notification_channel(request)
@@ -3397,28 +3597,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_verify_notification_channel_field_headers_async():
     client = NotificationChannelServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = notification_service.VerifyNotificationChannelRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.verify_notification_channel), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannel()
@@ -3428,15 +3631,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_verify_notification_channel_flattened():
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3445,15 +3651,16 @@
         type(client.transport.verify_notification_channel), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = notification.NotificationChannel()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         client.verify_notification_channel(
-            name="name_value", code="code_value",
+            name="name_value",
+            code="code_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -3494,15 +3701,16 @@
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             notification.NotificationChannel()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         response = await client.verify_notification_channel(
-            name="name_value", code="code_value",
+            name="name_value",
+            code="code_value",
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
@@ -3532,15 +3740,16 @@
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.NotificationChannelServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = NotificationChannelServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.NotificationChannelServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -3553,15 +3762,16 @@
     transport = transports.NotificationChannelServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = NotificationChannelServiceClient(
-            client_options=options, transport=transport,
+            client_options=options,
+            transport=transport,
         )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = NotificationChannelServiceClient(
@@ -3570,15 +3780,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.NotificationChannelServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = NotificationChannelServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.NotificationChannelServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3613,21 +3824,35 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = NotificationChannelServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     assert isinstance(
-        client.transport, transports.NotificationChannelServiceGrpcTransport,
+        client.transport,
+        transports.NotificationChannelServiceGrpcTransport,
     )
 
 
 def test_notification_channel_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.NotificationChannelServiceTransport(
@@ -3663,26 +3888,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_notification_channel_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.notification_channel_service.transports.NotificationChannelServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.NotificationChannelServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -3827,52 +4061,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_notification_channel_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_notification_channel_service_host_no_port(transport_name):
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_notification_channel_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_notification_channel_service_host_with_port(transport_name):
     client = NotificationChannelServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_notification_channel_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.NotificationChannelServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_notification_channel_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.NotificationChannelServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -3975,15 +4227,16 @@
             assert transport.grpc_channel == mock_grpc_channel
 
 
 def test_notification_channel_path():
     project = "squid"
     notification_channel = "clam"
     expected = "projects/{project}/notificationChannels/{notification_channel}".format(
-        project=project, notification_channel=notification_channel,
+        project=project,
+        notification_channel=notification_channel,
     )
     actual = NotificationChannelServiceClient.notification_channel_path(
         project, notification_channel
     )
     assert expected == actual
 
 
@@ -3998,16 +4251,19 @@
     actual = NotificationChannelServiceClient.parse_notification_channel_path(path)
     assert expected == actual
 
 
 def test_notification_channel_descriptor_path():
     project = "oyster"
     channel_descriptor = "nudibranch"
-    expected = "projects/{project}/notificationChannelDescriptors/{channel_descriptor}".format(
-        project=project, channel_descriptor=channel_descriptor,
+    expected = (
+        "projects/{project}/notificationChannelDescriptors/{channel_descriptor}".format(
+            project=project,
+            channel_descriptor=channel_descriptor,
+        )
     )
     actual = NotificationChannelServiceClient.notification_channel_descriptor_path(
         project, channel_descriptor
     )
     assert expected == actual
 
 
@@ -4017,16 +4273,18 @@
         "channel_descriptor": "mussel",
     }
     path = NotificationChannelServiceClient.notification_channel_descriptor_path(
         **expected
     )
 
     # Check that the path construction is reversible.
-    actual = NotificationChannelServiceClient.parse_notification_channel_descriptor_path(
-        path
+    actual = (
+        NotificationChannelServiceClient.parse_notification_channel_descriptor_path(
+            path
+        )
     )
     assert expected == actual
 
 
 def test_common_billing_account_path():
     billing_account = "winkle"
     expected = "billingAccounts/{billing_account}".format(
@@ -4047,15 +4305,17 @@
     # Check that the path construction is reversible.
     actual = NotificationChannelServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "scallop"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = NotificationChannelServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "abalone",
@@ -4065,15 +4325,17 @@
     # Check that the path construction is reversible.
     actual = NotificationChannelServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "squid"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = NotificationChannelServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "clam",
@@ -4083,15 +4345,17 @@
     # Check that the path construction is reversible.
     actual = NotificationChannelServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "whelk"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = NotificationChannelServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "octopus",
@@ -4103,15 +4367,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "oyster"
     location = "nudibranch"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = NotificationChannelServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -4128,32 +4393,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.NotificationChannelServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = NotificationChannelServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.NotificationChannelServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = NotificationChannelServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = NotificationChannelServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_query_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_query_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -78,27 +84,33 @@
     assert (
         QueryServiceClient._get_default_mtls_endpoint(sandbox_mtls_endpoint)
         == sandbox_mtls_endpoint
     )
     assert QueryServiceClient._get_default_mtls_endpoint(non_googleapi) == non_googleapi
 
 
-@pytest.mark.parametrize("client_class", [QueryServiceClient, QueryServiceAsyncClient,])
-def test_query_service_client_from_service_account_info(client_class):
+@pytest.mark.parametrize(
+    "client_class,transport_name",
+    [
+        (QueryServiceClient, "grpc"),
+        (QueryServiceAsyncClient, "grpc_asyncio"),
+    ],
+)
+def test_query_service_client_from_service_account_info(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.QueryServiceGrpcTransport, "grpc"),
         (transports.QueryServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -118,30 +130,40 @@
         service_account.Credentials, "with_always_use_jwt_access", create=True
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
-@pytest.mark.parametrize("client_class", [QueryServiceClient, QueryServiceAsyncClient,])
-def test_query_service_client_from_service_account_file(client_class):
+@pytest.mark.parametrize(
+    "client_class,transport_name",
+    [
+        (QueryServiceClient, "grpc"),
+        (QueryServiceAsyncClient, "grpc_asyncio"),
+    ],
+)
+def test_query_service_client_from_service_account_file(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_query_service_client_get_transport_class():
     transport = QueryServiceClient.get_transport_class()
     available_transports = [
         transports.QueryServiceGrpcTransport,
     ]
@@ -473,15 +495,17 @@
         ),
     ],
 )
 def test_query_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -615,18 +639,25 @@
             options=[
                 ("grpc.max_send_message_length", -1),
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
-@pytest.mark.parametrize("request_type", [metric_service.QueryTimeSeriesRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        metric_service.QueryTimeSeriesRequest,
+        dict,
+    ],
+)
 def test_query_time_series(request_type, transport: str = "grpc"):
     client = QueryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -649,15 +680,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_query_time_series_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = QueryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series), "__call__"
     ) as call:
         client.query_time_series()
@@ -667,15 +699,16 @@
 
 
 @pytest.mark.asyncio
 async def test_query_time_series_async(
     transport: str = "grpc_asyncio", request_type=metric_service.QueryTimeSeriesRequest
 ):
     client = QueryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -702,21 +735,23 @@
 
 @pytest.mark.asyncio
 async def test_query_time_series_async_from_dict():
     await test_query_time_series_async(request_type=dict)
 
 
 def test_query_time_series_field_headers():
-    client = QueryServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = QueryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.QueryTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series), "__call__"
     ) as call:
         call.return_value = metric_service.QueryTimeSeriesResponse()
         client.query_time_series(request)
@@ -724,26 +759,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_query_time_series_field_headers_async():
-    client = QueryServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials(),)
+    client = QueryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = metric_service.QueryTimeSeriesRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             metric_service.QueryTimeSeriesResponse()
@@ -753,20 +793,24 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_query_time_series_pager(transport_name: str = "grpc"):
     client = QueryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -776,41 +820,49 @@
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[], next_page_token="def",
+                time_series_data=[],
+                next_page_token="def",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(),], next_page_token="ghi",
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(), metric.TimeSeriesData(),],
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                    metric.TimeSeriesData(),
+                ],
             ),
             RuntimeError,
         )
 
         metadata = ()
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", ""),)),
         )
         pager = client.query_time_series(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, metric.TimeSeriesData) for i in results)
 
 
 def test_query_time_series_pages(transport_name: str = "grpc"):
     client = QueryServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -820,32 +872,41 @@
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[], next_page_token="def",
+                time_series_data=[],
+                next_page_token="def",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(),], next_page_token="ghi",
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(), metric.TimeSeriesData(),],
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                    metric.TimeSeriesData(),
+                ],
             ),
             RuntimeError,
         )
         pages = list(client.query_time_series(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.asyncio
 async def test_query_time_series_async_pager():
-    client = QueryServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = QueryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -856,37 +917,48 @@
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[], next_page_token="def",
+                time_series_data=[],
+                next_page_token="def",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(),], next_page_token="ghi",
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(), metric.TimeSeriesData(),],
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                    metric.TimeSeriesData(),
+                ],
             ),
             RuntimeError,
         )
-        async_pager = await client.query_time_series(request={},)
+        async_pager = await client.query_time_series(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, metric.TimeSeriesData) for i in responses)
 
 
 @pytest.mark.asyncio
 async def test_query_time_series_async_pages():
-    client = QueryServiceAsyncClient(credentials=ga_credentials.AnonymousCredentials,)
+    client = QueryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.query_time_series),
         "__call__",
         new_callable=mock.AsyncMock,
     ) as call:
@@ -897,39 +969,49 @@
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                     metric.TimeSeriesData(),
                 ],
                 next_page_token="abc",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[], next_page_token="def",
+                time_series_data=[],
+                next_page_token="def",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(),], next_page_token="ghi",
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                ],
+                next_page_token="ghi",
             ),
             metric_service.QueryTimeSeriesResponse(
-                time_series_data=[metric.TimeSeriesData(), metric.TimeSeriesData(),],
+                time_series_data=[
+                    metric.TimeSeriesData(),
+                    metric.TimeSeriesData(),
+                ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.query_time_series(request={})).pages:
+        async for page_ in (
+            await client.query_time_series(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.QueryServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = QueryServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.QueryServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -941,15 +1023,18 @@
     # It is an error to provide an api_key and a transport instance.
     transport = transports.QueryServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
-        client = QueryServiceClient(client_options=options, transport=transport,)
+        client = QueryServiceClient(
+            client_options=options,
+            transport=transport,
+        )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = QueryServiceClient(
             client_options=options, credentials=ga_credentials.AnonymousCredentials()
@@ -957,15 +1042,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.QueryServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = QueryServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.QueryServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1000,18 +1086,36 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = QueryServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
-    client = QueryServiceClient(credentials=ga_credentials.AnonymousCredentials(),)
-    assert isinstance(client.transport, transports.QueryServiceGrpcTransport,)
+    client = QueryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert isinstance(
+        client.transport,
+        transports.QueryServiceGrpcTransport,
+    )
 
 
 def test_query_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.QueryServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
@@ -1035,26 +1139,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_query_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.query_service.transports.QueryServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.QueryServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -1192,52 +1305,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_query_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_query_service_host_no_port(transport_name):
     client = QueryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_query_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_query_service_host_with_port(transport_name):
     client = QueryServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_query_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.QueryServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_query_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.QueryServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -1350,15 +1481,17 @@
     # Check that the path construction is reversible.
     actual = QueryServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "whelk"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = QueryServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "octopus",
@@ -1368,15 +1501,17 @@
     # Check that the path construction is reversible.
     actual = QueryServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "oyster"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = QueryServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "nudibranch",
@@ -1386,15 +1521,17 @@
     # Check that the path construction is reversible.
     actual = QueryServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "cuttlefish"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = QueryServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "mussel",
@@ -1406,15 +1543,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "winkle"
     location = "nautilus"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = QueryServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -1431,32 +1569,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.QueryServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = QueryServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.QueryServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = QueryServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = QueryServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_service_monitoring_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_service_monitoring_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -91,29 +97,34 @@
     assert (
         ServiceMonitoringServiceClient._get_default_mtls_endpoint(non_googleapi)
         == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class",
-    [ServiceMonitoringServiceClient, ServiceMonitoringServiceAsyncClient,],
+    "client_class,transport_name",
+    [
+        (ServiceMonitoringServiceClient, "grpc"),
+        (ServiceMonitoringServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_service_monitoring_service_client_from_service_account_info(client_class):
+def test_service_monitoring_service_client_from_service_account_info(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.ServiceMonitoringServiceGrpcTransport, "grpc"),
         (transports.ServiceMonitoringServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -134,32 +145,41 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class",
-    [ServiceMonitoringServiceClient, ServiceMonitoringServiceAsyncClient,],
+    "client_class,transport_name",
+    [
+        (ServiceMonitoringServiceClient, "grpc"),
+        (ServiceMonitoringServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_service_monitoring_service_client_from_service_account_file(client_class):
+def test_service_monitoring_service_client_from_service_account_file(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_service_monitoring_service_client_get_transport_class():
     transport = ServiceMonitoringServiceClient.get_transport_class()
     available_transports = [
         transports.ServiceMonitoringServiceGrpcTransport,
     ]
@@ -524,15 +544,17 @@
         ),
     ],
 )
 def test_service_monitoring_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -668,29 +690,38 @@
             options=[
                 ("grpc.max_send_message_length", -1),
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
-@pytest.mark.parametrize("request_type", [service_service.CreateServiceRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        service_service.CreateServiceRequest,
+        dict,
+    ],
+)
 def test_create_service(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_service.Service(
-            name="name_value", display_name="display_name_value", custom=None,
+            name="name_value",
+            display_name="display_name_value",
+            custom=None,
         )
         response = client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service_service.CreateServiceRequest()
@@ -701,15 +732,16 @@
     assert response.display_name == "display_name_value"
 
 
 def test_create_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         client.create_service()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -717,26 +749,30 @@
 
 
 @pytest.mark.asyncio
 async def test_create_service_async(
     transport: str = "grpc_asyncio", request_type=service_service.CreateServiceRequest
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            gm_service.Service(name="name_value", display_name="display_name_value",)
+            gm_service.Service(
+                name="name_value",
+                display_name="display_name_value",
+            )
         )
         response = await client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == service_service.CreateServiceRequest()
@@ -757,71 +793,78 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.CreateServiceRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         call.return_value = gm_service.Service()
         client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_service_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.CreateServiceRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_service.Service())
         await client.create_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 def test_create_service_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_service.Service()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         client.create_service(
-            parent="parent_value", service=gm_service.Service(name="name_value"),
+            parent="parent_value",
+            service=gm_service.Service(name="name_value"),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
@@ -858,15 +901,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = gm_service.Service()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_service.Service())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
         response = await client.create_service(
-            parent="parent_value", service=gm_service.Service(name="name_value"),
+            parent="parent_value",
+            service=gm_service.Service(name="name_value"),
         )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
@@ -889,29 +933,38 @@
         await client.create_service(
             service_service.CreateServiceRequest(),
             parent="parent_value",
             service=gm_service.Service(name="name_value"),
         )
 
 
-@pytest.mark.parametrize("request_type", [service_service.GetServiceRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        service_service.GetServiceRequest,
+        dict,
+    ],
+)
 def test_get_service(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = service.Service(
-            name="name_value", display_name="display_name_value", custom=None,
+            name="name_value",
+            display_name="display_name_value",
+            custom=None,
         )
         response = client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service_service.GetServiceRequest()
@@ -922,15 +975,16 @@
     assert response.display_name == "display_name_value"
 
 
 def test_get_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         client.get_service()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -938,26 +992,30 @@
 
 
 @pytest.mark.asyncio
 async def test_get_service_async(
     transport: str = "grpc_asyncio", request_type=service_service.GetServiceRequest
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            service.Service(name="name_value", display_name="display_name_value",)
+            service.Service(
+                name="name_value",
+                display_name="display_name_value",
+            )
         )
         response = await client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == service_service.GetServiceRequest()
@@ -978,70 +1036,78 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.GetServiceRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         call.return_value = service.Service()
         client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_service_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.GetServiceRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(service.Service())
         await client.get_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_service_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = service.Service()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_service(name="name_value",)
+        client.get_service(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1053,15 +1119,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_service(
-            service_service.GetServiceRequest(), name="name_value",
+            service_service.GetServiceRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_service_flattened_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1071,15 +1138,17 @@
     with mock.patch.object(type(client.transport.get_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = service.Service()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(service.Service())
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_service(name="name_value",)
+        response = await client.get_service(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1092,22 +1161,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_service(
-            service_service.GetServiceRequest(), name="name_value",
+            service_service.GetServiceRequest(),
+            name="name_value",
         )
 
 
-@pytest.mark.parametrize("request_type", [service_service.ListServicesRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        service_service.ListServicesRequest,
+        dict,
+    ],
+)
 def test_list_services(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1128,15 +1205,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_services_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_services), "__call__") as call:
         client.list_services()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1144,15 +1222,16 @@
 
 
 @pytest.mark.asyncio
 async def test_list_services_async(
     transport: str = "grpc_asyncio", request_type=service_service.ListServicesRequest
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1185,42 +1264,45 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.ListServicesRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_services), "__call__") as call:
         call.return_value = service_service.ListServicesResponse()
         client.list_services(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_services_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.ListServicesRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_services), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service_service.ListServicesResponse()
         )
         await client.list_services(request)
@@ -1228,29 +1310,34 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 def test_list_services_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_services), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = service_service.ListServicesResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_services(parent="parent_value",)
+        client.list_services(
+            parent="parent_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
         mock_val = "parent_value"
@@ -1262,15 +1349,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_services(
-            service_service.ListServicesRequest(), parent="parent_value",
+            service_service.ListServicesRequest(),
+            parent="parent_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_services_flattened_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1282,15 +1370,17 @@
         call.return_value = service_service.ListServicesResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service_service.ListServicesResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_services(parent="parent_value",)
+        response = await client.list_services(
+            parent="parent_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
         mock_val = "parent_value"
@@ -1303,73 +1393,102 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_services(
-            service_service.ListServicesRequest(), parent="parent_value",
+            service_service.ListServicesRequest(),
+            parent="parent_value",
         )
 
 
 def test_list_services_pager(transport_name: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_services), "__call__") as call:
         # Set the response to a series of pages.
         call.side_effect = (
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                    service.Service(),
+                ],
                 next_page_token="abc",
             ),
-            service_service.ListServicesResponse(services=[], next_page_token="def",),
             service_service.ListServicesResponse(
-                services=[service.Service(),], next_page_token="ghi",
+                services=[],
+                next_page_token="def",
+            ),
+            service_service.ListServicesResponse(
+                services=[
+                    service.Service(),
+                ],
+                next_page_token="ghi",
             ),
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                ],
             ),
             RuntimeError,
         )
 
         metadata = ()
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", ""),)),
         )
         pager = client.list_services(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, service.Service) for i in results)
 
 
 def test_list_services_pages(transport_name: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_services), "__call__") as call:
         # Set the response to a series of pages.
         call.side_effect = (
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                    service.Service(),
+                ],
                 next_page_token="abc",
             ),
-            service_service.ListServicesResponse(services=[], next_page_token="def",),
             service_service.ListServicesResponse(
-                services=[service.Service(),], next_page_token="ghi",
+                services=[],
+                next_page_token="def",
             ),
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                ],
+                next_page_token="ghi",
+            ),
+            service_service.ListServicesResponse(
+                services=[
+                    service.Service(),
+                    service.Service(),
+                ],
             ),
             RuntimeError,
         )
         pages = list(client.list_services(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
@@ -1383,30 +1502,45 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_services), "__call__", new_callable=mock.AsyncMock
     ) as call:
         # Set the response to a series of pages.
         call.side_effect = (
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                    service.Service(),
+                ],
                 next_page_token="abc",
             ),
-            service_service.ListServicesResponse(services=[], next_page_token="def",),
             service_service.ListServicesResponse(
-                services=[service.Service(),], next_page_token="ghi",
+                services=[],
+                next_page_token="def",
+            ),
+            service_service.ListServicesResponse(
+                services=[
+                    service.Service(),
+                ],
+                next_page_token="ghi",
             ),
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_services(request={},)
+        async_pager = await client.list_services(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, service.Service) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -1418,48 +1552,72 @@
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_services), "__call__", new_callable=mock.AsyncMock
     ) as call:
         # Set the response to a series of pages.
         call.side_effect = (
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                    service.Service(),
+                ],
                 next_page_token="abc",
             ),
-            service_service.ListServicesResponse(services=[], next_page_token="def",),
             service_service.ListServicesResponse(
-                services=[service.Service(),], next_page_token="ghi",
+                services=[],
+                next_page_token="def",
+            ),
+            service_service.ListServicesResponse(
+                services=[
+                    service.Service(),
+                ],
+                next_page_token="ghi",
             ),
             service_service.ListServicesResponse(
-                services=[service.Service(), service.Service(),],
+                services=[
+                    service.Service(),
+                    service.Service(),
+                ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_services(request={})).pages:
+        async for page_ in (
+            await client.list_services(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
-@pytest.mark.parametrize("request_type", [service_service.UpdateServiceRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        service_service.UpdateServiceRequest,
+        dict,
+    ],
+)
 def test_update_service(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_service.Service(
-            name="name_value", display_name="display_name_value", custom=None,
+            name="name_value",
+            display_name="display_name_value",
+            custom=None,
         )
         response = client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == service_service.UpdateServiceRequest()
@@ -1470,15 +1628,16 @@
     assert response.display_name == "display_name_value"
 
 
 def test_update_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         client.update_service()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1486,26 +1645,30 @@
 
 
 @pytest.mark.asyncio
 async def test_update_service_async(
     transport: str = "grpc_asyncio", request_type=service_service.UpdateServiceRequest
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            gm_service.Service(name="name_value", display_name="display_name_value",)
+            gm_service.Service(
+                name="name_value",
+                display_name="display_name_value",
+            )
         )
         response = await client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == service_service.UpdateServiceRequest()
@@ -1526,74 +1689,78 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.UpdateServiceRequest()
 
-    request.service.name = "service.name/value"
+    request.service.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         call.return_value = gm_service.Service()
         client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "service.name=service.name/value",) in kw[
-        "metadata"
-    ]
+    assert (
+        "x-goog-request-params",
+        "service.name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_update_service_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.UpdateServiceRequest()
 
-    request.service.name = "service.name/value"
+    request.service.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(gm_service.Service())
         await client.update_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "service.name=service.name/value",) in kw[
-        "metadata"
-    ]
+    assert (
+        "x-goog-request-params",
+        "service.name=name_value",
+    ) in kw["metadata"]
 
 
 def test_update_service_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.update_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = gm_service.Service()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.update_service(service=gm_service.Service(name="name_value"),)
+        client.update_service(
+            service=gm_service.Service(name="name_value"),
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].service
         mock_val = gm_service.Service(name="name_value")
@@ -1652,18 +1819,25 @@
     with pytest.raises(ValueError):
         await client.update_service(
             service_service.UpdateServiceRequest(),
             service=gm_service.Service(name="name_value"),
         )
 
 
-@pytest.mark.parametrize("request_type", [service_service.DeleteServiceRequest, dict,])
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        service_service.DeleteServiceRequest,
+        dict,
+    ],
+)
 def test_delete_service(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1681,15 +1855,16 @@
     assert response is None
 
 
 def test_delete_service_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_service), "__call__") as call:
         client.delete_service()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
@@ -1697,15 +1872,16 @@
 
 
 @pytest.mark.asyncio
 async def test_delete_service_async(
     transport: str = "grpc_asyncio", request_type=service_service.DeleteServiceRequest
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1733,70 +1909,78 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.DeleteServiceRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_service), "__call__") as call:
         call.return_value = None
         client.delete_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_service_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.DeleteServiceRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_service), "__call__") as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_service(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_service_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.delete_service(name="name_value",)
+        client.delete_service(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1808,15 +1992,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.delete_service(
-            service_service.DeleteServiceRequest(), name="name_value",
+            service_service.DeleteServiceRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_delete_service_flattened_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1826,15 +2011,17 @@
     with mock.patch.object(type(client.transport.delete_service), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.delete_service(name="name_value",)
+        response = await client.delete_service(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1847,24 +2034,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.delete_service(
-            service_service.DeleteServiceRequest(), name="name_value",
+            service_service.DeleteServiceRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [service_service.CreateServiceLevelObjectiveRequest, dict,]
+    "request_type",
+    [
+        service_service.CreateServiceLevelObjectiveRequest,
+        dict,
+    ],
 )
 def test_create_service_level_objective(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1892,15 +2085,16 @@
     assert math.isclose(response.goal, 0.419, rel_tol=1e-6)
 
 
 def test_create_service_level_objective_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_level_objective), "__call__"
     ) as call:
         client.create_service_level_objective()
@@ -1911,29 +2105,32 @@
 
 @pytest.mark.asyncio
 async def test_create_service_level_objective_async(
     transport: str = "grpc_asyncio",
     request_type=service_service.CreateServiceLevelObjectiveRequest,
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_level_objective), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective(
-                name="name_value", display_name="display_name_value", goal=0.419,
+                name="name_value",
+                display_name="display_name_value",
+                goal=0.419,
             )
         )
         response = await client.create_service_level_objective(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1956,15 +2153,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.CreateServiceLevelObjectiveRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_level_objective), "__call__"
     ) as call:
         call.return_value = service.ServiceLevelObjective()
         client.create_service_level_objective(request)
@@ -1972,28 +2169,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_service_level_objective_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.CreateServiceLevelObjectiveRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_service_level_objective), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective()
@@ -2003,15 +2203,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 def test_create_service_level_objective_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2103,19 +2306,24 @@
             service_service.CreateServiceLevelObjectiveRequest(),
             parent="parent_value",
             service_level_objective=service.ServiceLevelObjective(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [service_service.GetServiceLevelObjectiveRequest, dict,]
+    "request_type",
+    [
+        service_service.GetServiceLevelObjectiveRequest,
+        dict,
+    ],
 )
 def test_get_service_level_objective(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2143,15 +2351,16 @@
     assert math.isclose(response.goal, 0.419, rel_tol=1e-6)
 
 
 def test_get_service_level_objective_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_service_level_objective), "__call__"
     ) as call:
         client.get_service_level_objective()
@@ -2162,29 +2371,32 @@
 
 @pytest.mark.asyncio
 async def test_get_service_level_objective_async(
     transport: str = "grpc_asyncio",
     request_type=service_service.GetServiceLevelObjectiveRequest,
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_service_level_objective), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective(
-                name="name_value", display_name="display_name_value", goal=0.419,
+                name="name_value",
+                display_name="display_name_value",
+                goal=0.419,
             )
         )
         response = await client.get_service_level_objective(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -2207,15 +2419,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.GetServiceLevelObjectiveRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_service_level_objective), "__call__"
     ) as call:
         call.return_value = service.ServiceLevelObjective()
         client.get_service_level_objective(request)
@@ -2223,28 +2435,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_service_level_objective_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.GetServiceLevelObjectiveRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_service_level_objective), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective()
@@ -2254,15 +2469,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_service_level_objective_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2270,15 +2488,17 @@
     with mock.patch.object(
         type(client.transport.get_service_level_objective), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = service.ServiceLevelObjective()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_service_level_objective(name="name_value",)
+        client.get_service_level_objective(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -2290,15 +2510,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_service_level_objective(
-            service_service.GetServiceLevelObjectiveRequest(), name="name_value",
+            service_service.GetServiceLevelObjectiveRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_service_level_objective_flattened_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2312,15 +2533,17 @@
         call.return_value = service.ServiceLevelObjective()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_service_level_objective(name="name_value",)
+        response = await client.get_service_level_objective(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -2333,24 +2556,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_service_level_objective(
-            service_service.GetServiceLevelObjectiveRequest(), name="name_value",
+            service_service.GetServiceLevelObjectiveRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [service_service.ListServiceLevelObjectivesRequest, dict,]
+    "request_type",
+    [
+        service_service.ListServiceLevelObjectivesRequest,
+        dict,
+    ],
 )
 def test_list_service_level_objectives(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2373,15 +2602,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_service_level_objectives_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_service_level_objectives), "__call__"
     ) as call:
         client.list_service_level_objectives()
@@ -2392,15 +2622,16 @@
 
 @pytest.mark.asyncio
 async def test_list_service_level_objectives_async(
     transport: str = "grpc_asyncio",
     request_type=service_service.ListServiceLevelObjectivesRequest,
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2435,15 +2666,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.ListServiceLevelObjectivesRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_service_level_objectives), "__call__"
     ) as call:
         call.return_value = service_service.ListServiceLevelObjectivesResponse()
         client.list_service_level_objectives(request)
@@ -2451,28 +2682,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_service_level_objectives_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.ListServiceLevelObjectivesRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_service_level_objectives), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service_service.ListServiceLevelObjectivesResponse()
@@ -2482,15 +2716,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 def test_list_service_level_objectives_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -2498,15 +2735,17 @@
     with mock.patch.object(
         type(client.transport.list_service_level_objectives), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = service_service.ListServiceLevelObjectivesResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_service_level_objectives(parent="parent_value",)
+        client.list_service_level_objectives(
+            parent="parent_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
         mock_val = "parent_value"
@@ -2518,15 +2757,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_service_level_objectives(
-            service_service.ListServiceLevelObjectivesRequest(), parent="parent_value",
+            service_service.ListServiceLevelObjectivesRequest(),
+            parent="parent_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_service_level_objectives_flattened_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2540,15 +2780,17 @@
         call.return_value = service_service.ListServiceLevelObjectivesResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service_service.ListServiceLevelObjectivesResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_service_level_objectives(parent="parent_value",)
+        response = await client.list_service_level_objectives(
+            parent="parent_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
         mock_val = "parent_value"
@@ -2561,21 +2803,23 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_service_level_objectives(
-            service_service.ListServiceLevelObjectivesRequest(), parent="parent_value",
+            service_service.ListServiceLevelObjectivesRequest(),
+            parent="parent_value",
         )
 
 
 def test_list_service_level_objectives_pager(transport_name: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_service_level_objectives), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -2585,18 +2829,21 @@
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
                 next_page_token="abc",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[], next_page_token="def",
+                service_level_objectives=[],
+                next_page_token="def",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[service.ServiceLevelObjective(),],
+                service_level_objectives=[
+                    service.ServiceLevelObjective(),
+                ],
                 next_page_token="ghi",
             ),
             service_service.ListServiceLevelObjectivesResponse(
                 service_level_objectives=[
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
@@ -2608,22 +2855,23 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", ""),)),
         )
         pager = client.list_service_level_objectives(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, service.ServiceLevelObjective) for i in results)
 
 
 def test_list_service_level_objectives_pages(transport_name: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_service_level_objectives), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -2633,18 +2881,21 @@
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
                 next_page_token="abc",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[], next_page_token="def",
+                service_level_objectives=[],
+                next_page_token="def",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[service.ServiceLevelObjective(),],
+                service_level_objectives=[
+                    service.ServiceLevelObjective(),
+                ],
                 next_page_token="ghi",
             ),
             service_service.ListServiceLevelObjectivesResponse(
                 service_level_objectives=[
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
@@ -2675,32 +2926,37 @@
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
                 next_page_token="abc",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[], next_page_token="def",
+                service_level_objectives=[],
+                next_page_token="def",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[service.ServiceLevelObjective(),],
+                service_level_objectives=[
+                    service.ServiceLevelObjective(),
+                ],
                 next_page_token="ghi",
             ),
             service_service.ListServiceLevelObjectivesResponse(
                 service_level_objectives=[
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_service_level_objectives(request={},)
+        async_pager = await client.list_service_level_objectives(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, service.ServiceLevelObjective) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -2722,43 +2978,51 @@
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
                 next_page_token="abc",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[], next_page_token="def",
+                service_level_objectives=[],
+                next_page_token="def",
             ),
             service_service.ListServiceLevelObjectivesResponse(
-                service_level_objectives=[service.ServiceLevelObjective(),],
+                service_level_objectives=[
+                    service.ServiceLevelObjective(),
+                ],
                 next_page_token="ghi",
             ),
             service_service.ListServiceLevelObjectivesResponse(
                 service_level_objectives=[
                     service.ServiceLevelObjective(),
                     service.ServiceLevelObjective(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
         async for page_ in (
             await client.list_service_level_objectives(request={})
-        ).pages:
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
-    "request_type", [service_service.UpdateServiceLevelObjectiveRequest, dict,]
+    "request_type",
+    [
+        service_service.UpdateServiceLevelObjectiveRequest,
+        dict,
+    ],
 )
 def test_update_service_level_objective(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2786,15 +3050,16 @@
     assert math.isclose(response.goal, 0.419, rel_tol=1e-6)
 
 
 def test_update_service_level_objective_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_service_level_objective), "__call__"
     ) as call:
         client.update_service_level_objective()
@@ -2805,29 +3070,32 @@
 
 @pytest.mark.asyncio
 async def test_update_service_level_objective_async(
     transport: str = "grpc_asyncio",
     request_type=service_service.UpdateServiceLevelObjectiveRequest,
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_service_level_objective), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective(
-                name="name_value", display_name="display_name_value", goal=0.419,
+                name="name_value",
+                display_name="display_name_value",
+                goal=0.419,
             )
         )
         response = await client.update_service_level_objective(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -2850,15 +3118,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.UpdateServiceLevelObjectiveRequest()
 
-    request.service_level_objective.name = "service_level_objective.name/value"
+    request.service_level_objective.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_service_level_objective), "__call__"
     ) as call:
         call.return_value = service.ServiceLevelObjective()
         client.update_service_level_objective(request)
@@ -2868,29 +3136,29 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "service_level_objective.name=service_level_objective.name/value",
+        "service_level_objective.name=name_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_update_service_level_objective_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.UpdateServiceLevelObjectiveRequest()
 
-    request.service_level_objective.name = "service_level_objective.name/value"
+    request.service_level_objective.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_service_level_objective), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             service.ServiceLevelObjective()
@@ -2902,15 +3170,15 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "service_level_objective.name=service_level_objective.name/value",
+        "service_level_objective.name=name_value",
     ) in kw["metadata"]
 
 
 def test_update_service_level_objective_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -2993,19 +3261,24 @@
         await client.update_service_level_objective(
             service_service.UpdateServiceLevelObjectiveRequest(),
             service_level_objective=service.ServiceLevelObjective(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [service_service.DeleteServiceLevelObjectiveRequest, dict,]
+    "request_type",
+    [
+        service_service.DeleteServiceLevelObjectiveRequest,
+        dict,
+    ],
 )
 def test_delete_service_level_objective(request_type, transport: str = "grpc"):
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3025,15 +3298,16 @@
     assert response is None
 
 
 def test_delete_service_level_objective_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ServiceMonitoringServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_service_level_objective), "__call__"
     ) as call:
         client.delete_service_level_objective()
@@ -3044,15 +3318,16 @@
 
 @pytest.mark.asyncio
 async def test_delete_service_level_objective_async(
     transport: str = "grpc_asyncio",
     request_type=service_service.DeleteServiceLevelObjectiveRequest,
 ):
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -3082,15 +3357,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.DeleteServiceLevelObjectiveRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_service_level_objective), "__call__"
     ) as call:
         call.return_value = None
         client.delete_service_level_objective(request)
@@ -3098,28 +3373,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_service_level_objective_field_headers_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = service_service.DeleteServiceLevelObjectiveRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_service_level_objective), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_service_level_objective(request)
@@ -3127,15 +3405,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_service_level_objective_flattened():
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -3143,15 +3424,17 @@
     with mock.patch.object(
         type(client.transport.delete_service_level_objective), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.delete_service_level_objective(name="name_value",)
+        client.delete_service_level_objective(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -3163,15 +3446,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.delete_service_level_objective(
-            service_service.DeleteServiceLevelObjectiveRequest(), name="name_value",
+            service_service.DeleteServiceLevelObjectiveRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_delete_service_level_objective_flattened_async():
     client = ServiceMonitoringServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3183,15 +3467,17 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.delete_service_level_objective(name="name_value",)
+        response = await client.delete_service_level_objective(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -3204,26 +3490,28 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.delete_service_level_objective(
-            service_service.DeleteServiceLevelObjectiveRequest(), name="name_value",
+            service_service.DeleteServiceLevelObjectiveRequest(),
+            name="name_value",
         )
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.ServiceMonitoringServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = ServiceMonitoringServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.ServiceMonitoringServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -3236,15 +3524,16 @@
     transport = transports.ServiceMonitoringServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = ServiceMonitoringServiceClient(
-            client_options=options, transport=transport,
+            client_options=options,
+            transport=transport,
         )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = ServiceMonitoringServiceClient(
@@ -3253,15 +3542,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.ServiceMonitoringServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = ServiceMonitoringServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.ServiceMonitoringServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3296,21 +3586,35 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = ServiceMonitoringServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     assert isinstance(
-        client.transport, transports.ServiceMonitoringServiceGrpcTransport,
+        client.transport,
+        transports.ServiceMonitoringServiceGrpcTransport,
     )
 
 
 def test_service_monitoring_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.ServiceMonitoringServiceTransport(
@@ -3346,26 +3650,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_service_monitoring_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.service_monitoring_service.transports.ServiceMonitoringServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.ServiceMonitoringServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -3510,52 +3823,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_service_monitoring_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_service_monitoring_service_host_no_port(transport_name):
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_service_monitoring_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_service_monitoring_service_host_with_port(transport_name):
     client = ServiceMonitoringServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_service_monitoring_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.ServiceMonitoringServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_service_monitoring_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.ServiceMonitoringServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -3658,15 +3989,16 @@
             assert transport.grpc_channel == mock_grpc_channel
 
 
 def test_service_path():
     project = "squid"
     service = "clam"
     expected = "projects/{project}/services/{service}".format(
-        project=project, service=service,
+        project=project,
+        service=service,
     )
     actual = ServiceMonitoringServiceClient.service_path(project, service)
     assert expected == actual
 
 
 def test_parse_service_path():
     expected = {
@@ -3726,15 +4058,17 @@
     # Check that the path construction is reversible.
     actual = ServiceMonitoringServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "squid"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = ServiceMonitoringServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "clam",
@@ -3744,15 +4078,17 @@
     # Check that the path construction is reversible.
     actual = ServiceMonitoringServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "whelk"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = ServiceMonitoringServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "octopus",
@@ -3762,15 +4098,17 @@
     # Check that the path construction is reversible.
     actual = ServiceMonitoringServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "oyster"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = ServiceMonitoringServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "nudibranch",
@@ -3782,15 +4120,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "cuttlefish"
     location = "mussel"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = ServiceMonitoringServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -3807,32 +4146,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.ServiceMonitoringServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = ServiceMonitoringServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.ServiceMonitoringServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = ServiceMonitoringServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = ServiceMonitoringServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/gapic/monitoring_v3/test_uptime_check_service.py` & `google-cloud-monitoring-2.9.2/tests/unit/gapic/monitoring_v3/test_uptime_check_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 
@@ -90,28 +96,34 @@
     assert (
         UptimeCheckServiceClient._get_default_mtls_endpoint(non_googleapi)
         == non_googleapi
     )
 
 
 @pytest.mark.parametrize(
-    "client_class", [UptimeCheckServiceClient, UptimeCheckServiceAsyncClient,]
+    "client_class,transport_name",
+    [
+        (UptimeCheckServiceClient, "grpc"),
+        (UptimeCheckServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_uptime_check_service_client_from_service_account_info(client_class):
+def test_uptime_check_service_client_from_service_account_info(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
-        client = client_class.from_service_account_info(info)
+        client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.UptimeCheckServiceGrpcTransport, "grpc"),
         (transports.UptimeCheckServiceGrpcAsyncIOTransport, "grpc_asyncio"),
@@ -132,31 +144,41 @@
     ) as use_jwt:
         creds = service_account.Credentials(None, None, None)
         transport = transport_class(credentials=creds, always_use_jwt_access=False)
         use_jwt.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "client_class", [UptimeCheckServiceClient, UptimeCheckServiceAsyncClient,]
+    "client_class,transport_name",
+    [
+        (UptimeCheckServiceClient, "grpc"),
+        (UptimeCheckServiceAsyncClient, "grpc_asyncio"),
+    ],
 )
-def test_uptime_check_service_client_from_service_account_file(client_class):
+def test_uptime_check_service_client_from_service_account_file(
+    client_class, transport_name
+):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
         factory.return_value = creds
-        client = client_class.from_service_account_file("dummy/file/path.json")
+        client = client_class.from_service_account_file(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        client = client_class.from_service_account_json("dummy/file/path.json")
+        client = client_class.from_service_account_json(
+            "dummy/file/path.json", transport=transport_name
+        )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == "monitoring.googleapis.com:443"
+        assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
 def test_uptime_check_service_client_get_transport_class():
     transport = UptimeCheckServiceClient.get_transport_class()
     available_transports = [
         transports.UptimeCheckServiceGrpcTransport,
     ]
@@ -506,15 +528,17 @@
         ),
     ],
 )
 def test_uptime_check_service_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
-    options = client_options.ClientOptions(scopes=["1", "2"],)
+    options = client_options.ClientOptions(
+        scopes=["1", "2"],
+    )
     with mock.patch.object(transport_class, "__init__") as patched:
         patched.return_value = None
         client = client_class(client_options=options, transport=transport_name)
         patched.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
@@ -651,32 +675,38 @@
                 ("grpc.max_send_message_length", -1),
                 ("grpc.max_receive_message_length", -1),
             ],
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [uptime_service.ListUptimeCheckConfigsRequest, dict,]
+    "request_type",
+    [
+        uptime_service.ListUptimeCheckConfigsRequest,
+        dict,
+    ],
 )
 def test_list_uptime_check_configs(request_type, transport: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = uptime_service.ListUptimeCheckConfigsResponse(
-            next_page_token="next_page_token_value", total_size=1086,
+            next_page_token="next_page_token_value",
+            total_size=1086,
         )
         response = client.list_uptime_check_configs(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == uptime_service.ListUptimeCheckConfigsRequest()
@@ -687,15 +717,16 @@
     assert response.total_size == 1086
 
 
 def test_list_uptime_check_configs_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         client.list_uptime_check_configs()
@@ -706,29 +737,31 @@
 
 @pytest.mark.asyncio
 async def test_list_uptime_check_configs_async(
     transport: str = "grpc_asyncio",
     request_type=uptime_service.ListUptimeCheckConfigsRequest,
 ):
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime_service.ListUptimeCheckConfigsResponse(
-                next_page_token="next_page_token_value", total_size=1086,
+                next_page_token="next_page_token_value",
+                total_size=1086,
             )
         )
         response = await client.list_uptime_check_configs(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -750,15 +783,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.ListUptimeCheckConfigsRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         call.return_value = uptime_service.ListUptimeCheckConfigsResponse()
         client.list_uptime_check_configs(request)
@@ -766,28 +799,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_list_uptime_check_configs_field_headers_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.ListUptimeCheckConfigsRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime_service.ListUptimeCheckConfigsResponse()
@@ -797,15 +833,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 def test_list_uptime_check_configs_flattened():
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -813,15 +852,17 @@
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = uptime_service.ListUptimeCheckConfigsResponse()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.list_uptime_check_configs(parent="parent_value",)
+        client.list_uptime_check_configs(
+            parent="parent_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
         mock_val = "parent_value"
@@ -833,15 +874,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.list_uptime_check_configs(
-            uptime_service.ListUptimeCheckConfigsRequest(), parent="parent_value",
+            uptime_service.ListUptimeCheckConfigsRequest(),
+            parent="parent_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_list_uptime_check_configs_flattened_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -855,15 +897,17 @@
         call.return_value = uptime_service.ListUptimeCheckConfigsResponse()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime_service.ListUptimeCheckConfigsResponse()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.list_uptime_check_configs(parent="parent_value",)
+        response = await client.list_uptime_check_configs(
+            parent="parent_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].parent
         mock_val = "parent_value"
@@ -876,21 +920,23 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.list_uptime_check_configs(
-            uptime_service.ListUptimeCheckConfigsRequest(), parent="parent_value",
+            uptime_service.ListUptimeCheckConfigsRequest(),
+            parent="parent_value",
         )
 
 
 def test_list_uptime_check_configs_pager(transport_name: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -900,18 +946,21 @@
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[], next_page_token="def",
+                uptime_check_configs=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[uptime.UptimeCheckConfig(),],
+                uptime_check_configs=[
+                    uptime.UptimeCheckConfig(),
+                ],
                 next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
                 uptime_check_configs=[
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
@@ -923,22 +972,23 @@
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", ""),)),
         )
         pager = client.list_uptime_check_configs(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, uptime.UptimeCheckConfig) for i in results)
 
 
 def test_list_uptime_check_configs_pages(transport_name: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_configs), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -948,18 +998,21 @@
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[], next_page_token="def",
+                uptime_check_configs=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[uptime.UptimeCheckConfig(),],
+                uptime_check_configs=[
+                    uptime.UptimeCheckConfig(),
+                ],
                 next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
                 uptime_check_configs=[
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
@@ -990,32 +1043,37 @@
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[], next_page_token="def",
+                uptime_check_configs=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[uptime.UptimeCheckConfig(),],
+                uptime_check_configs=[
+                    uptime.UptimeCheckConfig(),
+                ],
                 next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
                 uptime_check_configs=[
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_uptime_check_configs(request={},)
+        async_pager = await client.list_uptime_check_configs(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, uptime.UptimeCheckConfig) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -1037,41 +1095,51 @@
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[], next_page_token="def",
+                uptime_check_configs=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
-                uptime_check_configs=[uptime.UptimeCheckConfig(),],
+                uptime_check_configs=[
+                    uptime.UptimeCheckConfig(),
+                ],
                 next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckConfigsResponse(
                 uptime_check_configs=[
                     uptime.UptimeCheckConfig(),
                     uptime.UptimeCheckConfig(),
                 ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_uptime_check_configs(request={})).pages:
+        async for page_ in (
+            await client.list_uptime_check_configs(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
-    "request_type", [uptime_service.GetUptimeCheckConfigRequest, dict,]
+    "request_type",
+    [
+        uptime_service.GetUptimeCheckConfigRequest,
+        dict,
+    ],
 )
 def test_get_uptime_check_config(request_type, transport: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1106,15 +1174,16 @@
     assert response.is_internal is True
 
 
 def test_get_uptime_check_config_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_uptime_check_config), "__call__"
     ) as call:
         client.get_uptime_check_config()
@@ -1125,15 +1194,16 @@
 
 @pytest.mark.asyncio
 async def test_get_uptime_check_config_async(
     transport: str = "grpc_asyncio",
     request_type=uptime_service.GetUptimeCheckConfigRequest,
 ):
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1174,15 +1244,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.GetUptimeCheckConfigRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_uptime_check_config), "__call__"
     ) as call:
         call.return_value = uptime.UptimeCheckConfig()
         client.get_uptime_check_config(request)
@@ -1190,28 +1260,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_get_uptime_check_config_field_headers_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.GetUptimeCheckConfigRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.get_uptime_check_config), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime.UptimeCheckConfig()
@@ -1221,15 +1294,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_get_uptime_check_config_flattened():
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1237,15 +1313,17 @@
     with mock.patch.object(
         type(client.transport.get_uptime_check_config), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = uptime.UptimeCheckConfig()
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.get_uptime_check_config(name="name_value",)
+        client.get_uptime_check_config(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1257,15 +1335,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.get_uptime_check_config(
-            uptime_service.GetUptimeCheckConfigRequest(), name="name_value",
+            uptime_service.GetUptimeCheckConfigRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_get_uptime_check_config_flattened_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1279,15 +1358,17 @@
         call.return_value = uptime.UptimeCheckConfig()
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime.UptimeCheckConfig()
         )
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.get_uptime_check_config(name="name_value",)
+        response = await client.get_uptime_check_config(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1300,24 +1381,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.get_uptime_check_config(
-            uptime_service.GetUptimeCheckConfigRequest(), name="name_value",
+            uptime_service.GetUptimeCheckConfigRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [uptime_service.CreateUptimeCheckConfigRequest, dict,]
+    "request_type",
+    [
+        uptime_service.CreateUptimeCheckConfigRequest,
+        dict,
+    ],
 )
 def test_create_uptime_check_config(request_type, transport: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1352,15 +1439,16 @@
     assert response.is_internal is True
 
 
 def test_create_uptime_check_config_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_uptime_check_config), "__call__"
     ) as call:
         client.create_uptime_check_config()
@@ -1371,15 +1459,16 @@
 
 @pytest.mark.asyncio
 async def test_create_uptime_check_config_async(
     transport: str = "grpc_asyncio",
     request_type=uptime_service.CreateUptimeCheckConfigRequest,
 ):
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1420,15 +1509,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.CreateUptimeCheckConfigRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_uptime_check_config), "__call__"
     ) as call:
         call.return_value = uptime.UptimeCheckConfig()
         client.create_uptime_check_config(request)
@@ -1436,28 +1525,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_create_uptime_check_config_field_headers_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.CreateUptimeCheckConfigRequest()
 
-    request.parent = "parent/value"
+    request.parent = "parent_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.create_uptime_check_config), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime.UptimeCheckConfig()
@@ -1467,15 +1559,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "parent=parent/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
 
 
 def test_create_uptime_check_config_flattened():
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1567,19 +1662,24 @@
             uptime_service.CreateUptimeCheckConfigRequest(),
             parent="parent_value",
             uptime_check_config=uptime.UptimeCheckConfig(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [uptime_service.UpdateUptimeCheckConfigRequest, dict,]
+    "request_type",
+    [
+        uptime_service.UpdateUptimeCheckConfigRequest,
+        dict,
+    ],
 )
 def test_update_uptime_check_config(request_type, transport: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1614,15 +1714,16 @@
     assert response.is_internal is True
 
 
 def test_update_uptime_check_config_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_uptime_check_config), "__call__"
     ) as call:
         client.update_uptime_check_config()
@@ -1633,15 +1734,16 @@
 
 @pytest.mark.asyncio
 async def test_update_uptime_check_config_async(
     transport: str = "grpc_asyncio",
     request_type=uptime_service.UpdateUptimeCheckConfigRequest,
 ):
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1682,15 +1784,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.UpdateUptimeCheckConfigRequest()
 
-    request.uptime_check_config.name = "uptime_check_config.name/value"
+    request.uptime_check_config.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_uptime_check_config), "__call__"
     ) as call:
         call.return_value = uptime.UptimeCheckConfig()
         client.update_uptime_check_config(request)
@@ -1700,29 +1802,29 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "uptime_check_config.name=uptime_check_config.name/value",
+        "uptime_check_config.name=name_value",
     ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_update_uptime_check_config_field_headers_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.UpdateUptimeCheckConfigRequest()
 
-    request.uptime_check_config.name = "uptime_check_config.name/value"
+    request.uptime_check_config.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_uptime_check_config), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             uptime.UptimeCheckConfig()
@@ -1734,15 +1836,15 @@
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
     assert (
         "x-goog-request-params",
-        "uptime_check_config.name=uptime_check_config.name/value",
+        "uptime_check_config.name=name_value",
     ) in kw["metadata"]
 
 
 def test_update_uptime_check_config_flattened():
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
@@ -1825,19 +1927,24 @@
         await client.update_uptime_check_config(
             uptime_service.UpdateUptimeCheckConfigRequest(),
             uptime_check_config=uptime.UptimeCheckConfig(name="name_value"),
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [uptime_service.DeleteUptimeCheckConfigRequest, dict,]
+    "request_type",
+    [
+        uptime_service.DeleteUptimeCheckConfigRequest,
+        dict,
+    ],
 )
 def test_delete_uptime_check_config(request_type, transport: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1857,15 +1964,16 @@
     assert response is None
 
 
 def test_delete_uptime_check_config_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_uptime_check_config), "__call__"
     ) as call:
         client.delete_uptime_check_config()
@@ -1876,15 +1984,16 @@
 
 @pytest.mark.asyncio
 async def test_delete_uptime_check_config_async(
     transport: str = "grpc_asyncio",
     request_type=uptime_service.DeleteUptimeCheckConfigRequest,
 ):
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -1914,15 +2023,15 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.DeleteUptimeCheckConfigRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_uptime_check_config), "__call__"
     ) as call:
         call.return_value = None
         client.delete_uptime_check_config(request)
@@ -1930,28 +2039,31 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 @pytest.mark.asyncio
 async def test_delete_uptime_check_config_field_headers_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Any value that is part of the HTTP/1.1 URI should be sent as
     # a field header. Set these to a non-empty value.
     request = uptime_service.DeleteUptimeCheckConfigRequest()
 
-    request.name = "name/value"
+    request.name = "name_value"
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.delete_uptime_check_config), "__call__"
     ) as call:
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         await client.delete_uptime_check_config(request)
@@ -1959,15 +2071,18 @@
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == request
 
     # Establish that the field header was sent.
     _, _, kw = call.mock_calls[0]
-    assert ("x-goog-request-params", "name=name/value",) in kw["metadata"]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
 
 
 def test_delete_uptime_check_config_flattened():
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
@@ -1975,15 +2090,17 @@
     with mock.patch.object(
         type(client.transport.delete_uptime_check_config), "__call__"
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        client.delete_uptime_check_config(name="name_value",)
+        client.delete_uptime_check_config(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -1995,15 +2112,16 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         client.delete_uptime_check_config(
-            uptime_service.DeleteUptimeCheckConfigRequest(), name="name_value",
+            uptime_service.DeleteUptimeCheckConfigRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.asyncio
 async def test_delete_uptime_check_config_flattened_async():
     client = UptimeCheckServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2015,15 +2133,17 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = None
 
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         # Call the method with a truthy value for each flattened field,
         # using the keyword arguments to the method.
-        response = await client.delete_uptime_check_config(name="name_value",)
+        response = await client.delete_uptime_check_config(
+            name="name_value",
+        )
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         arg = args[0].name
         mock_val = "name_value"
@@ -2036,24 +2156,30 @@
         credentials=ga_credentials.AnonymousCredentials(),
     )
 
     # Attempting to call a method with both a request object and flattened
     # fields is an error.
     with pytest.raises(ValueError):
         await client.delete_uptime_check_config(
-            uptime_service.DeleteUptimeCheckConfigRequest(), name="name_value",
+            uptime_service.DeleteUptimeCheckConfigRequest(),
+            name="name_value",
         )
 
 
 @pytest.mark.parametrize(
-    "request_type", [uptime_service.ListUptimeCheckIpsRequest, dict,]
+    "request_type",
+    [
+        uptime_service.ListUptimeCheckIpsRequest,
+        dict,
+    ],
 )
 def test_list_uptime_check_ips(request_type, transport: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2076,15 +2202,16 @@
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_uptime_check_ips_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_ips), "__call__"
     ) as call:
         client.list_uptime_check_ips()
@@ -2095,15 +2222,16 @@
 
 @pytest.mark.asyncio
 async def test_list_uptime_check_ips_async(
     transport: str = "grpc_asyncio",
     request_type=uptime_service.ListUptimeCheckIpsRequest,
 ):
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
     )
 
     # Everything is optional in proto3 as far as the runtime is concerned,
     # and we are mocking out the actual API, so just send an empty request.
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
@@ -2131,15 +2259,16 @@
 @pytest.mark.asyncio
 async def test_list_uptime_check_ips_async_from_dict():
     await test_list_uptime_check_ips_async(request_type=dict)
 
 
 def test_list_uptime_check_ips_pager(transport_name: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_ips), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -2149,38 +2278,46 @@
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[], next_page_token="def",
+                uptime_check_ips=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(),], next_page_token="ghi",
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                ],
+                next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(), uptime.UptimeCheckIp(),],
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                    uptime.UptimeCheckIp(),
+                ],
             ),
             RuntimeError,
         )
 
         metadata = ()
         pager = client.list_uptime_check_ips(request={})
 
         assert pager._metadata == metadata
 
-        results = [i for i in pager]
+        results = list(pager)
         assert len(results) == 6
         assert all(isinstance(i, uptime.UptimeCheckIp) for i in results)
 
 
 def test_list_uptime_check_ips_pages(transport_name: str = "grpc"):
     client = UptimeCheckServiceClient(
-        credentials=ga_credentials.AnonymousCredentials, transport=transport_name,
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.list_uptime_check_ips), "__call__"
     ) as call:
         # Set the response to a series of pages.
@@ -2190,21 +2327,28 @@
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[], next_page_token="def",
+                uptime_check_ips=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(),], next_page_token="ghi",
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                ],
+                next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(), uptime.UptimeCheckIp(),],
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                    uptime.UptimeCheckIp(),
+                ],
             ),
             RuntimeError,
         )
         pages = list(client.list_uptime_check_ips(request={}).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
@@ -2228,28 +2372,37 @@
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[], next_page_token="def",
+                uptime_check_ips=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(),], next_page_token="ghi",
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                ],
+                next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(), uptime.UptimeCheckIp(),],
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                    uptime.UptimeCheckIp(),
+                ],
             ),
             RuntimeError,
         )
-        async_pager = await client.list_uptime_check_ips(request={},)
+        async_pager = await client.list_uptime_check_ips(
+            request={},
+        )
         assert async_pager.next_page_token == "abc"
         responses = []
-        async for response in async_pager:
+        async for response in async_pager:  # pragma: no branch
             responses.append(response)
 
         assert len(responses) == 6
         assert all(isinstance(i, uptime.UptimeCheckIp) for i in responses)
 
 
 @pytest.mark.asyncio
@@ -2271,39 +2424,49 @@
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                     uptime.UptimeCheckIp(),
                 ],
                 next_page_token="abc",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[], next_page_token="def",
+                uptime_check_ips=[],
+                next_page_token="def",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(),], next_page_token="ghi",
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                ],
+                next_page_token="ghi",
             ),
             uptime_service.ListUptimeCheckIpsResponse(
-                uptime_check_ips=[uptime.UptimeCheckIp(), uptime.UptimeCheckIp(),],
+                uptime_check_ips=[
+                    uptime.UptimeCheckIp(),
+                    uptime.UptimeCheckIp(),
+                ],
             ),
             RuntimeError,
         )
         pages = []
-        async for page_ in (await client.list_uptime_check_ips(request={})).pages:
+        async for page_ in (
+            await client.list_uptime_check_ips(request={})
+        ).pages:  # pragma: no branch
             pages.append(page_)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.UptimeCheckServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = UptimeCheckServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), transport=transport,
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
         )
 
     # It is an error to provide a credentials file and a transport instance.
     transport = transports.UptimeCheckServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
@@ -2315,15 +2478,18 @@
     # It is an error to provide an api_key and a transport instance.
     transport = transports.UptimeCheckServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     options = client_options.ClientOptions()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
-        client = UptimeCheckServiceClient(client_options=options, transport=transport,)
+        client = UptimeCheckServiceClient(
+            client_options=options,
+            transport=transport,
+        )
 
     # It is an error to provide an api_key and a credential.
     options = mock.Mock()
     options.api_key = "api_key"
     with pytest.raises(ValueError):
         client = UptimeCheckServiceClient(
             client_options=options, credentials=ga_credentials.AnonymousCredentials()
@@ -2331,15 +2497,16 @@
 
     # It is an error to provide scopes and a transport instance.
     transport = transports.UptimeCheckServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = UptimeCheckServiceClient(
-            client_options={"scopes": ["1", "2"]}, transport=transport,
+            client_options={"scopes": ["1", "2"]},
+            transport=transport,
         )
 
 
 def test_transport_instance():
     # A client may be instantiated with a custom transport instance.
     transport = transports.UptimeCheckServiceGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2374,20 +2541,36 @@
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+    ],
+)
+def test_transport_kind(transport_name):
+    transport = UptimeCheckServiceClient.get_transport_class(transport_name)(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    assert transport.kind == transport_name
+
+
 def test_transport_grpc_default():
     # A client should use the gRPC transport by default.
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
     )
-    assert isinstance(client.transport, transports.UptimeCheckServiceGrpcTransport,)
+    assert isinstance(
+        client.transport,
+        transports.UptimeCheckServiceGrpcTransport,
+    )
 
 
 def test_uptime_check_service_base_transport_error():
     # Passing both a credentials object and credentials_file should raise an error
     with pytest.raises(core_exceptions.DuplicateCredentialArgs):
         transport = transports.UptimeCheckServiceTransport(
             credentials=ga_credentials.AnonymousCredentials(),
@@ -2418,26 +2601,35 @@
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
 
+    # Catch all for all remaining methods and properties
+    remainder = [
+        "kind",
+    ]
+    for r in remainder:
+        with pytest.raises(NotImplementedError):
+            getattr(transport, r)()
+
 
 def test_uptime_check_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
         "google.cloud.monitoring_v3.services.uptime_check_service.transports.UptimeCheckServiceTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.UptimeCheckServiceTransport(
-            credentials_file="credentials.json", quota_project_id="octopus",
+            credentials_file="credentials.json",
+            quota_project_id="octopus",
         )
         load_creds.assert_called_once_with(
             "credentials.json",
             scopes=None,
             default_scopes=(
                 "https://www.googleapis.com/auth/cloud-platform",
                 "https://www.googleapis.com/auth/monitoring",
@@ -2580,52 +2772,70 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
-def test_uptime_check_service_host_no_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_uptime_check_service_host_no_port(transport_name):
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:443"
+    assert client.transport._host == ("monitoring.googleapis.com:443")
 
 
-def test_uptime_check_service_host_with_port():
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "grpc",
+        "grpc_asyncio",
+    ],
+)
+def test_uptime_check_service_host_with_port(transport_name):
     client = UptimeCheckServiceClient(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="monitoring.googleapis.com:8000"
         ),
+        transport=transport_name,
     )
-    assert client.transport._host == "monitoring.googleapis.com:8000"
+    assert client.transport._host == ("monitoring.googleapis.com:8000")
 
 
 def test_uptime_check_service_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.UptimeCheckServiceGrpcTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 def test_uptime_check_service_grpc_asyncio_transport_channel():
     channel = aio.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.UptimeCheckServiceGrpcAsyncIOTransport(
-        host="squid.clam.whelk", channel=channel,
+        host="squid.clam.whelk",
+        channel=channel,
     )
     assert transport.grpc_channel == channel
     assert transport._host == "squid.clam.whelk:443"
     assert transport._ssl_channel_credentials == None
 
 
 # Remove this test when deprecated arguments (api_mtls_endpoint, client_cert_source) are
@@ -2728,15 +2938,16 @@
             assert transport.grpc_channel == mock_grpc_channel
 
 
 def test_uptime_check_config_path():
     project = "squid"
     uptime_check_config = "clam"
     expected = "projects/{project}/uptimeCheckConfigs/{uptime_check_config}".format(
-        project=project, uptime_check_config=uptime_check_config,
+        project=project,
+        uptime_check_config=uptime_check_config,
     )
     actual = UptimeCheckServiceClient.uptime_check_config_path(
         project, uptime_check_config
     )
     assert expected == actual
 
 
@@ -2770,15 +2981,17 @@
     # Check that the path construction is reversible.
     actual = UptimeCheckServiceClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
     folder = "cuttlefish"
-    expected = "folders/{folder}".format(folder=folder,)
+    expected = "folders/{folder}".format(
+        folder=folder,
+    )
     actual = UptimeCheckServiceClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
         "folder": "mussel",
@@ -2788,15 +3001,17 @@
     # Check that the path construction is reversible.
     actual = UptimeCheckServiceClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
     organization = "winkle"
-    expected = "organizations/{organization}".format(organization=organization,)
+    expected = "organizations/{organization}".format(
+        organization=organization,
+    )
     actual = UptimeCheckServiceClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
         "organization": "nautilus",
@@ -2806,15 +3021,17 @@
     # Check that the path construction is reversible.
     actual = UptimeCheckServiceClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
     project = "scallop"
-    expected = "projects/{project}".format(project=project,)
+    expected = "projects/{project}".format(
+        project=project,
+    )
     actual = UptimeCheckServiceClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
         "project": "abalone",
@@ -2826,15 +3043,16 @@
     assert expected == actual
 
 
 def test_common_location_path():
     project = "squid"
     location = "clam"
     expected = "projects/{project}/locations/{location}".format(
-        project=project, location=location,
+        project=project,
+        location=location,
     )
     actual = UptimeCheckServiceClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
@@ -2851,32 +3069,35 @@
 def test_client_with_default_client_info():
     client_info = gapic_v1.client_info.ClientInfo()
 
     with mock.patch.object(
         transports.UptimeCheckServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         client = UptimeCheckServiceClient(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
     with mock.patch.object(
         transports.UptimeCheckServiceTransport, "_prep_wrapped_messages"
     ) as prep:
         transport_class = UptimeCheckServiceClient.get_transport_class()
         transport = transport_class(
-            credentials=ga_credentials.AnonymousCredentials(), client_info=client_info,
+            credentials=ga_credentials.AnonymousCredentials(),
+            client_info=client_info,
         )
         prep.assert_called_once_with(client_info)
 
 
 @pytest.mark.asyncio
 async def test_transport_close_async():
     client = UptimeCheckServiceAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
     )
     with mock.patch.object(
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
```

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/test__dataframe.py` & `google-cloud-monitoring-2.9.2/tests/unit/test__dataframe.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-2.9.1/tests/unit/test_query.py` & `google-cloud-monitoring-2.9.2/tests/unit/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         T1 = datetime.datetime(2016, 4, 7, 2, 30, 0)
 
         client = self._create_client()
         query = self._make_one(client, PROJECT, METRIC_TYPE)
         query = query.select_interval(end_time=T1)
         actual = query._build_query_params()
         expected = {
-            "name": u"projects/{}".format(PROJECT),
+            "name": "projects/{}".format(PROJECT),
             "filter": 'metric.type = "{type}"'.format(type=METRIC_TYPE),
             "interval": self._make_interval(T1),
             "view": monitoring_v3.ListTimeSeriesRequest.TimeSeriesView.FULL,
         }
         self.assertEqual(actual, expected)
 
     def test_request_parameters_maximal(self):
```

