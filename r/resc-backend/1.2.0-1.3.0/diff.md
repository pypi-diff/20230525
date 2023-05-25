# Comparing `tmp/resc_backend-1.2.0.tar.gz` & `tmp/resc_backend-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_backend-1.2.0.tar", last modified: Fri Apr 14 15:10:27 2023, max compression
+gzip compressed data, was "resc_backend-1.3.0.tar", last modified: Thu May 25 09:51:22 2023, max compression
```

## Comparing `resc_backend-1.2.0.tar` & `resc_backend-1.3.0.tar`

### file list

```diff
@@ -1,108 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.245564 resc_backend-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-14 15:10:27.245564 resc_backend-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-14 15:10:27.245564 resc_backend-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 15:10:23.000000 resc_backend-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.233563 resc_backend-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.233563 resc_backend-1.2.0/src/resc_backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/bin/rabbitmq_bootup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/db/model/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/db/model/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/git_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend/resc_web_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.241563 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.241563 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.241563 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.245564 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/date_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/date_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/pagination_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/status_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.245564 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/rule_packs.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/scans.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 15:10:23.000000 resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:10:27.237563 resc_backend-1.2.0/src/resc_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 15:10:27.000000 resc_backend-1.2.0/src/resc_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.436169 resc_backend-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-05-25 09:51:22.436169 resc_backend-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 09:51:22.436169 resc_backend-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 09:51:15.000000 resc_backend-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/bin/rabbitmq_bootup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend/db/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/db/model/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/git_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17644 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.432169 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.436169 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/date_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/date_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_count_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_count_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/status_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/vcs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.436169 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-25 09:51:15.000000 resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:51:22.428169 resc_backend-1.3.0/src/resc_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 09:51:22.000000 resc_backend-1.3.0/src/resc_backend.egg-info/top_level.txt
```

### Comparing `resc_backend-1.2.0/PKG-INFO` & `resc_backend-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_backend
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-1.2.0/setup.cfg` & `resc_backend-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_backend
 description = Repository Scanner - Backend
-version = 1.2.0
+version = 1.3.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_backend-1.2.0/src/resc_backend/bin/rabbitmq_bootup.py` & `resc_backend-1.3.0/src/resc_backend/bin/rabbitmq_bootup.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/common.py` & `resc_backend-1.3.0/src/resc_backend/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/constants.py` & `resc_backend-1.3.0/src/resc_backend/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 RWS_VERSION_PREFIX = "/resc/v1"
 RWS_ROUTE_REPOSITORIES = "/repositories"
 RWS_ROUTE_BRANCHES = "/branches"
 RWS_ROUTE_SCANS = "/scans"
 RWS_ROUTE_LAST_SCAN = "/last-scan"
 RWS_ROUTE_FINDINGS = "/findings"
 RWS_ROUTE_RULES = "/rules"
+RWS_ROUTE_METRICS = "/metrics"
 RWS_ROUTE_DETAILED_FINDINGS = "/detailed-findings"
 RWS_ROUTE_TOTAL_COUNT_BY_RULE = "/total-count-by-rule"
 RWS_ROUTE_BY_RULE = "/by-rule"
 RWS_ROUTE_DETECTED_RULES = "/detected-rules"
 RWS_ROUTE_FINDINGS_METADATA = "/findings-metadata"
 RWS_ROUTE_FINDING_STATUS_COUNT = "/finding-status-count"
 RWS_ROUTE_RULE_PACKS = "/rule-packs"
 RWS_ROUTE_VCS = "/vcs-instances"
 
+RWS_ROUTE_AUDITED_COUNT_OVER_TIME = "/audited-count-over-time"
+RWS_ROUTE_UN_TRIAGED_COUNT_OVER_TIME = "/un-triaged-count-over-time"
 RWS_ROUTE_COUNT_BY_TIME = "/count-by-time"
+RWS_ROUTE_COUNT_PER_VCS_PROVIDER_BY_WEEK = "/count-per-vcs-provider-by-week"
 RWS_ROUTE_SUPPORTED_VCS_PROVIDERS = "/supported-vcs-providers"
 RWS_ROUTE_SUPPORTED_STATUSES = "/supported-statuses"
 RWS_ROUTE_DISTINCT_PROJECTS = "/distinct-projects"
 RWS_ROUTE_DISTINCT_REPOSITORIES = "/distinct-repositories"
 COMMON_TAG = "resc-common"
 
 RWS_ROUTE_AUDIT = "/audit"
@@ -39,14 +43,15 @@
 BRANCHES_TAG = "resc-branches"
 SCANS_TAG = "resc-scans"
 FINDINGS_TAG = "resc-findings"
 RULES_TAG = "resc-rules"
 RULE_PACKS_TAG = "resc-rule-packs"
 HEALTH_TAG = "health"
 VCS_TAG = "resc-vcs-instances"
+METRICS_TAG = "resc-metrics"
 
 DEFAULT_RECORDS_PER_PAGE_LIMIT = 100
 MAX_RECORDS_PER_PAGE_LIMIT = 500
 
 RESC_OPERATOR_ROLE = "SG_APP_RESC_OPERATOR"
 
 BASE_SCAN = "BASE"
```

### Comparing `resc_backend-1.2.0/src/resc_backend/db/connection.py` & `resc_backend-1.3.0/src/resc_backend/db/connection.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/__init__.py` & `resc_backend-1.3.0/src/resc_backend/db/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,12 @@
 from resc_backend.db.model.audit import DBaudit
 from resc_backend.db.model.branch import DBbranch
 from resc_backend.db.model.finding import DBfinding
 from resc_backend.db.model.repository import DBrepository
 from resc_backend.db.model.rule import DBrule
 from resc_backend.db.model.rule_allow_list import DBruleAllowList
 from resc_backend.db.model.rule_pack import DBrulePack
+from resc_backend.db.model.rule_tag import DBruleTag
 from resc_backend.db.model.scan import DBscan
 from resc_backend.db.model.scan_finding import DBscanFinding
+from resc_backend.db.model.tag import DBtag
 from resc_backend.db.model.vcs_instance import DBVcsInstance
```

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/audit.py` & `resc_backend-1.3.0/src/resc_backend/db/model/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/branch.py` & `resc_backend-1.3.0/src/resc_backend/db/model/branch.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/finding.py` & `resc_backend-1.3.0/src/resc_backend/db/model/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/repository.py` & `resc_backend-1.3.0/src/resc_backend/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/rule.py` & `resc_backend-1.3.0/src/resc_backend/db/model/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,45 +11,42 @@
 class DBrule(Base):
     __tablename__ = "rules"
     id_ = Column("id", Integer, primary_key=True)
     rule_pack = Column(String(100), ForeignKey(DBrulePack.version), nullable=False)
     allow_list = Column(Integer, ForeignKey(DBruleAllowList.id_), nullable=True)
     rule_name = Column(String(400), nullable=False)
     description = Column(String(2000), nullable=True)
-    tags = Column(String(2000), nullable=True)
     entropy = Column(Float, nullable=True)
     secret_group = Column(Integer, nullable=True)
     regex = Column(Text, nullable=True)
     path = Column(Text, nullable=True)
     keywords = Column(Text, nullable=True)
     __table_args__ = (UniqueConstraint("rule_name", "rule_pack", name="unique_rule_name_per_rule_pack_version"),)
 
     def __init__(self, rule_pack: str, rule_name: str, description: str, allow_list: int = None,
-                 entropy: float = None, secret_group: str = None, regex: str = None, path: str = None, tags: str = None,
+                 entropy: float = None, secret_group: str = None, regex: str = None, path: str = None,
                  keywords: str = None):
         self.rule_pack = rule_pack
         self.allow_list = allow_list
         self.rule_name = rule_name
         self.description = description
         self.entropy = entropy
         self.secret_group = secret_group
         self.regex = regex
         self.path = path
-        self.tags = tags
         self.keywords = keywords
 
     @staticmethod
-    def create_from_metadata(rule_pack: str, rule_name: str, description: str, tags: str, entropy: float,
+    def create_from_metadata(rule_pack: str, rule_name: str, description: str, entropy: float,
                              secret_group: str, regex: str, path: str, keywords: str,
                              allow_list: int):
         db_rule = DBrule(
             rule_pack=rule_pack,
             rule_name=rule_name,
             description=description,
-            tags=tags,
             entropy=entropy,
             secret_group=secret_group,
             regex=regex,
             path=path,
             keywords=keywords,
             allow_list=allow_list
         )
```

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/rule_allow_list.py` & `resc_backend-1.3.0/src/resc_backend/db/model/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/rule_pack.py` & `resc_backend-1.3.0/src/resc_backend/db/model/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/scan.py` & `resc_backend-1.3.0/src/resc_backend/db/model/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/db/model/vcs_instance.py` & `resc_backend-1.3.0/src/resc_backend/db/model/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/helpers/dict_remapper.py` & `resc_backend-1.3.0/src/resc_backend/helpers/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/helpers/environment_wrapper.py` & `resc_backend-1.3.0/src/resc_backend/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/helpers/git_operation.py` & `resc_backend-1.3.0/src/resc_backend/helpers/git_operation.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/configuration.py` & `resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py` & `resc_backend-1.3.0/src/resc_backend/helpers/rabbitmq/rabbitmq_initialization.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/api.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 )
 from resc_backend.resc_web_service.endpoints import (
     branches,
     common,
     detailed_findings,
     findings,
     health,
+    metrics,
     repositories,
     rules,
     rule_packs,
     scans,
     vcs_instances
 )
 from resc_backend.resc_web_service.helpers.exception_handler import add_exception_handlers
@@ -91,14 +92,15 @@
     {"name": "resc-rules", "description": "Manage rule information"},
     {"name": "resc-rule-packs", "description": "Manage rule pack information"},
     {"name": "resc-repositories", "description": "Manage repository information"},
     {"name": "resc-branches", "description": "Manage branch information"},
     {"name": "resc-scans", "description": "Manage scan information"},
     {"name": "resc-findings", "description": "Manage findings information"},
     {"name": "resc-vcs-instances", "description": "Manage vcs instance information"},
+    {"name": "resc-metrics", "description": "Retrieve metrics"},
 ]
 
 # Check if authentication is required for api endpoints
 AUTH = [Depends(requires_no_auth)] if os.getenv('AUTHENTICATION_REQUIRED', '') == 'false' else [Depends(requires_auth)]
 
 app = FastAPI(title="Repository Scanner (RESC)",
               description="RESC API helps you to perform several operations upon findings "
@@ -122,14 +124,15 @@
 app.include_router(rules.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(rule_packs.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(findings.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(detailed_findings.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(repositories.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(scans.router, prefix=RWS_VERSION_PREFIX)
 app.include_router(vcs_instances.router, prefix=RWS_VERSION_PREFIX)
+app.include_router(metrics.router, prefix=RWS_VERSION_PREFIX)
 
 # Add exception handlers
 add_exception_handlers(app=app)
 
 
 @app.on_event("startup")
 def app_startup():
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/audit.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/branch.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/branch.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/detailed_finding.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/detailed_finding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# pylint: disable=R0912,C0121
+# pylint: disable=R0912,C0121,R0915
 # Standard Library
 from typing import List
 
 # Third Party
 from sqlalchemy import and_, func, or_
 from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
 from resc_backend.resc_web_service.filters import FindingsFilter
 from resc_backend.resc_web_service.schema import detailed_finding as detailed_finding_schema
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
+from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 
 def get_detailed_findings(db_connection: Session, findings_filter: FindingsFilter, skip: int = 0,
                           limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT
                           ) -> List[detailed_finding_schema.DetailedFindingRead]:
     """
     Retrieve all detailed findings objects matching the provided FindingsFilter
@@ -28,33 +29,41 @@
         integer amount of records to skip to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [DetailedFindingRead]
         The output will contain a list of DetailedFindingRead objects,
         or an empty list if no finding was found for the given findings_filter
     """
-    max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
-                                            func.max(model.DBscanFinding.scan_id).label("scan_id"))
-
+    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+                                                 func.max(model.DBscan.id_).label("latest_base_scan_id"))
+    max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
     if findings_filter.rule_pack_versions:
-        max_scan_subquery = max_scan_subquery.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id) \
-            .filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
-
-    if findings_filter.scan_ids:
-        max_scan_subquery = max_scan_subquery.filter(model.DBscanFinding.scan_id.in_(findings_filter.scan_ids))
-
-    max_scan_subquery = max_scan_subquery.group_by(model.DBscanFinding.finding_id).subquery()
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
 
     # subquery to select latest audit ids of findings
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
+    rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
+        .join(model.DBtag, model.DBruleTag.tag_id == model.DBtag.id_)
+    if findings_filter.rule_tags:
+        rule_tag_subquery = rule_tag_subquery.filter(model.DBtag.name.in_(findings_filter.rule_tags))
+    if findings_filter.rule_pack_versions or findings_filter.rule_names:
+        rule_tag_subquery = rule_tag_subquery.join(model.DBrule, model.DBrule.id_ == model.DBruleTag.rule_id)
+        if findings_filter.rule_pack_versions:
+            rule_tag_subquery = rule_tag_subquery.filter(model.DBrule.rule_pack.in_(findings_filter.rule_pack_versions))
+        if findings_filter.rule_names:
+            rule_tag_subquery = rule_tag_subquery.filter(model.DBrule.rule_name.in_(findings_filter.rule_names))
+    rule_tag_subquery = rule_tag_subquery.group_by(model.DBruleTag.rule_id).subquery()
+
     limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
-    scan_id = model.DBscan.id_.label("scan_id")
+
     query = db_connection.query(
         model.DBfinding.id_,
         model.DBfinding.file_path,
         model.DBfinding.line_number,
         model.DBfinding.column_start,
         model.DBfinding.column_end,
         model.DBfinding.commit_id,
@@ -64,41 +73,49 @@
         model.DBfinding.email,
         model.DBaudit.status,
         model.DBaudit.comment,
         model.DBfinding.rule_name,
         model.DBscan.rule_pack,
         model.DBfinding.event_sent_on,
         model.DBscan.timestamp,
-        scan_id,
+        model.DBscan.id_.label("scan_id"),
         model.DBbranch.branch_name,
         model.DBscan.last_scanned_commit,
         model.DBVcsInstance.provider_type.label("vcs_provider"),
         model.DBrepository.project_key,
         model.DBrepository.repository_name,
         model.DBrepository.repository_url,
-    ).join(max_scan_subquery, model.finding.DBfinding.id_ == max_scan_subquery.c.finding_id) \
-        .join(model.DBscan,
-              model.scan.DBscan.id_ == max_scan_subquery.c.scan_id) \
-        .join(model.DBbranch,
-              model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
+    )
+    query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
+    if findings_filter.scan_ids:
+        query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
+                                              model.DBscan.id_.in_(findings_filter.scan_ids)))
+    else:
+        query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
+        query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
+                                              model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
+    query = query.join(model.DBbranch,
+                       model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
         .join(model.DBrepository,
               model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
         .join(model.DBVcsInstance,
-              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
-        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-              isouter=True) \
-        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
-              isouter=True)
+              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+    query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+                       isouter=True)
+    query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
+                       isouter=True)
 
     if findings_filter.rule_tags:
         query = query.join(model.DBrule, and_(model.DBrule.rule_name == model.DBfinding.rule_name,
                                               model.DBrule.rule_pack == model.DBscan.rule_pack))
-        for tag in findings_filter.rule_tags:
-            query = query.filter(model.DBrule.tags.like(f"%{tag}%"))
+        query = query.join(rule_tag_subquery, model.DBrule.id_ == rule_tag_subquery.c.rule_id)
 
+    if findings_filter.rule_pack_versions:
+        query = query.filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
     if findings_filter.start_date_time:
         query = query.filter(model.scan.DBscan.timestamp >= findings_filter.start_date_time)
     if findings_filter.end_date_time:
         query = query.filter(model.scan.DBscan.timestamp <= findings_filter.end_date_time)
 
     if findings_filter.event_sent is not None:
         if findings_filter.event_sent:
@@ -136,52 +153,69 @@
         Object of type FindingsFilter, only DetailedFindingRead objects matching the attributes in this filter will be
             fetched
     :param db_connection:
         Session of the database connection
     :return: total_count
         count of findings
     """
-    max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
-                                            func.max(model.DBscanFinding.scan_id).label("scan_id"))
-
     # subquery to select latest audit ids of findings
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
+    max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
+                                                 func.max(model.DBscan.id_).label("latest_base_scan_id"))
+    max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
     if findings_filter.rule_pack_versions:
-        max_scan_subquery = max_scan_subquery.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id) \
-            .filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
+        max_base_scan_subquery = max_base_scan_subquery.filter(
+            model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
+    max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
 
-    if findings_filter.scan_ids:
-        max_scan_subquery = max_scan_subquery.filter(model.DBscanFinding.scan_id.in_(findings_filter.scan_ids))
+    rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
+        .join(model.DBtag, model.DBruleTag.tag_id == model.DBtag.id_)
+    if findings_filter.rule_tags:
+        rule_tag_subquery = rule_tag_subquery.filter(model.DBtag.name.in_(findings_filter.rule_tags))
+    if findings_filter.rule_pack_versions or findings_filter.rule_names:
+        rule_tag_subquery = rule_tag_subquery.join(model.DBrule, model.DBrule.id_ == model.DBruleTag.rule_id)
+        if findings_filter.rule_pack_versions:
+            rule_tag_subquery = rule_tag_subquery.filter(model.DBrule.rule_pack.in_(findings_filter.rule_pack_versions))
+        if findings_filter.rule_names:
+            rule_tag_subquery = rule_tag_subquery.filter(model.DBrule.rule_name.in_(findings_filter.rule_names))
+    rule_tag_subquery = rule_tag_subquery.group_by(model.DBruleTag.rule_id).subquery()
 
-    max_scan_subquery = max_scan_subquery.group_by(model.DBscanFinding.finding_id).subquery()
+    query = db_connection.query(func.count(model.DBfinding.id_))
 
-    query = db_connection.query(func.count(model.DBfinding.id_)) \
-        .join(max_scan_subquery, model.finding.DBfinding.id_ == max_scan_subquery.c.finding_id) \
-        .join(model.DBscan,
-              model.scan.DBscan.id_ == max_scan_subquery.c.scan_id) \
-        .join(model.DBbranch,
-              model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
+    query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
+    if findings_filter.scan_ids:
+        query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
+                                              model.DBscan.id_.in_(findings_filter.scan_ids)))
+    else:
+        query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
+        query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
+                                              model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
+
+    query = query.join(model.DBbranch,
+                       model.branch.DBbranch.id_ == model.finding.DBfinding.branch_id) \
         .join(model.DBrepository,
               model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
         .join(model.DBVcsInstance,
-              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
-        .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
-              isouter=True) \
-        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
-              isouter=True)
+              model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
+    query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+                       isouter=True)
+    query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
+                       isouter=True)
 
     if findings_filter.rule_tags:
         query = query.join(model.DBrule, and_(model.DBrule.rule_name == model.DBfinding.rule_name,
                                               model.DBrule.rule_pack == model.DBscan.rule_pack))
-        for tag in findings_filter.rule_tags:
-            query = query.filter(model.DBrule.tags.like(f"%{tag}%"))
+        query = query.join(rule_tag_subquery, model.DBrule.id_ == rule_tag_subquery.c.rule_id)
 
+    if findings_filter.rule_pack_versions:
+        query = query.filter(model.DBscan.rule_pack.in_(findings_filter.rule_pack_versions))
     if findings_filter.start_date_time:
         query = query.filter(model.scan.DBscan.timestamp >= findings_filter.start_date_time)
     if findings_filter.end_date_time:
         query = query.filter(model.scan.DBscan.timestamp <= findings_filter.end_date_time)
 
     if findings_filter.event_sent is not None:
         if findings_filter.event_sent:
@@ -261,12 +295,13 @@
               model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
         .join(model.DBrepository,
               model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
         .join(model.DBVcsInstance,
               model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance) \
         .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
               isouter=True) \
-        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+        .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                  model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
               isouter=True) \
         .filter(model.finding.DBfinding.id_ == finding_id)
     finding = query.first()
     return finding
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/finding.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/finding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=R0916,R0912,C0121
 # Standard Library
 import logging
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import List
 
 # Third Party
-from sqlalchemy import and_, extract, func, or_
+from sqlalchemy import and_, extract, func, or_, union
+from sqlalchemy.engine import Row
 from sqlalchemy.orm import Session
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
 from resc_backend.resc_web_service.crud import scan_finding as scan_finding_crud
 from resc_backend.resc_web_service.filters import FindingsFilter
@@ -127,15 +128,16 @@
         max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                                  func.max(model.DBaudit.id_).label("audit_id")) \
             .group_by(model.DBaudit.finding_id).subquery()
 
         query = query \
             .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                   isouter=True) \
-            .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+            .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                      model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                   isouter=True)
         if FindingStatus.NOT_ANALYZED in statuses_filter:
             query = query.filter(or_(model.DBaudit.status.in_(statuses_filter),
                                      model.DBaudit.status == None))  # noqa: E711
         else:
             query = query.filter(model.DBaudit.status.in_(statuses_filter))
 
@@ -165,15 +167,16 @@
             max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                                      func.max(model.DBaudit.id_).label("audit_id")) \
                 .group_by(model.DBaudit.finding_id).subquery()
 
             total_count_query = total_count_query \
                 .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                       isouter=True) \
-                .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+                .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                          model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                       isouter=True)
         if (findings_filter.vcs_providers and findings_filter.vcs_providers is not None) \
                 or findings_filter.project_name or findings_filter.branch_name \
                 or findings_filter.repository_name or findings_filter.start_date_time \
                 or findings_filter.end_date_time:
             total_count_query = total_count_query \
                 .join(model.DBscanFinding,
@@ -182,28 +185,14 @@
                       model.scan.DBscan.id_ == model.scan_finding.DBscanFinding.scan_id) \
                 .join(model.DBbranch,
                       model.branch.DBbranch.id_ == model.scan.DBscan.branch_id) \
                 .join(model.DBrepository,
                       model.repository.DBrepository.id_ == model.branch.DBbranch.repository_id) \
                 .join(model.DBVcsInstance,
                       model.vcs_instance.DBVcsInstance.id_ == model.repository.DBrepository.vcs_instance)
-        elif findings_filter.rule_tags:
-            max_scan_subquery = db_connection.query(model.DBscanFinding.finding_id,
-                                                    func.max(model.DBscanFinding.scan_id).label("scan_id"))
-            max_scan_subquery = max_scan_subquery.group_by(model.DBscanFinding.finding_id).subquery()
-            total_count_query = total_count_query.join(max_scan_subquery,
-                                                       model.finding.DBfinding.id_ == max_scan_subquery.c.finding_id) \
-                .join(model.DBscan, model.scan.DBscan.id_ == max_scan_subquery.c.scan_id)
-
-        if findings_filter.rule_tags:
-            total_count_query = total_count_query.join(model.DBrule,
-                                                       and_(model.DBrule.rule_name == model.DBfinding.rule_name,
-                                                            model.DBrule.rule_pack == model.DBscan.rule_pack))
-            for tag in findings_filter.rule_tags:
-                total_count_query = total_count_query.filter(model.DBrule.tags.like(f"%{tag}%"))
 
         if findings_filter.start_date_time:
             total_count_query = total_count_query.filter(
                 model.scan.DBscan.timestamp >= findings_filter.start_date_time)
         if findings_filter.end_date_time:
             total_count_query = total_count_query.filter(model.scan.DBscan.timestamp <= findings_filter.end_date_time)
 
@@ -305,15 +294,16 @@
         max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                                  func.max(model.DBaudit.id_).label("audit_id")) \
             .group_by(model.DBaudit.finding_id).subquery()
 
         query = query \
             .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
                   isouter=True) \
-            .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+            .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                      model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
                   isouter=True)
     if scan_id > 0:
         query = query.join(model.DBscanFinding,
                            model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_)
         query = query.filter(model.DBscanFinding.scan_id == scan_id)
     else:
         if finding_statuses:
@@ -367,15 +357,16 @@
         .group_by(model.DBaudit.finding_id).subquery()
 
     query = db_connection.query(func.count(model.DBfinding.id_).label('status_count'), model.DBaudit.status)
 
     query = query \
         .join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
               isouter=True) \
-        .join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id,
+        .join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                  model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
               isouter=True)
 
     if scan_ids and len(scan_ids) > 0:
         query = query \
             .join(model.DBscanFinding,
                   model.scan_finding.DBscanFinding.finding_id == model.finding.DBfinding.id_) \
             .join(model.DBscan,
@@ -392,56 +383,82 @@
         query = query.filter(model.DBfinding.rule_name == rule_name)
 
     findings_count_by_status = query.group_by(model.DBaudit.status).all()
 
     return findings_count_by_status
 
 
-def get_rule_findings_count_by_status(db_connection: Session):
+def get_rule_findings_count_by_status(db_connection: Session, rule_pack_versions: [str] = None,
+                                      rule_tags: [str] = None):
     """
         Retrieve count of findings based on rulename and status
     :param db_connection:
         Session of the database connection
+    :param rule_pack_versions:
+        optional, filter on rule pack version
+    :param rule_tags:
+        optional, filter on rule tag
     :return: findings_count
         per rulename and status the count of findings
     """
     query = db_connection.query(model.DBfinding.rule_name,
                                 model.DBaudit.status,
                                 func.count(model.DBfinding.id_))
 
     max_base_scan_subquery = db_connection.query(model.DBscan.branch_id,
                                                  func.max(model.DBscan.id_).label("latest_base_scan_id"))
     max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.scan_type == ScanType.BASE)
+    if rule_pack_versions:
+        max_base_scan_subquery = max_base_scan_subquery.filter(model.DBscan.rule_pack.in_(rule_pack_versions))
     max_base_scan_subquery = max_base_scan_subquery.group_by(model.DBscan.branch_id).subquery()
 
     max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
                                              func.max(model.DBaudit.id_).label("audit_id")) \
         .group_by(model.DBaudit.finding_id).subquery()
 
     query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
     query = query.join(max_base_scan_subquery, model.DBfinding.branch_id == max_base_scan_subquery.c.branch_id)
     query = query.join(model.DBscan, and_(model.DBscanFinding.scan_id == model.DBscan.id_,
                                           model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
+    if rule_tags:
+        rule_tag_subquery = db_connection.query(model.DBruleTag.rule_id) \
+            .join(model.DBtag, model.DBruleTag.tag_id == model.DBtag.id_)
+        if rule_pack_versions:
+            rule_tag_subquery = rule_tag_subquery.join(model.DBrule, model.DBrule.id_ == model.DBruleTag.rule_id)
+            rule_tag_subquery = rule_tag_subquery.filter(model.DBrule.rule_pack.in_(rule_pack_versions))
+
+        rule_tag_subquery = rule_tag_subquery.filter(model.DBtag.name.in_(rule_tags))
+        rule_tag_subquery = rule_tag_subquery.group_by(model.DBruleTag.rule_id).subquery()
+
+        query = query.join(model.DBrule, and_(model.DBrule.rule_name == model.DBfinding.rule_name,
+                                              model.DBrule.rule_pack == model.DBscan.rule_pack))
+        query = query.join(rule_tag_subquery, model.DBrule.id_ == rule_tag_subquery.c.rule_id)
+
+    if rule_pack_versions:
+        query = query.filter(model.DBscan.rule_pack.in_(rule_pack_versions))
+
     query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.DBscanFinding.finding_id,
                        isouter=True)
-    query = query.join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id, isouter=True)
+    query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.DBscanFinding.finding_id,
+                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id), isouter=True)
     query = query.group_by(model.DBfinding.rule_name, model.DBaudit.status)
     query = query.order_by(model.DBfinding.rule_name, model.DBaudit.status)
     status_counts = query.all()
 
     rule_count_dict = {}
     for status_count in status_counts:
         rule_count_dict[status_count[0]] = {
             "true_positive": 0,
             "false_positive": 0,
             "not_analyzed": 0,
             "under_review": 0,
             "clarification_required": 0,
             "total_findings_count": 0
         }
+
     for status_count in status_counts:
         rule_count_dict[status_count[0]]["total_findings_count"] += status_count[2]
         if status_count[1] == FindingStatus.NOT_ANALYZED or status_count[1] is None:
             rule_count_dict[status_count[0]]["not_analyzed"] += status_count[2]
         elif status_count[1] == FindingStatus.FALSE_POSITIVE:
             rule_count_dict[status_count[0]]["false_positive"] += status_count[2]
         elif status_count[1] == FindingStatus.TRUE_POSITIVE:
@@ -624,7 +641,164 @@
     db_connection.query(model.DBfinding) \
         .filter(model.finding.DBfinding.branch_id == model.branch.DBbranch.id_,
                 model.branch.DBbranch.repository_id == model.repository.DBrepository.id_,
                 model.repository.DBrepository.vcs_instance == model.vcs_instance.DBVcsInstance.id_,
                 model.vcs_instance.DBVcsInstance.id_ == vcs_instance_id) \
         .delete(synchronize_session=False)
     db_connection.commit()
+
+
+def get_finding_audit_status_count_over_time(db_connection: Session, status: FindingStatus, weeks: int = 13) -> dict:
+    """
+        Retrieve count of true positive findings over time for given weeks
+    :param db_connection:
+        Session of the database connection
+    :param status:
+        mandatory, status for which to get the audit counts over time
+    :param weeks:
+        optional, filter on last n weeks, default 13
+    :return: true_positive_count_over_time
+        list of rows containing finding statuses count over time per week
+    """
+    all_tables = []
+    for week in range(0, weeks):
+        last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
+        query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
+                                    extract('week', last_nth_week_date_time).label("week"),
+                                    model.DBVcsInstance.provider_type.label("provider_type"),
+                                    func.count(model.DBaudit.id_).label("finding_count")
+                                    )
+        max_audit_subquery = db_connection.query(func.max(model.DBaudit.id_).label("audit_id")) \
+            .filter(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time)) \
+            .filter(extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time)) \
+            .group_by(model.DBaudit.finding_id).subquery()
+        query = query.join(max_audit_subquery, max_audit_subquery.c.audit_id == model.DBaudit.id_)
+        query = query.join(model.DBfinding, model.DBfinding.id_ == model.DBaudit.finding_id)
+        query = query.join(model.DBbranch, model.DBbranch.id_ == model.DBfinding.branch_id)
+        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBbranch.repository_id)
+        query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
+        query = query.filter(model.DBaudit.status == status)
+        query = query.group_by(model.DBVcsInstance.provider_type)
+
+        all_tables.append(query)
+
+    # union
+    unioned_query = union(*all_tables)
+    status_count_over_time = db_connection.execute(unioned_query).all()
+    return status_count_over_time
+
+
+def get_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+    """
+        Retrieve count findings over time for given weeks
+    :param db_connection:
+        Session of the database connection
+    :param weeks:
+        optional, filter on last n weeks, default 13
+    :return: count_over_time
+        list of rows containing finding count over time per week
+    """
+    all_tables = []
+    for week in range(0, weeks):
+        last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
+        query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
+                                    extract('week', last_nth_week_date_time).label("week"),
+                                    model.DBVcsInstance.provider_type.label("provider_type"),
+                                    func.count(model.DBfinding.id_).label("finding_count")
+                                    )
+        max_base_scan = db_connection.query(func.max(model.DBscan.id_).label("scan_id"),
+                                            model.DBscan.branch_id) \
+            .filter(extract('year', model.DBscan.timestamp) == extract('year', last_nth_week_date_time)) \
+            .filter(extract('week', model.DBscan.timestamp) <= extract('week', last_nth_week_date_time)) \
+            .filter(model.DBscan.scan_type == ScanType.BASE) \
+            .group_by(model.DBscan.branch_id).subquery()
+
+        query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
+        query = query.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id)
+        query = query.join(max_base_scan, and_(max_base_scan.c.branch_id == model.DBscan.branch_id,
+                                               or_(model.DBscan.id_ == max_base_scan.c.scan_id,
+                                                   (and_(model.DBscan.id_ > max_base_scan.c.scan_id,
+                                                         model.DBscan.scan_type == ScanType.INCREMENTAL,
+                                                         extract('week', model.DBscan.timestamp) <=
+                                                         extract('week', last_nth_week_date_time),
+                                                         extract('year', model.DBscan.timestamp) ==
+                                                         extract('year', last_nth_week_date_time)))
+                                                   )
+                                               )
+                           )
+        query = query.join(model.DBbranch, model.DBbranch.id_ == model.DBscan.branch_id)
+        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBbranch.repository_id)
+        query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
+        query = query.group_by(model.DBVcsInstance.provider_type)
+
+        all_tables.append(query)
+
+    # union
+    unioned_query = union(*all_tables)
+    count_over_time = db_connection.execute(unioned_query).all()
+    return count_over_time
+
+
+def get_un_triaged_finding_count_by_vcs_provider_over_time(db_connection: Session, weeks: int = 13) -> list[Row]:
+    """
+        Retrieve count of un triaged findings over time for given weeks
+    :param db_connection:
+        Session of the database connection
+    :param weeks:
+        optional, filter on last n weeks, default 13
+    :return: count_over_time
+        list of rows containing un triaged findings count over time per week
+    """
+    all_tables = []
+    for week in range(0, weeks):
+        last_nth_week_date_time = datetime.utcnow() - timedelta(weeks=week)
+        query = db_connection.query(extract('year', last_nth_week_date_time).label("year"),
+                                    extract('week', last_nth_week_date_time).label("week"),
+                                    model.DBVcsInstance.provider_type.label("provider_type"),
+                                    func.count(model.DBfinding.id_).label("finding_count")
+                                    )
+        max_base_scan = db_connection.query(func.max(model.DBscan.id_).label("scan_id"),
+                                            model.DBscan.branch_id) \
+            .filter(extract('year', model.DBscan.timestamp) == extract('year', last_nth_week_date_time)) \
+            .filter(extract('week', model.DBscan.timestamp) <= extract('week', last_nth_week_date_time)) \
+            .filter(model.DBscan.scan_type == ScanType.BASE) \
+            .group_by(model.DBscan.branch_id).subquery()
+
+        max_audit_subquery = db_connection.query(model.DBaudit.finding_id,
+                                                 func.max(model.DBaudit.id_).label("audit_id")) \
+            .filter(extract('year', model.DBaudit.timestamp) == extract('year', last_nth_week_date_time)) \
+            .filter(extract('week', model.DBaudit.timestamp) <= extract('week', last_nth_week_date_time)) \
+            .group_by(model.DBaudit.finding_id).subquery()
+
+        query = query.join(model.DBscanFinding, model.DBfinding.id_ == model.DBscanFinding.finding_id)
+        query = query.join(model.DBscan, model.DBscan.id_ == model.DBscanFinding.scan_id)
+        query = query.join(max_base_scan, and_(max_base_scan.c.branch_id == model.DBscan.branch_id,
+                                               or_(model.DBscan.id_ == max_base_scan.c.scan_id,
+                                                   (and_(model.DBscan.id_ > max_base_scan.c.scan_id,
+                                                         model.DBscan.scan_type == ScanType.INCREMENTAL,
+                                                         extract('week', model.DBscan.timestamp) <=
+                                                         extract('week', last_nth_week_date_time),
+                                                         extract('year', model.DBscan.timestamp) ==
+                                                         extract('year', last_nth_week_date_time)))
+                                                   )
+                                               )
+                           )
+        query = query.join(model.DBbranch, model.DBbranch.id_ == model.DBscan.branch_id)
+        query = query.join(model.DBrepository, model.DBrepository.id_ == model.DBbranch.repository_id)
+        query = query.join(model.DBVcsInstance, model.DBVcsInstance.id_ == model.DBrepository.vcs_instance)
+
+        query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.finding.DBfinding.id_,
+                           isouter=True)
+        query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.finding.DBfinding.id_,
+                                               model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id),
+                           isouter=True)
+        query = query.filter(
+            or_(model.DBaudit.id_ == None, model.DBaudit.status == FindingStatus.NOT_ANALYZED))  # noqa: E711
+
+        query = query.group_by(model.DBVcsInstance.provider_type)
+
+        all_tables.append(query)
+
+    # union
+    unioned_query = union(*all_tables)
+    count_over_time = db_connection.execute(unioned_query).all()
+    return count_over_time
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/repository.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,16 @@
     query = query.join(model.DBbranch, model.DBbranch.repository_id == model.DBrepository.id_)
     query = query.join(max_base_scan_subquery, model.DBbranch.id_ == max_base_scan_subquery.c.branch_id)
     query = query.join(model.DBscan, and_(model.DBbranch.id_ == model.DBscan.branch_id,
                                           model.DBscan.id_ >= max_base_scan_subquery.c.latest_base_scan_id))
     query = query.join(model.DBscanFinding, model.DBscan.id_ == model.DBscanFinding.scan_id)
     query = query.join(max_audit_subquery, max_audit_subquery.c.finding_id == model.DBscanFinding.finding_id,
                        isouter=True)
-    query = query.join(model.DBaudit, model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id, isouter=True)
+    query = query.join(model.DBaudit, and_(model.audit.DBaudit.finding_id == model.DBscanFinding.finding_id,
+                                           model.audit.DBaudit.id_ == max_audit_subquery.c.audit_id), isouter=True)
     query = query.filter(model.DBrepository.id_.in_(repository_ids))
     query = query.group_by(model.DBrepository.id_, model.DBaudit.status, )
     status_counts = query.all()
     repo_count_dict = {}
     for repository_id in repository_ids:
         repo_count_dict[repository_id] = {
             "true_positive": 0,
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         Session of the database connection
     :param rule:
         RuleCreate object to be created
     """
     db_rule = model.rule.DBrule(
         rule_name=rule.rule_name,
         description=rule.description,
-        tags=rule.tags,
         entropy=rule.entropy,
         secret_group=rule.secret_group,
         regex=rule.regex,
         path=rule.path,
         keywords=rule.keywords,
         rule_pack=rule.rule_pack,
         allow_list=rule.allow_list,
@@ -88,15 +87,14 @@
     :return: List[str]
         The output contains list of strings of global allow list
     """
     query = db_connection.query(
         model.DBrule.id_,
         model.DBrule.rule_pack,
         model.DBrule.rule_name,
-        model.DBrule.tags,
         model.DBrule.entropy,
         model.DBrule.secret_group,
         model.DBrule.regex,
         model.DBrule.path,
         model.DBrule.keywords,
         model.rule_allow_list.DBruleAllowList.description,
         model.rule_allow_list.DBruleAllowList.regexes,
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/rule_pack.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/rule_pack.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # Standard Library
 import logging
 from typing import List, Optional
 
 # Third Party
 from packaging.version import Version
-from sqlalchemy import func, update
+from sqlalchemy import and_, func, update
 from sqlalchemy.orm import Session
 from sqlalchemy.sql.expression import true
 
 # First Party
 from resc_backend.constants import DEFAULT_RECORDS_PER_PAGE_LIMIT, MAX_RECORDS_PER_PAGE_LIMIT
 from resc_backend.db import model
 from resc_backend.resc_web_service.schema import rule_pack as rule_pack_schema
 
 logger = logging.getLogger(__name__)
 
 
-def get_rule_pack(db_connection: Session, version: Optional[str]) -> rule_pack_schema.RulePackRead:
+def get_rule_pack(
+    db_connection: Session, version: Optional[str]
+) -> rule_pack_schema.RulePackRead:
     """
         Get active rule pack from database
     :param db_connection:
         Session of the database connection
     :param version:
         optional, version of the rule pack to be fetched else latest rule pack version will be fetched
     :return: RulePackRead
@@ -32,26 +34,28 @@
     else:
         logger.debug("rule pack version not specified, fetching currently active one")
         query = query.filter(model.rule_pack.DBrulePack.active == true())
     rule_pack = query.first()
     return rule_pack
 
 
-def create_rule_pack_version(db_connection: Session, rule_pack: rule_pack_schema.RulePackCreate):
+def create_rule_pack_version(
+    db_connection: Session, rule_pack: rule_pack_schema.RulePackCreate
+):
     """
         Create rule pack version in database
     :param db_connection:
         Session of the database connection
     :param rule_pack:
         RulePackCreate object to be created
     """
     db_rule_pack = model.rule_pack.DBrulePack(
         version=rule_pack.version,
         global_allow_list=rule_pack.global_allow_list,
-        active=rule_pack.active
+        active=rule_pack.active,
     )
     db_connection.add(db_rule_pack)
     db_connection.commit()
     db_connection.refresh(db_rule_pack)
     return db_rule_pack
 
 
@@ -69,16 +73,21 @@
         newest_rule_pack: rule_pack_schema.RulePackRead = rule_packs[0]
         for rule_pack in rule_packs[1:]:
             if Version(rule_pack.version) > Version(newest_rule_pack.version):
                 newest_rule_pack = rule_pack
     return newest_rule_pack
 
 
-def get_rule_packs(db_connection: Session, version: str = None, active: bool = None, skip: int = 0,
-                   limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT) -> List[model.rule_pack.DBrulePack]:
+def get_rule_packs(
+    db_connection: Session,
+    version: str = None,
+    active: bool = None,
+    skip: int = 0,
+    limit: int = DEFAULT_RECORDS_PER_PAGE_LIMIT,
+) -> List[model.rule_pack.DBrulePack]:
     """
         Retrieve rule packs from database
     :param db_connection:
         Session of the database connection
     :param version:
         optional, filter on rule pack version
     :param active:
@@ -87,52 +96,111 @@
         integer amount of records to skip, to support pagination
     :param limit:
         integer amount of records to return, to support pagination
     :return: [RulePackRead]
         The output will contain a PaginationModel containing the list of RulePackRead type objects,
         or an empty list if no rule pack was found
     """
-    limit_val = MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    limit_val = (
+        MAX_RECORDS_PER_PAGE_LIMIT if limit > MAX_RECORDS_PER_PAGE_LIMIT else limit
+    )
     query = db_connection.query(model.rule_pack.DBrulePack)
 
     if version:
         query = query.filter(model.rule_pack.DBrulePack.version == version)
     if active is not None:
         query = query.filter(model.rule_pack.DBrulePack.active == active)
-    rule_packs = query.order_by(model.rule_pack.DBrulePack.version.desc()).offset(skip).limit(limit_val).all()
+    rule_packs = (
+        query.order_by(model.rule_pack.DBrulePack.version.desc())
+        .offset(skip)
+        .limit(limit_val)
+        .all()
+    )
     return rule_packs
 
 
-def get_total_rule_packs_count(db_connection: Session, version: str = None, active: bool = None) -> int:
+def get_current_active_rule_pack(
+    db_connection: Session,
+) -> Optional[model.rule_pack.DBrulePack]:
+    """
+        Return the currently active rule_pack, if any.
+    :param db_connection:
+        Session of the database connection
+    :return: DBRulePack
+        returns the DBRulePack containing the active rule pack
+    """
+    query = db_connection.query(model.rule_pack.DBrulePack)
+    active_rule_pack = query.filter(model.rule_pack.DBrulePack.active == 1).one()
+    return active_rule_pack
+
+
+def get_rule_packs_tags(db_connection: Session, versions: list) -> List[str]:
+    """
+        Retrieve rule packs tags for versions from database
+    :param db_connection:
+        Session of the database connection
+    :param versions:
+        optional, filter on rule pack version
+    :return: [str]
+        The output will contain the list of str that are the tags, or an empty list.
+    """
+
+    query = db_connection.query(model.DBtag.name)
+    query = query.join(model.DBruleTag, model.DBruleTag.tag_id == model.DBtag.id_)
+    query = query.join(
+        model.DBrule,
+        and_(
+            model.DBrule.id_ == model.DBruleTag.rule_id,
+            model.DBrule.rule_pack.in_(versions),
+        ),
+    )
+    rule_packs_tags = query.distinct().all()
+    rule_packs_tags = [t for t, in rule_packs_tags]
+    return rule_packs_tags
+
+
+def get_total_rule_packs_count(
+    db_connection: Session, version: str = None, active: bool = None
+) -> int:
     """
         Retrieve total count of rule packs from database
     :param db_connection:
         Session of the database connection
     :param version:
         optional, filter on rule pack version
     :param active:
         optional, filter on active rule pack
     :return: int
         The output contains total count of rule packs
     """
-    total_count_query = db_connection.query(func.count(model.rule_pack.DBrulePack.version))
+    total_count_query = db_connection.query(
+        func.count(model.rule_pack.DBrulePack.version)
+    )
     if version:
-        total_count_query = total_count_query.filter(model.rule_pack.DBrulePack.version == version)
+        total_count_query = total_count_query.filter(
+            model.rule_pack.DBrulePack.version == version
+        )
     if active is not None:
-        total_count_query = total_count_query.filter(model.rule_pack.DBrulePack.active == active)
+        total_count_query = total_count_query.filter(
+            model.rule_pack.DBrulePack.active == active
+        )
 
     total_count = total_count_query.scalar()
     return total_count
 
 
-def make_older_rule_packs_to_inactive(latest_rule_pack_version: str, db_connection: Session):
+def make_older_rule_packs_to_inactive(
+    latest_rule_pack_version: str, db_connection: Session
+):
     """
         Make older rule packs to inactive
     :param latest_rule_pack_version:
         latest rule pack version
     :param db_connection:
         Session of the database connection
     """
-    db_connection.execute(update(model.rule_pack.DBrulePack)
-                          .where(model.rule_pack.DBrulePack.version != latest_rule_pack_version)
-                          .values(active=False))
+    db_connection.execute(
+        update(model.rule_pack.DBrulePack)
+        .where(model.rule_pack.DBrulePack.version != latest_rule_pack_version)
+        .values(active=False)
+    )
     db_connection.commit()
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/scan_finding.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/scan_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/crud/vcs_instance.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/crud/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/dependencies.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/dependencies.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/branches.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/branches.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/common.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/common.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/detailed_findings.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,16 @@
             - finding_statuses [enum of type FindingStatus], possible values are:NOT_ANALYZED,FALSE_POSITIVE,
               TRUE_POSITIVE. Will default to all if non-specified.
 
             - rule_pack_versions of type [String]
 
             - rule_names of type [String]
 
-            - rule_tags of type [String]
+            - rule_tags of type [String] findings in the result will have at least one of the specified tags
+              for the rules
 
             - project_name of type String
 
             - repository_names of type [String]
 
             - branch_name of type String
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/findings.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/health.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/repositories.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/repositories.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rule_packs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Standard Library
 import logging
 import re
-from typing import Optional
+from typing import List, Optional
 
 # Third Party
 import tomlkit
 from fastapi import APIRouter, Depends, File, HTTPException, Query, UploadFile, status
 from fastapi.responses import FileResponse
 from packaging.version import Version
 from pydantic import Required
@@ -17,14 +17,15 @@
     ERROR_MESSAGE_503,
     RULE_PACKS_TAG,
     RWS_ROUTE_RULE_PACKS
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.crud import rule as rule_crud
 from resc_backend.resc_web_service.crud import rule_pack as rule_pack_crud
+from resc_backend.resc_web_service.crud import rule_tag as rule_tag_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.helpers.resc_swagger_models import Model400, Model404, Model409, Model422
 from resc_backend.resc_web_service.helpers.rule import (
     create_toml_dictionary,
     create_toml_rule_file,
     get_mapped_global_allow_list_obj,
     map_dictionary_to_rule_allow_list_object,
@@ -93,19 +94,20 @@
     - **return**: [FileResponse] The output returns rule pack file downloaded in TOML format
     """
     if not version:
         logger.info("rule pack version not specified, downloading the currently active version")
     rule_pack_from_db = read_rule_pack(version=version, db_connection=db_connection)
     if rule_pack_from_db:
         version = rule_pack_from_db.version
-        rules = rule_crud.get_rules_by_rule_pack_version(db_connection=db_connection,
-                                                         rule_pack_version=version)
+        rules = rule_crud.get_rules_by_rule_pack_version(db_connection=db_connection, rule_pack_version=version)
+        rule_tag_names = rule_tag_crud.get_rule_tag_names_by_rule_pack_version(db_connection=db_connection,
+                                                                               rule_pack_version=version)
         global_allow_list = rule_crud.get_global_allow_list_by_rule_pack_version(db_connection=db_connection,
                                                                                  rule_pack_version=version)
-        generated_toml_dict = create_toml_dictionary(version, rules, global_allow_list)
+        generated_toml_dict = create_toml_dictionary(version, rules, global_allow_list, rule_tag_names)
     else:
         raise HTTPException(status_code=404, detail=f"No rule pack found with version {version}")
 
     toml_file = create_toml_rule_file(generated_toml_dict)
     return FileResponse(toml_file.name, filename="RESC-SECRETS-RULE.toml")
 
 
@@ -232,27 +234,22 @@
         rule pack toml in dictionary format
     :param db_connection:
         Session of the database connection
     """
     if "rules" in toml_rule_dictionary:
         rule_list = toml_rule_dictionary.get("rules")
         for rule in rule_list:
-            tags = None
             keywords = None
             rule_name = rule["id"] if "id" in rule else None
             description = rule["description"] if "description" in rule else None
             regex = rule["regex"] if "regex" in rule else None
             entropy = rule["entropy"] if "entropy" in rule else None
             secret_group = rule["secretGroup"] if "secretGroup" in rule else None
             path = rule["path"] if "path" in rule else None
 
-            if "tags" in rule:
-                tag_array = rule["tags"]
-                tags = ",".join(tag_array)
-
             if "keywords" in rule:
                 keyword_array = rule["keywords"]
                 keywords = ",".join(keyword_array)
 
             # Insert in to RULE_ALLOW_LIST for storing individual rule specific  allow list
             allow_list = rule["allowlist"] if "allowlist" in rule else None
             rule_allow_list_obj = map_dictionary_to_rule_allow_list_object(allow_list)
@@ -264,19 +261,50 @@
             # Insert in to RULES
             if allow_list and created_rule_allow_list and created_rule_allow_list.id_:
                 created_allow_list_id = created_rule_allow_list.id_
             else:
                 created_allow_list_id = None
             rule_obj = RuleCreate(rule_pack=version,
                                   allow_list=created_allow_list_id,
-                                  rule_name=rule_name, description=description, tags=tags, entropy=entropy,
+                                  rule_name=rule_name, description=description, entropy=entropy,
                                   secret_group=secret_group, regex=regex, path=path, keywords=keywords)
             created_rule = rule_crud.create_rule(rule=rule_obj, db_connection=db_connection)
             if not created_rule.id_:
                 logger.warning(f"Creating rule failed for Rule: {rule_name}")
+            if "tags" in rule:
+                _ = rule_tag_crud.create_rule_tag(db_connection=db_connection, rule_id=created_rule.id_,
+                                                  tags=rule["tags"])
+
+
+@router.get("/tags",
+            response_model=List[str],
+            summary="Get rule packs' tags",
+            status_code=status.HTTP_200_OK,
+            responses={
+                200: {"description": "Retrieve all the tags related to a rule-pack[s]"},
+                500: {"description": ERROR_MESSAGE_500},
+                503: {"description": ERROR_MESSAGE_503}
+            })
+def get_rule_packs_tags(versions: Optional[List[str]] = Query(None, alias="version", title="version"),
+                        db_connection: Session = Depends(get_db_connection)) -> List[str]:
+    """
+        Retrieve rule pack related tags
+
+    :param db_connection: Session of the database connection
+    :param versions: Optional, filter on rule pack version, if not provided filter on active.
+    :return: List[str]
+        The output will contain a list of tags related to one or more rule-packs.
+    """
+    if not versions:
+        active_rule_pack = rule_pack_crud.get_current_active_rule_pack(db_connection=db_connection)
+        if not active_rule_pack:
+            raise HTTPException(status_code=500, detail="No currently active rule pack.")
+        versions = [active_rule_pack.version]
+    rule_packs_tags = rule_pack_crud.get_rule_packs_tags(db_connection=db_connection, versions=versions)
+    return rule_packs_tags
 
 
 def determine_uploaded_rule_pack_activation(requested_rule_pack_version: str,
                                             latest_rule_pack_from_db: RulePackRead) -> bool:
     """
         Determine if rule pack needs to be activated
     :param requested_rule_pack_version:
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/rules.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,16 @@
     RULES_TAG,
     RWS_ROUTE_DETECTED_RULES,
     RWS_ROUTE_FINDING_STATUS_COUNT,
     RWS_ROUTE_RULES
 )
 from resc_backend.db.connection import Session
 from resc_backend.resc_web_service.crud import finding as finding_crud
-from resc_backend.resc_web_service.crud import rule as rule_crud
 from resc_backend.resc_web_service.dependencies import get_db_connection
 from resc_backend.resc_web_service.schema.finding_status import FindingStatus
-from resc_backend.resc_web_service.schema.rule import RuleCreate
 from resc_backend.resc_web_service.schema.rule_count_model import RuleFindingCountModel
 from resc_backend.resc_web_service.schema.status_count import StatusCount
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 router = APIRouter(tags=[RULES_TAG])
 
 logger = logging.getLogger(__name__)
@@ -78,22 +76,29 @@
             summary="Get detected rules with counts per status",
             status_code=status.HTTP_200_OK,
             responses={
                 200: {"description": "Retrieve all the detected rules with counts per status"},
                 500: {"description": ERROR_MESSAGE_500},
                 503: {"description": ERROR_MESSAGE_503}
             })
-def get_rules_finding_status_count(db_connection: Session = Depends(get_db_connection)) -> List[RuleFindingCountModel]:
+def get_rules_finding_status_count(
+        rule_pack_versions: Optional[List[str]] = Query(None, alias="rule_pack_version", title="RulePackVersion"),
+        rule_tags: Optional[List[str]] = Query(None, alias="rule_tag", title="RuleTag"),
+        db_connection: Session = Depends(get_db_connection)) -> List[RuleFindingCountModel]:
     """
         Retrieve all detected rules with finding counts per supported status
 
+    - **rule_pack_version**: Optional, filter on rule pack version
+    - **rule_tag**: Optional, filter on rule tag
     - **db_connection**: Session of the database connection
     - **return**: List[str] The output will contain a list of strings of unique rules with counts per status
     """
-    rule_finding_counts = finding_crud.get_rule_findings_count_by_status(db_connection)
+    rule_finding_counts = finding_crud.get_rule_findings_count_by_status(db_connection,
+                                                                         rule_pack_versions=rule_pack_versions,
+                                                                         rule_tags=rule_tags)
     rule_findings_counts = []
 
     for rule_name, rule_counts in rule_finding_counts.items():
         rule_finding_count = RuleFindingCountModel(rule_name=rule_name,
                                                    finding_count=rule_counts["total_findings_count"])
         rule_finding_count.finding_statuses_count.append(
             StatusCount(status=FindingStatus.TRUE_POSITIVE, count=rule_counts["true_positive"]))
@@ -104,21 +109,7 @@
         rule_finding_count.finding_statuses_count.append(
             StatusCount(status=FindingStatus.UNDER_REVIEW, count=rule_counts["under_review"]))
         rule_finding_count.finding_statuses_count.append(
             StatusCount(status=FindingStatus.CLARIFICATION_REQUIRED, count=rule_counts["clarification_required"]))
         rule_findings_counts.append(rule_finding_count)
 
     return rule_findings_counts
-
-
-def create_rule(
-        rule: RuleCreate,
-        db_connection: Session = Depends(get_db_connection)):
-    """
-        Create rule in database
-    :param rule:
-        RuleCreate object to be created
-    :param db_connection:
-        Session of the database connection
-    """
-    return rule_crud.create_rule(db_connection=db_connection,
-                                 rule=rule)
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/scans.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/scans.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/endpoints/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/filters.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/filters.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/exception_handler.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/exception_handler.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/resc_swagger_models.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/helpers/rule.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/helpers/rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,30 +40,32 @@
         if allow_list.commits:
             allow_list_dict["commits"] = allow_list.commits
         if allow_list.stop_words:
             allow_list_dict["stop_words"] = allow_list.stop_words
     return allow_list_dict
 
 
-def create_rule_dictionary(rule: Rule, allow_list_dict: dict) -> dict:
+def create_rule_dictionary(rule: Rule, allow_list_dict: dict, tags: str) -> dict:
     """
         Create a dictionary for rule when Rule object and RuleAllowList dict are supplied
     :param rule:
         Rule object
     :param allow_list_dict:
         Allow list dictionary
+    :param tags:
+        String of tags of the rule
     :return: Rule dictionary
         The output will contain a dictionary of Rule
     """
     rule_dict = {}
     if rule.rule_name:
         rule_dict["id"] = rule.rule_name
         rule_dict["description"] = rule.rule_name
-    if rule.tags:
-        rule_dict["tags"] = rule.tags
+    if tags:
+        rule_dict["tags"] = tags
     if rule.entropy:
         rule_dict["entropy"] = rule.entropy
     if rule.secret_group:
         rule_dict["secret_group"] = rule.secret_group
     if rule.regex:
         rule_dict["regex"] = rule.regex
     if rule.path:
@@ -71,30 +73,37 @@
     if rule.keywords:
         rule_dict["keywords"] = rule.keywords
     if allow_list_dict:
         rule_dict["allow_list"] = allow_list_dict
     return rule_dict
 
 
-def create_toml_dictionary(rule_pack_version: str, rules: List[str], global_allow_list: List[str]) -> dict:
+def create_toml_dictionary(rule_pack_version: str, rules: List[str], global_allow_list: List[str], rule_tag_names) \
+        -> dict:
     """
         Create a dictionary for gitleaks toml rule for specified rule pack version, rules and global allow list
     :param rule_pack_version:
         Rule pack version
     :param rules:
         Rule list
     :param global_allow_list:
         Global Allow list
+    :param rule_tag_names:
+        List of rule names and tags
     :return: toml dictionary
         The output will contain a dictionary for gitleaks toml rule
     """
     rule_list = []
     for rule in rules:
         allow_list_dict = create_allow_list_dictionary(rule)
-        rule_dict = create_rule_dictionary(rule, allow_list_dict)
+        tags_list = [x.name for x in rule_tag_names if x.rule_name == rule.rule_name]
+        tags = None
+        if len(tags_list) >= 1:
+            tags = ','.join(tags_list)
+        rule_dict = create_rule_dictionary(rule, allow_list_dict, tags)
         rule_list.append(rule_dict)
 
     global_allow_list_dict = create_allow_list_dictionary(global_allow_list)
 
     rule_toml_dict = {"title": "gitleaks config"}
     if rule_pack_version:
         rule_toml_dict["version"] = rule_pack_version
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/audit.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/audit.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/branch.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/branch.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/detailed_finding.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/detailed_finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/finding_count_model.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/finding_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/pagination_model.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/pagination_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/repository.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/repository_enriched.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/repository_enriched.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # Third Party
 from pydantic import BaseModel, conint, constr
 
 
 class RuleBase(BaseModel):
     rule_name: constr(min_length=1, max_length=400)
     description: Optional[constr(max_length=2000)] = None
-    tags: Optional[constr(max_length=2000)] = None
     entropy: Optional[float] = None
     secret_group: Optional[int] = None
     regex: Optional[str] = None
     path: Optional[str] = None
     keywords: Optional[str] = None
```

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_allow_list.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_count_model.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_count_model.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/rule_pack.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/rule_pack.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/scan.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/scan.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service/schema/vcs_instance.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service/schema/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/branches.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/branches.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/findings.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/findings.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/rule_packs.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/rule_packs.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend/resc_web_service_interface/vcs_instances.py` & `resc_backend-1.3.0/src/resc_backend/resc_web_service_interface/vcs_instances.py`

 * *Files identical despite different names*

### Comparing `resc_backend-1.2.0/src/resc_backend.egg-info/PKG-INFO` & `resc_backend-1.3.0/src/resc_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-backend
-Version: 1.2.0
+Version: 1.3.0
 Summary: Repository Scanner - Backend
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_backend-1.2.0/src/resc_backend.egg-info/SOURCES.txt` & `resc_backend-1.3.0/src/resc_backend.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 src/resc_backend/db/model/audit.py
 src/resc_backend/db/model/branch.py
 src/resc_backend/db/model/finding.py
 src/resc_backend/db/model/repository.py
 src/resc_backend/db/model/rule.py
 src/resc_backend/db/model/rule_allow_list.py
 src/resc_backend/db/model/rule_pack.py
+src/resc_backend/db/model/rule_tag.py
 src/resc_backend/db/model/scan.py
 src/resc_backend/db/model/scan_finding.py
+src/resc_backend/db/model/tag.py
 src/resc_backend/db/model/vcs_instance.py
 src/resc_backend/helpers/__init__.py
 src/resc_backend/helpers/dict_remapper.py
 src/resc_backend/helpers/environment_wrapper.py
 src/resc_backend/helpers/git_operation.py
 src/resc_backend/helpers/rabbitmq/__init__.py
 src/resc_backend/helpers/rabbitmq/configuration.py
@@ -40,23 +42,25 @@
 src/resc_backend/resc_web_service/crud/audit.py
 src/resc_backend/resc_web_service/crud/branch.py
 src/resc_backend/resc_web_service/crud/detailed_finding.py
 src/resc_backend/resc_web_service/crud/finding.py
 src/resc_backend/resc_web_service/crud/repository.py
 src/resc_backend/resc_web_service/crud/rule.py
 src/resc_backend/resc_web_service/crud/rule_pack.py
+src/resc_backend/resc_web_service/crud/rule_tag.py
 src/resc_backend/resc_web_service/crud/scan.py
 src/resc_backend/resc_web_service/crud/scan_finding.py
 src/resc_backend/resc_web_service/crud/vcs_instance.py
 src/resc_backend/resc_web_service/endpoints/__init__.py
 src/resc_backend/resc_web_service/endpoints/branches.py
 src/resc_backend/resc_web_service/endpoints/common.py
 src/resc_backend/resc_web_service/endpoints/detailed_findings.py
 src/resc_backend/resc_web_service/endpoints/findings.py
 src/resc_backend/resc_web_service/endpoints/health.py
+src/resc_backend/resc_web_service/endpoints/metrics.py
 src/resc_backend/resc_web_service/endpoints/repositories.py
 src/resc_backend/resc_web_service/endpoints/rule_packs.py
 src/resc_backend/resc_web_service/endpoints/rules.py
 src/resc_backend/resc_web_service/endpoints/scans.py
 src/resc_backend/resc_web_service/endpoints/vcs_instances.py
 src/resc_backend/resc_web_service/helpers/__init__.py
 src/resc_backend/resc_web_service/helpers/exception_handler.py
@@ -66,14 +70,15 @@
 src/resc_backend/resc_web_service/schema/audit.py
 src/resc_backend/resc_web_service/schema/branch.py
 src/resc_backend/resc_web_service/schema/date_count_model.py
 src/resc_backend/resc_web_service/schema/date_filter.py
 src/resc_backend/resc_web_service/schema/detailed_finding.py
 src/resc_backend/resc_web_service/schema/finding.py
 src/resc_backend/resc_web_service/schema/finding_count_model.py
+src/resc_backend/resc_web_service/schema/finding_count_over_time.py
 src/resc_backend/resc_web_service/schema/finding_status.py
 src/resc_backend/resc_web_service/schema/pagination_model.py
 src/resc_backend/resc_web_service/schema/repository.py
 src/resc_backend/resc_web_service/schema/repository_enriched.py
 src/resc_backend/resc_web_service/schema/rule.py
 src/resc_backend/resc_web_service/schema/rule_allow_list.py
 src/resc_backend/resc_web_service/schema/rule_count_model.py
```

