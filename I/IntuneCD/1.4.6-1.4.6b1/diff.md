# Comparing `tmp/IntuneCD-1.4.6.tar.gz` & `tmp/IntuneCD-1.4.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.6.tar", last modified: Thu May 25 06:57:32 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.6b1.tar", last modified: Mon May 22 06:52:59 2023, max compression
```

## Comparing `IntuneCD-1.4.6.tar` & `IntuneCD-1.4.6b1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:32.343035 IntuneCD-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-25 06:57:32.343035 IntuneCD-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 06:57:32.343035 IntuneCD-1.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:32.335035 IntuneCD-1.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:32.343035 IntuneCD-1.4.6/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_apns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/run_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:32.343035 IntuneCD-1.4.6/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-25 06:57:32.000000 IntuneCD-1.4.6/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-25 06:57:32.000000 IntuneCD-1.4.6/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:57:32.000000 IntuneCD-1.4.6/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-25 06:57:32.000000 IntuneCD-1.4.6/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 06:57:32.000000 IntuneCD-1.4.6/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 06:57:32.000000 IntuneCD-1.4.6/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:57:32.343035 IntuneCD-1.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_get_added_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_group_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-25 06:57:21.000000 IntuneCD-1.4.6/tests/test_update_frontend.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.992976 IntuneCD-1.4.6b1/
+-rw-r--r--   0 tobias     (501) staff       (20)     1059 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/LICENSE
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-05-22 06:52:59.993116 IntuneCD-1.4.6b1/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     2697 2023-01-24 09:42:37.000000 IntuneCD-1.4.6b1/README.md
+-rw-r--r--   0 tobias     (501) staff       (20)      103 2022-05-03 19:33:01.000000 IntuneCD-1.4.6b1/pyproject.toml
+-rw-r--r--   0 tobias     (501) staff       (20)      999 2023-05-22 06:52:59.993592 IntuneCD-1.4.6b1/setup.cfg
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.958227 IntuneCD-1.4.6b1/src/
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.987295 IntuneCD-1.4.6b1/src/IntuneCD/
+-rw-r--r--   0 tobias     (501) staff       (20)        0 2022-05-03 19:33:01.000000 IntuneCD-1.4.6b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2344 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3938 2023-03-20 07:54:18.000000 IntuneCD-1.4.6b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2241 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1327 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3001 2023-05-22 06:37:51.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1865 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4651 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1370 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1090 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2473 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1454 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1655 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2386 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2718 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1245 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2359 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2926 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2508 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1378 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2467 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1445 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1754 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2710 2023-05-16 06:42:29.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3289 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)     4962 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1486 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2589 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1312 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1961 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)      548 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      515 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1933 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)    15819 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3701 2023-03-08 08:59:36.000000 IntuneCD-1.4.6b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3198 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10342 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7753 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)      622 2022-08-09 15:09:09.000000 IntuneCD-1.4.6b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      987 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12362 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12356 2023-03-20 12:09:40.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11471 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 tobias     (501) staff       (20)      934 2023-03-06 07:57:06.000000 IntuneCD-1.4.6b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7900 2023-05-22 06:40:42.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7963 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3524 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7443 2023-03-06 09:55:38.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 tobias     (501) staff       (20)     3741 2023-04-25 08:44:13.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9372 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7193 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7703 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8929 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2630 2023-03-20 12:09:40.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 tobias     (501) staff       (20)    11648 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8715 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 tobias     (501) staff       (20)      749 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 tobias     (501) staff       (20)    24286 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9069 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8066 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8428 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)    10612 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 tobias     (501) staff       (20)    16118 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 tobias     (501) staff       (20)     8385 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7197 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.988462 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 tobias     (501) staff       (20)     3230 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 tobias     (501) staff       (20)     3153 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        1 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      179 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 tobias     (501) staff       (20)      102 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 tobias     (501) staff       (20)        9 2023-05-22 06:52:59.000000 IntuneCD-1.4.6b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 tobias     (501) staff       (20)        0 2023-05-22 06:52:59.992787 IntuneCD-1.4.6b1/tests/
+-rw-r--r--   0 tobias     (501) staff       (20)     2042 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_archive.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2005 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_check_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)      848 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_clean_filename.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2096 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_diff_summary.py
+-rw-r--r--   0 tobias     (501) staff       (20)     7233 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_documentation_functions.py
+-rw-r--r--   0 tobias     (501) staff       (20)      953 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_get_added_removed.py
+-rw-r--r--   0 tobias     (501) staff       (20)     9753 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_get_authparams.py
+-rw-r--r--   0 tobias     (501) staff       (20)    12241 2023-03-08 09:16:49.000000 IntuneCD-1.4.6b1/tests/test_graph_batch.py
+-rw-r--r--   0 tobias     (501) staff       (20)    17428 2023-05-11 10:04:49.000000 IntuneCD-1.4.6b1/tests/test_graph_request.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2980 2023-03-08 10:43:23.000000 IntuneCD-1.4.6b1/tests/test_group_report.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1279 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_load_file.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1622 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_match.py
+-rw-r--r--   0 tobias     (501) staff       (20)      559 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_remove_keys.py
+-rw-r--r--   0 tobias     (501) staff       (20)     1888 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_save_output.py
+-rw-r--r--   0 tobias     (501) staff       (20)     2292 2023-01-24 09:42:30.000000 IntuneCD-1.4.6b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.6/LICENSE` & `IntuneCD-1.4.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/PKG-INFO` & `IntuneCD-1.4.6b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.6
+Version: 1.4.6b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.6/README.md` & `IntuneCD-1.4.6b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/setup.cfg` & `IntuneCD-1.4.6b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.6
+version = 1.4.6.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.6/src/IntuneCD/archive.py` & `IntuneCD-1.4.6b1/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.6b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/check_file.py` & `IntuneCD-1.4.6b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.6b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.6b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.6b1/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.6b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.6b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.6b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.6b1/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/load_file.py` & `IntuneCD-1.4.6b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.6b1/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.6b1/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.6b1/src/IntuneCD/run_documentation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/run_update.py` & `IntuneCD-1.4.6b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/save_output.py` & `IntuneCD-1.4.6b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_appConfiguration.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,30 +122,24 @@
                                 token,
                             )
 
                 # If App Configuration does not exist, create it and assign
                 else:
                     print("-" * 90)
                     print("App Configuration not found, creating: " + repo_data["displayName"])
-
-                    if repo_data.get("payloadJson"):
-                        repo_data["payloadJson"] = base64.b64encode(
-                            json.dumps(repo_data["payloadJson"]).encode("utf-8")
-                        ).decode("utf-8")
-
                     app_ids = {}
                     # If backup contains targeted apps, search for the app
                     if repo_data["targetedMobileApps"]:
                         q_param = {
                             "$filter": "(isof("
                             + "'"
                             + str(repo_data["targetedMobileApps"]["type"]).replace("#", "")
                             + "'"
                             + "))",
-                            "$search": f'"{repo_data["targetedMobileApps"]["appName"]}"',
+                            "$search": repo_data["targetedMobileApps"]["appName"],
                         }
                         app_request = makeapirequest(APP_ENDPOINT, token, q_param)
                         if app_request["value"]:
                             app_ids = app_request["value"][0]["id"]
                     # If the app could be found and matches type and name in
                     # backup, continue to create
                     if app_ids and report is False:
```

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_appProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.6b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.6b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.6
+Version: 1.4.6b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.6/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.6b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_archive.py` & `IntuneCD-1.4.6b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_check_file.py` & `IntuneCD-1.4.6b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_clean_filename.py` & `IntuneCD-1.4.6b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_diff_summary.py` & `IntuneCD-1.4.6b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_documentation_functions.py` & `IntuneCD-1.4.6b1/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_get_added_removed.py` & `IntuneCD-1.4.6b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_get_authparams.py` & `IntuneCD-1.4.6b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_graph_batch.py` & `IntuneCD-1.4.6b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_graph_request.py` & `IntuneCD-1.4.6b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_group_report.py` & `IntuneCD-1.4.6b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_load_file.py` & `IntuneCD-1.4.6b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_match.py` & `IntuneCD-1.4.6b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_remove_keys.py` & `IntuneCD-1.4.6b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_save_output.py` & `IntuneCD-1.4.6b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.6/tests/test_update_frontend.py` & `IntuneCD-1.4.6b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

