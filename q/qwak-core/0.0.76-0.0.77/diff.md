# Comparing `tmp/qwak_core-0.0.76.tar.gz` & `tmp/qwak_core-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.76.tar", max compression
+gzip compressed data, was "qwak_core-0.0.77.tar", max compression
```

## Comparing `qwak_core-0.0.76.tar` & `qwak_core-0.0.77.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-24 08:19:56.544032 qwak_core-0.0.76/README.md
--rw-r--r--   0        0        0        0 2023-05-24 08:21:43.292896 qwak_core-0.0.76/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-24 08:21:43.316896 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-24 08:21:21.052716 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.316896 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-24 08:21:43.312896 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-24 08:21:20.656713 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.312896 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-24 08:21:43.316896 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-24 08:21:20.852714 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.316896 qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-24 08:21:43.304896 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-24 08:21:20.064708 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-24 08:21:43.308896 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-24 08:21:43.308896 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-24 08:21:20.260710 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.308896 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-24 08:21:43.308896 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-24 08:21:20.460711 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.312896 qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-24 08:21:43.292896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-24 08:21:19.864706 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-24 08:21:43.292896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-24 08:21:43.296896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-24 08:21:21.252718 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.296896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-24 08:21:43.300896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-24 08:21:21.644721 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.300896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-24 08:21:43.300896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-24 08:21:21.844722 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-24 08:21:43.304896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-24 08:21:43.296896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-24 08:21:21.448719 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.296896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-24 08:21:43.304896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-24 08:21:22.040724 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.304896 qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-24 08:21:43.348896 qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-24 08:21:24.764746 qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.348896 qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-24 08:21:43.348896 qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-24 08:21:24.960748 qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-24 08:21:43.352896 qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-24 08:21:43.420897 qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-24 08:21:30.552793 qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.420897 qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-24 08:21:43.420897 qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-24 08:21:30.752794 qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-24 08:21:43.420897 qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-24 08:21:43.424897 qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-24 08:21:31.772803 qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-24 08:21:43.428897 qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-24 08:21:43.424897 qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-24 08:21:31.548801 qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.424897 qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-24 08:21:43.428897 qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-24 08:21:31.972804 qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.428897 qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-24 08:21:43.428897 qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-24 08:21:32.168806 qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-24 08:21:43.432897 qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-24 08:21:43.524898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-24 08:21:40.844876 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.524898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-24 08:21:43.516898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-24 08:21:40.448873 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.520898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-24 08:21:43.520898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-24 08:21:40.640874 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.520898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-24 08:21:43.512898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-24 08:21:40.040870 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-24 08:21:43.516898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-24 08:21:43.516898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-24 08:21:40.252871 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.516898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-24 08:21:43.528898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-24 08:21:41.428881 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.528898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-24 08:21:43.528898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-24 08:21:41.236879 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.528898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-24 08:21:43.524898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-24 08:21:41.040878 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.524898 qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-24 08:21:43.512898 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-24 08:21:39.832868 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.512898 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-24 08:21:43.508898 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-24 08:21:39.404864 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.508898 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-24 08:21:43.508898 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-24 08:21:39.632866 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-24 08:21:43.512898 qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-24 08:21:43.456897 qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-24 08:21:34.212822 qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-24 08:21:43.456897 qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-24 08:21:43.452897 qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-24 08:21:34.008821 qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.456897 qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-24 08:21:43.444897 qwak_core-0.0.76/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-24 08:21:33.600818 qwak_core-0.0.76/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.444897 qwak_core-0.0.76/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-24 08:21:43.448897 qwak_core-0.0.76/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-24 08:21:33.800819 qwak_core-0.0.76/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.448897 qwak_core-0.0.76/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-24 08:21:43.448897 qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-24 08:21:34.416824 qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-24 08:21:43.452897 qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-24 08:21:43.452897 qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-24 08:21:34.856828 qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-24 08:21:43.452897 qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-24 08:21:43.464897 qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-24 08:21:35.284831 qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.464897 qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-24 08:21:43.464897 qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-24 08:21:35.484833 qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-24 08:21:43.468897 qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-24 08:21:43.440897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-24 08:21:33.000813 qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.440897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-24 08:21:43.440897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-24 08:21:33.200814 qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-24 08:21:43.440897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-24 08:21:43.432897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-24 08:21:32.584809 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.436897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-24 08:21:43.432897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-24 08:21:32.384808 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.432897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-24 08:21:43.436897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-24 08:21:32.800811 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-24 08:21:43.436897 qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-24 08:21:43.336896 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-24 08:21:23.792738 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.336896 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-24 08:21:43.340896 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-24 08:21:23.988740 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.340896 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-24 08:21:43.340896 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-24 08:21:24.188741 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-24 08:21:43.340896 qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-24 08:21:43.400897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-24 08:21:29.336783 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.400897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-24 08:21:43.396897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-24 08:21:29.144781 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-24 08:21:43.396897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-24 08:21:43.376896 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-24 08:21:27.392767 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.376896 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-24 08:21:43.376896 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-24 08:21:27.204766 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.376896 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-24 08:21:43.368896 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-24 08:21:26.584761 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.368896 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-24 08:21:43.372897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-24 08:21:27.012764 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-24 08:21:43.372897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-24 08:21:43.380897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-24 08:21:27.584769 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.380897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-24 08:21:43.380897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-24 08:21:27.772770 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-24 08:21:43.384897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-24 08:21:43.372897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-24 08:21:26.788762 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.372897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-24 08:21:43.384897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-24 08:21:27.960772 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.384897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11224 2023-05-24 08:21:43.384897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    14819 2023-05-24 08:21:28.152773 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.388897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-24 08:21:43.400897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-24 08:21:42.808892 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.404897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-24 08:21:43.404897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-24 08:21:43.004893 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-24 08:21:43.404897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-24 08:21:43.404897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-24 08:21:29.964788 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.408897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-24 08:21:43.408897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-24 08:21:30.164790 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-24 08:21:43.408897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-24 08:21:43.408897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-24 08:21:30.356791 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.412897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-24 08:21:43.416897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-24 08:21:31.160798 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.416897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-24 08:21:43.412897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-24 08:21:30.956796 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-24 08:21:43.412897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-24 08:21:43.416897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-24 08:21:31.352799 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.416897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-24 08:21:43.388897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-24 08:21:28.348775 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.388897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-24 08:21:43.388897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-24 08:21:28.544777 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.392897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-24 08:21:43.392897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-24 08:21:28.740778 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-24 08:21:43.392897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-24 08:21:43.396897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-24 08:21:28.944780 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.396897 qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-24 08:21:43.532898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-24 08:21:41.624882 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.532898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-24 08:21:43.532898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-24 08:21:41.816884 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-24 08:21:43.532898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-24 08:21:43.536898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-24 08:21:42.012885 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.536898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-24 08:21:43.536898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-24 08:21:42.216887 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-24 08:21:43.540898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-24 08:21:43.540898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-24 08:21:42.420889 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-24 08:21:43.540898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-24 08:21:43.540898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-24 08:21:42.616890 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.544898 qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-24 08:21:43.468897 qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-24 08:21:35.684834 qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.468897 qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-24 08:21:43.468897 qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-24 08:21:35.888836 qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-24 08:21:43.472897 qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-24 08:21:43.352896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-24 08:21:25.800754 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.356896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-24 08:21:43.356896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-24 08:21:25.992756 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.360896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-24 08:21:43.360896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-24 08:21:26.188758 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-24 08:21:43.364896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-24 08:21:43.364896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-24 08:21:26.384759 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.368896 qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-24 08:21:43.444897 qwak_core-0.0.76/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-24 08:21:33.400816 qwak_core-0.0.76/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-24 08:21:43.444897 qwak_core-0.0.76/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-24 08:21:43.472897 qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-24 08:21:36.088837 qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.472897 qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-24 08:21:43.472897 qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-24 08:21:36.292839 qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-24 08:21:43.476897 qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-24 08:21:43.488897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-24 08:21:37.572850 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.488897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-24 08:21:43.488897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-24 08:21:37.772851 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.488897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-24 08:21:43.492897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-24 08:21:37.976853 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.492897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-24 08:21:43.492897 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-24 08:21:38.176854 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.496898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-24 08:21:43.496898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-24 08:21:38.384856 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.496898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-24 08:21:43.496898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-24 08:21:38.600858 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-24 08:21:43.500898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-24 08:21:43.500898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-24 08:21:38.796859 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.500898 qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-24 08:21:43.476897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-24 08:21:36.720843 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.480897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-24 08:21:43.484897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-24 08:21:37.356848 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.484897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-24 08:21:43.480897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-24 08:21:36.932844 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-24 08:21:43.480897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-24 08:21:43.484897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-24 08:21:37.140846 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.484897 qwak_core-0.0.76/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-24 08:21:43.460897 qwak_core-0.0.76/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-24 08:21:35.080829 qwak_core-0.0.76/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-24 08:21:43.460897 qwak_core-0.0.76/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-24 08:21:43.332896 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-24 08:21:25.404751 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-24 08:21:43.332896 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-24 08:21:43.328896 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-24 08:21:25.172749 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.332896 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-24 08:21:43.332896 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-24 08:21:25.608753 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-24 08:21:43.336896 qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-24 08:21:43.460897 qwak_core-0.0.76/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-24 08:21:34.632826 qwak_core-0.0.76/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-24 08:21:43.460897 qwak_core-0.0.76/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-24 08:21:43.476897 qwak_core-0.0.76/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-24 08:21:36.512841 qwak_core-0.0.76/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-24 08:21:43.476897 qwak_core-0.0.76/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-24 08:21:43.328896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-24 08:21:23.016732 qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.328896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-24 08:21:43.324896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-24 08:21:22.820730 qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-24 08:21:43.328896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-24 08:21:43.320896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-24 08:21:22.236725 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.320896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-24 08:21:43.320896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-24 08:21:22.428727 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.320896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-24 08:21:43.324896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-24 08:21:22.624729 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-24 08:21:43.324896 qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-24 08:21:43.504897 qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-24 08:21:39.192863 qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-24 08:21:43.504897 qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-24 08:21:43.504897 qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-24 08:21:38.992861 qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.504897 qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-24 08:21:43.344896 qwak_core-0.0.76/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-24 08:21:24.380743 qwak_core-0.0.76/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.344896 qwak_core-0.0.76/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-24 08:21:43.344896 qwak_core-0.0.76/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-24 08:21:24.568744 qwak_core-0.0.76/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-24 08:21:43.344896 qwak_core-0.0.76/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-24 08:21:45.016910 qwak_core-0.0.76/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-24 08:21:45.016910 qwak_core-0.0.76/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-24 08:19:56.544032 qwak_core-0.0.76/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-24 08:19:56.548032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-24 08:19:56.552032 qwak_core-0.0.76/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.76/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.76/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-24 08:48:48.826043 qwak_core-0.0.77/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 08:50:38.358937 qwak_core-0.0.77/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-24 08:50:38.382938 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-24 08:50:16.866762 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.382938 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-24 08:50:38.378938 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-24 08:50:16.470759 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.378938 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-24 08:50:38.382938 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-24 08:50:16.658760 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.382938 qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-24 08:50:38.370937 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-24 08:50:15.886754 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-24 08:50:38.374937 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-24 08:50:38.374937 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-24 08:50:16.086756 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.374937 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-24 08:50:38.378938 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-24 08:50:16.278757 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.378938 qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-24 08:50:38.358937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-24 08:50:15.670752 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-24 08:50:38.358937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-24 08:50:38.362937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-24 08:50:17.062764 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.362937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-24 08:50:38.366937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-24 08:50:17.446767 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.366937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-24 08:50:38.366937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-24 08:50:17.650769 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-24 08:50:38.370937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-24 08:50:38.362937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-24 08:50:17.254765 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.366937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-24 08:50:38.370937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-24 08:50:17.846770 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.370937 qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-24 08:50:38.414938 qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-24 08:50:20.578792 qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.414938 qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-24 08:50:38.414938 qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-24 08:50:20.770794 qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-24 08:50:38.418938 qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-24 08:50:38.486938 qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-24 08:50:26.226838 qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.486938 qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-24 08:50:38.486938 qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-24 08:50:26.418840 qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-24 08:50:38.490939 qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-24 08:50:38.490939 qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-24 08:50:27.394848 qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-24 08:50:38.494938 qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-24 08:50:38.490939 qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-24 08:50:27.206847 qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.490939 qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-24 08:50:38.494938 qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-24 08:50:27.586850 qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.494938 qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-24 08:50:38.498938 qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-24 08:50:27.778851 qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-24 08:50:38.498938 qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-24 08:50:38.590939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-24 08:50:35.986918 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.590939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-24 08:50:38.586939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-24 08:50:35.602915 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.586939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-24 08:50:38.586939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-24 08:50:35.790917 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.586939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-24 08:50:38.578939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-24 08:50:35.218912 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-24 08:50:38.582939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-24 08:50:38.582939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-24 08:50:35.414913 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.582939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-24 08:50:38.594939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-24 08:50:36.546923 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.594939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-24 08:50:38.594939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-24 08:50:36.362921 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.594939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-24 08:50:38.590939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-24 08:50:36.174919 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.590939 qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-24 08:50:38.578939 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-24 08:50:35.014910 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.578939 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-24 08:50:38.574939 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-24 08:50:34.614907 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.574939 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-24 08:50:38.574939 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-24 08:50:34.822908 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-24 08:50:38.578939 qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-24 08:50:38.522939 qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-24 08:50:29.742867 qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-24 08:50:38.522939 qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-24 08:50:38.522939 qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-24 08:50:29.530866 qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.522939 qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-24 08:50:38.510939 qwak_core-0.0.77/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-24 08:50:29.146862 qwak_core-0.0.77/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.514939 qwak_core-0.0.77/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-24 08:50:38.514939 qwak_core-0.0.77/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-24 08:50:29.334864 qwak_core-0.0.77/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.514939 qwak_core-0.0.77/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-24 08:50:38.514939 qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-24 08:50:29.934869 qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-24 08:50:38.518939 qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-24 08:50:38.518939 qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-24 08:50:30.374872 qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-24 08:50:38.518939 qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-24 08:50:38.530939 qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-24 08:50:30.774875 qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.530939 qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-24 08:50:38.530939 qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-24 08:50:30.966877 qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-24 08:50:38.534939 qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-24 08:50:38.506939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-24 08:50:28.578858 qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.506939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-24 08:50:38.506939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-24 08:50:28.766859 qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-24 08:50:38.510939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-24 08:50:38.502939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-24 08:50:28.182855 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.502939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-24 08:50:38.498938 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-24 08:50:27.982853 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.498938 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-24 08:50:38.502939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-24 08:50:28.386856 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-24 08:50:38.506939 qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-24 08:50:38.402938 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-24 08:50:19.594784 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.402938 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-24 08:50:38.406938 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-24 08:50:19.794786 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.406938 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-24 08:50:38.406938 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-24 08:50:19.994788 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-24 08:50:38.410938 qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-24 08:50:38.466938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-24 08:50:25.074829 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.466938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-24 08:50:38.462938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-24 08:50:24.886828 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-24 08:50:38.462938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-24 08:50:38.442938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-24 08:50:23.118813 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.442938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-24 08:50:38.442938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-24 08:50:22.930812 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.442938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-24 08:50:38.434938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-24 08:50:22.338807 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.434938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-24 08:50:38.438938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-24 08:50:22.742810 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-24 08:50:38.438938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-24 08:50:38.446938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-24 08:50:23.310815 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.446938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-24 08:50:38.446938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-24 08:50:23.498816 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-24 08:50:38.450938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-24 08:50:38.438938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-24 08:50:22.538808 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.438938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-24 08:50:38.450938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-24 08:50:23.686818 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.450938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11224 2023-05-24 08:50:38.450938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    14819 2023-05-24 08:50:23.902819 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.454938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-24 08:50:38.466938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-24 08:50:37.894934 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.470938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-24 08:50:38.470938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-24 08:50:38.086935 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-24 08:50:38.470938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-24 08:50:38.470938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-24 08:50:25.650834 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.474938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-24 08:50:38.474938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-24 08:50:25.842835 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-24 08:50:38.474938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-24 08:50:38.478938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-24 08:50:26.030837 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.478938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-24 08:50:38.482938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-24 08:50:26.806843 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.482938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-24 08:50:38.478938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-24 08:50:26.606842 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-24 08:50:38.478938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-24 08:50:38.482938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-24 08:50:27.014845 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.482938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-24 08:50:38.454938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-24 08:50:24.102821 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.454938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-24 08:50:38.454938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-24 08:50:24.302823 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.458938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-24 08:50:38.458938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-24 08:50:24.494824 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-24 08:50:38.458938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-24 08:50:38.462938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-24 08:50:24.694826 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.462938 qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-24 08:50:38.598939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-24 08:50:36.734924 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.598939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-24 08:50:38.598939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-24 08:50:36.922926 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-24 08:50:38.602939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-24 08:50:38.602939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-24 08:50:37.118927 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.602939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-24 08:50:38.602939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-24 08:50:37.314929 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-24 08:50:38.606939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-24 08:50:38.606939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-24 08:50:37.514931 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-24 08:50:38.606939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-24 08:50:38.606939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-24 08:50:37.702932 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.610939 qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-24 08:50:38.534939 qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-24 08:50:31.162879 qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.534939 qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-24 08:50:38.534939 qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-24 08:50:31.350880 qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-24 08:50:38.538939 qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-24 08:50:38.418938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-24 08:50:21.534800 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.422938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-24 08:50:38.422938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-24 08:50:21.726802 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.426938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-24 08:50:38.426938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-24 08:50:21.918803 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-24 08:50:38.430938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-24 08:50:38.430938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-24 08:50:22.126805 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.434938 qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-24 08:50:38.510939 qwak_core-0.0.77/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-24 08:50:28.958861 qwak_core-0.0.77/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-24 08:50:38.510939 qwak_core-0.0.77/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-24 08:50:38.538939 qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-24 08:50:31.538882 qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.538939 qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-24 08:50:38.542939 qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-24 08:50:31.726883 qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-24 08:50:38.542939 qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-24 08:50:38.554939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-24 08:50:32.874893 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.554939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-24 08:50:38.554939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-24 08:50:33.062894 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.558939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-24 08:50:38.558939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-24 08:50:33.254896 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.558939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-24 08:50:38.558939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-24 08:50:33.450897 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.562939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-24 08:50:38.562939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-24 08:50:33.646899 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.562939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-24 08:50:38.566939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-24 08:50:33.854901 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-24 08:50:38.566939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-24 08:50:38.566939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-24 08:50:34.046902 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.566939 qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-24 08:50:38.546939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-24 08:50:32.110886 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.546939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-24 08:50:38.550939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-24 08:50:32.686891 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.550939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-24 08:50:38.546939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-24 08:50:32.302888 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-24 08:50:38.546939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-24 08:50:38.550939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-24 08:50:32.498890 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.550939 qwak_core-0.0.77/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-24 08:50:38.526939 qwak_core-0.0.77/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-24 08:50:30.582874 qwak_core-0.0.77/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-24 08:50:38.530939 qwak_core-0.0.77/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-24 08:50:38.398938 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-24 08:50:21.150797 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-24 08:50:38.398938 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-24 08:50:38.394938 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-24 08:50:20.958796 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.398938 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-24 08:50:38.402938 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-24 08:50:21.342799 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-24 08:50:38.402938 qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-24 08:50:38.526939 qwak_core-0.0.77/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-24 08:50:30.162871 qwak_core-0.0.77/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-24 08:50:38.526939 qwak_core-0.0.77/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-24 08:50:38.542939 qwak_core-0.0.77/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-24 08:50:31.918885 qwak_core-0.0.77/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-24 08:50:38.542939 qwak_core-0.0.77/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-24 08:50:38.394938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-24 08:50:18.814778 qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.394938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-24 08:50:38.390938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-24 08:50:18.618776 qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-24 08:50:38.394938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-24 08:50:38.386937 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-24 08:50:18.038772 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.386937 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-24 08:50:38.386937 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-24 08:50:18.230773 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.390938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-24 08:50:38.390938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-24 08:50:18.422775 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-24 08:50:38.390938 qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-24 08:50:38.570939 qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-24 08:50:34.430905 qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-24 08:50:38.570939 qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-24 08:50:38.570939 qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-24 08:50:34.238904 qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.570939 qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-24 08:50:38.410938 qwak_core-0.0.77/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-24 08:50:20.186789 qwak_core-0.0.77/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.410938 qwak_core-0.0.77/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-24 08:50:38.410938 qwak_core-0.0.77/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-24 08:50:20.382791 qwak_core-0.0.77/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-24 08:50:38.414938 qwak_core-0.0.77/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-24 08:50:40.646956 qwak_core-0.0.77/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-24 08:50:40.646956 qwak_core-0.0.77/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.826043 qwak_core-0.0.77/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-24 08:48:48.830043 qwak_core-0.0.77/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-24 08:48:48.834043 qwak_core-0.0.77/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.77/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.77/PKG-INFO
```

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/common/v0/resources.proto\x12\x1fqwak.user_application.common.v0\"u\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x03 \x01(\x0e\x32+.qwak.user_application.common.v0.MemoryUnit\"^\n\x0cGpuResources\x12:\n\x08gpu_type\x18\x01 \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"s\n SparkClusterResourceTemplateSpec\x12O\n\x08template\x18\x01 \x01(\x0e\x32=.qwak.user_application.common.v0.SparkClusterResourceTemplate\"\xc3\x01\n\x1aSparkResourceConfiguration\x12\x15\n\rdriver_memory\x18\x01 \x01(\t\x12\x14\n\x0c\x64river_cores\x18\x02 \x01(\x05\x12\x19\n\x11initial_executors\x18\x03 \x01(\x05\x12\x15\n\rmin_executors\x18\x04 \x01(\x05\x12\x15\n\rmax_executors\x18\x05 \x01(\x05\x12\x17\n\x0f\x65xecutor_memory\x18\x06 \x01(\t\x12\x16\n\x0e\x65xecutor_cores\x18\x07 \x01(\x05\"o\n\x1ePodComputeResourceTemplateSpec\x12M\n\x08template\x18\x01 \x01(\x0e\x32;.qwak.user_application.common.v0.PodComputeResourceTemplate\"\xf3\x01\n\x13PodComputeResources\x12P\n\x11optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12\x44\n\rcpu_resources\x18\x02 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResources\x12\x44\n\rgpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"t\n\x15SparkComputeResources\x12[\n\x16resource_configuration\x18\x01 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfiguration\"\xe5\x01\n\x1b\x43lientSparkComputeResources\x12Z\n\rtemplate_spec\x18\x01 \x01(\x0b\x32\x41.qwak.user_application.common.v0.SparkClusterResourceTemplateSpecH\x00\x12]\n\x16resource_configuration\x18\x02 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfigurationH\x00\x42\x0b\n\tresources\"\xe9\x02\n\x19\x43lientPodComputeResources\x12U\n\x16node_optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12X\n\rtemplate_spec\x18\x02 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpecH\x00\x12\x46\n\rcpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResourcesH\x00\x12\x46\n\rgpu_resources\x18\x04 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesH\x00\x42\x0b\n\tresources*7\n\nMemoryUnit\x12\x17\n\x13INVALID_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*q\n\x07GpuType\x12\x14\n\x10INVALID_GPU_TYPE\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*\x88\x02\n\x1cSparkClusterResourceTemplate\x12\"\n\x1eSPARK_CLUSTER_RESOURCE_INVALID\x10\x00\x12 \n\x1cSPARK_CLUSTER_RESOURCE_SMALL\x10\x01\x12!\n\x1dSPARK_CLUSTER_RESOURCE_MEDIUM\x10\x02\x12 \n\x1cSPARK_CLUSTER_RESOURCE_LARGE\x10\x03\x12\x1d\n\x19SPARK_CLUSTER_RESOURCE_XL\x10\x04\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_2XL\x10\x05\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_3XL\x10\x06*\x8a\x01\n\x14NodeOptimizationType\x12\x1d\n\x19NODE_OPTIMIZATION_INVALID\x10\x00\x12\x1a\n\x16NODE_OPTIMIZATION_NONE\x10\x01\x12\x19\n\x15NODE_OPTIMIZATION_CPU\x10\x02\x12\x1c\n\x18NODE_OPTIMIZATION_MEMORY\x10\x03*\xb4\x02\n\x1aPodComputeResourceTemplate\x12 \n\x1cPOD_COMPUTE_RESOURCE_INVALID\x10\x00\x12\x1e\n\x1aPOD_COMPUTE_RESOURCE_SMALL\x10\x01\x12\x1f\n\x1bPOD_COMPUTE_RESOURCE_MEDIUM\x10\x02\x12\x1e\n\x1aPOD_COMPUTE_RESOURCE_LARGE\x10\x03\x12\x1b\n\x17POD_COMPUTE_RESOURCE_XL\x10\x04\x12\x1c\n\x18POD_COMPUTE_RESOURCE_2XL\x10\x05\x12\x1c\n\x18POD_COMPUTE_RESOURCE_3XL\x10\x06\x12\x1c\n\x18POD_COMPUTE_RESOURCE_4XL\x10\x07\x12\x1c\n\x18POD_COMPUTE_RESOURCE_5XL\x10\x08\x42\xc5\x01\n&com.qwak.ai.user_application.common.v0P\x01Z\x98\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/qwak/user_application/common/v0/resources.proto\x12\x1fqwak.user_application.common.v0\"u\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12\x41\n\x0cmemory_units\x18\x03 \x01(\x0e\x32+.qwak.user_application.common.v0.MemoryUnit\"^\n\x0cGpuResources\x12:\n\x08gpu_type\x18\x01 \x01(\x0e\x32(.qwak.user_application.common.v0.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"s\n SparkClusterResourceTemplateSpec\x12O\n\x08template\x18\x01 \x01(\x0e\x32=.qwak.user_application.common.v0.SparkClusterResourceTemplate\"\xc3\x01\n\x1aSparkResourceConfiguration\x12\x15\n\rdriver_memory\x18\x01 \x01(\t\x12\x14\n\x0c\x64river_cores\x18\x02 \x01(\x05\x12\x19\n\x11initial_executors\x18\x03 \x01(\x05\x12\x15\n\rmin_executors\x18\x04 \x01(\x05\x12\x15\n\rmax_executors\x18\x05 \x01(\x05\x12\x17\n\x0f\x65xecutor_memory\x18\x06 \x01(\t\x12\x16\n\x0e\x65xecutor_cores\x18\x07 \x01(\x05\"5\n\x1ePodComputeResourceTemplateSpec\x12\x13\n\x0btemplate_id\x18\x01 \x01(\t\"\xf3\x01\n\x13PodComputeResources\x12P\n\x11optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12\x44\n\rcpu_resources\x18\x02 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResources\x12\x44\n\rgpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"t\n\x15SparkComputeResources\x12[\n\x16resource_configuration\x18\x01 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfiguration\"\xe5\x01\n\x1b\x43lientSparkComputeResources\x12Z\n\rtemplate_spec\x18\x01 \x01(\x0b\x32\x41.qwak.user_application.common.v0.SparkClusterResourceTemplateSpecH\x00\x12]\n\x16resource_configuration\x18\x02 \x01(\x0b\x32;.qwak.user_application.common.v0.SparkResourceConfigurationH\x00\x42\x0b\n\tresources\"\xe9\x02\n\x19\x43lientPodComputeResources\x12U\n\x16node_optimization_type\x18\x01 \x01(\x0e\x32\x35.qwak.user_application.common.v0.NodeOptimizationType\x12X\n\rtemplate_spec\x18\x02 \x01(\x0b\x32?.qwak.user_application.common.v0.PodComputeResourceTemplateSpecH\x00\x12\x46\n\rcpu_resources\x18\x03 \x01(\x0b\x32-.qwak.user_application.common.v0.CpuResourcesH\x00\x12\x46\n\rgpu_resources\x18\x04 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResourcesH\x00\x42\x0b\n\tresources*7\n\nMemoryUnit\x12\x17\n\x13INVALID_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*q\n\x07GpuType\x12\x14\n\x10INVALID_GPU_TYPE\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*\x88\x02\n\x1cSparkClusterResourceTemplate\x12\"\n\x1eSPARK_CLUSTER_RESOURCE_INVALID\x10\x00\x12 \n\x1cSPARK_CLUSTER_RESOURCE_SMALL\x10\x01\x12!\n\x1dSPARK_CLUSTER_RESOURCE_MEDIUM\x10\x02\x12 \n\x1cSPARK_CLUSTER_RESOURCE_LARGE\x10\x03\x12\x1d\n\x19SPARK_CLUSTER_RESOURCE_XL\x10\x04\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_2XL\x10\x05\x12\x1e\n\x1aSPARK_CLUSTER_RESOURCE_3XL\x10\x06*\x8a\x01\n\x14NodeOptimizationType\x12\x1d\n\x19NODE_OPTIMIZATION_INVALID\x10\x00\x12\x1a\n\x16NODE_OPTIMIZATION_NONE\x10\x01\x12\x19\n\x15NODE_OPTIMIZATION_CPU\x10\x02\x12\x1c\n\x18NODE_OPTIMIZATION_MEMORY\x10\x03\x42\xc5\x01\n&com.qwak.ai.user_application.common.v0P\x01Z\x98\x01github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0b\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 _SPARKCLUSTERRESOURCETEMPLATE = DESCRIPTOR.enum_types_by_name['SparkClusterResourceTemplate']
 SparkClusterResourceTemplate = enum_type_wrapper.EnumTypeWrapper(_SPARKCLUSTERRESOURCETEMPLATE)
 _NODEOPTIMIZATIONTYPE = DESCRIPTOR.enum_types_by_name['NodeOptimizationType']
 NodeOptimizationType = enum_type_wrapper.EnumTypeWrapper(_NODEOPTIMIZATIONTYPE)
-_PODCOMPUTERESOURCETEMPLATE = DESCRIPTOR.enum_types_by_name['PodComputeResourceTemplate']
-PodComputeResourceTemplate = enum_type_wrapper.EnumTypeWrapper(_PODCOMPUTERESOURCETEMPLATE)
 INVALID_MEMORY_UNIT = 0
 MIB = 1
 GIB = 2
 INVALID_GPU_TYPE = 0
 NVIDIA_K80 = 1
 NVIDIA_V100 = 2
 NVIDIA_A100 = 3
@@ -43,23 +41,14 @@
 SPARK_CLUSTER_RESOURCE_XL = 4
 SPARK_CLUSTER_RESOURCE_2XL = 5
 SPARK_CLUSTER_RESOURCE_3XL = 6
 NODE_OPTIMIZATION_INVALID = 0
 NODE_OPTIMIZATION_NONE = 1
 NODE_OPTIMIZATION_CPU = 2
 NODE_OPTIMIZATION_MEMORY = 3
-POD_COMPUTE_RESOURCE_INVALID = 0
-POD_COMPUTE_RESOURCE_SMALL = 1
-POD_COMPUTE_RESOURCE_MEDIUM = 2
-POD_COMPUTE_RESOURCE_LARGE = 3
-POD_COMPUTE_RESOURCE_XL = 4
-POD_COMPUTE_RESOURCE_2XL = 5
-POD_COMPUTE_RESOURCE_3XL = 6
-POD_COMPUTE_RESOURCE_4XL = 7
-POD_COMPUTE_RESOURCE_5XL = 8
 
 
 _CPURESOURCES = DESCRIPTOR.message_types_by_name['CpuResources']
 _GPURESOURCES = DESCRIPTOR.message_types_by_name['GpuResources']
 _SPARKCLUSTERRESOURCETEMPLATESPEC = DESCRIPTOR.message_types_by_name['SparkClusterResourceTemplateSpec']
 _SPARKRESOURCECONFIGURATION = DESCRIPTOR.message_types_by_name['SparkResourceConfiguration']
 _PODCOMPUTERESOURCETEMPLATESPEC = DESCRIPTOR.message_types_by_name['PodComputeResourceTemplateSpec']
@@ -130,36 +119,34 @@
   })
 _sym_db.RegisterMessage(ClientPodComputeResources)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.qwak.ai.user_application.common.v0P\001Z\230\001github.com/qwak-ai/qwak-platform/services/core/go/admiral/user-application-value-api/pb/qwak/user_application_value/common/v0;user_application_common_v0'
-  _MEMORYUNIT._serialized_start=1687
-  _MEMORYUNIT._serialized_end=1742
-  _GPUTYPE._serialized_start=1744
-  _GPUTYPE._serialized_end=1857
-  _SPARKCLUSTERRESOURCETEMPLATE._serialized_start=1860
-  _SPARKCLUSTERRESOURCETEMPLATE._serialized_end=2124
-  _NODEOPTIMIZATIONTYPE._serialized_start=2127
-  _NODEOPTIMIZATIONTYPE._serialized_end=2265
-  _PODCOMPUTERESOURCETEMPLATE._serialized_start=2268
-  _PODCOMPUTERESOURCETEMPLATE._serialized_end=2576
+  _MEMORYUNIT._serialized_start=1629
+  _MEMORYUNIT._serialized_end=1684
+  _GPUTYPE._serialized_start=1686
+  _GPUTYPE._serialized_end=1799
+  _SPARKCLUSTERRESOURCETEMPLATE._serialized_start=1802
+  _SPARKCLUSTERRESOURCETEMPLATE._serialized_end=2066
+  _NODEOPTIMIZATIONTYPE._serialized_start=2069
+  _NODEOPTIMIZATIONTYPE._serialized_end=2207
   _CPURESOURCES._serialized_start=84
   _CPURESOURCES._serialized_end=201
   _GPURESOURCES._serialized_start=203
   _GPURESOURCES._serialized_end=297
   _SPARKCLUSTERRESOURCETEMPLATESPEC._serialized_start=299
   _SPARKCLUSTERRESOURCETEMPLATESPEC._serialized_end=414
   _SPARKRESOURCECONFIGURATION._serialized_start=417
   _SPARKRESOURCECONFIGURATION._serialized_end=612
   _PODCOMPUTERESOURCETEMPLATESPEC._serialized_start=614
-  _PODCOMPUTERESOURCETEMPLATESPEC._serialized_end=725
-  _PODCOMPUTERESOURCES._serialized_start=728
-  _PODCOMPUTERESOURCES._serialized_end=971
-  _SPARKCOMPUTERESOURCES._serialized_start=973
-  _SPARKCOMPUTERESOURCES._serialized_end=1089
-  _CLIENTSPARKCOMPUTERESOURCES._serialized_start=1092
-  _CLIENTSPARKCOMPUTERESOURCES._serialized_end=1321
-  _CLIENTPODCOMPUTERESOURCES._serialized_start=1324
-  _CLIENTPODCOMPUTERESOURCES._serialized_end=1685
+  _PODCOMPUTERESOURCETEMPLATESPEC._serialized_end=667
+  _PODCOMPUTERESOURCES._serialized_start=670
+  _PODCOMPUTERESOURCES._serialized_end=913
+  _SPARKCOMPUTERESOURCES._serialized_start=915
+  _SPARKCOMPUTERESOURCES._serialized_end=1031
+  _CLIENTSPARKCOMPUTERESOURCES._serialized_start=1034
+  _CLIENTSPARKCOMPUTERESOURCES._serialized_end=1263
+  _CLIENTPODCOMPUTERESOURCES._serialized_start=1266
+  _CLIENTPODCOMPUTERESOURCES._serialized_end=1627
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -97,43 +97,14 @@
 
 NODE_OPTIMIZATION_INVALID: NodeOptimizationType.ValueType  # 0
 NODE_OPTIMIZATION_NONE: NodeOptimizationType.ValueType  # 1
 NODE_OPTIMIZATION_CPU: NodeOptimizationType.ValueType  # 2
 NODE_OPTIMIZATION_MEMORY: NodeOptimizationType.ValueType  # 3
 global___NodeOptimizationType = NodeOptimizationType
 
-class _PodComputeResourceTemplate:
-    ValueType = typing.NewType("ValueType", builtins.int)
-    V: typing_extensions.TypeAlias = ValueType
-
-class _PodComputeResourceTemplateEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_PodComputeResourceTemplate.ValueType], builtins.type):  # noqa: F821
-    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-    POD_COMPUTE_RESOURCE_INVALID: _PodComputeResourceTemplate.ValueType  # 0
-    POD_COMPUTE_RESOURCE_SMALL: _PodComputeResourceTemplate.ValueType  # 1
-    POD_COMPUTE_RESOURCE_MEDIUM: _PodComputeResourceTemplate.ValueType  # 2
-    POD_COMPUTE_RESOURCE_LARGE: _PodComputeResourceTemplate.ValueType  # 3
-    POD_COMPUTE_RESOURCE_XL: _PodComputeResourceTemplate.ValueType  # 4
-    POD_COMPUTE_RESOURCE_2XL: _PodComputeResourceTemplate.ValueType  # 5
-    POD_COMPUTE_RESOURCE_3XL: _PodComputeResourceTemplate.ValueType  # 6
-    POD_COMPUTE_RESOURCE_4XL: _PodComputeResourceTemplate.ValueType  # 7
-    POD_COMPUTE_RESOURCE_5XL: _PodComputeResourceTemplate.ValueType  # 8
-
-class PodComputeResourceTemplate(_PodComputeResourceTemplate, metaclass=_PodComputeResourceTemplateEnumTypeWrapper): ...
-
-POD_COMPUTE_RESOURCE_INVALID: PodComputeResourceTemplate.ValueType  # 0
-POD_COMPUTE_RESOURCE_SMALL: PodComputeResourceTemplate.ValueType  # 1
-POD_COMPUTE_RESOURCE_MEDIUM: PodComputeResourceTemplate.ValueType  # 2
-POD_COMPUTE_RESOURCE_LARGE: PodComputeResourceTemplate.ValueType  # 3
-POD_COMPUTE_RESOURCE_XL: PodComputeResourceTemplate.ValueType  # 4
-POD_COMPUTE_RESOURCE_2XL: PodComputeResourceTemplate.ValueType  # 5
-POD_COMPUTE_RESOURCE_3XL: PodComputeResourceTemplate.ValueType  # 6
-POD_COMPUTE_RESOURCE_4XL: PodComputeResourceTemplate.ValueType  # 7
-POD_COMPUTE_RESOURCE_5XL: PodComputeResourceTemplate.ValueType  # 8
-global___PodComputeResourceTemplate = PodComputeResourceTemplate
-
 class CpuResources(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CPU_FIELD_NUMBER: builtins.int
     MEMORY_AMOUNT_FIELD_NUMBER: builtins.int
     MEMORY_UNITS_FIELD_NUMBER: builtins.int
     cpu: builtins.float
@@ -224,22 +195,22 @@
     def ClearField(self, field_name: typing_extensions.Literal["driver_cores", b"driver_cores", "driver_memory", b"driver_memory", "executor_cores", b"executor_cores", "executor_memory", b"executor_memory", "initial_executors", b"initial_executors", "max_executors", b"max_executors", "min_executors", b"min_executors"]) -> None: ...
 
 global___SparkResourceConfiguration = SparkResourceConfiguration
 
 class PodComputeResourceTemplateSpec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TEMPLATE_FIELD_NUMBER: builtins.int
-    template: global___PodComputeResourceTemplate.ValueType
+    TEMPLATE_ID_FIELD_NUMBER: builtins.int
+    template_id: builtins.str
     def __init__(
         self,
         *,
-        template: global___PodComputeResourceTemplate.ValueType = ...,
+        template_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["template", b"template"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["template_id", b"template_id"]) -> None: ...
 
 global___PodComputeResourceTemplateSpec = PodComputeResourceTemplateSpec
 
 class PodComputeResources(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OPTIMIZATION_TYPE_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.77/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.77/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/pyproject.toml` & `qwak_core-0.0.77/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.76"
+version = "0.0.77"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.76/qwak/automations/__init__.py` & `qwak_core-0.0.77/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/automations/automation_executions.py` & `qwak_core-0.0.77/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/automations/automations.py` & `qwak_core-0.0.77/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.77/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.77/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/automations/common.py` & `qwak_core-0.0.77/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.77/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.77/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.77/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.77/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.77/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/alert_management/client.py` & `qwak_core-0.0.77/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/analytics/client.py` & `qwak_core-0.0.77/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/audience/client.py` & `qwak_core-0.0.77/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/automation_management/client.py` & `qwak_core-0.0.77/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.77/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.77/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.77/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.77/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/build_management/client.py` & `qwak_core-0.0.77/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.77/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.77/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/deployment/client.py` & `qwak_core-0.0.77/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.77/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.77/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.77/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.77/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/instance_template/client.py` & `qwak_core-0.0.77/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.77/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/logging_client/client.py` & `qwak_core-0.0.77/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/model_management/client.py` & `qwak_core-0.0.77/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/project/client.py` & `qwak_core-0.0.77/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/secret_service/client.py` & `qwak_core-0.0.77/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.77/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.77/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.77/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.77/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.77/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.77/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.77/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.77/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.77/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.77/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.77/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.77/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.77/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.77/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.77/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/offline/client.py` & `qwak_core-0.0.77/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/feature_store/online/client.py` & `qwak_core-0.0.77/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/const.py` & `qwak_core-0.0.77/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.77/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.77/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.77/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.77/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/singleton_meta.py` & `qwak_core-0.0.77/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/tool/auth.py` & `qwak_core-0.0.77/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.77/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.77/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.77/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.77/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/adapters/__init__.py` & `qwak_core-0.0.77/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.77/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.77/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.77/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.77/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.77/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/base.py` & `qwak_core-0.0.77/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/decorators/api.py` & `qwak_core-0.0.77/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.77/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/experiment_tracking.py` & `qwak_core-0.0.77/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/schema.py` & `qwak_core-0.0.77/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/schema_entities.py` & `qwak_core-0.0.77/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.77/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.77/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.77/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.77/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.77/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.77/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.77/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.77/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/client.py` & `qwak_core-0.0.77/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.77/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/models/model.py` & `qwak_core-0.0.77/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.77/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.77/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/tools/logger/logger.py` & `qwak_core-0.0.77/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak/tools/logger/logging.yml` & `qwak_core-0.0.77/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.77/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/qwak_services_mock/services_mock.py` & `qwak_core-0.0.77/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.76/setup.py` & `qwak_core-0.0.77/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.76',
+    'version': '0.0.77',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.76/PKG-INFO` & `qwak_core-0.0.77/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.76
+Version: 0.0.77
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

