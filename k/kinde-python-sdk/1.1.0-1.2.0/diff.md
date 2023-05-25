# Comparing `tmp/kinde-python-sdk-1.1.0.tar.gz` & `tmp/kinde-python-sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinde-python-sdk-1.1.0.tar", last modified: Wed Apr 12 02:14:07 2023, max compression
+gzip compressed data, was "kinde-python-sdk-1.2.0.tar", last modified: Thu May 25 05:25:32 2023, max compression
```

## Comparing `kinde-python-sdk-1.1.0.tar` & `kinde-python-sdk-1.2.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.413782 kinde-python-sdk-1.1.0/
--rw-r--r--   0 rai        (501) staff       (20)     1385 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/LICENSE
--rw-r--r--   0 rai        (501) staff       (20)    15849 2023-04-12 02:14:07.413317 kinde-python-sdk-1.1.0/PKG-INFO
--rw-r--r--   0 rai        (501) staff       (20)    15142 2023-04-12 01:44:00.000000 kinde-python-sdk-1.1.0/README.md
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.375890 kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/
--rw-r--r--   0 rai        (501) staff       (20)    15849 2023-04-12 02:14:07.000000 kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 rai        (501) staff       (20)     5976 2023-04-12 02:14:07.000000 kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 rai        (501) staff       (20)        1 2023-04-12 02:14:07.000000 kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 rai        (501) staff       (20)      147 2023-04-12 02:14:07.000000 kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/requires.txt
--rw-r--r--   0 rai        (501) staff       (20)       10 2023-04-12 02:14:07.000000 kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.378714 kinde-python-sdk-1.1.0/kinde_sdk/
--rw-r--r--   0 rai        (501) staff       (20)      726 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    58495 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/api_client.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.379852 kinde-python-sdk-1.1.0/kinde_sdk/apis/
--rw-r--r--   0 rai        (501) staff       (20)      214 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     4009 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/path_to_api.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.383710 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/
--rw-r--r--   0 rai        (501) staff       (20)      236 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)      135 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_connected_apps_auth_url.py
--rw-r--r--   0 rai        (501) staff       (20)      135 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_connected_apps_revoke.py
--rw-r--r--   0 rai        (501) staff       (20)      130 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_connected_apps_token.py
--rw-r--r--   0 rai        (501) staff       (20)      150 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_environment_feature_flags_.py
--rw-r--r--   0 rai        (501) staff       (20)      293 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_environment_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      120 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_feature_flags.py
--rw-r--r--   0 rai        (501) staff       (20)      252 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      196 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_organization.py
--rw-r--r--   0 rai        (501) staff       (20)      302 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_organization_users.py
--rw-r--r--   0 rai        (501) staff       (20)      118 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_organizations.py
--rw-r--r--   0 rai        (501) staff       (20)      169 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags.py
--rw-r--r--   0 rai        (501) staff       (20)      324 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      325 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_user.py
--rw-r--r--   0 rai        (501) staff       (20)      102 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/api_v1_users.py
--rw-r--r--   0 rai        (501) staff       (20)      116 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/oauth2_user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)      121 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/paths/oauth2_v2_user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)     1090 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tag_to_api.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.385046 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/
--rw-r--r--   0 rai        (501) staff       (20)      466 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)      767 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/connected_apps_api.py
--rw-r--r--   0 rai        (501) staff       (20)      913 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/environments_api.py
--rw-r--r--   0 rai        (501) staff       (20)      750 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/feature_flags_api.py
--rw-r--r--   0 rai        (501) staff       (20)      590 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/o_auth_api.py
--rw-r--r--   0 rai        (501) staff       (20)     1547 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/organizations_api.py
--rw-r--r--   0 rai        (501) staff       (20)     1107 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/users_api.py
--rw-r--r--   0 rai        (501) staff       (20)    15765 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/configuration.py
--rw-r--r--   0 rai        (501) staff       (20)     4684 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/exceptions.py
--rw-r--r--   0 rai        (501) staff       (20)     7911 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/kinde_api_client.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.390929 kinde-python-sdk-1.1.0/kinde_sdk/model/
--rw-r--r--   0 rai        (501) staff       (20)      343 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     4320 2023-04-12 01:28:05.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/add_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     2410 2023-04-12 01:28:05.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/api_result.py
--rw-r--r--   0 rai        (501) staff       (20)     3192 2023-04-12 01:28:05.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/connected_apps_access_token.py
--rw-r--r--   0 rai        (501) staff       (20)     2950 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/connected_apps_auth_url.py
--rw-r--r--   0 rai        (501) staff       (20)     4393 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/create_user_response.py
--rw-r--r--   0 rai        (501) staff       (20)     2894 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/error.py
--rw-r--r--   0 rai        (501) staff       (20)     3304 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/error_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5027 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/get_organizations_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5136 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/get_organizations_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     3428 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/organization.py
--rw-r--r--   0 rai        (501) staff       (20)     4509 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/organization_user.py
--rw-r--r--   0 rai        (501) staff       (20)     1428 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/organization_users.py
--rw-r--r--   0 rai        (501) staff       (20)     1391 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/organizations.py
--rw-r--r--   0 rai        (501) staff       (20)     3847 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/remove_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     2914 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/success_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5646 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/user.py
--rw-r--r--   0 rai        (501) staff       (20)     5883 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/user_identity.py
--rw-r--r--   0 rai        (501) staff       (20)     5261 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)     6214 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/user_profile_v2.py
--rw-r--r--   0 rai        (501) staff       (20)     1340 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/users.py
--rw-r--r--   0 rai        (501) staff       (20)     4837 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/model/users_response.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.391279 kinde-python-sdk-1.1.0/kinde_sdk/models/
--rw-r--r--   0 rai        (501) staff       (20)     1706 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/models/__init__.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.391478 kinde-python-sdk-1.1.0/kinde_sdk/paths/
--rw-r--r--   0 rai        (501) staff       (20)     1381 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/__init__.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.392066 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/
--rw-r--r--   0 rai        (501) staff       (20)      337 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    10986 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.392522 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_revoke/
--rw-r--r--   0 rai        (501) staff       (20)      333 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_revoke/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12670 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.393010 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_token/
--rw-r--r--   0 rai        (501) staff       (20)      331 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_token/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    10943 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_token/get.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.393428 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_/
--rw-r--r--   0 rai        (501) staff       (20)      343 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     9503 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_/delete.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.394208 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      375 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11529 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    13689 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.394759 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags/
--rw-r--r--   0 rai        (501) staff       (20)      317 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13704 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags/post.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.395450 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      351 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11270 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    15736 2023-04-12 01:28:08.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.396227 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization/
--rw-r--r--   0 rai        (501) staff       (20)      315 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11300 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization/get.py
--rw-r--r--   0 rai        (501) staff       (20)    17779 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization/post.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.397637 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/
--rw-r--r--   0 rai        (501) staff       (20)      327 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    14378 2023-04-12 01:28:11.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/get.py
--rw-r--r--   0 rai        (501) staff       (20)    18695 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    19176 2023-04-12 01:28:11.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/post.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.398088 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations/
--rw-r--r--   0 rai        (501) staff       (20)      317 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12879 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations/get.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.398580 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/
--rw-r--r--   0 rai        (501) staff       (20)      363 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11493 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.399433 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      397 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11817 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    13977 2023-04-12 01:28:10.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.400803 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/
--rw-r--r--   0 rai        (501) staff       (20)      299 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11247 2023-04-12 01:28:11.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11221 2023-04-12 01:28:11.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/get.py
--rw-r--r--   0 rai        (501) staff       (20)    18473 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    26292 2023-04-12 01:28:11.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/post.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.401274 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_users/
--rw-r--r--   0 rai        (501) staff       (20)      301 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_users/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13397 2023-04-12 01:28:11.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_users/get.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.401880 kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_user_profile/
--rw-r--r--   0 rai        (501) staff       (20)      315 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_user_profile/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     7957 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_user_profile/get.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.402318 kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_v2_user_profile/
--rw-r--r--   0 rai        (501) staff       (20)      321 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_v2_user_profile/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     8083 2023-04-12 01:28:09.000000 kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_v2_user_profile/get.py
--rw-r--r--   0 rai        (501) staff       (20)    10552 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/rest.py
--rw-r--r--   0 rai        (501) staff       (20)    97655 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/schemas.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.402703 kinde-python-sdk-1.1.0/kinde_sdk/test/
--rw-r--r--   0 rai        (501) staff       (20)        0 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     9003 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_kinde_api_client.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-04-12 02:14:07.412884 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/
--rw-r--r--   0 rai        (501) staff       (20)        0 2023-04-12 01:28:12.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)      620 2023-04-12 01:28:05.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_add_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      543 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_api_result.py
--rw-r--r--   0 rai        (501) staff       (20)      605 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_connected_apps_access_token.py
--rw-r--r--   0 rai        (501) staff       (20)      589 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_connected_apps_auth_url.py
--rw-r--r--   0 rai        (501) staff       (20)      579 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_create_user_response.py
--rw-r--r--   0 rai        (501) staff       (20)      526 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_error.py
--rw-r--r--   0 rai        (501) staff       (20)      559 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_error_response.py
--rw-r--r--   0 rai        (501) staff       (20)      603 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_get_organizations_response.py
--rw-r--r--   0 rai        (501) staff       (20)      624 2023-04-12 01:28:06.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_get_organizations_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      554 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_organization.py
--rw-r--r--   0 rai        (501) staff       (20)      571 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_organization_user.py
--rw-r--r--   0 rai        (501) staff       (20)      575 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_organization_users.py
--rw-r--r--   0 rai        (501) staff       (20)      558 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_organizations.py
--rw-r--r--   0 rai        (501) staff       (20)      632 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_remove_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      567 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_success_response.py
--rw-r--r--   0 rai        (501) staff       (20)      522 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_user.py
--rw-r--r--   0 rai        (501) staff       (20)      555 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_user_identity.py
--rw-r--r--   0 rai        (501) staff       (20)      551 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)      560 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_user_profile_v2.py
--rw-r--r--   0 rai        (501) staff       (20)      526 2023-03-30 23:40:23.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_users.py
--rw-r--r--   0 rai        (501) staff       (20)      558 2023-04-12 01:28:07.000000 kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     1000 2023-04-12 02:12:02.000000 kinde-python-sdk-1.1.0/pyproject.toml
--rw-r--r--   0 rai        (501) staff       (20)       38 2023-04-12 02:14:07.413838 kinde-python-sdk-1.1.0/setup.cfg
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.702093 kinde-python-sdk-1.2.0/
+-rw-r--r--   0 rai        (501) staff       (20)     1385 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/LICENSE
+-rw-r--r--   0 rai        (501) staff       (20)    21746 2023-05-25 05:25:32.701923 kinde-python-sdk-1.2.0/PKG-INFO
+-rw-r--r--   0 rai        (501) staff       (20)    21040 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/README.md
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.671037 kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/
+-rw-r--r--   0 rai        (501) staff       (20)    21746 2023-05-25 05:25:32.000000 kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 rai        (501) staff       (20)     5976 2023-05-25 05:25:32.000000 kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 rai        (501) staff       (20)        1 2023-05-25 05:25:32.000000 kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 rai        (501) staff       (20)      147 2023-05-25 05:25:32.000000 kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 rai        (501) staff       (20)       10 2023-05-25 05:25:32.000000 kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.673430 kinde-python-sdk-1.2.0/kinde_sdk/
+-rw-r--r--   0 rai        (501) staff       (20)      726 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    58495 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/api_client.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.674237 kinde-python-sdk-1.2.0/kinde_sdk/apis/
+-rw-r--r--   0 rai        (501) staff       (20)      214 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     4009 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/path_to_api.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.677775 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/
+-rw-r--r--   0 rai        (501) staff       (20)      236 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)      135 2023-04-12 01:28:08.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_connected_apps_auth_url.py
+-rw-r--r--   0 rai        (501) staff       (20)      135 2023-04-12 01:28:08.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_connected_apps_revoke.py
+-rw-r--r--   0 rai        (501) staff       (20)      130 2023-04-12 01:28:08.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_connected_apps_token.py
+-rw-r--r--   0 rai        (501) staff       (20)      150 2023-04-12 01:28:08.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_environment_feature_flags_.py
+-rw-r--r--   0 rai        (501) staff       (20)      293 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_environment_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      120 2023-04-12 01:28:09.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_feature_flags.py
+-rw-r--r--   0 rai        (501) staff       (20)      252 2023-04-12 01:28:09.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      196 2023-04-12 01:28:10.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_organization.py
+-rw-r--r--   0 rai        (501) staff       (20)      302 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_organization_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      118 2023-04-12 01:28:10.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_organizations.py
+-rw-r--r--   0 rai        (501) staff       (20)      169 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags.py
+-rw-r--r--   0 rai        (501) staff       (20)      324 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      325 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_user.py
+-rw-r--r--   0 rai        (501) staff       (20)      102 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/api_v1_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      116 2023-04-12 01:28:09.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/oauth2_user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)      121 2023-04-12 01:28:09.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/paths/oauth2_v2_user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)     1090 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tag_to_api.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.678896 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/
+-rw-r--r--   0 rai        (501) staff       (20)      466 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)      767 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/connected_apps_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      913 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/environments_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      750 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/feature_flags_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      590 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/o_auth_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     1547 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/organizations_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     1107 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/users_api.py
+-rw-r--r--   0 rai        (501) staff       (20)    15765 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/configuration.py
+-rw-r--r--   0 rai        (501) staff       (20)     4736 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/exceptions.py
+-rw-r--r--   0 rai        (501) staff       (20)    10447 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/kinde_api_client.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.685789 kinde-python-sdk-1.2.0/kinde_sdk/model/
+-rw-r--r--   0 rai        (501) staff       (20)      343 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     4320 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/add_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     2410 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/api_result.py
+-rw-r--r--   0 rai        (501) staff       (20)     3192 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/connected_apps_access_token.py
+-rw-r--r--   0 rai        (501) staff       (20)     2950 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/connected_apps_auth_url.py
+-rw-r--r--   0 rai        (501) staff       (20)     4393 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/create_user_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     2894 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/error.py
+-rw-r--r--   0 rai        (501) staff       (20)     3304 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/error_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5027 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/get_organizations_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5136 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/get_organizations_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     3428 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/organization.py
+-rw-r--r--   0 rai        (501) staff       (20)     4509 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/organization_user.py
+-rw-r--r--   0 rai        (501) staff       (20)     1428 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/organization_users.py
+-rw-r--r--   0 rai        (501) staff       (20)     1391 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/organizations.py
+-rw-r--r--   0 rai        (501) staff       (20)     3847 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/remove_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     2914 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/success_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5646 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/user.py
+-rw-r--r--   0 rai        (501) staff       (20)     5883 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/user_identity.py
+-rw-r--r--   0 rai        (501) staff       (20)     5261 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)     6680 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/user_profile_v2.py
+-rw-r--r--   0 rai        (501) staff       (20)     1340 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/users.py
+-rw-r--r--   0 rai        (501) staff       (20)     4837 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/model/users_response.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.686062 kinde-python-sdk-1.2.0/kinde_sdk/models/
+-rw-r--r--   0 rai        (501) staff       (20)     1706 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/models/__init__.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.686256 kinde-python-sdk-1.2.0/kinde_sdk/paths/
+-rw-r--r--   0 rai        (501) staff       (20)     1381 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/__init__.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.686886 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/
+-rw-r--r--   0 rai        (501) staff       (20)      337 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12604 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.687454 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_revoke/
+-rw-r--r--   0 rai        (501) staff       (20)      333 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_revoke/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12284 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.688049 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_token/
+-rw-r--r--   0 rai        (501) staff       (20)      331 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_token/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11982 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_token/get.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.688627 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_/
+-rw-r--r--   0 rai        (501) staff       (20)      343 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     9503 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_/delete.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.689395 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      375 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11529 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    13689 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.690046 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags/
+-rw-r--r--   0 rai        (501) staff       (20)      317 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13704 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags/post.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.690642 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      351 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11270 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    15736 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.691383 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization/
+-rw-r--r--   0 rai        (501) staff       (20)      315 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11300 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    17779 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization/post.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.692509 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/
+-rw-r--r--   0 rai        (501) staff       (20)      327 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    14378 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    18695 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    19176 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/post.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.693075 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations/
+-rw-r--r--   0 rai        (501) staff       (20)      317 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12879 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations/get.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.693476 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/
+-rw-r--r--   0 rai        (501) staff       (20)      363 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11493 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.694094 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      397 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11817 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    13977 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.695272 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/
+-rw-r--r--   0 rai        (501) staff       (20)      299 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11247 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11221 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    18473 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    26292 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/post.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.695692 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_users/
+-rw-r--r--   0 rai        (501) staff       (20)      301 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_users/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13397 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_users/get.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.696228 kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_user_profile/
+-rw-r--r--   0 rai        (501) staff       (20)      315 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_user_profile/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     7957 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_user_profile/get.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.696606 kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_v2_user_profile/
+-rw-r--r--   0 rai        (501) staff       (20)      321 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_v2_user_profile/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     8091 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_v2_user_profile/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    10552 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/rest.py
+-rw-r--r--   0 rai        (501) staff       (20)    97655 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/schemas.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.697034 kinde-python-sdk-1.2.0/kinde_sdk/test/
+-rw-r--r--   0 rai        (501) staff       (20)        0 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    60776 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_kinde_api_client.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2023-05-25 05:25:32.701614 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/
+-rw-r--r--   0 rai        (501) staff       (20)        0 2023-04-12 01:28:12.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     1017 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_add_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      844 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_api_result.py
+-rw-r--r--   0 rai        (501) staff       (20)      995 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_connected_apps_access_token.py
+-rw-r--r--   0 rai        (501) staff       (20)      905 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_connected_apps_auth_url.py
+-rw-r--r--   0 rai        (501) staff       (20)      886 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_create_user_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      801 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_error.py
+-rw-r--r--   0 rai        (501) staff       (20)      943 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_error_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      942 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_get_organizations_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      974 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_get_organizations_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      850 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_organization.py
+-rw-r--r--   0 rai        (501) staff       (20)      866 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_organization_user.py
+-rw-r--r--   0 rai        (501) staff       (20)      575 2023-03-30 23:40:23.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_organization_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      558 2023-03-30 23:40:23.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_organizations.py
+-rw-r--r--   0 rai        (501) staff       (20)     1024 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_remove_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      907 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_success_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      780 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user.py
+-rw-r--r--   0 rai        (501) staff       (20)      852 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user_identity.py
+-rw-r--r--   0 rai        (501) staff       (20)      831 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)      847 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user_profile_v2.py
+-rw-r--r--   0 rai        (501) staff       (20)      526 2023-03-30 23:40:23.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      858 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     1000 2023-05-25 05:22:38.000000 kinde-python-sdk-1.2.0/pyproject.toml
+-rw-r--r--   0 rai        (501) staff       (20)       38 2023-05-25 05:25:32.702135 kinde-python-sdk-1.2.0/setup.cfg
```

### Comparing `kinde-python-sdk-1.1.0/LICENSE` & `kinde-python-sdk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_python_sdk.egg-info/SOURCES.txt` & `kinde-python-sdk-1.2.0/kinde_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/__init__.py` & `kinde-python-sdk-1.2.0/kinde_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Provides endpoints to manage your Kinde Businesses  # noqa: E501
 
     The version of the OpenAPI document: 1
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.0.0"
+__version__ = "1.2.0"
 
 # import ApiClient
 from kinde_sdk.api_client import ApiClient
 
 # import Configuration
 from kinde_sdk.configuration import Configuration
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/api_client.py` & `kinde-python-sdk-1.2.0/kinde_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/path_to_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tag_to_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/connected_apps_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/connected_apps_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/environments_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/environments_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/feature_flags_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/feature_flags_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/o_auth_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/o_auth_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/organizations_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/organizations_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/apis/tags/users_api.py` & `kinde-python-sdk-1.2.0/kinde_sdk/apis/tags/users_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/configuration.py` & `kinde-python-sdk-1.2.0/kinde_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/exceptions.py` & `kinde-python-sdk-1.2.0/kinde_sdk/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,7 +154,11 @@
 
 class KindeLoginException(Exception):
     pass
 
 
 class KindeTokenException(Exception):
     pass
+
+
+class KindeRetrieveException(Exception):
+    pass
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/kinde_api_client.py` & `kinde-python-sdk-1.2.0/kinde_sdk/kinde_api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 import jwt
 from authlib.integrations.requests_client import OAuth2Session
 from kinde_sdk.api_client import ApiClient
 from kinde_sdk.exceptions import (
     KindeConfigurationException,
     KindeLoginException,
     KindeTokenException,
+    KindeRetrieveException,
 )
+from kinde_sdk import __version__ as kinde_sdk_version
+
+
+class FlagType(Enum):
+    s = "string"
+    i = "integer"
+    b = "boolean"
 
 
 class GrantType(Enum):
     CLIENT_CREDENTIALS = "client_credentials"
     AUTHORIZATION_CODE = "authorization_code"
     AUTHORIZATION_CODE_WITH_PKCE = "authorization_code_with_pkce"
 
@@ -110,46 +118,86 @@
 
     def get_claim(self, key: str, token_name: str = "access_token") -> Any:
         if token_name not in self.TOKEN_NAMES:
             raise KindeTokenException(
                 f"Please use only tokens from the list: {self.TOKEN_NAMES}"
             )
         self._decode_token_if_needed(token_name)
-        return self.__decoded_tokens[token_name].get(key)
+        value = self.__decoded_tokens[token_name].get(key)
+        return {"name": key, "value": value}
 
     def get_permission(self, permission: str) -> Dict[str, Any]:
         return {
-            "org_code": self.get_claim("org_code"),
-            "is_granted": permission in self.get_claim("permissions"),
+            "org_code": self.get_claim("org_code")["value"],
+            "is_granted": permission in self.get_claim("permissions")["value"],
         }
 
     def get_permissions(self) -> Dict[str, Any]:
         return {
-            "org_code": self.get_claim("org_code"),
-            "permissions": self.get_claim("permissions"),
+            "org_code": self.get_claim("org_code")["value"],
+            "permissions": self.get_claim("permissions")["value"],
         }
 
     def get_organization(self) -> Dict[str, str]:
         return {
-            "org_code": self.get_claim("org_code"),
+            "org_code": self.get_claim("org_code")["value"],
         }
 
     def get_user_details(self) -> Dict[str, str]:
         return {
-            "id": self.get_claim("sub", "id_token"),
-            "given_name": self.get_claim("given_name", "id_token"),
-            "family_name": self.get_claim("family_name", "id_token"),
-            "email": self.get_claim("email", "id_token"),
+            "id": self.get_claim("sub", "id_token")["value"],
+            "given_name": self.get_claim("given_name", "id_token")["value"],
+            "family_name": self.get_claim("family_name", "id_token")["value"],
+            "email": self.get_claim("email", "id_token")["value"],
+            "picture": self.get_claim("picture", "id_token")["value"],
         }
 
     def get_user_organizations(self) -> Dict[str, List[str]]:
         return {
-            "org_codes": self.get_claim("org_codes", "id_token"),
+            "org_codes": self.get_claim("org_codes", "id_token")["value"],
         }
 
+    def get_flag(
+        self, code: str, default_value: Any = None, flag_type: str = ""
+    ) -> Any:
+        flags = self.get_claim("feature_flags")["value"] or {}
+        flag = {}
+
+        if code not in list(flags.keys()):
+            if default_value is None:
+                raise KindeRetrieveException(
+                    f"Flag {code} was not found, and no default value has been provided"
+                )
+        else:
+            flag = flags[code]
+            if flag_type and flag.get("t") and flag_type != flag.get("t"):
+                raise KindeRetrieveException(
+                    f"Flag {code} is of type {FlagType[flag.get('t')].value} - requested type {FlagType[flag_type].value}"
+                )
+
+        result_flag = {
+            "code": code,
+            "value": flag.get("v") if flag else default_value,
+            "is_default": not bool(flag),
+        }
+        flag_type = flag["t"] if flag else flag_type
+        if flag_type:
+            result_flag["type"] = FlagType[flag_type].value
+
+        return result_flag
+
+    def get_boolean_flag(self, code: str, default_value: Any = None) -> bool:
+        return self.get_flag(code, default_value, "b")["value"]
+
+    def get_string_flag(self, code: str, default_value: Any = None) -> str:
+        return self.get_flag(code, default_value, "s")["value"]
+
+    def get_integer_flag(self, code: str, default_value: Any = None) -> int:
+        return self.get_flag(code, default_value, "i")["value"]
+
     def call_api(self, *args, **kwargs) -> Any:
         self._get_or_refresh_access_token()
         return super().call_api(*args, **kwargs)
 
     def _clear_decoded_tokens(self) -> None:
         self.__decoded_tokens = {}
 
@@ -158,14 +206,15 @@
             if not self.__access_token_obj:
                 raise KindeTokenException(
                     "Access token doesn't exist.\n"
                     "When grant_type is CLIENT_CREDENTIALS use fetch_token().\n"
                     'For other grant_type use "get_login_url()" or "get_register_url()".'
                 )
             token = self.__access_token_obj.get(token_name)
+
             if token:
                 self.__decoded_tokens[token_name] = jwt.decode(
                     token, options={"verify_signature": False}
                 )
             else:
                 raise KindeTokenException(f"Token {token_name} doesn't exist.")
 
@@ -178,15 +227,23 @@
             if authorization_response is None:
                 raise KindeConfigurationException(
                     '"authorization_response" parameter is required when grant_type is different than CLIENT_CREDENTIALS.'
                 )
             params = {"authorization_response": authorization_response}
         if self.grant_type == GrantType.AUTHORIZATION_CODE_WITH_PKCE:
             params["code_verifier"] = self.code_verifier
-        self.__access_token_obj = self.client.fetch_token(self.token_endpoint, **params)
+
+        self.__access_token_obj = self.client.fetch_token(
+            self.token_endpoint,
+            headers={
+                "Content-Type": "application/x-www-form-urlencoded",
+                "Kinde-SDK": "/".join(("Python", kinde_sdk_version)),
+            },
+            **params,
+        )
         self.configuration.access_token = self.__access_token_obj.get("access_token")
         self._clear_decoded_tokens()
 
     def _get_or_refresh_access_token(self) -> None:
         if self.grant_type == GrantType.CLIENT_CREDENTIALS:
             if not self.__access_token_obj or self.__access_token_obj.is_expired():
                 self.fetch_token()
@@ -196,16 +253,28 @@
                     'Please use "get_login_url()" or "get_register_url()" first.'
                 )
             if self.__access_token_obj.is_expired():
                 self._refresh_token()
 
     def _refresh_token(self) -> None:
         refresh_token = self.__access_token_obj.get("refresh_token")
+
         if refresh_token:
             self.__access_token_obj = self.client.refresh_token(
                 self.token_endpoint,
+                headers={
+                    "Content-Type": "application/x-www-form-urlencoded",
+                    "Kinde-SDK": "/".join(("Python", kinde_sdk_version)),
+                },
                 refresh_token=refresh_token,
             )
+            if not self.__access_token_obj:
+                raise KindeTokenException(
+                    '"Access token" and "Refresh token" are invalid.'
+                )
+
             self.configuration.access_token = self.__access_token_obj.get(
                 "access_token"
             )
-            self._clear_decoded_tokens()
+            self._clear_decoded_tokens()
+        else:
+            raise KindeTokenException('"Access token" and "Refresh token" are invalid.')
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/add_organization_users_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/add_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/api_result.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/api_result.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/connected_apps_access_token.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/connected_apps_access_token.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/connected_apps_auth_url.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/connected_apps_auth_url.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/create_user_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/create_user_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/error.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/error_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/error_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/get_organizations_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/get_organizations_users_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/get_organizations_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/organization.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/organization.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/organization_user.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/organization_user.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/organization_users.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/organization_users.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/organizations.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/organizations.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/remove_organization_users_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/remove_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/success_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/success_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/user.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/user.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/user_identity.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/user_identity.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/user_profile.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/user_profile.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/user_profile_v2.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/user_profile_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     """
 
 
     class MetaOapg:
         
         class properties:
             id = schemas.StrSchema
+            sub = schemas.StrSchema
             
             
             class provided_id(
                 schemas.StrBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneStrMixin
@@ -61,26 +62,30 @@
             name = schemas.StrSchema
             given_name = schemas.StrSchema
             family_name = schemas.StrSchema
             updated_at = schemas.IntSchema
             email = schemas.StrSchema
             __annotations__ = {
                 "id": id,
+                "sub": sub,
                 "provided_id": provided_id,
                 "name": name,
                 "given_name": given_name,
                 "family_name": family_name,
                 "updated_at": updated_at,
                 "email": email,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["sub"]) -> MetaOapg.properties.sub: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provided_id"]) -> MetaOapg.properties.provided_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["given_name"]) -> MetaOapg.properties.given_name: ...
@@ -93,23 +98,26 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "provided_id", "name", "given_name", "family_name", "updated_at", "email", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "sub", "provided_id", "name", "given_name", "family_name", "updated_at", "email", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["sub"]) -> typing.Union[MetaOapg.properties.sub, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provided_id"]) -> typing.Union[MetaOapg.properties.provided_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["given_name"]) -> typing.Union[MetaOapg.properties.given_name, schemas.Unset]: ...
@@ -122,35 +130,37 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["email"]) -> typing.Union[MetaOapg.properties.email, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "provided_id", "name", "given_name", "family_name", "updated_at", "email", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "sub", "provided_id", "name", "given_name", "family_name", "updated_at", "email", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
+        sub: typing.Union[MetaOapg.properties.sub, str, schemas.Unset] = schemas.unset,
         provided_id: typing.Union[MetaOapg.properties.provided_id, None, str, schemas.Unset] = schemas.unset,
         name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
         given_name: typing.Union[MetaOapg.properties.given_name, str, schemas.Unset] = schemas.unset,
         family_name: typing.Union[MetaOapg.properties.family_name, str, schemas.Unset] = schemas.unset,
         updated_at: typing.Union[MetaOapg.properties.updated_at, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         email: typing.Union[MetaOapg.properties.email, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'UserProfileV2':
         return super().__new__(
             cls,
             *_args,
             id=id,
+            sub=sub,
             provided_id=provided_id,
             name=name,
             given_name=given_name,
             family_name=family_name,
             updated_at=updated_at,
             email=email,
             _configuration=_configuration,
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/users.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/users.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/model/users_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/model/users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/models/__init__.py` & `kinde-python-sdk-1.2.0/kinde_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/__init__.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,59 +21,50 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from kinde_sdk import schemas  # noqa: F401
 
-from kinde_sdk.model.connected_apps_auth_url import ConnectedAppsAuthUrl
+from kinde_sdk.model.user import User
+from kinde_sdk.model.error_response import ErrorResponse
 
 from . import path
 
 # Query params
-KeyCodeRefSchema = schemas.StrSchema
-UserIdSchema = schemas.IntSchema
+IdSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'key_code_ref': typing.Union[KeyCodeRefSchema, str, ],
-        'user_id': typing.Union[UserIdSchema, decimal.Decimal, int, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
+        'id': typing.Union[IdSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_key_code_ref = api_client.QueryParameter(
-    name="key_code_ref",
+request_query_id = api_client.QueryParameter(
+    name="id",
     style=api_client.ParameterStyle.FORM,
-    schema=KeyCodeRefSchema,
-    required=True,
-    explode=True,
-)
-request_query_user_id = api_client.QueryParameter(
-    name="user_id",
-    style=api_client.ParameterStyle.FORM,
-    schema=UserIdSchema,
-    required=True,
+    schema=IdSchema,
     explode=True,
 )
 _auth = [
     'kindeBearerAuth',
 ]
-SchemaFor200ResponseBodyApplicationJson = ConnectedAppsAuthUrl
-SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ConnectedAppsAuthUrl
+SchemaFor200ResponseBodyApplicationJson = User
+SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -87,93 +78,116 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
     },
 )
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor400(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJsonCharsetutf8,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJson),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJsonCharsetutf8),
+    },
+)
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
 )
 _status_code_to_response = {
     '200': _response_for_200,
+    '400': _response_for_400,
     '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_connected_app_auth_url_oapg(
+    def _get_user_data_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_connected_app_auth_url_oapg(
+    def _get_user_data_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_connected_app_auth_url_oapg(
+    def _get_user_data_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_connected_app_auth_url_oapg(
+    def _get_user_data_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get Connected App URL
+        Get User
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_key_code_ref,
-            request_query_user_id,
+            request_query_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -210,61 +224,61 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetConnectedAppAuthUrl(BaseApi):
+class GetUserData(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_connected_app_auth_url(
+    def get_user_data(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_connected_app_auth_url(
+    def get_user_data(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_connected_app_auth_url(
+    def get_user_data(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_connected_app_auth_url(
+    def get_user_data(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_connected_app_auth_url_oapg(
+        return self._get_user_data_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
@@ -311,15 +325,15 @@
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_connected_app_auth_url_oapg(
+        return self._get_user_data_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,50 +21,50 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from kinde_sdk import schemas  # noqa: F401
 
-from kinde_sdk.model.api_result import ApiResult
+from kinde_sdk.model.success_response import SuccessResponse
+from kinde_sdk.model.error_response import ErrorResponse
 
 from . import path
 
 # Query params
-SessionIdSchema = schemas.StrSchema
+IdSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'session_id': typing.Union[SessionIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
+        'id': typing.Union[IdSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_session_id = api_client.QueryParameter(
-    name="session_id",
+request_query_id = api_client.QueryParameter(
+    name="id",
     style=api_client.ParameterStyle.FORM,
-    schema=SessionIdSchema,
-    required=True,
+    schema=IdSchema,
     explode=True,
 )
 _auth = [
     'kindeBearerAuth',
 ]
-SchemaFor200ResponseBodyApplicationJson = ApiResult
-SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ApiResult
+SchemaFor200ResponseBodyApplicationJson = SuccessResponse
+SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = SuccessResponse
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -78,16 +78,16 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ApiResult
-SchemaFor400ResponseBodyApplicationJsonCharsetutf8 = ApiResult
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor400ResponseBodyApplicationJson,
@@ -101,128 +101,93 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJsonCharsetutf8),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ApiResult
-SchemaFor403ResponseBodyApplicationJsonCharsetutf8 = ApiResult
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-        SchemaFor403ResponseBodyApplicationJsonCharsetutf8,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-        'application/json; charset=utf-8': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJsonCharsetutf8),
-    },
-)
-SchemaFor405ResponseBodyApplicationJson = ApiResult
-SchemaFor405ResponseBodyApplicationJsonCharsetutf8 = ApiResult
-
-
-@dataclass
-class ApiResponseFor405(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor405ResponseBodyApplicationJson,
-        SchemaFor405ResponseBodyApplicationJsonCharsetutf8,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_405 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor405,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor405ResponseBodyApplicationJson),
-        'application/json; charset=utf-8': api_client.MediaType(
-            schema=SchemaFor405ResponseBodyApplicationJsonCharsetutf8),
-    },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '400': _response_for_400,
     '403': _response_for_403,
-    '405': _response_for_405,
 }
 _all_accept_content_types = (
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _revoke_connected_app_token_oapg(
+    def _deleteuser_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _revoke_connected_app_token_oapg(
+    def _deleteuser_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _revoke_connected_app_token_oapg(
+    def _deleteuser_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _revoke_connected_app_token_oapg(
+    def _deleteuser_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Revoke Connected App Token
+        Delete User
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_session_id,
+            request_query_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -233,15 +198,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='delete'.upper(),
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
@@ -259,116 +224,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class RevokeConnectedAppToken(BaseApi):
+class Deleteuser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def revoke_connected_app_token(
+    def deleteuser(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def revoke_connected_app_token(
+    def deleteuser(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def revoke_connected_app_token(
+    def deleteuser(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def revoke_connected_app_token(
+    def deleteuser(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._revoke_connected_app_token_oapg(
+        return self._deleteuser_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForpost(BaseApi):
+class ApiFordelete(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def post(
+    def delete(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def post(
+    def delete(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def post(
+    def delete(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def post(
+    def delete(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._revoke_connected_app_token_oapg(
+        return self._deleteuser_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_connected_apps_token/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization/get.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,50 +21,50 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from kinde_sdk import schemas  # noqa: F401
 
-from kinde_sdk.model.connected_apps_access_token import ConnectedAppsAccessToken
+from kinde_sdk.model.organization import Organization
+from kinde_sdk.model.error_response import ErrorResponse
 
 from . import path
 
 # Query params
-SessionIdSchema = schemas.StrSchema
+CodeSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'session_id': typing.Union[SessionIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
+        'code': typing.Union[CodeSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_session_id = api_client.QueryParameter(
-    name="session_id",
+request_query_code = api_client.QueryParameter(
+    name="code",
     style=api_client.ParameterStyle.FORM,
-    schema=SessionIdSchema,
-    required=True,
+    schema=CodeSchema,
     explode=True,
 )
 _auth = [
     'kindeBearerAuth',
 ]
-SchemaFor200ResponseBodyApplicationJson = ConnectedAppsAccessToken
-SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ConnectedAppsAccessToken
+SchemaFor200ResponseBodyApplicationJson = Organization
+SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = Organization
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -78,25 +78,36 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
     },
 )
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJsonCharsetutf8,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJson),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJsonCharsetutf8),
+    },
 )
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
@@ -115,68 +126,68 @@
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_connected_app_token_oapg(
+    def _get_organization_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_connected_app_token_oapg(
+    def _get_organization_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_connected_app_token_oapg(
+    def _get_organization_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_connected_app_token_oapg(
+    def _get_organization_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get Connected App Token
+        Get Organization
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_session_id,
+            request_query_code,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -213,61 +224,61 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetConnectedAppToken(BaseApi):
+class GetOrganization(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_connected_app_token(
+    def get_organization(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_connected_app_token(
+    def get_organization(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_connected_app_token(
+    def get_organization(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_connected_app_token(
+    def get_organization(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_connected_app_token_oapg(
+        return self._get_organization_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
@@ -314,15 +325,15 @@
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_connected_app_token_oapg(
+        return self._get_organization_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_/delete.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags/post.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,50 +21,51 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from kinde_sdk import schemas  # noqa: F401
 
-from kinde_sdk.model.organization import Organization
+from kinde_sdk.model.success_response import SuccessResponse
 from kinde_sdk.model.error_response import ErrorResponse
 
 from . import path
 
 # Query params
-CodeSchema = schemas.StrSchema
+SessionIdSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
+        'session_id': typing.Union[SessionIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
-        'code': typing.Union[CodeSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_code = api_client.QueryParameter(
-    name="code",
+request_query_session_id = api_client.QueryParameter(
+    name="session_id",
     style=api_client.ParameterStyle.FORM,
-    schema=CodeSchema,
+    schema=SessionIdSchema,
+    required=True,
     explode=True,
 )
 _auth = [
     'kindeBearerAuth',
 ]
-SchemaFor200ResponseBodyApplicationJson = Organization
-SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = Organization
+SchemaFor200ResponseBodyApplicationJson = SuccessResponse
+SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = SuccessResponse
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -101,93 +102,117 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJsonCharsetutf8),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJsonCharsetutf8,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJsonCharsetutf8),
+    },
+)
+
+
+@dataclass
+class ApiResponseFor405(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: schemas.Unset = schemas.unset
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_405 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor405,
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '400': _response_for_400,
     '403': _response_for_403,
+    '405': _response_for_405,
 }
 _all_accept_content_types = (
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_organization_oapg(
+    def _revoke_connected_app_token_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_organization_oapg(
+    def _revoke_connected_app_token_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_organization_oapg(
+    def _revoke_connected_app_token_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_organization_oapg(
+    def _revoke_connected_app_token_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get Organization
+        Revoke Connected App Token
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_code,
+            request_query_session_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -198,15 +223,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
@@ -224,116 +249,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetOrganization(BaseApi):
+class RevokeConnectedAppToken(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_organization(
+    def revoke_connected_app_token(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_organization(
+    def revoke_connected_app_token(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_organization(
+    def revoke_connected_app_token(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_organization(
+    def revoke_connected_app_token(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_organization_oapg(
+        return self._revoke_connected_app_token_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def post(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def post(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_organization_oapg(
+        return self._revoke_connected_app_token_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization/post.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/patch.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organization_users/post.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organization_users/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/delete.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_token/get.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,50 +21,51 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from kinde_sdk import schemas  # noqa: F401
 
-from kinde_sdk.model.success_response import SuccessResponse
+from kinde_sdk.model.connected_apps_access_token import ConnectedAppsAccessToken
 from kinde_sdk.model.error_response import ErrorResponse
 
 from . import path
 
 # Query params
-IdSchema = schemas.StrSchema
+SessionIdSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
+        'session_id': typing.Union[SessionIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
-        'id': typing.Union[IdSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_id = api_client.QueryParameter(
-    name="id",
+request_query_session_id = api_client.QueryParameter(
+    name="session_id",
     style=api_client.ParameterStyle.FORM,
-    schema=IdSchema,
+    schema=SessionIdSchema,
+    required=True,
     explode=True,
 )
 _auth = [
     'kindeBearerAuth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SuccessResponse
-SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = SuccessResponse
+SchemaFor200ResponseBodyApplicationJson = ConnectedAppsAccessToken
+SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ConnectedAppsAccessToken
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -101,93 +102,104 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJsonCharsetutf8),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJsonCharsetutf8,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJsonCharsetutf8),
+    },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '400': _response_for_400,
     '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _deleteuser_oapg(
+    def _get_connected_app_token_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _deleteuser_oapg(
+    def _get_connected_app_token_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _deleteuser_oapg(
+    def _get_connected_app_token_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _deleteuser_oapg(
+    def _get_connected_app_token_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Delete User
+        Get Connected App Token
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_id,
+            request_query_session_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -198,15 +210,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='delete'.upper(),
+            method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
@@ -224,116 +236,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class Deleteuser(BaseApi):
+class GetConnectedAppToken(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def deleteuser(
+    def get_connected_app_token(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def deleteuser(
+    def get_connected_app_token(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def deleteuser(
+    def get_connected_app_token(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def deleteuser(
+    def get_connected_app_token(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._deleteuser_oapg(
+        return self._get_connected_app_token_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiFordelete(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def delete(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete(
+    def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._deleteuser_oapg(
+        return self._get_connected_app_token_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,50 +21,60 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from kinde_sdk import schemas  # noqa: F401
 
-from kinde_sdk.model.user import User
+from kinde_sdk.model.connected_apps_auth_url import ConnectedAppsAuthUrl
 from kinde_sdk.model.error_response import ErrorResponse
 
 from . import path
 
 # Query params
-IdSchema = schemas.StrSchema
+KeyCodeRefSchema = schemas.StrSchema
+UserIdSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
+        'key_code_ref': typing.Union[KeyCodeRefSchema, str, ],
+        'user_id': typing.Union[UserIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
-        'id': typing.Union[IdSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_id = api_client.QueryParameter(
-    name="id",
+request_query_key_code_ref = api_client.QueryParameter(
+    name="key_code_ref",
     style=api_client.ParameterStyle.FORM,
-    schema=IdSchema,
+    schema=KeyCodeRefSchema,
+    required=True,
+    explode=True,
+)
+request_query_user_id = api_client.QueryParameter(
+    name="user_id",
+    style=api_client.ParameterStyle.FORM,
+    schema=UserIdSchema,
+    required=True,
     explode=True,
 )
 _auth = [
     'kindeBearerAuth',
 ]
-SchemaFor200ResponseBodyApplicationJson = User
-SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = ConnectedAppsAuthUrl
+SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = ConnectedAppsAuthUrl
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -101,14 +111,37 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
         'application/json; charset=utf-8': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJsonCharsetutf8),
     },
 )
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJsonCharsetutf8 = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor404(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJsonCharsetutf8,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJsonCharsetutf8),
+    },
+)
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
@@ -116,78 +149,80 @@
 
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '400': _response_for_400,
+    '404': _response_for_404,
     '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
     'application/json; charset=utf-8',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_user_data_oapg(
+    def _get_connected_app_auth_url_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_user_data_oapg(
+    def _get_connected_app_auth_url_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_user_data_oapg(
+    def _get_connected_app_auth_url_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_user_data_oapg(
+    def _get_connected_app_auth_url_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get User
+        Get Connected App URL
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_id,
+            request_query_key_code_ref,
+            request_query_user_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -224,61 +259,61 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetUserData(BaseApi):
+class GetConnectedAppAuthUrl(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_user_data(
+    def get_connected_app_auth_url(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_user_data(
+    def get_connected_app_auth_url(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_user_data(
+    def get_connected_app_auth_url(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_user_data(
+    def get_connected_app_auth_url(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_user_data_oapg(
+        return self._get_connected_app_auth_url_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
@@ -325,15 +360,15 @@
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_user_data_oapg(
+        return self._get_connected_app_auth_url_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/patch.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_user/post.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_user/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/api_v1_users/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/api_v1_users/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_user_profile/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_user_profile/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/paths/oauth2_v2_user_profile/get.py` & `kinde-python-sdk-1.2.0/kinde_sdk/paths/oauth2_v2_user_profile/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         if not 200 <= response.status <= 299:
             raise exceptions.ApiException(
                 status=response.status,
                 reason=response.reason,
                 api_response=api_response
             )
-
+        
         return api_response
 
 
 class GetUserProfileV2(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/rest.py` & `kinde-python-sdk-1.2.0/kinde_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/schemas.py` & `kinde-python-sdk-1.2.0/kinde_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_add_organization_users_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_organization_users.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
-from kinde_sdk.model.add_organization_users_response import AddOrganizationUsersResponse
+from kinde_sdk.model.organization_users import OrganizationUsers
 from kinde_sdk import configuration
 
 
-class TestAddOrganizationUsersResponse(unittest.TestCase):
-    """AddOrganizationUsersResponse unit test stubs"""
+class TestOrganizationUsers(unittest.TestCase):
+    """OrganizationUsers unit test stubs"""
+
     _configuration = configuration.Configuration()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_api_result.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_users.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
-from kinde_sdk.model.api_result import ApiResult
+from kinde_sdk.model.users import Users
 from kinde_sdk import configuration
 
 
-class TestApiResult(unittest.TestCase):
-    """ApiResult unit test stubs"""
+class TestUsers(unittest.TestCase):
+    """Users unit test stubs"""
 
     _configuration = configuration.Configuration()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_create_user_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user_identity.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,29 @@
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
-from kinde_sdk.model.create_user_response import CreateUserResponse
-from kinde_sdk import configuration
+from kinde_sdk.model.user_identity import UserIdentity
+from kinde_sdk import schemas
 
 
-class TestCreateUserResponse(unittest.TestCase):
-    """CreateUserResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+class TestUserIdentity(unittest.TestCase):
+    """UserIdentity unit test stubs"""
 
+    def test_user_identity(self):
+        inst = UserIdentity({})
+        with self.assertRaises(KeyError):
+            inst["type"]
+        assert inst.get_item_oapg("type") is schemas.unset
+        with self.assertRaises(AttributeError):
+            inst.type
 
-if __name__ == '__main__':
+        inst = UserIdentity(type="")
+        type = inst["type"]
+        assert type == ""
+
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_error.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,18 +10,28 @@
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
 from kinde_sdk.model.error import Error
-from kinde_sdk import configuration
+from kinde_sdk import schemas
 
 
 class TestError(unittest.TestCase):
     """Error unit test stubs"""
 
-    _configuration = configuration.Configuration()
+    def test_error(self):
+        inst = Error({})
+        with self.assertRaises(KeyError):
+            inst["code"]
+        assert inst.get_item_oapg("code") is schemas.unset
+        with self.assertRaises(AttributeError):
+            inst.code
+
+        inst = Error(code="")
+        code = inst["code"]
+        assert code == ""
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_get_organizations_users_response.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,18 +9,29 @@
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
-from kinde_sdk.model.get_organizations_users_response import GetOrganizationsUsersResponse
-from kinde_sdk import configuration
+from kinde_sdk.model.user import User
+from kinde_sdk import schemas
 
 
-class TestGetOrganizationsUsersResponse(unittest.TestCase):
-    """GetOrganizationsUsersResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
+    def test_user(self):
+        inst = User({})
+        with self.assertRaises(KeyError):
+            inst["id"]
+        assert inst.get_item_oapg("id") is schemas.unset
+        with self.assertRaises(AttributeError):
+            inst.id
 
-if __name__ == '__main__':
+        inst = User(id="")
+        id = inst["id"]
+        assert id == ""
+
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_organization.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_organizations.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
-from kinde_sdk.model.organization import Organization
+from kinde_sdk.model.organizations import Organizations
 from kinde_sdk import configuration
 
 
-class TestOrganization(unittest.TestCase):
-    """Organization unit test stubs"""
+class TestOrganizations(unittest.TestCase):
+    """Organizations unit test stubs"""
 
     _configuration = configuration.Configuration()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/kinde_sdk/test/test_models/test_user_profile_v2.py` & `kinde-python-sdk-1.2.0/kinde_sdk/test/test_models/test_user_profile.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,29 @@
     Contact: support@kinde.com
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import kinde_sdk
-from kinde_sdk.model.user_profile_v2 import UserProfileV2
-from kinde_sdk import configuration
+from kinde_sdk.model.user_profile import UserProfile
+from kinde_sdk import schemas
 
 
-class TestUserProfileV2(unittest.TestCase):
-    """UserProfileV2 unit test stubs"""
+class TestUserProfile(unittest.TestCase):
+    """UserProfile unit test stubs"""
 
-    _configuration = configuration.Configuration()
+    def test_user_profile(self):
+        inst = UserProfile({})
+        with self.assertRaises(KeyError):
+            inst["id"]
+        assert inst.get_item_oapg("id") is schemas.unset
+        with self.assertRaises(AttributeError):
+            inst.id
+
+        inst = UserProfile(id="")
+        id = inst["id"]
+        assert id == ""
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `kinde-python-sdk-1.1.0/pyproject.toml` & `kinde-python-sdk-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kinde-python-sdk"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
     { name = "Kinde Engineering", email = "engineering@kinde.com" },
 ]
 description = "Connect your app to the Kinde platform"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

