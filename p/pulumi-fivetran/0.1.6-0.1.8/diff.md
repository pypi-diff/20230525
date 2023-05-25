# Comparing `tmp/pulumi_fivetran-0.1.6.tar.gz` & `tmp/pulumi_fivetran-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fivetran-0.1.6.tar", last modified: Wed Nov 10 00:31:30 2021, max compression
+gzip compressed data, was "pulumi_fivetran-0.1.8.tar", last modified: Mon Aug 22 14:21:56 2022, max compression
```

## Comparing `pulumi_fivetran-0.1.6.tar` & `pulumi_fivetran-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 00:31:30.459405 pulumi_fivetran-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-11-10 00:31:30.459405 pulumi_fivetran-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 00:31:30.455404 pulumi_fivetran-0.1.6/pulumi_fivetran/
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   120840 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7576 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 00:31:30.459405 pulumi_fivetran-0.1.6/pulumi_fivetran/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    25893 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/connector.py
--rw-r--r--   0 runner    (1001) docker     (121)    17058 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/destination.py
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_connectors_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     4505 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_destination.py
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3135 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_group_connectors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_group_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     5378 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/get_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     8664 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/group.py
--rw-r--r--   0 runner    (1001) docker     (121)   163431 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5056 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    13766 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/pulumi_fivetran/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 00:31:30.459405 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-11-10 00:31:30.000000 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      892 2021-11-10 00:31:30.000000 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 00:31:30.000000 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 00:31:30.000000 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-10 00:31:30.000000 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-10 00:31:30.000000 pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-10 00:31:30.459405 pulumi_fivetran-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2021-11-10 00:31:29.000000 pulumi_fivetran-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:21:56.217453 pulumi_fivetran-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-08-22 14:21:56.217453 pulumi_fivetran-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:21:56.213453 pulumi_fivetran-0.1.8/pulumi_fivetran/
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   133590 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7576 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:21:56.217453 pulumi_fivetran-0.1.8/pulumi_fivetran/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28784 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17058 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/destination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8941 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_connectors_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4505 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_destination.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3135 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_group_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5703 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6377 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)   180627 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    14900 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/pulumi_fivetran/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 14:21:56.213453 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-08-22 14:21:56.000000 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-08-22 14:21:56.000000 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 14:21:56.000000 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 14:21:56.000000 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-22 14:21:56.000000 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 14:21:56.000000 pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 14:21:56.217453 pulumi_fivetran-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-08-22 14:21:55.000000 pulumi_fivetran-0.1.8/setup.py
```

### Comparing `pulumi_fivetran-0.1.6/PKG-INFO` & `pulumi_fivetran-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fivetran
-Version: 0.1.6
+Version: 0.1.8
 Summary: A Pulumi package for creating and managing Fivetran resources.
 Home-page: https://github.com/benesch/pulumi-fivetran
 License: Apache-2.0
 Project-URL: Repository, https://github.com/benesch/pulumi-fivetran
 Description: # Fivetran Pulumi Provider
         
         A [Pulumi](https://pulumi.com) provider for the [Fivetran] ETL platform.
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/__init__.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/_inputs.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'ConnectorAuthArgs',
     'ConnectorAuthClientAccessArgs',
     'ConnectorConfigArgs',
+    'ConnectorConfigAdobeAnalyticsConfigurationArgs',
     'ConnectorConfigCustomTableArgs',
     'ConnectorConfigProjectCredentialArgs',
     'ConnectorConfigReportArgs',
+    'ConnectorDestinationSchemaArgs',
     'ConnectorStatusArgs',
     'ConnectorStatusTaskArgs',
     'ConnectorStatusWarningArgs',
     'DestinationConfigArgs',
-    'GroupUserArgs',
 ]
 
 @pulumi.input_type
 class ConnectorAuthArgs:
     def __init__(__self__, *,
                  access_token: Optional[pulumi.Input[str]] = None,
                  client_access: Optional[pulumi.Input['ConnectorAuthClientAccessArgs']] = None,
@@ -133,52 +134,57 @@
     def __init__(__self__, *,
                  abs_connection_string: Optional[pulumi.Input[str]] = None,
                  abs_container_name: Optional[pulumi.Input[str]] = None,
                  access_key_id: Optional[pulumi.Input[str]] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  account: Optional[pulumi.Input[str]] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
-                 account_ids: Optional[pulumi.Input[str]] = None,
+                 account_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  accounts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  action_breakdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  action_report_time: Optional[pulumi.Input[str]] = None,
+                 adobe_analytics_configurations: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorConfigAdobeAnalyticsConfigurationArgs']]]] = None,
                  advertisables: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  advertisers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  advertisers_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  aggregation: Optional[pulumi.Input[str]] = None,
+                 always_encrypted: Optional[pulumi.Input[str]] = None,
                  api_access_token: Optional[pulumi.Input[str]] = None,
                  api_key: Optional[pulumi.Input[str]] = None,
-                 api_keys: Optional[pulumi.Input[str]] = None,
+                 api_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  api_quota: Optional[pulumi.Input[str]] = None,
                  api_secret: Optional[pulumi.Input[str]] = None,
                  api_token: Optional[pulumi.Input[str]] = None,
+                 api_type: Optional[pulumi.Input[str]] = None,
                  api_url: Optional[pulumi.Input[str]] = None,
                  api_version: Optional[pulumi.Input[str]] = None,
                  app_sync_mode: Optional[pulumi.Input[str]] = None,
                  append_file_option: Optional[pulumi.Input[str]] = None,
                  apps: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  archive_pattern: Optional[pulumi.Input[str]] = None,
                  auth_mode: Optional[pulumi.Input[str]] = None,
                  auth_type: Optional[pulumi.Input[str]] = None,
                  authorization_method: Optional[pulumi.Input[str]] = None,
                  aws_region_code: Optional[pulumi.Input[str]] = None,
+                 base_url: Optional[pulumi.Input[str]] = None,
                  breakdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  bucket: Optional[pulumi.Input[str]] = None,
                  bucket_name: Optional[pulumi.Input[str]] = None,
                  bucket_service: Optional[pulumi.Input[str]] = None,
                  certificate: Optional[pulumi.Input[str]] = None,
                  click_attribution_window: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_secret: Optional[pulumi.Input[str]] = None,
                  cloud_storage_type: Optional[pulumi.Input[str]] = None,
                  columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  compression: Optional[pulumi.Input[str]] = None,
                  config_method: Optional[pulumi.Input[str]] = None,
                  config_type: Optional[pulumi.Input[str]] = None,
                  connection_string: Optional[pulumi.Input[str]] = None,
+                 connection_type: Optional[pulumi.Input[str]] = None,
                  consumer_group: Optional[pulumi.Input[str]] = None,
                  consumer_key: Optional[pulumi.Input[str]] = None,
                  consumer_secret: Optional[pulumi.Input[str]] = None,
                  container_name: Optional[pulumi.Input[str]] = None,
                  conversion_report_time: Optional[pulumi.Input[str]] = None,
                  conversion_window_size: Optional[pulumi.Input[str]] = None,
                  custom_tables: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorConfigCustomTableArgs']]]] = None,
@@ -193,22 +199,26 @@
                  dimension_attributes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  dimensions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
                  domain_name: Optional[pulumi.Input[str]] = None,
                  elements: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  enable_all_dimension_combinations: Optional[pulumi.Input[str]] = None,
+                 encryption_key: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  engagement_attribution_window: Optional[pulumi.Input[str]] = None,
+                 entity_id: Optional[pulumi.Input[str]] = None,
                  escape_char: Optional[pulumi.Input[str]] = None,
+                 eu_region: Optional[pulumi.Input[str]] = None,
                  external_id: Optional[pulumi.Input[str]] = None,
                  fields: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  file_type: Optional[pulumi.Input[str]] = None,
                  finance_account_sync_mode: Optional[pulumi.Input[str]] = None,
                  finance_accounts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 folder_id: Optional[pulumi.Input[str]] = None,
                  ftp_host: Optional[pulumi.Input[str]] = None,
                  ftp_password: Optional[pulumi.Input[str]] = None,
                  ftp_port: Optional[pulumi.Input[str]] = None,
                  ftp_user: Optional[pulumi.Input[str]] = None,
                  function: Optional[pulumi.Input[str]] = None,
                  function_app: Optional[pulumi.Input[str]] = None,
                  function_key: Optional[pulumi.Input[str]] = None,
@@ -219,14 +229,16 @@
                  home_folder: Optional[pulumi.Input[str]] = None,
                  host: Optional[pulumi.Input[str]] = None,
                  hosts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  identity: Optional[pulumi.Input[str]] = None,
                  instance: Optional[pulumi.Input[str]] = None,
                  integration_key: Optional[pulumi.Input[str]] = None,
                  is_ftps: Optional[pulumi.Input[str]] = None,
+                 is_multi_entity_feature_enabled: Optional[pulumi.Input[str]] = None,
+                 is_new_package: Optional[pulumi.Input[str]] = None,
                  is_secure: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  last_synced_changes_utc: Optional[pulumi.Input[str]] = None,
                  latest_version: Optional[pulumi.Input[str]] = None,
                  manager_accounts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  merchant_id: Optional[pulumi.Input[str]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
@@ -238,27 +250,29 @@
                  oauth_token_secret: Optional[pulumi.Input[str]] = None,
                  on_error: Optional[pulumi.Input[str]] = None,
                  on_premise: Optional[pulumi.Input[str]] = None,
                  organization_id: Optional[pulumi.Input[str]] = None,
                  organizations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  pages: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 pat: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pattern: Optional[pulumi.Input[str]] = None,
                  pem_certificate: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  post_click_attribution_window_size: Optional[pulumi.Input[str]] = None,
                  prebuilt_report: Optional[pulumi.Input[str]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  private_key: Optional[pulumi.Input[str]] = None,
                  profiles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  project_credentials: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorConfigProjectCredentialArgs']]]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  projects: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
+                 publication_name: Optional[pulumi.Input[str]] = None,
                  query_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  replication_slot: Optional[pulumi.Input[str]] = None,
                  report_configuration_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  report_suites: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  report_type: Optional[pulumi.Input[str]] = None,
                  report_url: Optional[pulumi.Input[str]] = None,
@@ -269,16 +283,14 @@
                  role_arn: Optional[pulumi.Input[str]] = None,
                  s3bucket: Optional[pulumi.Input[str]] = None,
                  s3external_id: Optional[pulumi.Input[str]] = None,
                  s3folder: Optional[pulumi.Input[str]] = None,
                  s3role_arn: Optional[pulumi.Input[str]] = None,
                  sales_account_sync_mode: Optional[pulumi.Input[str]] = None,
                  sales_accounts: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 schema: Optional[pulumi.Input[str]] = None,
-                 schema_prefix: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  secrets: Optional[pulumi.Input[str]] = None,
                  security_protocol: Optional[pulumi.Input[str]] = None,
                  selected_exports: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  server_url: Optional[pulumi.Input[str]] = None,
                  servers: Optional[pulumi.Input[str]] = None,
@@ -290,36 +302,39 @@
                  sftp_user: Optional[pulumi.Input[str]] = None,
                  sheet_id: Optional[pulumi.Input[str]] = None,
                  shop: Optional[pulumi.Input[str]] = None,
                  sid: Optional[pulumi.Input[str]] = None,
                  site_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  skip_after: Optional[pulumi.Input[str]] = None,
                  skip_before: Optional[pulumi.Input[str]] = None,
+                 soap_uri: Optional[pulumi.Input[str]] = None,
                  source: Optional[pulumi.Input[str]] = None,
                  sub_domain: Optional[pulumi.Input[str]] = None,
                  subdomain: Optional[pulumi.Input[str]] = None,
                  swipe_attribution_window: Optional[pulumi.Input[str]] = None,
                  sync_data_locker: Optional[pulumi.Input[str]] = None,
                  sync_format: Optional[pulumi.Input[str]] = None,
                  sync_mode: Optional[pulumi.Input[str]] = None,
                  sync_type: Optional[pulumi.Input[str]] = None,
-                 table: Optional[pulumi.Input[str]] = None,
                  technical_account_id: Optional[pulumi.Input[str]] = None,
                  test_table_name: Optional[pulumi.Input[str]] = None,
                  time_zone: Optional[pulumi.Input[str]] = None,
                  timeframe_months: Optional[pulumi.Input[str]] = None,
+                 token_key: Optional[pulumi.Input[str]] = None,
+                 token_secret: Optional[pulumi.Input[str]] = None,
                  tunnel_host: Optional[pulumi.Input[str]] = None,
                  tunnel_port: Optional[pulumi.Input[str]] = None,
                  tunnel_user: Optional[pulumi.Input[str]] = None,
                  unique_id: Optional[pulumi.Input[str]] = None,
                  update_config_on_each_sync: Optional[pulumi.Input[str]] = None,
                  update_method: Optional[pulumi.Input[str]] = None,
                  use_api_keys: Optional[pulumi.Input[str]] = None,
                  use_webhooks: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  user_key: Optional[pulumi.Input[str]] = None,
                  user_name: Optional[pulumi.Input[str]] = None,
                  user_profiles: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  view_attribution_window: Optional[pulumi.Input[str]] = None,
                  view_through_attribution_window_size: Optional[pulumi.Input[str]] = None):
         if abs_connection_string is not None:
@@ -338,34 +353,40 @@
             pulumi.set(__self__, "account_ids", account_ids)
         if accounts is not None:
             pulumi.set(__self__, "accounts", accounts)
         if action_breakdowns is not None:
             pulumi.set(__self__, "action_breakdowns", action_breakdowns)
         if action_report_time is not None:
             pulumi.set(__self__, "action_report_time", action_report_time)
+        if adobe_analytics_configurations is not None:
+            pulumi.set(__self__, "adobe_analytics_configurations", adobe_analytics_configurations)
         if advertisables is not None:
             pulumi.set(__self__, "advertisables", advertisables)
         if advertisers is not None:
             pulumi.set(__self__, "advertisers", advertisers)
         if advertisers_ids is not None:
             pulumi.set(__self__, "advertisers_ids", advertisers_ids)
         if aggregation is not None:
             pulumi.set(__self__, "aggregation", aggregation)
+        if always_encrypted is not None:
+            pulumi.set(__self__, "always_encrypted", always_encrypted)
         if api_access_token is not None:
             pulumi.set(__self__, "api_access_token", api_access_token)
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if api_keys is not None:
             pulumi.set(__self__, "api_keys", api_keys)
         if api_quota is not None:
             pulumi.set(__self__, "api_quota", api_quota)
         if api_secret is not None:
             pulumi.set(__self__, "api_secret", api_secret)
         if api_token is not None:
             pulumi.set(__self__, "api_token", api_token)
+        if api_type is not None:
+            pulumi.set(__self__, "api_type", api_type)
         if api_url is not None:
             pulumi.set(__self__, "api_url", api_url)
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
         if app_sync_mode is not None:
             pulumi.set(__self__, "app_sync_mode", app_sync_mode)
         if append_file_option is not None:
@@ -378,14 +399,16 @@
             pulumi.set(__self__, "auth_mode", auth_mode)
         if auth_type is not None:
             pulumi.set(__self__, "auth_type", auth_type)
         if authorization_method is not None:
             pulumi.set(__self__, "authorization_method", authorization_method)
         if aws_region_code is not None:
             pulumi.set(__self__, "aws_region_code", aws_region_code)
+        if base_url is not None:
+            pulumi.set(__self__, "base_url", base_url)
         if breakdowns is not None:
             pulumi.set(__self__, "breakdowns", breakdowns)
         if bucket is not None:
             pulumi.set(__self__, "bucket", bucket)
         if bucket_name is not None:
             pulumi.set(__self__, "bucket_name", bucket_name)
         if bucket_service is not None:
@@ -406,14 +429,16 @@
             pulumi.set(__self__, "compression", compression)
         if config_method is not None:
             pulumi.set(__self__, "config_method", config_method)
         if config_type is not None:
             pulumi.set(__self__, "config_type", config_type)
         if connection_string is not None:
             pulumi.set(__self__, "connection_string", connection_string)
+        if connection_type is not None:
+            pulumi.set(__self__, "connection_type", connection_type)
         if consumer_group is not None:
             pulumi.set(__self__, "consumer_group", consumer_group)
         if consumer_key is not None:
             pulumi.set(__self__, "consumer_key", consumer_key)
         if consumer_secret is not None:
             pulumi.set(__self__, "consumer_secret", consumer_secret)
         if container_name is not None:
@@ -450,30 +475,38 @@
             pulumi.set(__self__, "domain_name", domain_name)
         if elements is not None:
             pulumi.set(__self__, "elements", elements)
         if email is not None:
             pulumi.set(__self__, "email", email)
         if enable_all_dimension_combinations is not None:
             pulumi.set(__self__, "enable_all_dimension_combinations", enable_all_dimension_combinations)
+        if encryption_key is not None:
+            pulumi.set(__self__, "encryption_key", encryption_key)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if engagement_attribution_window is not None:
             pulumi.set(__self__, "engagement_attribution_window", engagement_attribution_window)
+        if entity_id is not None:
+            pulumi.set(__self__, "entity_id", entity_id)
         if escape_char is not None:
             pulumi.set(__self__, "escape_char", escape_char)
+        if eu_region is not None:
+            pulumi.set(__self__, "eu_region", eu_region)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
         if fields is not None:
             pulumi.set(__self__, "fields", fields)
         if file_type is not None:
             pulumi.set(__self__, "file_type", file_type)
         if finance_account_sync_mode is not None:
             pulumi.set(__self__, "finance_account_sync_mode", finance_account_sync_mode)
         if finance_accounts is not None:
             pulumi.set(__self__, "finance_accounts", finance_accounts)
+        if folder_id is not None:
+            pulumi.set(__self__, "folder_id", folder_id)
         if ftp_host is not None:
             pulumi.set(__self__, "ftp_host", ftp_host)
         if ftp_password is not None:
             pulumi.set(__self__, "ftp_password", ftp_password)
         if ftp_port is not None:
             pulumi.set(__self__, "ftp_port", ftp_port)
         if ftp_user is not None:
@@ -502,14 +535,18 @@
             pulumi.set(__self__, "identity", identity)
         if instance is not None:
             pulumi.set(__self__, "instance", instance)
         if integration_key is not None:
             pulumi.set(__self__, "integration_key", integration_key)
         if is_ftps is not None:
             pulumi.set(__self__, "is_ftps", is_ftps)
+        if is_multi_entity_feature_enabled is not None:
+            pulumi.set(__self__, "is_multi_entity_feature_enabled", is_multi_entity_feature_enabled)
+        if is_new_package is not None:
+            pulumi.set(__self__, "is_new_package", is_new_package)
         if is_secure is not None:
             pulumi.set(__self__, "is_secure", is_secure)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if last_synced_changes_utc is not None:
             pulumi.set(__self__, "last_synced_changes_utc", last_synced_changes_utc)
         if latest_version is not None:
@@ -540,14 +577,16 @@
             pulumi.set(__self__, "organization_id", organization_id)
         if organizations is not None:
             pulumi.set(__self__, "organizations", organizations)
         if pages is not None:
             pulumi.set(__self__, "pages", pages)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if pat is not None:
+            pulumi.set(__self__, "pat", pat)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if pattern is not None:
             pulumi.set(__self__, "pattern", pattern)
         if pem_certificate is not None:
             pulumi.set(__self__, "pem_certificate", pem_certificate)
         if port is not None:
@@ -566,14 +605,16 @@
             pulumi.set(__self__, "project_credentials", project_credentials)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
         if projects is not None:
             pulumi.set(__self__, "projects", projects)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
+        if publication_name is not None:
+            pulumi.set(__self__, "publication_name", publication_name)
         if query_id is not None:
             pulumi.set(__self__, "query_id", query_id)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if replication_slot is not None:
             pulumi.set(__self__, "replication_slot", replication_slot)
         if report_configuration_ids is not None:
@@ -602,18 +643,14 @@
             pulumi.set(__self__, "s3folder", s3folder)
         if s3role_arn is not None:
             pulumi.set(__self__, "s3role_arn", s3role_arn)
         if sales_account_sync_mode is not None:
             pulumi.set(__self__, "sales_account_sync_mode", sales_account_sync_mode)
         if sales_accounts is not None:
             pulumi.set(__self__, "sales_accounts", sales_accounts)
-        if schema is not None:
-            pulumi.set(__self__, "schema", schema)
-        if schema_prefix is not None:
-            pulumi.set(__self__, "schema_prefix", schema_prefix)
         if secret is not None:
             pulumi.set(__self__, "secret", secret)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
         if security_protocol is not None:
@@ -644,14 +681,16 @@
             pulumi.set(__self__, "sid", sid)
         if site_urls is not None:
             pulumi.set(__self__, "site_urls", site_urls)
         if skip_after is not None:
             pulumi.set(__self__, "skip_after", skip_after)
         if skip_before is not None:
             pulumi.set(__self__, "skip_before", skip_before)
+        if soap_uri is not None:
+            pulumi.set(__self__, "soap_uri", soap_uri)
         if source is not None:
             pulumi.set(__self__, "source", source)
         if sub_domain is not None:
             pulumi.set(__self__, "sub_domain", sub_domain)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if swipe_attribution_window is not None:
@@ -660,24 +699,26 @@
             pulumi.set(__self__, "sync_data_locker", sync_data_locker)
         if sync_format is not None:
             pulumi.set(__self__, "sync_format", sync_format)
         if sync_mode is not None:
             pulumi.set(__self__, "sync_mode", sync_mode)
         if sync_type is not None:
             pulumi.set(__self__, "sync_type", sync_type)
-        if table is not None:
-            pulumi.set(__self__, "table", table)
         if technical_account_id is not None:
             pulumi.set(__self__, "technical_account_id", technical_account_id)
         if test_table_name is not None:
             pulumi.set(__self__, "test_table_name", test_table_name)
         if time_zone is not None:
             pulumi.set(__self__, "time_zone", time_zone)
         if timeframe_months is not None:
             pulumi.set(__self__, "timeframe_months", timeframe_months)
+        if token_key is not None:
+            pulumi.set(__self__, "token_key", token_key)
+        if token_secret is not None:
+            pulumi.set(__self__, "token_secret", token_secret)
         if tunnel_host is not None:
             pulumi.set(__self__, "tunnel_host", tunnel_host)
         if tunnel_port is not None:
             pulumi.set(__self__, "tunnel_port", tunnel_port)
         if tunnel_user is not None:
             pulumi.set(__self__, "tunnel_user", tunnel_user)
         if unique_id is not None:
@@ -688,14 +729,16 @@
             pulumi.set(__self__, "update_method", update_method)
         if use_api_keys is not None:
             pulumi.set(__self__, "use_api_keys", use_api_keys)
         if use_webhooks is not None:
             pulumi.set(__self__, "use_webhooks", use_webhooks)
         if user is not None:
             pulumi.set(__self__, "user", user)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
         if user_key is not None:
             pulumi.set(__self__, "user_key", user_key)
         if user_name is not None:
             pulumi.set(__self__, "user_name", user_name)
         if user_profiles is not None:
             pulumi.set(__self__, "user_profiles", user_profiles)
         if username is not None:
@@ -757,19 +800,19 @@
 
     @account_id.setter
     def account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "account_id", value)
 
     @property
     @pulumi.getter(name="accountIds")
-    def account_ids(self) -> Optional[pulumi.Input[str]]:
+    def account_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "account_ids")
 
     @account_ids.setter
-    def account_ids(self, value: Optional[pulumi.Input[str]]):
+    def account_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "account_ids", value)
 
     @property
     @pulumi.getter
     def accounts(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "accounts")
 
@@ -792,14 +835,23 @@
         return pulumi.get(self, "action_report_time")
 
     @action_report_time.setter
     def action_report_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "action_report_time", value)
 
     @property
+    @pulumi.getter(name="adobeAnalyticsConfigurations")
+    def adobe_analytics_configurations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorConfigAdobeAnalyticsConfigurationArgs']]]]:
+        return pulumi.get(self, "adobe_analytics_configurations")
+
+    @adobe_analytics_configurations.setter
+    def adobe_analytics_configurations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorConfigAdobeAnalyticsConfigurationArgs']]]]):
+        pulumi.set(self, "adobe_analytics_configurations", value)
+
+    @property
     @pulumi.getter
     def advertisables(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "advertisables")
 
     @advertisables.setter
     def advertisables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "advertisables", value)
@@ -828,14 +880,23 @@
         return pulumi.get(self, "aggregation")
 
     @aggregation.setter
     def aggregation(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aggregation", value)
 
     @property
+    @pulumi.getter(name="alwaysEncrypted")
+    def always_encrypted(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "always_encrypted")
+
+    @always_encrypted.setter
+    def always_encrypted(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "always_encrypted", value)
+
+    @property
     @pulumi.getter(name="apiAccessToken")
     def api_access_token(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "api_access_token")
 
     @api_access_token.setter
     def api_access_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_access_token", value)
@@ -847,19 +908,19 @@
 
     @api_key.setter
     def api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_key", value)
 
     @property
     @pulumi.getter(name="apiKeys")
-    def api_keys(self) -> Optional[pulumi.Input[str]]:
+    def api_keys(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "api_keys")
 
     @api_keys.setter
-    def api_keys(self, value: Optional[pulumi.Input[str]]):
+    def api_keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "api_keys", value)
 
     @property
     @pulumi.getter(name="apiQuota")
     def api_quota(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "api_quota")
 
@@ -882,14 +943,23 @@
         return pulumi.get(self, "api_token")
 
     @api_token.setter
     def api_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_token", value)
 
     @property
+    @pulumi.getter(name="apiType")
+    def api_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "api_type")
+
+    @api_type.setter
+    def api_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_type", value)
+
+    @property
     @pulumi.getter(name="apiUrl")
     def api_url(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "api_url")
 
     @api_url.setter
     def api_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_url", value)
@@ -972,14 +1042,23 @@
         return pulumi.get(self, "aws_region_code")
 
     @aws_region_code.setter
     def aws_region_code(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aws_region_code", value)
 
     @property
+    @pulumi.getter(name="baseUrl")
+    def base_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "base_url")
+
+    @base_url.setter
+    def base_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_url", value)
+
+    @property
     @pulumi.getter
     def breakdowns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "breakdowns")
 
     @breakdowns.setter
     def breakdowns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "breakdowns", value)
@@ -1098,14 +1177,23 @@
         return pulumi.get(self, "connection_string")
 
     @connection_string.setter
     def connection_string(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "connection_string", value)
 
     @property
+    @pulumi.getter(name="connectionType")
+    def connection_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "connection_type")
+
+    @connection_type.setter
+    def connection_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "connection_type", value)
+
+    @property
     @pulumi.getter(name="consumerGroup")
     def consumer_group(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "consumer_group")
 
     @consumer_group.setter
     def consumer_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "consumer_group", value)
@@ -1296,14 +1384,23 @@
         return pulumi.get(self, "enable_all_dimension_combinations")
 
     @enable_all_dimension_combinations.setter
     def enable_all_dimension_combinations(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "enable_all_dimension_combinations", value)
 
     @property
+    @pulumi.getter(name="encryptionKey")
+    def encryption_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "encryption_key")
+
+    @encryption_key.setter
+    def encryption_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "encryption_key", value)
+
+    @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "endpoint")
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
@@ -1314,23 +1411,41 @@
         return pulumi.get(self, "engagement_attribution_window")
 
     @engagement_attribution_window.setter
     def engagement_attribution_window(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engagement_attribution_window", value)
 
     @property
+    @pulumi.getter(name="entityId")
+    def entity_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "entity_id")
+
+    @entity_id.setter
+    def entity_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "entity_id", value)
+
+    @property
     @pulumi.getter(name="escapeChar")
     def escape_char(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "escape_char")
 
     @escape_char.setter
     def escape_char(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "escape_char", value)
 
     @property
+    @pulumi.getter(name="euRegion")
+    def eu_region(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "eu_region")
+
+    @eu_region.setter
+    def eu_region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "eu_region", value)
+
+    @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "external_id")
 
     @external_id.setter
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
@@ -1368,14 +1483,23 @@
         return pulumi.get(self, "finance_accounts")
 
     @finance_accounts.setter
     def finance_accounts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "finance_accounts", value)
 
     @property
+    @pulumi.getter(name="folderId")
+    def folder_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "folder_id")
+
+    @folder_id.setter
+    def folder_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "folder_id", value)
+
+    @property
     @pulumi.getter(name="ftpHost")
     def ftp_host(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "ftp_host")
 
     @ftp_host.setter
     def ftp_host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ftp_host", value)
@@ -1530,14 +1654,32 @@
         return pulumi.get(self, "is_ftps")
 
     @is_ftps.setter
     def is_ftps(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "is_ftps", value)
 
     @property
+    @pulumi.getter(name="isMultiEntityFeatureEnabled")
+    def is_multi_entity_feature_enabled(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "is_multi_entity_feature_enabled")
+
+    @is_multi_entity_feature_enabled.setter
+    def is_multi_entity_feature_enabled(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "is_multi_entity_feature_enabled", value)
+
+    @property
+    @pulumi.getter(name="isNewPackage")
+    def is_new_package(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "is_new_package")
+
+    @is_new_package.setter
+    def is_new_package(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "is_new_package", value)
+
+    @property
     @pulumi.getter(name="isSecure")
     def is_secure(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "is_secure")
 
     @is_secure.setter
     def is_secure(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "is_secure", value)
@@ -1702,14 +1844,23 @@
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
+    def pat(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "pat")
+
+    @pat.setter
+    def pat(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pat", value)
+
+    @property
+    @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
@@ -1818,14 +1969,23 @@
         return pulumi.get(self, "public_key")
 
     @public_key.setter
     def public_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_key", value)
 
     @property
+    @pulumi.getter(name="publicationName")
+    def publication_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "publication_name")
+
+    @publication_name.setter
+    def publication_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "publication_name", value)
+
+    @property
     @pulumi.getter(name="queryId")
     def query_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "query_id")
 
     @query_id.setter
     def query_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "query_id", value)
@@ -1981,32 +2141,14 @@
 
     @sales_accounts.setter
     def sales_accounts(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "sales_accounts", value)
 
     @property
     @pulumi.getter
-    def schema(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "schema")
-
-    @schema.setter
-    def schema(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema", value)
-
-    @property
-    @pulumi.getter(name="schemaPrefix")
-    def schema_prefix(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "schema_prefix")
-
-    @schema_prefix.setter
-    def schema_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema_prefix", value)
-
-    @property
-    @pulumi.getter
     def secret(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "secret")
 
     @secret.setter
     def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
@@ -2169,14 +2311,23 @@
         return pulumi.get(self, "skip_before")
 
     @skip_before.setter
     def skip_before(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "skip_before", value)
 
     @property
+    @pulumi.getter(name="soapUri")
+    def soap_uri(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "soap_uri")
+
+    @soap_uri.setter
+    def soap_uri(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "soap_uri", value)
+
+    @property
     @pulumi.getter
     def source(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "source")
 
     @source.setter
     def source(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source", value)
@@ -2241,23 +2392,14 @@
         return pulumi.get(self, "sync_type")
 
     @sync_type.setter
     def sync_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sync_type", value)
 
     @property
-    @pulumi.getter
-    def table(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "table")
-
-    @table.setter
-    def table(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "table", value)
-
-    @property
     @pulumi.getter(name="technicalAccountId")
     def technical_account_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "technical_account_id")
 
     @technical_account_id.setter
     def technical_account_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "technical_account_id", value)
@@ -2286,14 +2428,32 @@
         return pulumi.get(self, "timeframe_months")
 
     @timeframe_months.setter
     def timeframe_months(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "timeframe_months", value)
 
     @property
+    @pulumi.getter(name="tokenKey")
+    def token_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "token_key")
+
+    @token_key.setter
+    def token_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token_key", value)
+
+    @property
+    @pulumi.getter(name="tokenSecret")
+    def token_secret(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "token_secret")
+
+    @token_secret.setter
+    def token_secret(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token_secret", value)
+
+    @property
     @pulumi.getter(name="tunnelHost")
     def tunnel_host(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "tunnel_host")
 
     @tunnel_host.setter
     def tunnel_host(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tunnel_host", value)
@@ -2367,14 +2527,23 @@
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
     @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
+
+    @property
     @pulumi.getter(name="userKey")
     def user_key(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "user_key")
 
     @user_key.setter
     def user_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_key", value)
@@ -2422,14 +2591,91 @@
 
     @view_through_attribution_window_size.setter
     def view_through_attribution_window_size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "view_through_attribution_window_size", value)
 
 
 @pulumi.input_type
+class ConnectorConfigAdobeAnalyticsConfigurationArgs:
+    def __init__(__self__, *,
+                 calculated_metrics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elements: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 metrics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 report_suites: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 segments: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 sync_mode: Optional[pulumi.Input[str]] = None):
+        if calculated_metrics is not None:
+            pulumi.set(__self__, "calculated_metrics", calculated_metrics)
+        if elements is not None:
+            pulumi.set(__self__, "elements", elements)
+        if metrics is not None:
+            pulumi.set(__self__, "metrics", metrics)
+        if report_suites is not None:
+            pulumi.set(__self__, "report_suites", report_suites)
+        if segments is not None:
+            pulumi.set(__self__, "segments", segments)
+        if sync_mode is not None:
+            pulumi.set(__self__, "sync_mode", sync_mode)
+
+    @property
+    @pulumi.getter(name="calculatedMetrics")
+    def calculated_metrics(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "calculated_metrics")
+
+    @calculated_metrics.setter
+    def calculated_metrics(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "calculated_metrics", value)
+
+    @property
+    @pulumi.getter
+    def elements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "elements")
+
+    @elements.setter
+    def elements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "elements", value)
+
+    @property
+    @pulumi.getter
+    def metrics(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "metrics")
+
+    @metrics.setter
+    def metrics(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "metrics", value)
+
+    @property
+    @pulumi.getter(name="reportSuites")
+    def report_suites(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "report_suites")
+
+    @report_suites.setter
+    def report_suites(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "report_suites", value)
+
+    @property
+    @pulumi.getter
+    def segments(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "segments")
+
+    @segments.setter
+    def segments(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "segments", value)
+
+    @property
+    @pulumi.getter(name="syncMode")
+    def sync_mode(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "sync_mode")
+
+    @sync_mode.setter
+    def sync_mode(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "sync_mode", value)
+
+
+@pulumi.input_type
 class ConnectorConfigCustomTableArgs:
     def __init__(__self__, *,
                  action_breakdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  action_report_time: Optional[pulumi.Input[str]] = None,
                  aggregation: Optional[pulumi.Input[str]] = None,
                  breakdowns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  click_attribution_window: Optional[pulumi.Input[str]] = None,
@@ -2701,14 +2947,55 @@
 
     @table.setter
     def table(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "table", value)
 
 
 @pulumi.input_type
+class ConnectorDestinationSchemaArgs:
+    def __init__(__self__, *,
+                 name: Optional[pulumi.Input[str]] = None,
+                 prefix: Optional[pulumi.Input[str]] = None,
+                 table: Optional[pulumi.Input[str]] = None):
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if prefix is not None:
+            pulumi.set(__self__, "prefix", prefix)
+        if table is not None:
+            pulumi.set(__self__, "table", table)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def prefix(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "prefix")
+
+    @prefix.setter
+    def prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "prefix", value)
+
+    @property
+    @pulumi.getter
+    def table(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "table")
+
+    @table.setter
+    def table(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "table", value)
+
+
+@pulumi.input_type
 class ConnectorStatusArgs:
     def __init__(__self__, *,
                  is_historical_sync: Optional[pulumi.Input[str]] = None,
                  setup_state: Optional[pulumi.Input[str]] = None,
                  sync_state: Optional[pulumi.Input[str]] = None,
                  tasks: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorStatusTaskArgs']]]] = None,
                  update_state: Optional[pulumi.Input[str]] = None,
@@ -2841,38 +3128,46 @@
 
 @pulumi.input_type
 class DestinationConfigArgs:
     def __init__(__self__, *,
                  auth: Optional[pulumi.Input[str]] = None,
                  auth_type: Optional[pulumi.Input[str]] = None,
                  bucket: Optional[pulumi.Input[str]] = None,
+                 cluster_id: Optional[pulumi.Input[str]] = None,
+                 cluster_region: Optional[pulumi.Input[str]] = None,
                  connection_type: Optional[pulumi.Input[str]] = None,
                  create_external_tables: Optional[pulumi.Input[str]] = None,
                  data_set_location: Optional[pulumi.Input[str]] = None,
                  database: Optional[pulumi.Input[str]] = None,
                  external_location: Optional[pulumi.Input[str]] = None,
                  host: Optional[pulumi.Input[str]] = None,
                  http_path: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  personal_access_token: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
+                 private_key: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 public_key: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None,
                  server_host_name: Optional[pulumi.Input[str]] = None,
                  tunnel_host: Optional[pulumi.Input[str]] = None,
                  tunnel_port: Optional[pulumi.Input[str]] = None,
                  tunnel_user: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if auth_type is not None:
             pulumi.set(__self__, "auth_type", auth_type)
         if bucket is not None:
             pulumi.set(__self__, "bucket", bucket)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
+        if cluster_region is not None:
+            pulumi.set(__self__, "cluster_region", cluster_region)
         if connection_type is not None:
             pulumi.set(__self__, "connection_type", connection_type)
         if create_external_tables is not None:
             pulumi.set(__self__, "create_external_tables", create_external_tables)
         if data_set_location is not None:
             pulumi.set(__self__, "data_set_location", data_set_location)
         if database is not None:
@@ -2885,16 +3180,20 @@
             pulumi.set(__self__, "http_path", http_path)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if personal_access_token is not None:
             pulumi.set(__self__, "personal_access_token", personal_access_token)
         if port is not None:
             pulumi.set(__self__, "port", port)
+        if private_key is not None:
+            pulumi.set(__self__, "private_key", private_key)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
+        if public_key is not None:
+            pulumi.set(__self__, "public_key", public_key)
         if role_arn is not None:
             pulumi.set(__self__, "role_arn", role_arn)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if server_host_name is not None:
             pulumi.set(__self__, "server_host_name", server_host_name)
         if tunnel_host is not None:
@@ -2930,14 +3229,32 @@
         return pulumi.get(self, "bucket")
 
     @bucket.setter
     def bucket(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bucket", value)
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cluster_id")
+
+    @cluster_id.setter
+    def cluster_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_id", value)
+
+    @property
+    @pulumi.getter(name="clusterRegion")
+    def cluster_region(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cluster_region")
+
+    @cluster_region.setter
+    def cluster_region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_region", value)
+
+    @property
     @pulumi.getter(name="connectionType")
     def connection_type(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "connection_type")
 
     @connection_type.setter
     def connection_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "connection_type", value)
@@ -3020,23 +3337,41 @@
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port", value)
 
     @property
+    @pulumi.getter(name="privateKey")
+    def private_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "private_key")
+
+    @private_key.setter
+    def private_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "private_key", value)
+
+    @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
     @property
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "public_key")
+
+    @public_key.setter
+    def public_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "public_key", value)
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "role_arn")
 
     @role_arn.setter
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
@@ -3092,34 +3427,7 @@
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
 
-@pulumi.input_type
-class GroupUserArgs:
-    def __init__(__self__, *,
-                 id: pulumi.Input[str],
-                 role: pulumi.Input[str]):
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "role", role)
-
-    @property
-    @pulumi.getter
-    def id(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "id", value)
-
-    @property
-    @pulumi.getter
-    def role(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "role")
-
-    @role.setter
-    def role(self, value: pulumi.Input[str]):
-        pulumi.set(self, "role", value)
-
-
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/_utilities.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/config/vars.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/connector.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,39 @@
 
 __all__ = ['ConnectorArgs', 'Connector']
 
 @pulumi.input_type
 class ConnectorArgs:
     def __init__(__self__, *,
                  config: pulumi.Input['ConnectorConfigArgs'],
+                 destination_schema: pulumi.Input['ConnectorDestinationSchemaArgs'],
                  group_id: pulumi.Input[str],
                  pause_after_trial: pulumi.Input[str],
                  paused: pulumi.Input[str],
-                 schema: pulumi.Input[str],
                  service: pulumi.Input[str],
                  sync_frequency: pulumi.Input[str],
                  auth: Optional[pulumi.Input['ConnectorAuthArgs']] = None,
+                 daily_sync_time: Optional[pulumi.Input[str]] = None,
                  run_setup_tests: Optional[pulumi.Input[str]] = None,
                  trust_certificates: Optional[pulumi.Input[str]] = None,
                  trust_fingerprints: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Connector resource.
         """
         pulumi.set(__self__, "config", config)
+        pulumi.set(__self__, "destination_schema", destination_schema)
         pulumi.set(__self__, "group_id", group_id)
         pulumi.set(__self__, "pause_after_trial", pause_after_trial)
         pulumi.set(__self__, "paused", paused)
-        pulumi.set(__self__, "schema", schema)
         pulumi.set(__self__, "service", service)
         pulumi.set(__self__, "sync_frequency", sync_frequency)
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
+        if daily_sync_time is not None:
+            pulumi.set(__self__, "daily_sync_time", daily_sync_time)
         if run_setup_tests is not None:
             pulumi.set(__self__, "run_setup_tests", run_setup_tests)
         if trust_certificates is not None:
             pulumi.set(__self__, "trust_certificates", trust_certificates)
         if trust_fingerprints is not None:
             pulumi.set(__self__, "trust_fingerprints", trust_fingerprints)
 
@@ -51,14 +54,23 @@
         return pulumi.get(self, "config")
 
     @config.setter
     def config(self, value: pulumi.Input['ConnectorConfigArgs']):
         pulumi.set(self, "config", value)
 
     @property
+    @pulumi.getter(name="destinationSchema")
+    def destination_schema(self) -> pulumi.Input['ConnectorDestinationSchemaArgs']:
+        return pulumi.get(self, "destination_schema")
+
+    @destination_schema.setter
+    def destination_schema(self, value: pulumi.Input['ConnectorDestinationSchemaArgs']):
+        pulumi.set(self, "destination_schema", value)
+
+    @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Input[str]:
         return pulumi.get(self, "group_id")
 
     @group_id.setter
     def group_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "group_id", value)
@@ -79,23 +91,14 @@
 
     @paused.setter
     def paused(self, value: pulumi.Input[str]):
         pulumi.set(self, "paused", value)
 
     @property
     @pulumi.getter
-    def schema(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "schema")
-
-    @schema.setter
-    def schema(self, value: pulumi.Input[str]):
-        pulumi.set(self, "schema", value)
-
-    @property
-    @pulumi.getter
     def service(self) -> pulumi.Input[str]:
         return pulumi.get(self, "service")
 
     @service.setter
     def service(self, value: pulumi.Input[str]):
         pulumi.set(self, "service", value)
 
@@ -114,14 +117,23 @@
         return pulumi.get(self, "auth")
 
     @auth.setter
     def auth(self, value: Optional[pulumi.Input['ConnectorAuthArgs']]):
         pulumi.set(self, "auth", value)
 
     @property
+    @pulumi.getter(name="dailySyncTime")
+    def daily_sync_time(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "daily_sync_time")
+
+    @daily_sync_time.setter
+    def daily_sync_time(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "daily_sync_time", value)
+
+    @property
     @pulumi.getter(name="runSetupTests")
     def run_setup_tests(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "run_setup_tests")
 
     @run_setup_tests.setter
     def run_setup_tests(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "run_setup_tests", value)
@@ -148,22 +160,24 @@
 @pulumi.input_type
 class _ConnectorState:
     def __init__(__self__, *,
                  auth: Optional[pulumi.Input['ConnectorAuthArgs']] = None,
                  config: Optional[pulumi.Input['ConnectorConfigArgs']] = None,
                  connected_by: Optional[pulumi.Input[str]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
+                 daily_sync_time: Optional[pulumi.Input[str]] = None,
+                 destination_schema: Optional[pulumi.Input['ConnectorDestinationSchemaArgs']] = None,
                  failed_at: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  last_updated: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  pause_after_trial: Optional[pulumi.Input[str]] = None,
                  paused: Optional[pulumi.Input[str]] = None,
                  run_setup_tests: Optional[pulumi.Input[str]] = None,
                  schedule_type: Optional[pulumi.Input[str]] = None,
-                 schema: Optional[pulumi.Input[str]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  service_version: Optional[pulumi.Input[str]] = None,
                  statuses: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectorStatusArgs']]]] = None,
                  succeeded_at: Optional[pulumi.Input[str]] = None,
                  sync_frequency: Optional[pulumi.Input[str]] = None,
                  trust_certificates: Optional[pulumi.Input[str]] = None,
                  trust_fingerprints: Optional[pulumi.Input[str]] = None):
@@ -174,30 +188,34 @@
             pulumi.set(__self__, "auth", auth)
         if config is not None:
             pulumi.set(__self__, "config", config)
         if connected_by is not None:
             pulumi.set(__self__, "connected_by", connected_by)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
+        if daily_sync_time is not None:
+            pulumi.set(__self__, "daily_sync_time", daily_sync_time)
+        if destination_schema is not None:
+            pulumi.set(__self__, "destination_schema", destination_schema)
         if failed_at is not None:
             pulumi.set(__self__, "failed_at", failed_at)
         if group_id is not None:
             pulumi.set(__self__, "group_id", group_id)
         if last_updated is not None:
             pulumi.set(__self__, "last_updated", last_updated)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if pause_after_trial is not None:
             pulumi.set(__self__, "pause_after_trial", pause_after_trial)
         if paused is not None:
             pulumi.set(__self__, "paused", paused)
         if run_setup_tests is not None:
             pulumi.set(__self__, "run_setup_tests", run_setup_tests)
         if schedule_type is not None:
             pulumi.set(__self__, "schedule_type", schedule_type)
-        if schema is not None:
-            pulumi.set(__self__, "schema", schema)
         if service is not None:
             pulumi.set(__self__, "service", service)
         if service_version is not None:
             pulumi.set(__self__, "service_version", service_version)
         if statuses is not None:
             pulumi.set(__self__, "statuses", statuses)
         if succeeded_at is not None:
@@ -242,14 +260,32 @@
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
+    @pulumi.getter(name="dailySyncTime")
+    def daily_sync_time(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "daily_sync_time")
+
+    @daily_sync_time.setter
+    def daily_sync_time(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "daily_sync_time", value)
+
+    @property
+    @pulumi.getter(name="destinationSchema")
+    def destination_schema(self) -> Optional[pulumi.Input['ConnectorDestinationSchemaArgs']]:
+        return pulumi.get(self, "destination_schema")
+
+    @destination_schema.setter
+    def destination_schema(self, value: Optional[pulumi.Input['ConnectorDestinationSchemaArgs']]):
+        pulumi.set(self, "destination_schema", value)
+
+    @property
     @pulumi.getter(name="failedAt")
     def failed_at(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "failed_at")
 
     @failed_at.setter
     def failed_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "failed_at", value)
@@ -269,14 +305,23 @@
         return pulumi.get(self, "last_updated")
 
     @last_updated.setter
     def last_updated(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_updated", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="pauseAfterTrial")
     def pause_after_trial(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "pause_after_trial")
 
     @pause_after_trial.setter
     def pause_after_trial(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pause_after_trial", value)
@@ -306,23 +351,14 @@
 
     @schedule_type.setter
     def schedule_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schedule_type", value)
 
     @property
     @pulumi.getter
-    def schema(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "schema")
-
-    @schema.setter
-    def schema(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema", value)
-
-    @property
-    @pulumi.getter
     def service(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "service")
 
     @service.setter
     def service(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service", value)
 
@@ -384,19 +420,20 @@
 class Connector(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth: Optional[pulumi.Input[pulumi.InputType['ConnectorAuthArgs']]] = None,
                  config: Optional[pulumi.Input[pulumi.InputType['ConnectorConfigArgs']]] = None,
+                 daily_sync_time: Optional[pulumi.Input[str]] = None,
+                 destination_schema: Optional[pulumi.Input[pulumi.InputType['ConnectorDestinationSchemaArgs']]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  pause_after_trial: Optional[pulumi.Input[str]] = None,
                  paused: Optional[pulumi.Input[str]] = None,
                  run_setup_tests: Optional[pulumi.Input[str]] = None,
-                 schema: Optional[pulumi.Input[str]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  sync_frequency: Optional[pulumi.Input[str]] = None,
                  trust_certificates: Optional[pulumi.Input[str]] = None,
                  trust_fingerprints: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a Connector resource with the given unique name, props, and options.
@@ -424,19 +461,20 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  auth: Optional[pulumi.Input[pulumi.InputType['ConnectorAuthArgs']]] = None,
                  config: Optional[pulumi.Input[pulumi.InputType['ConnectorConfigArgs']]] = None,
+                 daily_sync_time: Optional[pulumi.Input[str]] = None,
+                 destination_schema: Optional[pulumi.Input[pulumi.InputType['ConnectorDestinationSchemaArgs']]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  pause_after_trial: Optional[pulumi.Input[str]] = None,
                  paused: Optional[pulumi.Input[str]] = None,
                  run_setup_tests: Optional[pulumi.Input[str]] = None,
-                 schema: Optional[pulumi.Input[str]] = None,
                  service: Optional[pulumi.Input[str]] = None,
                  sync_frequency: Optional[pulumi.Input[str]] = None,
                  trust_certificates: Optional[pulumi.Input[str]] = None,
                  trust_fingerprints: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
@@ -449,39 +487,41 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ConnectorArgs.__new__(ConnectorArgs)
 
             __props__.__dict__["auth"] = auth
             if config is None and not opts.urn:
                 raise TypeError("Missing required property 'config'")
             __props__.__dict__["config"] = config
+            __props__.__dict__["daily_sync_time"] = daily_sync_time
+            if destination_schema is None and not opts.urn:
+                raise TypeError("Missing required property 'destination_schema'")
+            __props__.__dict__["destination_schema"] = destination_schema
             if group_id is None and not opts.urn:
                 raise TypeError("Missing required property 'group_id'")
             __props__.__dict__["group_id"] = group_id
             if pause_after_trial is None and not opts.urn:
                 raise TypeError("Missing required property 'pause_after_trial'")
             __props__.__dict__["pause_after_trial"] = pause_after_trial
             if paused is None and not opts.urn:
                 raise TypeError("Missing required property 'paused'")
             __props__.__dict__["paused"] = paused
             __props__.__dict__["run_setup_tests"] = run_setup_tests
-            if schema is None and not opts.urn:
-                raise TypeError("Missing required property 'schema'")
-            __props__.__dict__["schema"] = schema
             if service is None and not opts.urn:
                 raise TypeError("Missing required property 'service'")
             __props__.__dict__["service"] = service
             if sync_frequency is None and not opts.urn:
                 raise TypeError("Missing required property 'sync_frequency'")
             __props__.__dict__["sync_frequency"] = sync_frequency
             __props__.__dict__["trust_certificates"] = trust_certificates
             __props__.__dict__["trust_fingerprints"] = trust_fingerprints
             __props__.__dict__["connected_by"] = None
             __props__.__dict__["created_at"] = None
             __props__.__dict__["failed_at"] = None
             __props__.__dict__["last_updated"] = None
+            __props__.__dict__["name"] = None
             __props__.__dict__["schedule_type"] = None
             __props__.__dict__["service_version"] = None
             __props__.__dict__["statuses"] = None
             __props__.__dict__["succeeded_at"] = None
         super(Connector, __self__).__init__(
             'fivetran:index/connector:Connector',
             resource_name,
@@ -492,22 +532,24 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             auth: Optional[pulumi.Input[pulumi.InputType['ConnectorAuthArgs']]] = None,
             config: Optional[pulumi.Input[pulumi.InputType['ConnectorConfigArgs']]] = None,
             connected_by: Optional[pulumi.Input[str]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
+            daily_sync_time: Optional[pulumi.Input[str]] = None,
+            destination_schema: Optional[pulumi.Input[pulumi.InputType['ConnectorDestinationSchemaArgs']]] = None,
             failed_at: Optional[pulumi.Input[str]] = None,
             group_id: Optional[pulumi.Input[str]] = None,
             last_updated: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
             pause_after_trial: Optional[pulumi.Input[str]] = None,
             paused: Optional[pulumi.Input[str]] = None,
             run_setup_tests: Optional[pulumi.Input[str]] = None,
             schedule_type: Optional[pulumi.Input[str]] = None,
-            schema: Optional[pulumi.Input[str]] = None,
             service: Optional[pulumi.Input[str]] = None,
             service_version: Optional[pulumi.Input[str]] = None,
             statuses: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ConnectorStatusArgs']]]]] = None,
             succeeded_at: Optional[pulumi.Input[str]] = None,
             sync_frequency: Optional[pulumi.Input[str]] = None,
             trust_certificates: Optional[pulumi.Input[str]] = None,
             trust_fingerprints: Optional[pulumi.Input[str]] = None) -> 'Connector':
@@ -523,22 +565,24 @@
 
         __props__ = _ConnectorState.__new__(_ConnectorState)
 
         __props__.__dict__["auth"] = auth
         __props__.__dict__["config"] = config
         __props__.__dict__["connected_by"] = connected_by
         __props__.__dict__["created_at"] = created_at
+        __props__.__dict__["daily_sync_time"] = daily_sync_time
+        __props__.__dict__["destination_schema"] = destination_schema
         __props__.__dict__["failed_at"] = failed_at
         __props__.__dict__["group_id"] = group_id
         __props__.__dict__["last_updated"] = last_updated
+        __props__.__dict__["name"] = name
         __props__.__dict__["pause_after_trial"] = pause_after_trial
         __props__.__dict__["paused"] = paused
         __props__.__dict__["run_setup_tests"] = run_setup_tests
         __props__.__dict__["schedule_type"] = schedule_type
-        __props__.__dict__["schema"] = schema
         __props__.__dict__["service"] = service
         __props__.__dict__["service_version"] = service_version
         __props__.__dict__["statuses"] = statuses
         __props__.__dict__["succeeded_at"] = succeeded_at
         __props__.__dict__["sync_frequency"] = sync_frequency
         __props__.__dict__["trust_certificates"] = trust_certificates
         __props__.__dict__["trust_fingerprints"] = trust_fingerprints
@@ -561,14 +605,24 @@
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         return pulumi.get(self, "created_at")
 
     @property
+    @pulumi.getter(name="dailySyncTime")
+    def daily_sync_time(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "daily_sync_time")
+
+    @property
+    @pulumi.getter(name="destinationSchema")
+    def destination_schema(self) -> pulumi.Output['outputs.ConnectorDestinationSchema']:
+        return pulumi.get(self, "destination_schema")
+
+    @property
     @pulumi.getter(name="failedAt")
     def failed_at(self) -> pulumi.Output[str]:
         return pulumi.get(self, "failed_at")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> pulumi.Output[str]:
@@ -576,14 +630,19 @@
 
     @property
     @pulumi.getter(name="lastUpdated")
     def last_updated(self) -> pulumi.Output[str]:
         return pulumi.get(self, "last_updated")
 
     @property
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "name")
+
+    @property
     @pulumi.getter(name="pauseAfterTrial")
     def pause_after_trial(self) -> pulumi.Output[str]:
         return pulumi.get(self, "pause_after_trial")
 
     @property
     @pulumi.getter
     def paused(self) -> pulumi.Output[str]:
@@ -597,19 +656,14 @@
     @property
     @pulumi.getter(name="scheduleType")
     def schedule_type(self) -> pulumi.Output[str]:
         return pulumi.get(self, "schedule_type")
 
     @property
     @pulumi.getter
-    def schema(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "schema")
-
-    @property
-    @pulumi.getter
     def service(self) -> pulumi.Output[str]:
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter(name="serviceVersion")
     def service_version(self) -> pulumi.Output[str]:
         return pulumi.get(self, "service_version")
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/destination.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_connector.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,45 +17,51 @@
 ]
 
 @pulumi.output_type
 class GetConnectorResult:
     """
     A collection of values returned by getConnector.
     """
-    def __init__(__self__, configs=None, connected_by=None, created_at=None, failed_at=None, group_id=None, id=None, pause_after_trial=None, paused=None, schedule_type=None, schema=None, service=None, service_version=None, statuses=None, succeeded_at=None, sync_frequency=None):
+    def __init__(__self__, configs=None, connected_by=None, created_at=None, daily_sync_time=None, destination_schemas=None, failed_at=None, group_id=None, id=None, name=None, pause_after_trial=None, paused=None, schedule_type=None, service=None, service_version=None, statuses=None, succeeded_at=None, sync_frequency=None):
         if configs and not isinstance(configs, list):
             raise TypeError("Expected argument 'configs' to be a list")
         pulumi.set(__self__, "configs", configs)
         if connected_by and not isinstance(connected_by, str):
             raise TypeError("Expected argument 'connected_by' to be a str")
         pulumi.set(__self__, "connected_by", connected_by)
         if created_at and not isinstance(created_at, str):
             raise TypeError("Expected argument 'created_at' to be a str")
         pulumi.set(__self__, "created_at", created_at)
+        if daily_sync_time and not isinstance(daily_sync_time, str):
+            raise TypeError("Expected argument 'daily_sync_time' to be a str")
+        pulumi.set(__self__, "daily_sync_time", daily_sync_time)
+        if destination_schemas and not isinstance(destination_schemas, list):
+            raise TypeError("Expected argument 'destination_schemas' to be a list")
+        pulumi.set(__self__, "destination_schemas", destination_schemas)
         if failed_at and not isinstance(failed_at, str):
             raise TypeError("Expected argument 'failed_at' to be a str")
         pulumi.set(__self__, "failed_at", failed_at)
         if group_id and not isinstance(group_id, str):
             raise TypeError("Expected argument 'group_id' to be a str")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
         if pause_after_trial and not isinstance(pause_after_trial, str):
             raise TypeError("Expected argument 'pause_after_trial' to be a str")
         pulumi.set(__self__, "pause_after_trial", pause_after_trial)
         if paused and not isinstance(paused, str):
             raise TypeError("Expected argument 'paused' to be a str")
         pulumi.set(__self__, "paused", paused)
         if schedule_type and not isinstance(schedule_type, str):
             raise TypeError("Expected argument 'schedule_type' to be a str")
         pulumi.set(__self__, "schedule_type", schedule_type)
-        if schema and not isinstance(schema, str):
-            raise TypeError("Expected argument 'schema' to be a str")
-        pulumi.set(__self__, "schema", schema)
         if service and not isinstance(service, str):
             raise TypeError("Expected argument 'service' to be a str")
         pulumi.set(__self__, "service", service)
         if service_version and not isinstance(service_version, str):
             raise TypeError("Expected argument 'service_version' to be a str")
         pulumi.set(__self__, "service_version", service_version)
         if statuses and not isinstance(statuses, list):
@@ -80,14 +86,24 @@
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> str:
         return pulumi.get(self, "created_at")
 
     @property
+    @pulumi.getter(name="dailySyncTime")
+    def daily_sync_time(self) -> str:
+        return pulumi.get(self, "daily_sync_time")
+
+    @property
+    @pulumi.getter(name="destinationSchemas")
+    def destination_schemas(self) -> Sequence['outputs.GetConnectorDestinationSchemaResult']:
+        return pulumi.get(self, "destination_schemas")
+
+    @property
     @pulumi.getter(name="failedAt")
     def failed_at(self) -> str:
         return pulumi.get(self, "failed_at")
 
     @property
     @pulumi.getter(name="groupId")
     def group_id(self) -> str:
@@ -95,14 +111,19 @@
 
     @property
     @pulumi.getter
     def id(self) -> str:
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
     @pulumi.getter(name="pauseAfterTrial")
     def pause_after_trial(self) -> str:
         return pulumi.get(self, "pause_after_trial")
 
     @property
     @pulumi.getter
     def paused(self) -> str:
@@ -111,19 +132,14 @@
     @property
     @pulumi.getter(name="scheduleType")
     def schedule_type(self) -> str:
         return pulumi.get(self, "schedule_type")
 
     @property
     @pulumi.getter
-    def schema(self) -> str:
-        return pulumi.get(self, "schema")
-
-    @property
-    @pulumi.getter
     def service(self) -> str:
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter(name="serviceVersion")
     def service_version(self) -> str:
         return pulumi.get(self, "service_version")
@@ -149,21 +165,23 @@
     def __await__(self):
         if False:
             yield self
         return GetConnectorResult(
             configs=self.configs,
             connected_by=self.connected_by,
             created_at=self.created_at,
+            daily_sync_time=self.daily_sync_time,
+            destination_schemas=self.destination_schemas,
             failed_at=self.failed_at,
             group_id=self.group_id,
             id=self.id,
+            name=self.name,
             pause_after_trial=self.pause_after_trial,
             paused=self.paused,
             schedule_type=self.schedule_type,
-            schema=self.schema,
             service=self.service,
             service_version=self.service_version,
             statuses=self.statuses,
             succeeded_at=self.succeeded_at,
             sync_frequency=self.sync_frequency)
 
 
@@ -180,21 +198,23 @@
         opts.version = _utilities.get_version()
     __ret__ = pulumi.runtime.invoke('fivetran:index/getConnector:getConnector', __args__, opts=opts, typ=GetConnectorResult).value
 
     return AwaitableGetConnectorResult(
         configs=__ret__.configs,
         connected_by=__ret__.connected_by,
         created_at=__ret__.created_at,
+        daily_sync_time=__ret__.daily_sync_time,
+        destination_schemas=__ret__.destination_schemas,
         failed_at=__ret__.failed_at,
         group_id=__ret__.group_id,
         id=__ret__.id,
+        name=__ret__.name,
         pause_after_trial=__ret__.pause_after_trial,
         paused=__ret__.paused,
         schedule_type=__ret__.schedule_type,
-        schema=__ret__.schema,
         service=__ret__.service,
         service_version=__ret__.service_version,
         statuses=__ret__.statuses,
         succeeded_at=__ret__.succeeded_at,
         sync_frequency=__ret__.sync_frequency)
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_connectors_metadata.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_connectors_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_destination.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_destination.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_group.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_group_connectors.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_group_connectors.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_group_users.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_groups.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_user.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 
 @pulumi.output_type
 class GetUserResult:
     """
     A collection of values returned by getUser.
     """
-    def __init__(__self__, created_at=None, email=None, family_name=None, given_name=None, id=None, invited=None, logged_in_at=None, phone=None, picture=None, verified=None):
+    def __init__(__self__, created_at=None, email=None, family_name=None, given_name=None, id=None, invited=None, logged_in_at=None, phone=None, picture=None, role=None, verified=None):
         if created_at and not isinstance(created_at, str):
             raise TypeError("Expected argument 'created_at' to be a str")
         pulumi.set(__self__, "created_at", created_at)
         if email and not isinstance(email, str):
             raise TypeError("Expected argument 'email' to be a str")
         pulumi.set(__self__, "email", email)
         if family_name and not isinstance(family_name, str):
@@ -44,14 +44,17 @@
         pulumi.set(__self__, "logged_in_at", logged_in_at)
         if phone and not isinstance(phone, str):
             raise TypeError("Expected argument 'phone' to be a str")
         pulumi.set(__self__, "phone", phone)
         if picture and not isinstance(picture, str):
             raise TypeError("Expected argument 'picture' to be a str")
         pulumi.set(__self__, "picture", picture)
+        if role and not isinstance(role, str):
+            raise TypeError("Expected argument 'role' to be a str")
+        pulumi.set(__self__, "role", role)
         if verified and not isinstance(verified, bool):
             raise TypeError("Expected argument 'verified' to be a bool")
         pulumi.set(__self__, "verified", verified)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> str:
@@ -95,14 +98,19 @@
     @property
     @pulumi.getter
     def picture(self) -> str:
         return pulumi.get(self, "picture")
 
     @property
     @pulumi.getter
+    def role(self) -> str:
+        return pulumi.get(self, "role")
+
+    @property
+    @pulumi.getter
     def verified(self) -> bool:
         return pulumi.get(self, "verified")
 
 
 class AwaitableGetUserResult(GetUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
@@ -114,14 +122,15 @@
             family_name=self.family_name,
             given_name=self.given_name,
             id=self.id,
             invited=self.invited,
             logged_in_at=self.logged_in_at,
             phone=self.phone,
             picture=self.picture,
+            role=self.role,
             verified=self.verified)
 
 
 def get_user(id: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Use this data source to access information about an existing resource.
@@ -140,14 +149,15 @@
         family_name=__ret__.family_name,
         given_name=__ret__.given_name,
         id=__ret__.id,
         invited=__ret__.invited,
         logged_in_at=__ret__.logged_in_at,
         phone=__ret__.phone,
         picture=__ret__.picture,
+        role=__ret__.role,
         verified=__ret__.verified)
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/get_users.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/group.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/group.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,92 +3,63 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
-from ._inputs import *
 
 __all__ = ['GroupArgs', 'Group']
 
 @pulumi.input_type
 class GroupArgs:
     def __init__(__self__, *,
-                 name: Optional[pulumi.Input[str]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['GroupUserArgs']]]] = None):
+                 name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Group resource.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GroupUserArgs']]]]:
-        return pulumi.get(self, "users")
-
-    @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GroupUserArgs']]]]):
-        pulumi.set(self, "users", value)
-
 
 @pulumi.input_type
 class _GroupState:
     def __init__(__self__, *,
                  created_at: Optional[pulumi.Input[str]] = None,
-                 creator: Optional[pulumi.Input[str]] = None,
                  last_updated: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input['GroupUserArgs']]]] = None):
+                 name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Group resources.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
-        if creator is not None:
-            pulumi.set(__self__, "creator", creator)
         if last_updated is not None:
             pulumi.set(__self__, "last_updated", last_updated)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if users is not None:
-            pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "created_at")
 
     @created_at.setter
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
-    @pulumi.getter
-    def creator(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "creator")
-
-    @creator.setter
-    def creator(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "creator", value)
-
-    @property
     @pulumi.getter(name="lastUpdated")
     def last_updated(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "last_updated")
 
     @last_updated.setter
     def last_updated(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "last_updated", value)
@@ -98,31 +69,21 @@
     def name(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
-    @property
-    @pulumi.getter
-    def users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['GroupUserArgs']]]]:
-        return pulumi.get(self, "users")
-
-    @users.setter
-    def users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['GroupUserArgs']]]]):
-        pulumi.set(self, "users", value)
-
 
 class Group(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupUserArgs']]]]] = None,
                  __props__=None):
         """
         Create a Group resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -145,84 +106,67 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 users: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupUserArgs']]]]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GroupArgs.__new__(GroupArgs)
 
             __props__.__dict__["name"] = name
-            __props__.__dict__["users"] = users
             __props__.__dict__["created_at"] = None
-            __props__.__dict__["creator"] = None
             __props__.__dict__["last_updated"] = None
         super(Group, __self__).__init__(
             'fivetran:index/group:Group',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             created_at: Optional[pulumi.Input[str]] = None,
-            creator: Optional[pulumi.Input[str]] = None,
             last_updated: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            users: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['GroupUserArgs']]]]] = None) -> 'Group':
+            name: Optional[pulumi.Input[str]] = None) -> 'Group':
         """
         Get an existing Group resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupState.__new__(_GroupState)
 
         __props__.__dict__["created_at"] = created_at
-        __props__.__dict__["creator"] = creator
         __props__.__dict__["last_updated"] = last_updated
         __props__.__dict__["name"] = name
-        __props__.__dict__["users"] = users
         return Group(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         return pulumi.get(self, "created_at")
 
     @property
-    @pulumi.getter
-    def creator(self) -> pulumi.Output[str]:
-        return pulumi.get(self, "creator")
-
-    @property
     @pulumi.getter(name="lastUpdated")
     def last_updated(self) -> pulumi.Output[str]:
         return pulumi.get(self, "last_updated")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         return pulumi.get(self, "name")
 
-    @property
-    @pulumi.getter
-    def users(self) -> pulumi.Output[Optional[Sequence['outputs.GroupUser']]]:
-        return pulumi.get(self, "users")
-
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/outputs.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 from . import _utilities
 from . import outputs
 
 __all__ = [
     'ConnectorAuth',
     'ConnectorAuthClientAccess',
     'ConnectorConfig',
+    'ConnectorConfigAdobeAnalyticsConfiguration',
     'ConnectorConfigCustomTable',
     'ConnectorConfigProjectCredential',
     'ConnectorConfigReport',
+    'ConnectorDestinationSchema',
     'ConnectorStatus',
     'ConnectorStatusTask',
     'ConnectorStatusWarning',
     'DestinationConfig',
-    'GroupUser',
     'GetConnectorConfigResult',
+    'GetConnectorConfigAdobeAnalyticsConfigurationResult',
     'GetConnectorConfigCustomTableResult',
     'GetConnectorConfigProjectCredentialResult',
     'GetConnectorConfigReportResult',
+    'GetConnectorDestinationSchemaResult',
     'GetConnectorStatusResult',
     'GetConnectorStatusTaskResult',
     'GetConnectorStatusWarningResult',
     'GetConnectorsMetadataSourceResult',
     'GetDestinationConfigResult',
     'GetGroupConnectorsConnectorResult',
     'GetGroupConnectorsConnectorStatusResult',
@@ -176,28 +179,34 @@
             suggest = "account_id"
         elif key == "accountIds":
             suggest = "account_ids"
         elif key == "actionBreakdowns":
             suggest = "action_breakdowns"
         elif key == "actionReportTime":
             suggest = "action_report_time"
+        elif key == "adobeAnalyticsConfigurations":
+            suggest = "adobe_analytics_configurations"
         elif key == "advertisersIds":
             suggest = "advertisers_ids"
+        elif key == "alwaysEncrypted":
+            suggest = "always_encrypted"
         elif key == "apiAccessToken":
             suggest = "api_access_token"
         elif key == "apiKey":
             suggest = "api_key"
         elif key == "apiKeys":
             suggest = "api_keys"
         elif key == "apiQuota":
             suggest = "api_quota"
         elif key == "apiSecret":
             suggest = "api_secret"
         elif key == "apiToken":
             suggest = "api_token"
+        elif key == "apiType":
+            suggest = "api_type"
         elif key == "apiUrl":
             suggest = "api_url"
         elif key == "apiVersion":
             suggest = "api_version"
         elif key == "appSyncMode":
             suggest = "app_sync_mode"
         elif key == "appendFileOption":
@@ -208,14 +217,16 @@
             suggest = "auth_mode"
         elif key == "authType":
             suggest = "auth_type"
         elif key == "authorizationMethod":
             suggest = "authorization_method"
         elif key == "awsRegionCode":
             suggest = "aws_region_code"
+        elif key == "baseUrl":
+            suggest = "base_url"
         elif key == "bucketName":
             suggest = "bucket_name"
         elif key == "bucketService":
             suggest = "bucket_service"
         elif key == "clickAttributionWindow":
             suggest = "click_attribution_window"
         elif key == "clientId":
@@ -226,14 +237,16 @@
             suggest = "cloud_storage_type"
         elif key == "configMethod":
             suggest = "config_method"
         elif key == "configType":
             suggest = "config_type"
         elif key == "connectionString":
             suggest = "connection_string"
+        elif key == "connectionType":
+            suggest = "connection_type"
         elif key == "consumerGroup":
             suggest = "consumer_group"
         elif key == "consumerKey":
             suggest = "consumer_key"
         elif key == "consumerSecret":
             suggest = "consumer_secret"
         elif key == "containerName":
@@ -256,26 +269,34 @@
             suggest = "date_granularity"
         elif key == "dimensionAttributes":
             suggest = "dimension_attributes"
         elif key == "domainName":
             suggest = "domain_name"
         elif key == "enableAllDimensionCombinations":
             suggest = "enable_all_dimension_combinations"
+        elif key == "encryptionKey":
+            suggest = "encryption_key"
         elif key == "engagementAttributionWindow":
             suggest = "engagement_attribution_window"
+        elif key == "entityId":
+            suggest = "entity_id"
         elif key == "escapeChar":
             suggest = "escape_char"
+        elif key == "euRegion":
+            suggest = "eu_region"
         elif key == "externalId":
             suggest = "external_id"
         elif key == "fileType":
             suggest = "file_type"
         elif key == "financeAccountSyncMode":
             suggest = "finance_account_sync_mode"
         elif key == "financeAccounts":
             suggest = "finance_accounts"
+        elif key == "folderId":
+            suggest = "folder_id"
         elif key == "ftpHost":
             suggest = "ftp_host"
         elif key == "ftpPassword":
             suggest = "ftp_password"
         elif key == "ftpPort":
             suggest = "ftp_port"
         elif key == "ftpUser":
@@ -294,14 +315,18 @@
             suggest = "gcs_folder"
         elif key == "homeFolder":
             suggest = "home_folder"
         elif key == "integrationKey":
             suggest = "integration_key"
         elif key == "isFtps":
             suggest = "is_ftps"
+        elif key == "isMultiEntityFeatureEnabled":
+            suggest = "is_multi_entity_feature_enabled"
+        elif key == "isNewPackage":
+            suggest = "is_new_package"
         elif key == "isSecure":
             suggest = "is_secure"
         elif key == "latestVersion":
             suggest = "latest_version"
         elif key == "managerAccounts":
             suggest = "manager_accounts"
         elif key == "merchantId":
@@ -334,14 +359,16 @@
             suggest = "private_key"
         elif key == "projectCredentials":
             suggest = "project_credentials"
         elif key == "projectId":
             suggest = "project_id"
         elif key == "publicKey":
             suggest = "public_key"
+        elif key == "publicationName":
+            suggest = "publication_name"
         elif key == "queryId":
             suggest = "query_id"
         elif key == "replicationSlot":
             suggest = "replication_slot"
         elif key == "reportConfigurationIds":
             suggest = "report_configuration_ids"
         elif key == "reportSuites":
@@ -358,16 +385,14 @@
             suggest = "s3external_id"
         elif key == "s3roleArn":
             suggest = "s3role_arn"
         elif key == "salesAccountSyncMode":
             suggest = "sales_account_sync_mode"
         elif key == "salesAccounts":
             suggest = "sales_accounts"
-        elif key == "schemaPrefix":
-            suggest = "schema_prefix"
         elif key == "secretKey":
             suggest = "secret_key"
         elif key == "securityProtocol":
             suggest = "security_protocol"
         elif key == "selectedExports":
             suggest = "selected_exports"
         elif key == "serverUrl":
@@ -388,14 +413,16 @@
             suggest = "sheet_id"
         elif key == "siteUrls":
             suggest = "site_urls"
         elif key == "skipAfter":
             suggest = "skip_after"
         elif key == "skipBefore":
             suggest = "skip_before"
+        elif key == "soapUri":
+            suggest = "soap_uri"
         elif key == "subDomain":
             suggest = "sub_domain"
         elif key == "swipeAttributionWindow":
             suggest = "swipe_attribution_window"
         elif key == "syncDataLocker":
             suggest = "sync_data_locker"
         elif key == "syncFormat":
@@ -408,14 +435,18 @@
             suggest = "technical_account_id"
         elif key == "testTableName":
             suggest = "test_table_name"
         elif key == "timeZone":
             suggest = "time_zone"
         elif key == "timeframeMonths":
             suggest = "timeframe_months"
+        elif key == "tokenKey":
+            suggest = "token_key"
+        elif key == "tokenSecret":
+            suggest = "token_secret"
         elif key == "tunnelHost":
             suggest = "tunnel_host"
         elif key == "tunnelPort":
             suggest = "tunnel_port"
         elif key == "tunnelUser":
             suggest = "tunnel_user"
         elif key == "uniqueId":
@@ -424,14 +455,16 @@
             suggest = "update_config_on_each_sync"
         elif key == "updateMethod":
             suggest = "update_method"
         elif key == "useApiKeys":
             suggest = "use_api_keys"
         elif key == "useWebhooks":
             suggest = "use_webhooks"
+        elif key == "userId":
+            suggest = "user_id"
         elif key == "userKey":
             suggest = "user_key"
         elif key == "userName":
             suggest = "user_name"
         elif key == "userProfiles":
             suggest = "user_profiles"
         elif key == "viewAttributionWindow":
@@ -453,52 +486,57 @@
     def __init__(__self__, *,
                  abs_connection_string: Optional[str] = None,
                  abs_container_name: Optional[str] = None,
                  access_key_id: Optional[str] = None,
                  access_token: Optional[str] = None,
                  account: Optional[str] = None,
                  account_id: Optional[str] = None,
-                 account_ids: Optional[str] = None,
+                 account_ids: Optional[Sequence[str]] = None,
                  accounts: Optional[Sequence[str]] = None,
                  action_breakdowns: Optional[Sequence[str]] = None,
                  action_report_time: Optional[str] = None,
+                 adobe_analytics_configurations: Optional[Sequence['outputs.ConnectorConfigAdobeAnalyticsConfiguration']] = None,
                  advertisables: Optional[Sequence[str]] = None,
                  advertisers: Optional[Sequence[str]] = None,
                  advertisers_ids: Optional[Sequence[str]] = None,
                  aggregation: Optional[str] = None,
+                 always_encrypted: Optional[str] = None,
                  api_access_token: Optional[str] = None,
                  api_key: Optional[str] = None,
-                 api_keys: Optional[str] = None,
+                 api_keys: Optional[Sequence[str]] = None,
                  api_quota: Optional[str] = None,
                  api_secret: Optional[str] = None,
                  api_token: Optional[str] = None,
+                 api_type: Optional[str] = None,
                  api_url: Optional[str] = None,
                  api_version: Optional[str] = None,
                  app_sync_mode: Optional[str] = None,
                  append_file_option: Optional[str] = None,
                  apps: Optional[Sequence[str]] = None,
                  archive_pattern: Optional[str] = None,
                  auth_mode: Optional[str] = None,
                  auth_type: Optional[str] = None,
                  authorization_method: Optional[str] = None,
                  aws_region_code: Optional[str] = None,
+                 base_url: Optional[str] = None,
                  breakdowns: Optional[Sequence[str]] = None,
                  bucket: Optional[str] = None,
                  bucket_name: Optional[str] = None,
                  bucket_service: Optional[str] = None,
                  certificate: Optional[str] = None,
                  click_attribution_window: Optional[str] = None,
                  client_id: Optional[str] = None,
                  client_secret: Optional[str] = None,
                  cloud_storage_type: Optional[str] = None,
                  columns: Optional[Sequence[str]] = None,
                  compression: Optional[str] = None,
                  config_method: Optional[str] = None,
                  config_type: Optional[str] = None,
                  connection_string: Optional[str] = None,
+                 connection_type: Optional[str] = None,
                  consumer_group: Optional[str] = None,
                  consumer_key: Optional[str] = None,
                  consumer_secret: Optional[str] = None,
                  container_name: Optional[str] = None,
                  conversion_report_time: Optional[str] = None,
                  conversion_window_size: Optional[str] = None,
                  custom_tables: Optional[Sequence['outputs.ConnectorConfigCustomTable']] = None,
@@ -513,22 +551,26 @@
                  dimension_attributes: Optional[Sequence[str]] = None,
                  dimensions: Optional[Sequence[str]] = None,
                  domain: Optional[str] = None,
                  domain_name: Optional[str] = None,
                  elements: Optional[Sequence[str]] = None,
                  email: Optional[str] = None,
                  enable_all_dimension_combinations: Optional[str] = None,
+                 encryption_key: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  engagement_attribution_window: Optional[str] = None,
+                 entity_id: Optional[str] = None,
                  escape_char: Optional[str] = None,
+                 eu_region: Optional[str] = None,
                  external_id: Optional[str] = None,
                  fields: Optional[Sequence[str]] = None,
                  file_type: Optional[str] = None,
                  finance_account_sync_mode: Optional[str] = None,
                  finance_accounts: Optional[Sequence[str]] = None,
+                 folder_id: Optional[str] = None,
                  ftp_host: Optional[str] = None,
                  ftp_password: Optional[str] = None,
                  ftp_port: Optional[str] = None,
                  ftp_user: Optional[str] = None,
                  function: Optional[str] = None,
                  function_app: Optional[str] = None,
                  function_key: Optional[str] = None,
@@ -539,14 +581,16 @@
                  home_folder: Optional[str] = None,
                  host: Optional[str] = None,
                  hosts: Optional[Sequence[str]] = None,
                  identity: Optional[str] = None,
                  instance: Optional[str] = None,
                  integration_key: Optional[str] = None,
                  is_ftps: Optional[str] = None,
+                 is_multi_entity_feature_enabled: Optional[str] = None,
+                 is_new_package: Optional[str] = None,
                  is_secure: Optional[str] = None,
                  key: Optional[str] = None,
                  last_synced_changes_utc: Optional[str] = None,
                  latest_version: Optional[str] = None,
                  manager_accounts: Optional[Sequence[str]] = None,
                  merchant_id: Optional[str] = None,
                  message_type: Optional[str] = None,
@@ -558,27 +602,29 @@
                  oauth_token_secret: Optional[str] = None,
                  on_error: Optional[str] = None,
                  on_premise: Optional[str] = None,
                  organization_id: Optional[str] = None,
                  organizations: Optional[Sequence[str]] = None,
                  pages: Optional[Sequence[str]] = None,
                  password: Optional[str] = None,
+                 pat: Optional[str] = None,
                  path: Optional[str] = None,
                  pattern: Optional[str] = None,
                  pem_certificate: Optional[str] = None,
                  port: Optional[str] = None,
                  post_click_attribution_window_size: Optional[str] = None,
                  prebuilt_report: Optional[str] = None,
                  prefix: Optional[str] = None,
                  private_key: Optional[str] = None,
                  profiles: Optional[Sequence[str]] = None,
                  project_credentials: Optional[Sequence['outputs.ConnectorConfigProjectCredential']] = None,
                  project_id: Optional[str] = None,
                  projects: Optional[Sequence[str]] = None,
                  public_key: Optional[str] = None,
+                 publication_name: Optional[str] = None,
                  query_id: Optional[str] = None,
                  region: Optional[str] = None,
                  replication_slot: Optional[str] = None,
                  report_configuration_ids: Optional[Sequence[str]] = None,
                  report_suites: Optional[Sequence[str]] = None,
                  report_type: Optional[str] = None,
                  report_url: Optional[str] = None,
@@ -589,16 +635,14 @@
                  role_arn: Optional[str] = None,
                  s3bucket: Optional[str] = None,
                  s3external_id: Optional[str] = None,
                  s3folder: Optional[str] = None,
                  s3role_arn: Optional[str] = None,
                  sales_account_sync_mode: Optional[str] = None,
                  sales_accounts: Optional[Sequence[str]] = None,
-                 schema: Optional[str] = None,
-                 schema_prefix: Optional[str] = None,
                  secret: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  secrets: Optional[str] = None,
                  security_protocol: Optional[str] = None,
                  selected_exports: Optional[Sequence[str]] = None,
                  server_url: Optional[str] = None,
                  servers: Optional[str] = None,
@@ -610,36 +654,39 @@
                  sftp_user: Optional[str] = None,
                  sheet_id: Optional[str] = None,
                  shop: Optional[str] = None,
                  sid: Optional[str] = None,
                  site_urls: Optional[Sequence[str]] = None,
                  skip_after: Optional[str] = None,
                  skip_before: Optional[str] = None,
+                 soap_uri: Optional[str] = None,
                  source: Optional[str] = None,
                  sub_domain: Optional[str] = None,
                  subdomain: Optional[str] = None,
                  swipe_attribution_window: Optional[str] = None,
                  sync_data_locker: Optional[str] = None,
                  sync_format: Optional[str] = None,
                  sync_mode: Optional[str] = None,
                  sync_type: Optional[str] = None,
-                 table: Optional[str] = None,
                  technical_account_id: Optional[str] = None,
                  test_table_name: Optional[str] = None,
                  time_zone: Optional[str] = None,
                  timeframe_months: Optional[str] = None,
+                 token_key: Optional[str] = None,
+                 token_secret: Optional[str] = None,
                  tunnel_host: Optional[str] = None,
                  tunnel_port: Optional[str] = None,
                  tunnel_user: Optional[str] = None,
                  unique_id: Optional[str] = None,
                  update_config_on_each_sync: Optional[str] = None,
                  update_method: Optional[str] = None,
                  use_api_keys: Optional[str] = None,
                  use_webhooks: Optional[str] = None,
                  user: Optional[str] = None,
+                 user_id: Optional[str] = None,
                  user_key: Optional[str] = None,
                  user_name: Optional[str] = None,
                  user_profiles: Optional[Sequence[str]] = None,
                  username: Optional[str] = None,
                  view_attribution_window: Optional[str] = None,
                  view_through_attribution_window_size: Optional[str] = None):
         if abs_connection_string is not None:
@@ -658,34 +705,40 @@
             pulumi.set(__self__, "account_ids", account_ids)
         if accounts is not None:
             pulumi.set(__self__, "accounts", accounts)
         if action_breakdowns is not None:
             pulumi.set(__self__, "action_breakdowns", action_breakdowns)
         if action_report_time is not None:
             pulumi.set(__self__, "action_report_time", action_report_time)
+        if adobe_analytics_configurations is not None:
+            pulumi.set(__self__, "adobe_analytics_configurations", adobe_analytics_configurations)
         if advertisables is not None:
             pulumi.set(__self__, "advertisables", advertisables)
         if advertisers is not None:
             pulumi.set(__self__, "advertisers", advertisers)
         if advertisers_ids is not None:
             pulumi.set(__self__, "advertisers_ids", advertisers_ids)
         if aggregation is not None:
             pulumi.set(__self__, "aggregation", aggregation)
+        if always_encrypted is not None:
+            pulumi.set(__self__, "always_encrypted", always_encrypted)
         if api_access_token is not None:
             pulumi.set(__self__, "api_access_token", api_access_token)
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if api_keys is not None:
             pulumi.set(__self__, "api_keys", api_keys)
         if api_quota is not None:
             pulumi.set(__self__, "api_quota", api_quota)
         if api_secret is not None:
             pulumi.set(__self__, "api_secret", api_secret)
         if api_token is not None:
             pulumi.set(__self__, "api_token", api_token)
+        if api_type is not None:
+            pulumi.set(__self__, "api_type", api_type)
         if api_url is not None:
             pulumi.set(__self__, "api_url", api_url)
         if api_version is not None:
             pulumi.set(__self__, "api_version", api_version)
         if app_sync_mode is not None:
             pulumi.set(__self__, "app_sync_mode", app_sync_mode)
         if append_file_option is not None:
@@ -698,14 +751,16 @@
             pulumi.set(__self__, "auth_mode", auth_mode)
         if auth_type is not None:
             pulumi.set(__self__, "auth_type", auth_type)
         if authorization_method is not None:
             pulumi.set(__self__, "authorization_method", authorization_method)
         if aws_region_code is not None:
             pulumi.set(__self__, "aws_region_code", aws_region_code)
+        if base_url is not None:
+            pulumi.set(__self__, "base_url", base_url)
         if breakdowns is not None:
             pulumi.set(__self__, "breakdowns", breakdowns)
         if bucket is not None:
             pulumi.set(__self__, "bucket", bucket)
         if bucket_name is not None:
             pulumi.set(__self__, "bucket_name", bucket_name)
         if bucket_service is not None:
@@ -726,14 +781,16 @@
             pulumi.set(__self__, "compression", compression)
         if config_method is not None:
             pulumi.set(__self__, "config_method", config_method)
         if config_type is not None:
             pulumi.set(__self__, "config_type", config_type)
         if connection_string is not None:
             pulumi.set(__self__, "connection_string", connection_string)
+        if connection_type is not None:
+            pulumi.set(__self__, "connection_type", connection_type)
         if consumer_group is not None:
             pulumi.set(__self__, "consumer_group", consumer_group)
         if consumer_key is not None:
             pulumi.set(__self__, "consumer_key", consumer_key)
         if consumer_secret is not None:
             pulumi.set(__self__, "consumer_secret", consumer_secret)
         if container_name is not None:
@@ -770,30 +827,38 @@
             pulumi.set(__self__, "domain_name", domain_name)
         if elements is not None:
             pulumi.set(__self__, "elements", elements)
         if email is not None:
             pulumi.set(__self__, "email", email)
         if enable_all_dimension_combinations is not None:
             pulumi.set(__self__, "enable_all_dimension_combinations", enable_all_dimension_combinations)
+        if encryption_key is not None:
+            pulumi.set(__self__, "encryption_key", encryption_key)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if engagement_attribution_window is not None:
             pulumi.set(__self__, "engagement_attribution_window", engagement_attribution_window)
+        if entity_id is not None:
+            pulumi.set(__self__, "entity_id", entity_id)
         if escape_char is not None:
             pulumi.set(__self__, "escape_char", escape_char)
+        if eu_region is not None:
+            pulumi.set(__self__, "eu_region", eu_region)
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
         if fields is not None:
             pulumi.set(__self__, "fields", fields)
         if file_type is not None:
             pulumi.set(__self__, "file_type", file_type)
         if finance_account_sync_mode is not None:
             pulumi.set(__self__, "finance_account_sync_mode", finance_account_sync_mode)
         if finance_accounts is not None:
             pulumi.set(__self__, "finance_accounts", finance_accounts)
+        if folder_id is not None:
+            pulumi.set(__self__, "folder_id", folder_id)
         if ftp_host is not None:
             pulumi.set(__self__, "ftp_host", ftp_host)
         if ftp_password is not None:
             pulumi.set(__self__, "ftp_password", ftp_password)
         if ftp_port is not None:
             pulumi.set(__self__, "ftp_port", ftp_port)
         if ftp_user is not None:
@@ -822,14 +887,18 @@
             pulumi.set(__self__, "identity", identity)
         if instance is not None:
             pulumi.set(__self__, "instance", instance)
         if integration_key is not None:
             pulumi.set(__self__, "integration_key", integration_key)
         if is_ftps is not None:
             pulumi.set(__self__, "is_ftps", is_ftps)
+        if is_multi_entity_feature_enabled is not None:
+            pulumi.set(__self__, "is_multi_entity_feature_enabled", is_multi_entity_feature_enabled)
+        if is_new_package is not None:
+            pulumi.set(__self__, "is_new_package", is_new_package)
         if is_secure is not None:
             pulumi.set(__self__, "is_secure", is_secure)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if last_synced_changes_utc is not None:
             pulumi.set(__self__, "last_synced_changes_utc", last_synced_changes_utc)
         if latest_version is not None:
@@ -860,14 +929,16 @@
             pulumi.set(__self__, "organization_id", organization_id)
         if organizations is not None:
             pulumi.set(__self__, "organizations", organizations)
         if pages is not None:
             pulumi.set(__self__, "pages", pages)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if pat is not None:
+            pulumi.set(__self__, "pat", pat)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if pattern is not None:
             pulumi.set(__self__, "pattern", pattern)
         if pem_certificate is not None:
             pulumi.set(__self__, "pem_certificate", pem_certificate)
         if port is not None:
@@ -886,14 +957,16 @@
             pulumi.set(__self__, "project_credentials", project_credentials)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
         if projects is not None:
             pulumi.set(__self__, "projects", projects)
         if public_key is not None:
             pulumi.set(__self__, "public_key", public_key)
+        if publication_name is not None:
+            pulumi.set(__self__, "publication_name", publication_name)
         if query_id is not None:
             pulumi.set(__self__, "query_id", query_id)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if replication_slot is not None:
             pulumi.set(__self__, "replication_slot", replication_slot)
         if report_configuration_ids is not None:
@@ -922,18 +995,14 @@
             pulumi.set(__self__, "s3folder", s3folder)
         if s3role_arn is not None:
             pulumi.set(__self__, "s3role_arn", s3role_arn)
         if sales_account_sync_mode is not None:
             pulumi.set(__self__, "sales_account_sync_mode", sales_account_sync_mode)
         if sales_accounts is not None:
             pulumi.set(__self__, "sales_accounts", sales_accounts)
-        if schema is not None:
-            pulumi.set(__self__, "schema", schema)
-        if schema_prefix is not None:
-            pulumi.set(__self__, "schema_prefix", schema_prefix)
         if secret is not None:
             pulumi.set(__self__, "secret", secret)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if secrets is not None:
             pulumi.set(__self__, "secrets", secrets)
         if security_protocol is not None:
@@ -964,14 +1033,16 @@
             pulumi.set(__self__, "sid", sid)
         if site_urls is not None:
             pulumi.set(__self__, "site_urls", site_urls)
         if skip_after is not None:
             pulumi.set(__self__, "skip_after", skip_after)
         if skip_before is not None:
             pulumi.set(__self__, "skip_before", skip_before)
+        if soap_uri is not None:
+            pulumi.set(__self__, "soap_uri", soap_uri)
         if source is not None:
             pulumi.set(__self__, "source", source)
         if sub_domain is not None:
             pulumi.set(__self__, "sub_domain", sub_domain)
         if subdomain is not None:
             pulumi.set(__self__, "subdomain", subdomain)
         if swipe_attribution_window is not None:
@@ -980,24 +1051,26 @@
             pulumi.set(__self__, "sync_data_locker", sync_data_locker)
         if sync_format is not None:
             pulumi.set(__self__, "sync_format", sync_format)
         if sync_mode is not None:
             pulumi.set(__self__, "sync_mode", sync_mode)
         if sync_type is not None:
             pulumi.set(__self__, "sync_type", sync_type)
-        if table is not None:
-            pulumi.set(__self__, "table", table)
         if technical_account_id is not None:
             pulumi.set(__self__, "technical_account_id", technical_account_id)
         if test_table_name is not None:
             pulumi.set(__self__, "test_table_name", test_table_name)
         if time_zone is not None:
             pulumi.set(__self__, "time_zone", time_zone)
         if timeframe_months is not None:
             pulumi.set(__self__, "timeframe_months", timeframe_months)
+        if token_key is not None:
+            pulumi.set(__self__, "token_key", token_key)
+        if token_secret is not None:
+            pulumi.set(__self__, "token_secret", token_secret)
         if tunnel_host is not None:
             pulumi.set(__self__, "tunnel_host", tunnel_host)
         if tunnel_port is not None:
             pulumi.set(__self__, "tunnel_port", tunnel_port)
         if tunnel_user is not None:
             pulumi.set(__self__, "tunnel_user", tunnel_user)
         if unique_id is not None:
@@ -1008,14 +1081,16 @@
             pulumi.set(__self__, "update_method", update_method)
         if use_api_keys is not None:
             pulumi.set(__self__, "use_api_keys", use_api_keys)
         if use_webhooks is not None:
             pulumi.set(__self__, "use_webhooks", use_webhooks)
         if user is not None:
             pulumi.set(__self__, "user", user)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
         if user_key is not None:
             pulumi.set(__self__, "user_key", user_key)
         if user_name is not None:
             pulumi.set(__self__, "user_name", user_name)
         if user_profiles is not None:
             pulumi.set(__self__, "user_profiles", user_profiles)
         if username is not None:
@@ -1053,15 +1128,15 @@
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> Optional[str]:
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter(name="accountIds")
-    def account_ids(self) -> Optional[str]:
+    def account_ids(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "account_ids")
 
     @property
     @pulumi.getter
     def accounts(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "accounts")
 
@@ -1072,14 +1147,19 @@
 
     @property
     @pulumi.getter(name="actionReportTime")
     def action_report_time(self) -> Optional[str]:
         return pulumi.get(self, "action_report_time")
 
     @property
+    @pulumi.getter(name="adobeAnalyticsConfigurations")
+    def adobe_analytics_configurations(self) -> Optional[Sequence['outputs.ConnectorConfigAdobeAnalyticsConfiguration']]:
+        return pulumi.get(self, "adobe_analytics_configurations")
+
+    @property
     @pulumi.getter
     def advertisables(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "advertisables")
 
     @property
     @pulumi.getter
     def advertisers(self) -> Optional[Sequence[str]]:
@@ -1092,26 +1172,31 @@
 
     @property
     @pulumi.getter
     def aggregation(self) -> Optional[str]:
         return pulumi.get(self, "aggregation")
 
     @property
+    @pulumi.getter(name="alwaysEncrypted")
+    def always_encrypted(self) -> Optional[str]:
+        return pulumi.get(self, "always_encrypted")
+
+    @property
     @pulumi.getter(name="apiAccessToken")
     def api_access_token(self) -> Optional[str]:
         return pulumi.get(self, "api_access_token")
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> Optional[str]:
         return pulumi.get(self, "api_key")
 
     @property
     @pulumi.getter(name="apiKeys")
-    def api_keys(self) -> Optional[str]:
+    def api_keys(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "api_keys")
 
     @property
     @pulumi.getter(name="apiQuota")
     def api_quota(self) -> Optional[str]:
         return pulumi.get(self, "api_quota")
 
@@ -1122,14 +1207,19 @@
 
     @property
     @pulumi.getter(name="apiToken")
     def api_token(self) -> Optional[str]:
         return pulumi.get(self, "api_token")
 
     @property
+    @pulumi.getter(name="apiType")
+    def api_type(self) -> Optional[str]:
+        return pulumi.get(self, "api_type")
+
+    @property
     @pulumi.getter(name="apiUrl")
     def api_url(self) -> Optional[str]:
         return pulumi.get(self, "api_url")
 
     @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> Optional[str]:
@@ -1172,14 +1262,19 @@
 
     @property
     @pulumi.getter(name="awsRegionCode")
     def aws_region_code(self) -> Optional[str]:
         return pulumi.get(self, "aws_region_code")
 
     @property
+    @pulumi.getter(name="baseUrl")
+    def base_url(self) -> Optional[str]:
+        return pulumi.get(self, "base_url")
+
+    @property
     @pulumi.getter
     def breakdowns(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "breakdowns")
 
     @property
     @pulumi.getter
     def bucket(self) -> Optional[str]:
@@ -1242,14 +1337,19 @@
 
     @property
     @pulumi.getter(name="connectionString")
     def connection_string(self) -> Optional[str]:
         return pulumi.get(self, "connection_string")
 
     @property
+    @pulumi.getter(name="connectionType")
+    def connection_type(self) -> Optional[str]:
+        return pulumi.get(self, "connection_type")
+
+    @property
     @pulumi.getter(name="consumerGroup")
     def consumer_group(self) -> Optional[str]:
         return pulumi.get(self, "consumer_group")
 
     @property
     @pulumi.getter(name="consumerKey")
     def consumer_key(self) -> Optional[str]:
@@ -1352,29 +1452,44 @@
 
     @property
     @pulumi.getter(name="enableAllDimensionCombinations")
     def enable_all_dimension_combinations(self) -> Optional[str]:
         return pulumi.get(self, "enable_all_dimension_combinations")
 
     @property
+    @pulumi.getter(name="encryptionKey")
+    def encryption_key(self) -> Optional[str]:
+        return pulumi.get(self, "encryption_key")
+
+    @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="engagementAttributionWindow")
     def engagement_attribution_window(self) -> Optional[str]:
         return pulumi.get(self, "engagement_attribution_window")
 
     @property
+    @pulumi.getter(name="entityId")
+    def entity_id(self) -> Optional[str]:
+        return pulumi.get(self, "entity_id")
+
+    @property
     @pulumi.getter(name="escapeChar")
     def escape_char(self) -> Optional[str]:
         return pulumi.get(self, "escape_char")
 
     @property
+    @pulumi.getter(name="euRegion")
+    def eu_region(self) -> Optional[str]:
+        return pulumi.get(self, "eu_region")
+
+    @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> Optional[str]:
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter
     def fields(self) -> Optional[Sequence[str]]:
@@ -1392,14 +1507,19 @@
 
     @property
     @pulumi.getter(name="financeAccounts")
     def finance_accounts(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "finance_accounts")
 
     @property
+    @pulumi.getter(name="folderId")
+    def folder_id(self) -> Optional[str]:
+        return pulumi.get(self, "folder_id")
+
+    @property
     @pulumi.getter(name="ftpHost")
     def ftp_host(self) -> Optional[str]:
         return pulumi.get(self, "ftp_host")
 
     @property
     @pulumi.getter(name="ftpPassword")
     def ftp_password(self) -> Optional[str]:
@@ -1482,14 +1602,24 @@
 
     @property
     @pulumi.getter(name="isFtps")
     def is_ftps(self) -> Optional[str]:
         return pulumi.get(self, "is_ftps")
 
     @property
+    @pulumi.getter(name="isMultiEntityFeatureEnabled")
+    def is_multi_entity_feature_enabled(self) -> Optional[str]:
+        return pulumi.get(self, "is_multi_entity_feature_enabled")
+
+    @property
+    @pulumi.getter(name="isNewPackage")
+    def is_new_package(self) -> Optional[str]:
+        return pulumi.get(self, "is_new_package")
+
+    @property
     @pulumi.getter(name="isSecure")
     def is_secure(self) -> Optional[str]:
         return pulumi.get(self, "is_secure")
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
@@ -1578,14 +1708,19 @@
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
+    def pat(self) -> Optional[str]:
+        return pulumi.get(self, "pat")
+
+    @property
+    @pulumi.getter
     def path(self) -> Optional[str]:
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def pattern(self) -> Optional[str]:
         return pulumi.get(self, "pattern")
@@ -1642,14 +1777,19 @@
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> Optional[str]:
         return pulumi.get(self, "public_key")
 
     @property
+    @pulumi.getter(name="publicationName")
+    def publication_name(self) -> Optional[str]:
+        return pulumi.get(self, "publication_name")
+
+    @property
     @pulumi.getter(name="queryId")
     def query_id(self) -> Optional[str]:
         return pulumi.get(self, "query_id")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
@@ -1733,24 +1873,14 @@
     @property
     @pulumi.getter(name="salesAccounts")
     def sales_accounts(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "sales_accounts")
 
     @property
     @pulumi.getter
-    def schema(self) -> Optional[str]:
-        return pulumi.get(self, "schema")
-
-    @property
-    @pulumi.getter(name="schemaPrefix")
-    def schema_prefix(self) -> Optional[str]:
-        return pulumi.get(self, "schema_prefix")
-
-    @property
-    @pulumi.getter
     def secret(self) -> Optional[str]:
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
         return pulumi.get(self, "secret_key")
@@ -1837,14 +1967,19 @@
 
     @property
     @pulumi.getter(name="skipBefore")
     def skip_before(self) -> Optional[str]:
         return pulumi.get(self, "skip_before")
 
     @property
+    @pulumi.getter(name="soapUri")
+    def soap_uri(self) -> Optional[str]:
+        return pulumi.get(self, "soap_uri")
+
+    @property
     @pulumi.getter
     def source(self) -> Optional[str]:
         return pulumi.get(self, "source")
 
     @property
     @pulumi.getter(name="subDomain")
     def sub_domain(self) -> Optional[str]:
@@ -1877,19 +2012,14 @@
 
     @property
     @pulumi.getter(name="syncType")
     def sync_type(self) -> Optional[str]:
         return pulumi.get(self, "sync_type")
 
     @property
-    @pulumi.getter
-    def table(self) -> Optional[str]:
-        return pulumi.get(self, "table")
-
-    @property
     @pulumi.getter(name="technicalAccountId")
     def technical_account_id(self) -> Optional[str]:
         return pulumi.get(self, "technical_account_id")
 
     @property
     @pulumi.getter(name="testTableName")
     def test_table_name(self) -> Optional[str]:
@@ -1902,14 +2032,24 @@
 
     @property
     @pulumi.getter(name="timeframeMonths")
     def timeframe_months(self) -> Optional[str]:
         return pulumi.get(self, "timeframe_months")
 
     @property
+    @pulumi.getter(name="tokenKey")
+    def token_key(self) -> Optional[str]:
+        return pulumi.get(self, "token_key")
+
+    @property
+    @pulumi.getter(name="tokenSecret")
+    def token_secret(self) -> Optional[str]:
+        return pulumi.get(self, "token_secret")
+
+    @property
     @pulumi.getter(name="tunnelHost")
     def tunnel_host(self) -> Optional[str]:
         return pulumi.get(self, "tunnel_host")
 
     @property
     @pulumi.getter(name="tunnelPort")
     def tunnel_port(self) -> Optional[str]:
@@ -1947,14 +2087,19 @@
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         return pulumi.get(self, "user")
 
     @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[str]:
+        return pulumi.get(self, "user_id")
+
+    @property
     @pulumi.getter(name="userKey")
     def user_key(self) -> Optional[str]:
         return pulumi.get(self, "user_key")
 
     @property
     @pulumi.getter(name="userName")
     def user_name(self) -> Optional[str]:
@@ -1978,14 +2123,88 @@
     @property
     @pulumi.getter(name="viewThroughAttributionWindowSize")
     def view_through_attribution_window_size(self) -> Optional[str]:
         return pulumi.get(self, "view_through_attribution_window_size")
 
 
 @pulumi.output_type
+class ConnectorConfigAdobeAnalyticsConfiguration(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "calculatedMetrics":
+            suggest = "calculated_metrics"
+        elif key == "reportSuites":
+            suggest = "report_suites"
+        elif key == "syncMode":
+            suggest = "sync_mode"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ConnectorConfigAdobeAnalyticsConfiguration. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ConnectorConfigAdobeAnalyticsConfiguration.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ConnectorConfigAdobeAnalyticsConfiguration.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 calculated_metrics: Optional[Sequence[str]] = None,
+                 elements: Optional[Sequence[str]] = None,
+                 metrics: Optional[Sequence[str]] = None,
+                 report_suites: Optional[Sequence[str]] = None,
+                 segments: Optional[Sequence[str]] = None,
+                 sync_mode: Optional[str] = None):
+        if calculated_metrics is not None:
+            pulumi.set(__self__, "calculated_metrics", calculated_metrics)
+        if elements is not None:
+            pulumi.set(__self__, "elements", elements)
+        if metrics is not None:
+            pulumi.set(__self__, "metrics", metrics)
+        if report_suites is not None:
+            pulumi.set(__self__, "report_suites", report_suites)
+        if segments is not None:
+            pulumi.set(__self__, "segments", segments)
+        if sync_mode is not None:
+            pulumi.set(__self__, "sync_mode", sync_mode)
+
+    @property
+    @pulumi.getter(name="calculatedMetrics")
+    def calculated_metrics(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "calculated_metrics")
+
+    @property
+    @pulumi.getter
+    def elements(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "elements")
+
+    @property
+    @pulumi.getter
+    def metrics(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "metrics")
+
+    @property
+    @pulumi.getter(name="reportSuites")
+    def report_suites(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "report_suites")
+
+    @property
+    @pulumi.getter
+    def segments(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "segments")
+
+    @property
+    @pulumi.getter(name="syncMode")
+    def sync_mode(self) -> Optional[str]:
+        return pulumi.get(self, "sync_mode")
+
+
+@pulumi.output_type
 class ConnectorConfigCustomTable(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "actionBreakdowns":
             suggest = "action_breakdowns"
         elif key == "actionReportTime":
@@ -2238,14 +2457,43 @@
     @property
     @pulumi.getter
     def table(self) -> Optional[str]:
         return pulumi.get(self, "table")
 
 
 @pulumi.output_type
+class ConnectorDestinationSchema(dict):
+    def __init__(__self__, *,
+                 name: Optional[str] = None,
+                 prefix: Optional[str] = None,
+                 table: Optional[str] = None):
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if prefix is not None:
+            pulumi.set(__self__, "prefix", prefix)
+        if table is not None:
+            pulumi.set(__self__, "table", table)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def prefix(self) -> Optional[str]:
+        return pulumi.get(self, "prefix")
+
+    @property
+    @pulumi.getter
+    def table(self) -> Optional[str]:
+        return pulumi.get(self, "table")
+
+
+@pulumi.output_type
 class ConnectorStatus(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "isHistoricalSync":
             suggest = "is_historical_sync"
         elif key == "setupState":
@@ -2362,28 +2610,36 @@
 @pulumi.output_type
 class DestinationConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "authType":
             suggest = "auth_type"
+        elif key == "clusterId":
+            suggest = "cluster_id"
+        elif key == "clusterRegion":
+            suggest = "cluster_region"
         elif key == "connectionType":
             suggest = "connection_type"
         elif key == "createExternalTables":
             suggest = "create_external_tables"
         elif key == "dataSetLocation":
             suggest = "data_set_location"
         elif key == "externalLocation":
             suggest = "external_location"
         elif key == "httpPath":
             suggest = "http_path"
         elif key == "personalAccessToken":
             suggest = "personal_access_token"
+        elif key == "privateKey":
+            suggest = "private_key"
         elif key == "projectId":
             suggest = "project_id"
+        elif key == "publicKey":
+            suggest = "public_key"
         elif key == "roleArn":
             suggest = "role_arn"
         elif key == "secretKey":
             suggest = "secret_key"
         elif key == "serverHostName":
             suggest = "server_host_name"
         elif key == "tunnelHost":
@@ -2404,38 +2660,46 @@
         DestinationConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  auth: Optional[str] = None,
                  auth_type: Optional[str] = None,
                  bucket: Optional[str] = None,
+                 cluster_id: Optional[str] = None,
+                 cluster_region: Optional[str] = None,
                  connection_type: Optional[str] = None,
                  create_external_tables: Optional[str] = None,
                  data_set_location: Optional[str] = None,
                  database: Optional[str] = None,
                  external_location: Optional[str] = None,
                  host: Optional[str] = None,
                  http_path: Optional[str] = None,
                  password: Optional[str] = None,
                  personal_access_token: Optional[str] = None,
                  port: Optional[int] = None,
+                 private_key: Optional[str] = None,
                  project_id: Optional[str] = None,
+                 public_key: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  secret_key: Optional[str] = None,
                  server_host_name: Optional[str] = None,
                  tunnel_host: Optional[str] = None,
                  tunnel_port: Optional[str] = None,
                  tunnel_user: Optional[str] = None,
                  user: Optional[str] = None):
         if auth is not None:
             pulumi.set(__self__, "auth", auth)
         if auth_type is not None:
             pulumi.set(__self__, "auth_type", auth_type)
         if bucket is not None:
             pulumi.set(__self__, "bucket", bucket)
+        if cluster_id is not None:
+            pulumi.set(__self__, "cluster_id", cluster_id)
+        if cluster_region is not None:
+            pulumi.set(__self__, "cluster_region", cluster_region)
         if connection_type is not None:
             pulumi.set(__self__, "connection_type", connection_type)
         if create_external_tables is not None:
             pulumi.set(__self__, "create_external_tables", create_external_tables)
         if data_set_location is not None:
             pulumi.set(__self__, "data_set_location", data_set_location)
         if database is not None:
@@ -2448,16 +2712,20 @@
             pulumi.set(__self__, "http_path", http_path)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if personal_access_token is not None:
             pulumi.set(__self__, "personal_access_token", personal_access_token)
         if port is not None:
             pulumi.set(__self__, "port", port)
+        if private_key is not None:
+            pulumi.set(__self__, "private_key", private_key)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
+        if public_key is not None:
+            pulumi.set(__self__, "public_key", public_key)
         if role_arn is not None:
             pulumi.set(__self__, "role_arn", role_arn)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
         if server_host_name is not None:
             pulumi.set(__self__, "server_host_name", server_host_name)
         if tunnel_host is not None:
@@ -2481,14 +2749,24 @@
 
     @property
     @pulumi.getter
     def bucket(self) -> Optional[str]:
         return pulumi.get(self, "bucket")
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> Optional[str]:
+        return pulumi.get(self, "cluster_id")
+
+    @property
+    @pulumi.getter(name="clusterRegion")
+    def cluster_region(self) -> Optional[str]:
+        return pulumi.get(self, "cluster_region")
+
+    @property
     @pulumi.getter(name="connectionType")
     def connection_type(self) -> Optional[str]:
         return pulumi.get(self, "connection_type")
 
     @property
     @pulumi.getter(name="createExternalTables")
     def create_external_tables(self) -> Optional[str]:
@@ -2531,19 +2809,29 @@
 
     @property
     @pulumi.getter
     def port(self) -> Optional[int]:
         return pulumi.get(self, "port")
 
     @property
+    @pulumi.getter(name="privateKey")
+    def private_key(self) -> Optional[str]:
+        return pulumi.get(self, "private_key")
+
+    @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[str]:
         return pulumi.get(self, "project_id")
 
     @property
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> Optional[str]:
+        return pulumi.get(self, "public_key")
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
@@ -2572,79 +2860,65 @@
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         return pulumi.get(self, "user")
 
 
 @pulumi.output_type
-class GroupUser(dict):
-    def __init__(__self__, *,
-                 id: str,
-                 role: str):
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "role", role)
-
-    @property
-    @pulumi.getter
-    def id(self) -> str:
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter
-    def role(self) -> str:
-        return pulumi.get(self, "role")
-
-
-@pulumi.output_type
 class GetConnectorConfigResult(dict):
     def __init__(__self__, *,
                  abs_connection_string: str,
                  abs_container_name: str,
                  access_key_id: str,
                  access_token: str,
                  account: str,
                  account_id: str,
-                 account_ids: str,
+                 account_ids: Sequence[str],
                  accounts: Sequence[str],
                  action_breakdowns: Sequence[str],
                  action_report_time: str,
+                 adobe_analytics_configurations: Sequence['outputs.GetConnectorConfigAdobeAnalyticsConfigurationResult'],
                  advertisables: Sequence[str],
                  advertisers: Sequence[str],
                  advertisers_ids: Sequence[str],
                  aggregation: str,
+                 always_encrypted: str,
                  api_access_token: str,
                  api_key: str,
                  api_keys: str,
                  api_quota: str,
                  api_secret: str,
                  api_token: str,
+                 api_type: str,
                  api_url: str,
                  api_version: str,
                  app_sync_mode: str,
                  append_file_option: str,
                  apps: Sequence[str],
                  archive_pattern: str,
                  auth_mode: str,
                  auth_type: str,
                  authorization_method: str,
                  aws_region_code: str,
+                 base_url: str,
                  breakdowns: Sequence[str],
                  bucket: str,
                  bucket_name: str,
                  bucket_service: str,
                  certificate: str,
                  click_attribution_window: str,
                  client_id: str,
                  client_secret: str,
                  cloud_storage_type: str,
                  columns: Sequence[str],
                  compression: str,
                  config_method: str,
                  config_type: str,
                  connection_string: str,
+                 connection_type: str,
                  consumer_group: str,
                  consumer_key: str,
                  consumer_secret: str,
                  container_name: str,
                  conversion_report_time: str,
                  conversion_window_size: str,
                  custom_tables: Sequence['outputs.GetConnectorConfigCustomTableResult'],
@@ -2659,22 +2933,26 @@
                  dimension_attributes: Sequence[str],
                  dimensions: Sequence[str],
                  domain: str,
                  domain_name: str,
                  elements: Sequence[str],
                  email: str,
                  enable_all_dimension_combinations: str,
+                 encryption_key: str,
                  endpoint: str,
                  engagement_attribution_window: str,
+                 entity_id: str,
                  escape_char: str,
+                 eu_region: str,
                  external_id: str,
                  fields: Sequence[str],
                  file_type: str,
                  finance_account_sync_mode: str,
                  finance_accounts: Sequence[str],
+                 folder_id: str,
                  ftp_host: str,
                  ftp_password: str,
                  ftp_port: str,
                  ftp_user: str,
                  function: str,
                  function_app: str,
                  function_key: str,
@@ -2685,14 +2963,16 @@
                  home_folder: str,
                  host: str,
                  hosts: Sequence[str],
                  identity: str,
                  instance: str,
                  integration_key: str,
                  is_ftps: str,
+                 is_multi_entity_feature_enabled: str,
+                 is_new_package: str,
                  is_secure: str,
                  key: str,
                  last_synced_changes_utc: str,
                  latest_version: str,
                  manager_accounts: Sequence[str],
                  merchant_id: str,
                  message_type: str,
@@ -2704,27 +2984,29 @@
                  oauth_token_secret: str,
                  on_error: str,
                  on_premise: str,
                  organization_id: str,
                  organizations: Sequence[str],
                  pages: Sequence[str],
                  password: str,
+                 pat: str,
                  path: str,
                  pattern: str,
                  pem_certificate: str,
                  port: str,
                  post_click_attribution_window_size: str,
                  prebuilt_report: str,
                  prefix: str,
                  private_key: str,
                  profiles: Sequence[str],
                  project_credentials: Sequence['outputs.GetConnectorConfigProjectCredentialResult'],
                  project_id: str,
                  projects: Sequence[str],
                  public_key: str,
+                 publication_name: str,
                  query_id: str,
                  region: str,
                  replication_slot: str,
                  report_configuration_ids: Sequence[str],
                  report_suites: Sequence[str],
                  report_type: str,
                  report_url: str,
@@ -2735,16 +3017,14 @@
                  role_arn: str,
                  s3bucket: str,
                  s3external_id: str,
                  s3folder: str,
                  s3role_arn: str,
                  sales_account_sync_mode: str,
                  sales_accounts: Sequence[str],
-                 schema: str,
-                 schema_prefix: str,
                  secret: str,
                  secret_key: str,
                  secrets: str,
                  security_protocol: str,
                  selected_exports: Sequence[str],
                  server_url: str,
                  servers: str,
@@ -2756,36 +3036,40 @@
                  sftp_user: str,
                  sheet_id: str,
                  shop: str,
                  sid: str,
                  site_urls: Sequence[str],
                  skip_after: str,
                  skip_before: str,
+                 soap_uri: str,
                  source: str,
                  sub_domain: str,
                  subdomain: str,
                  swipe_attribution_window: str,
                  sync_data_locker: str,
                  sync_format: str,
                  sync_mode: str,
                  sync_type: str,
                  table: str,
                  technical_account_id: str,
                  test_table_name: str,
                  time_zone: str,
                  timeframe_months: str,
+                 token_key: str,
+                 token_secret: str,
                  tunnel_host: str,
                  tunnel_port: str,
                  tunnel_user: str,
                  unique_id: str,
                  update_config_on_each_sync: str,
                  update_method: str,
                  use_api_keys: str,
                  use_webhooks: str,
                  user: str,
+                 user_id: str,
                  user_key: str,
                  user_name: str,
                  user_profiles: Sequence[str],
                  username: str,
                  view_attribution_window: str,
                  view_through_attribution_window_size: str):
         pulumi.set(__self__, "abs_connection_string", abs_connection_string)
@@ -2794,48 +3078,53 @@
         pulumi.set(__self__, "access_token", access_token)
         pulumi.set(__self__, "account", account)
         pulumi.set(__self__, "account_id", account_id)
         pulumi.set(__self__, "account_ids", account_ids)
         pulumi.set(__self__, "accounts", accounts)
         pulumi.set(__self__, "action_breakdowns", action_breakdowns)
         pulumi.set(__self__, "action_report_time", action_report_time)
+        pulumi.set(__self__, "adobe_analytics_configurations", adobe_analytics_configurations)
         pulumi.set(__self__, "advertisables", advertisables)
         pulumi.set(__self__, "advertisers", advertisers)
         pulumi.set(__self__, "advertisers_ids", advertisers_ids)
         pulumi.set(__self__, "aggregation", aggregation)
+        pulumi.set(__self__, "always_encrypted", always_encrypted)
         pulumi.set(__self__, "api_access_token", api_access_token)
         pulumi.set(__self__, "api_key", api_key)
         pulumi.set(__self__, "api_keys", api_keys)
         pulumi.set(__self__, "api_quota", api_quota)
         pulumi.set(__self__, "api_secret", api_secret)
         pulumi.set(__self__, "api_token", api_token)
+        pulumi.set(__self__, "api_type", api_type)
         pulumi.set(__self__, "api_url", api_url)
         pulumi.set(__self__, "api_version", api_version)
         pulumi.set(__self__, "app_sync_mode", app_sync_mode)
         pulumi.set(__self__, "append_file_option", append_file_option)
         pulumi.set(__self__, "apps", apps)
         pulumi.set(__self__, "archive_pattern", archive_pattern)
         pulumi.set(__self__, "auth_mode", auth_mode)
         pulumi.set(__self__, "auth_type", auth_type)
         pulumi.set(__self__, "authorization_method", authorization_method)
         pulumi.set(__self__, "aws_region_code", aws_region_code)
+        pulumi.set(__self__, "base_url", base_url)
         pulumi.set(__self__, "breakdowns", breakdowns)
         pulumi.set(__self__, "bucket", bucket)
         pulumi.set(__self__, "bucket_name", bucket_name)
         pulumi.set(__self__, "bucket_service", bucket_service)
         pulumi.set(__self__, "certificate", certificate)
         pulumi.set(__self__, "click_attribution_window", click_attribution_window)
         pulumi.set(__self__, "client_id", client_id)
         pulumi.set(__self__, "client_secret", client_secret)
         pulumi.set(__self__, "cloud_storage_type", cloud_storage_type)
         pulumi.set(__self__, "columns", columns)
         pulumi.set(__self__, "compression", compression)
         pulumi.set(__self__, "config_method", config_method)
         pulumi.set(__self__, "config_type", config_type)
         pulumi.set(__self__, "connection_string", connection_string)
+        pulumi.set(__self__, "connection_type", connection_type)
         pulumi.set(__self__, "consumer_group", consumer_group)
         pulumi.set(__self__, "consumer_key", consumer_key)
         pulumi.set(__self__, "consumer_secret", consumer_secret)
         pulumi.set(__self__, "container_name", container_name)
         pulumi.set(__self__, "conversion_report_time", conversion_report_time)
         pulumi.set(__self__, "conversion_window_size", conversion_window_size)
         pulumi.set(__self__, "custom_tables", custom_tables)
@@ -2850,22 +3139,26 @@
         pulumi.set(__self__, "dimension_attributes", dimension_attributes)
         pulumi.set(__self__, "dimensions", dimensions)
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "domain_name", domain_name)
         pulumi.set(__self__, "elements", elements)
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "enable_all_dimension_combinations", enable_all_dimension_combinations)
+        pulumi.set(__self__, "encryption_key", encryption_key)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "engagement_attribution_window", engagement_attribution_window)
+        pulumi.set(__self__, "entity_id", entity_id)
         pulumi.set(__self__, "escape_char", escape_char)
+        pulumi.set(__self__, "eu_region", eu_region)
         pulumi.set(__self__, "external_id", external_id)
         pulumi.set(__self__, "fields", fields)
         pulumi.set(__self__, "file_type", file_type)
         pulumi.set(__self__, "finance_account_sync_mode", finance_account_sync_mode)
         pulumi.set(__self__, "finance_accounts", finance_accounts)
+        pulumi.set(__self__, "folder_id", folder_id)
         pulumi.set(__self__, "ftp_host", ftp_host)
         pulumi.set(__self__, "ftp_password", ftp_password)
         pulumi.set(__self__, "ftp_port", ftp_port)
         pulumi.set(__self__, "ftp_user", ftp_user)
         pulumi.set(__self__, "function", function)
         pulumi.set(__self__, "function_app", function_app)
         pulumi.set(__self__, "function_key", function_key)
@@ -2876,14 +3169,16 @@
         pulumi.set(__self__, "home_folder", home_folder)
         pulumi.set(__self__, "host", host)
         pulumi.set(__self__, "hosts", hosts)
         pulumi.set(__self__, "identity", identity)
         pulumi.set(__self__, "instance", instance)
         pulumi.set(__self__, "integration_key", integration_key)
         pulumi.set(__self__, "is_ftps", is_ftps)
+        pulumi.set(__self__, "is_multi_entity_feature_enabled", is_multi_entity_feature_enabled)
+        pulumi.set(__self__, "is_new_package", is_new_package)
         pulumi.set(__self__, "is_secure", is_secure)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "last_synced_changes_utc", last_synced_changes_utc)
         pulumi.set(__self__, "latest_version", latest_version)
         pulumi.set(__self__, "manager_accounts", manager_accounts)
         pulumi.set(__self__, "merchant_id", merchant_id)
         pulumi.set(__self__, "message_type", message_type)
@@ -2895,27 +3190,29 @@
         pulumi.set(__self__, "oauth_token_secret", oauth_token_secret)
         pulumi.set(__self__, "on_error", on_error)
         pulumi.set(__self__, "on_premise", on_premise)
         pulumi.set(__self__, "organization_id", organization_id)
         pulumi.set(__self__, "organizations", organizations)
         pulumi.set(__self__, "pages", pages)
         pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "pat", pat)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "pattern", pattern)
         pulumi.set(__self__, "pem_certificate", pem_certificate)
         pulumi.set(__self__, "port", port)
         pulumi.set(__self__, "post_click_attribution_window_size", post_click_attribution_window_size)
         pulumi.set(__self__, "prebuilt_report", prebuilt_report)
         pulumi.set(__self__, "prefix", prefix)
         pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "profiles", profiles)
         pulumi.set(__self__, "project_credentials", project_credentials)
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "projects", projects)
         pulumi.set(__self__, "public_key", public_key)
+        pulumi.set(__self__, "publication_name", publication_name)
         pulumi.set(__self__, "query_id", query_id)
         pulumi.set(__self__, "region", region)
         pulumi.set(__self__, "replication_slot", replication_slot)
         pulumi.set(__self__, "report_configuration_ids", report_configuration_ids)
         pulumi.set(__self__, "report_suites", report_suites)
         pulumi.set(__self__, "report_type", report_type)
         pulumi.set(__self__, "report_url", report_url)
@@ -2926,16 +3223,14 @@
         pulumi.set(__self__, "role_arn", role_arn)
         pulumi.set(__self__, "s3bucket", s3bucket)
         pulumi.set(__self__, "s3external_id", s3external_id)
         pulumi.set(__self__, "s3folder", s3folder)
         pulumi.set(__self__, "s3role_arn", s3role_arn)
         pulumi.set(__self__, "sales_account_sync_mode", sales_account_sync_mode)
         pulumi.set(__self__, "sales_accounts", sales_accounts)
-        pulumi.set(__self__, "schema", schema)
-        pulumi.set(__self__, "schema_prefix", schema_prefix)
         pulumi.set(__self__, "secret", secret)
         pulumi.set(__self__, "secret_key", secret_key)
         pulumi.set(__self__, "secrets", secrets)
         pulumi.set(__self__, "security_protocol", security_protocol)
         pulumi.set(__self__, "selected_exports", selected_exports)
         pulumi.set(__self__, "server_url", server_url)
         pulumi.set(__self__, "servers", servers)
@@ -2947,36 +3242,40 @@
         pulumi.set(__self__, "sftp_user", sftp_user)
         pulumi.set(__self__, "sheet_id", sheet_id)
         pulumi.set(__self__, "shop", shop)
         pulumi.set(__self__, "sid", sid)
         pulumi.set(__self__, "site_urls", site_urls)
         pulumi.set(__self__, "skip_after", skip_after)
         pulumi.set(__self__, "skip_before", skip_before)
+        pulumi.set(__self__, "soap_uri", soap_uri)
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "sub_domain", sub_domain)
         pulumi.set(__self__, "subdomain", subdomain)
         pulumi.set(__self__, "swipe_attribution_window", swipe_attribution_window)
         pulumi.set(__self__, "sync_data_locker", sync_data_locker)
         pulumi.set(__self__, "sync_format", sync_format)
         pulumi.set(__self__, "sync_mode", sync_mode)
         pulumi.set(__self__, "sync_type", sync_type)
         pulumi.set(__self__, "table", table)
         pulumi.set(__self__, "technical_account_id", technical_account_id)
         pulumi.set(__self__, "test_table_name", test_table_name)
         pulumi.set(__self__, "time_zone", time_zone)
         pulumi.set(__self__, "timeframe_months", timeframe_months)
+        pulumi.set(__self__, "token_key", token_key)
+        pulumi.set(__self__, "token_secret", token_secret)
         pulumi.set(__self__, "tunnel_host", tunnel_host)
         pulumi.set(__self__, "tunnel_port", tunnel_port)
         pulumi.set(__self__, "tunnel_user", tunnel_user)
         pulumi.set(__self__, "unique_id", unique_id)
         pulumi.set(__self__, "update_config_on_each_sync", update_config_on_each_sync)
         pulumi.set(__self__, "update_method", update_method)
         pulumi.set(__self__, "use_api_keys", use_api_keys)
         pulumi.set(__self__, "use_webhooks", use_webhooks)
         pulumi.set(__self__, "user", user)
+        pulumi.set(__self__, "user_id", user_id)
         pulumi.set(__self__, "user_key", user_key)
         pulumi.set(__self__, "user_name", user_name)
         pulumi.set(__self__, "user_profiles", user_profiles)
         pulumi.set(__self__, "username", username)
         pulumi.set(__self__, "view_attribution_window", view_attribution_window)
         pulumi.set(__self__, "view_through_attribution_window_size", view_through_attribution_window_size)
 
@@ -3008,15 +3307,15 @@
     @property
     @pulumi.getter(name="accountId")
     def account_id(self) -> str:
         return pulumi.get(self, "account_id")
 
     @property
     @pulumi.getter(name="accountIds")
-    def account_ids(self) -> str:
+    def account_ids(self) -> Sequence[str]:
         return pulumi.get(self, "account_ids")
 
     @property
     @pulumi.getter
     def accounts(self) -> Sequence[str]:
         return pulumi.get(self, "accounts")
 
@@ -3027,14 +3326,19 @@
 
     @property
     @pulumi.getter(name="actionReportTime")
     def action_report_time(self) -> str:
         return pulumi.get(self, "action_report_time")
 
     @property
+    @pulumi.getter(name="adobeAnalyticsConfigurations")
+    def adobe_analytics_configurations(self) -> Sequence['outputs.GetConnectorConfigAdobeAnalyticsConfigurationResult']:
+        return pulumi.get(self, "adobe_analytics_configurations")
+
+    @property
     @pulumi.getter
     def advertisables(self) -> Sequence[str]:
         return pulumi.get(self, "advertisables")
 
     @property
     @pulumi.getter
     def advertisers(self) -> Sequence[str]:
@@ -3047,14 +3351,19 @@
 
     @property
     @pulumi.getter
     def aggregation(self) -> str:
         return pulumi.get(self, "aggregation")
 
     @property
+    @pulumi.getter(name="alwaysEncrypted")
+    def always_encrypted(self) -> str:
+        return pulumi.get(self, "always_encrypted")
+
+    @property
     @pulumi.getter(name="apiAccessToken")
     def api_access_token(self) -> str:
         return pulumi.get(self, "api_access_token")
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> str:
@@ -3077,14 +3386,19 @@
 
     @property
     @pulumi.getter(name="apiToken")
     def api_token(self) -> str:
         return pulumi.get(self, "api_token")
 
     @property
+    @pulumi.getter(name="apiType")
+    def api_type(self) -> str:
+        return pulumi.get(self, "api_type")
+
+    @property
     @pulumi.getter(name="apiUrl")
     def api_url(self) -> str:
         return pulumi.get(self, "api_url")
 
     @property
     @pulumi.getter(name="apiVersion")
     def api_version(self) -> str:
@@ -3127,14 +3441,19 @@
 
     @property
     @pulumi.getter(name="awsRegionCode")
     def aws_region_code(self) -> str:
         return pulumi.get(self, "aws_region_code")
 
     @property
+    @pulumi.getter(name="baseUrl")
+    def base_url(self) -> str:
+        return pulumi.get(self, "base_url")
+
+    @property
     @pulumi.getter
     def breakdowns(self) -> Sequence[str]:
         return pulumi.get(self, "breakdowns")
 
     @property
     @pulumi.getter
     def bucket(self) -> str:
@@ -3197,14 +3516,19 @@
 
     @property
     @pulumi.getter(name="connectionString")
     def connection_string(self) -> str:
         return pulumi.get(self, "connection_string")
 
     @property
+    @pulumi.getter(name="connectionType")
+    def connection_type(self) -> str:
+        return pulumi.get(self, "connection_type")
+
+    @property
     @pulumi.getter(name="consumerGroup")
     def consumer_group(self) -> str:
         return pulumi.get(self, "consumer_group")
 
     @property
     @pulumi.getter(name="consumerKey")
     def consumer_key(self) -> str:
@@ -3307,29 +3631,44 @@
 
     @property
     @pulumi.getter(name="enableAllDimensionCombinations")
     def enable_all_dimension_combinations(self) -> str:
         return pulumi.get(self, "enable_all_dimension_combinations")
 
     @property
+    @pulumi.getter(name="encryptionKey")
+    def encryption_key(self) -> str:
+        return pulumi.get(self, "encryption_key")
+
+    @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter(name="engagementAttributionWindow")
     def engagement_attribution_window(self) -> str:
         return pulumi.get(self, "engagement_attribution_window")
 
     @property
+    @pulumi.getter(name="entityId")
+    def entity_id(self) -> str:
+        return pulumi.get(self, "entity_id")
+
+    @property
     @pulumi.getter(name="escapeChar")
     def escape_char(self) -> str:
         return pulumi.get(self, "escape_char")
 
     @property
+    @pulumi.getter(name="euRegion")
+    def eu_region(self) -> str:
+        return pulumi.get(self, "eu_region")
+
+    @property
     @pulumi.getter(name="externalId")
     def external_id(self) -> str:
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter
     def fields(self) -> Sequence[str]:
@@ -3347,14 +3686,19 @@
 
     @property
     @pulumi.getter(name="financeAccounts")
     def finance_accounts(self) -> Sequence[str]:
         return pulumi.get(self, "finance_accounts")
 
     @property
+    @pulumi.getter(name="folderId")
+    def folder_id(self) -> str:
+        return pulumi.get(self, "folder_id")
+
+    @property
     @pulumi.getter(name="ftpHost")
     def ftp_host(self) -> str:
         return pulumi.get(self, "ftp_host")
 
     @property
     @pulumi.getter(name="ftpPassword")
     def ftp_password(self) -> str:
@@ -3437,14 +3781,24 @@
 
     @property
     @pulumi.getter(name="isFtps")
     def is_ftps(self) -> str:
         return pulumi.get(self, "is_ftps")
 
     @property
+    @pulumi.getter(name="isMultiEntityFeatureEnabled")
+    def is_multi_entity_feature_enabled(self) -> str:
+        return pulumi.get(self, "is_multi_entity_feature_enabled")
+
+    @property
+    @pulumi.getter(name="isNewPackage")
+    def is_new_package(self) -> str:
+        return pulumi.get(self, "is_new_package")
+
+    @property
     @pulumi.getter(name="isSecure")
     def is_secure(self) -> str:
         return pulumi.get(self, "is_secure")
 
     @property
     @pulumi.getter
     def key(self) -> str:
@@ -3533,14 +3887,19 @@
     @property
     @pulumi.getter
     def password(self) -> str:
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
+    def pat(self) -> str:
+        return pulumi.get(self, "pat")
+
+    @property
+    @pulumi.getter
     def path(self) -> str:
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def pattern(self) -> str:
         return pulumi.get(self, "pattern")
@@ -3597,14 +3956,19 @@
 
     @property
     @pulumi.getter(name="publicKey")
     def public_key(self) -> str:
         return pulumi.get(self, "public_key")
 
     @property
+    @pulumi.getter(name="publicationName")
+    def publication_name(self) -> str:
+        return pulumi.get(self, "publication_name")
+
+    @property
     @pulumi.getter(name="queryId")
     def query_id(self) -> str:
         return pulumi.get(self, "query_id")
 
     @property
     @pulumi.getter
     def region(self) -> str:
@@ -3688,24 +4052,14 @@
     @property
     @pulumi.getter(name="salesAccounts")
     def sales_accounts(self) -> Sequence[str]:
         return pulumi.get(self, "sales_accounts")
 
     @property
     @pulumi.getter
-    def schema(self) -> str:
-        return pulumi.get(self, "schema")
-
-    @property
-    @pulumi.getter(name="schemaPrefix")
-    def schema_prefix(self) -> str:
-        return pulumi.get(self, "schema_prefix")
-
-    @property
-    @pulumi.getter
     def secret(self) -> str:
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> str:
         return pulumi.get(self, "secret_key")
@@ -3792,14 +4146,19 @@
 
     @property
     @pulumi.getter(name="skipBefore")
     def skip_before(self) -> str:
         return pulumi.get(self, "skip_before")
 
     @property
+    @pulumi.getter(name="soapUri")
+    def soap_uri(self) -> str:
+        return pulumi.get(self, "soap_uri")
+
+    @property
     @pulumi.getter
     def source(self) -> str:
         return pulumi.get(self, "source")
 
     @property
     @pulumi.getter(name="subDomain")
     def sub_domain(self) -> str:
@@ -3857,14 +4216,24 @@
 
     @property
     @pulumi.getter(name="timeframeMonths")
     def timeframe_months(self) -> str:
         return pulumi.get(self, "timeframe_months")
 
     @property
+    @pulumi.getter(name="tokenKey")
+    def token_key(self) -> str:
+        return pulumi.get(self, "token_key")
+
+    @property
+    @pulumi.getter(name="tokenSecret")
+    def token_secret(self) -> str:
+        return pulumi.get(self, "token_secret")
+
+    @property
     @pulumi.getter(name="tunnelHost")
     def tunnel_host(self) -> str:
         return pulumi.get(self, "tunnel_host")
 
     @property
     @pulumi.getter(name="tunnelPort")
     def tunnel_port(self) -> str:
@@ -3902,14 +4271,19 @@
 
     @property
     @pulumi.getter
     def user(self) -> str:
         return pulumi.get(self, "user")
 
     @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> str:
+        return pulumi.get(self, "user_id")
+
+    @property
     @pulumi.getter(name="userKey")
     def user_key(self) -> str:
         return pulumi.get(self, "user_key")
 
     @property
     @pulumi.getter(name="userName")
     def user_name(self) -> str:
@@ -3933,14 +4307,61 @@
     @property
     @pulumi.getter(name="viewThroughAttributionWindowSize")
     def view_through_attribution_window_size(self) -> str:
         return pulumi.get(self, "view_through_attribution_window_size")
 
 
 @pulumi.output_type
+class GetConnectorConfigAdobeAnalyticsConfigurationResult(dict):
+    def __init__(__self__, *,
+                 calculated_metrics: Sequence[str],
+                 elements: Sequence[str],
+                 metrics: Sequence[str],
+                 report_suites: Sequence[str],
+                 segments: Sequence[str],
+                 sync_mode: str):
+        pulumi.set(__self__, "calculated_metrics", calculated_metrics)
+        pulumi.set(__self__, "elements", elements)
+        pulumi.set(__self__, "metrics", metrics)
+        pulumi.set(__self__, "report_suites", report_suites)
+        pulumi.set(__self__, "segments", segments)
+        pulumi.set(__self__, "sync_mode", sync_mode)
+
+    @property
+    @pulumi.getter(name="calculatedMetrics")
+    def calculated_metrics(self) -> Sequence[str]:
+        return pulumi.get(self, "calculated_metrics")
+
+    @property
+    @pulumi.getter
+    def elements(self) -> Sequence[str]:
+        return pulumi.get(self, "elements")
+
+    @property
+    @pulumi.getter
+    def metrics(self) -> Sequence[str]:
+        return pulumi.get(self, "metrics")
+
+    @property
+    @pulumi.getter(name="reportSuites")
+    def report_suites(self) -> Sequence[str]:
+        return pulumi.get(self, "report_suites")
+
+    @property
+    @pulumi.getter
+    def segments(self) -> Sequence[str]:
+        return pulumi.get(self, "segments")
+
+    @property
+    @pulumi.getter(name="syncMode")
+    def sync_mode(self) -> str:
+        return pulumi.get(self, "sync_mode")
+
+
+@pulumi.output_type
 class GetConnectorConfigCustomTableResult(dict):
     def __init__(__self__, *,
                  action_breakdowns: Sequence[str],
                  action_report_time: str,
                  aggregation: str,
                  breakdowns: Sequence[str],
                  click_attribution_window: str,
@@ -4102,14 +4523,40 @@
     @property
     @pulumi.getter
     def table(self) -> str:
         return pulumi.get(self, "table")
 
 
 @pulumi.output_type
+class GetConnectorDestinationSchemaResult(dict):
+    def __init__(__self__, *,
+                 name: str,
+                 prefix: str,
+                 table: str):
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "prefix", prefix)
+        pulumi.set(__self__, "table", table)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def prefix(self) -> str:
+        return pulumi.get(self, "prefix")
+
+    @property
+    @pulumi.getter
+    def table(self) -> str:
+        return pulumi.get(self, "table")
+
+
+@pulumi.output_type
 class GetConnectorStatusResult(dict):
     def __init__(__self__, *,
                  is_historical_sync: str,
                  setup_state: str,
                  sync_state: str,
                  tasks: Sequence['outputs.GetConnectorStatusTaskResult'],
                  update_state: str,
@@ -4246,46 +4693,54 @@
 
 @pulumi.output_type
 class GetDestinationConfigResult(dict):
     def __init__(__self__, *,
                  auth: str,
                  auth_type: str,
                  bucket: str,
+                 cluster_id: str,
+                 cluster_region: str,
                  connection_type: str,
                  create_external_tables: str,
                  data_set_location: str,
                  database: str,
                  external_location: str,
                  host: str,
                  http_path: str,
                  password: str,
                  personal_access_token: str,
                  port: int,
+                 private_key: str,
                  project_id: str,
+                 public_key: str,
                  role_arn: str,
                  secret_key: str,
                  server_host_name: str,
                  tunnel_host: str,
                  tunnel_port: str,
                  tunnel_user: str,
                  user: str):
         pulumi.set(__self__, "auth", auth)
         pulumi.set(__self__, "auth_type", auth_type)
         pulumi.set(__self__, "bucket", bucket)
+        pulumi.set(__self__, "cluster_id", cluster_id)
+        pulumi.set(__self__, "cluster_region", cluster_region)
         pulumi.set(__self__, "connection_type", connection_type)
         pulumi.set(__self__, "create_external_tables", create_external_tables)
         pulumi.set(__self__, "data_set_location", data_set_location)
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "external_location", external_location)
         pulumi.set(__self__, "host", host)
         pulumi.set(__self__, "http_path", http_path)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "personal_access_token", personal_access_token)
         pulumi.set(__self__, "port", port)
+        pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "project_id", project_id)
+        pulumi.set(__self__, "public_key", public_key)
         pulumi.set(__self__, "role_arn", role_arn)
         pulumi.set(__self__, "secret_key", secret_key)
         pulumi.set(__self__, "server_host_name", server_host_name)
         pulumi.set(__self__, "tunnel_host", tunnel_host)
         pulumi.set(__self__, "tunnel_port", tunnel_port)
         pulumi.set(__self__, "tunnel_user", tunnel_user)
         pulumi.set(__self__, "user", user)
@@ -4302,14 +4757,24 @@
 
     @property
     @pulumi.getter
     def bucket(self) -> str:
         return pulumi.get(self, "bucket")
 
     @property
+    @pulumi.getter(name="clusterId")
+    def cluster_id(self) -> str:
+        return pulumi.get(self, "cluster_id")
+
+    @property
+    @pulumi.getter(name="clusterRegion")
+    def cluster_region(self) -> str:
+        return pulumi.get(self, "cluster_region")
+
+    @property
     @pulumi.getter(name="connectionType")
     def connection_type(self) -> str:
         return pulumi.get(self, "connection_type")
 
     @property
     @pulumi.getter(name="createExternalTables")
     def create_external_tables(self) -> str:
@@ -4352,19 +4817,29 @@
 
     @property
     @pulumi.getter
     def port(self) -> int:
         return pulumi.get(self, "port")
 
     @property
+    @pulumi.getter(name="privateKey")
+    def private_key(self) -> str:
+        return pulumi.get(self, "private_key")
+
+    @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> str:
         return pulumi.get(self, "project_id")
 
     @property
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> str:
+        return pulumi.get(self, "public_key")
+
+    @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> str:
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> str:
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/provider.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran/user.py` & `pulumi_fivetran-0.1.8/pulumi_fivetran/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 @pulumi.input_type
 class UserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
                  family_name: pulumi.Input[str],
                  given_name: pulumi.Input[str],
                  phone: Optional[pulumi.Input[str]] = None,
-                 picture: Optional[pulumi.Input[str]] = None):
+                 picture: Optional[pulumi.Input[str]] = None,
+                 role: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a User resource.
         """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "family_name", family_name)
         pulumi.set(__self__, "given_name", given_name)
         if phone is not None:
             pulumi.set(__self__, "phone", phone)
         if picture is not None:
             pulumi.set(__self__, "picture", picture)
+        if role is not None:
+            pulumi.set(__self__, "role", role)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
         return pulumi.get(self, "email")
 
     @email.setter
@@ -70,27 +73,37 @@
     def picture(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "picture")
 
     @picture.setter
     def picture(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "picture", value)
 
+    @property
+    @pulumi.getter
+    def role(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role")
+
+    @role.setter
+    def role(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role", value)
+
 
 @pulumi.input_type
 class _UserState:
     def __init__(__self__, *,
                  created_at: Optional[pulumi.Input[str]] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  family_name: Optional[pulumi.Input[str]] = None,
                  given_name: Optional[pulumi.Input[str]] = None,
                  invited: Optional[pulumi.Input[bool]] = None,
                  last_updated: Optional[pulumi.Input[str]] = None,
                  logged_in_at: Optional[pulumi.Input[str]] = None,
                  phone: Optional[pulumi.Input[str]] = None,
                  picture: Optional[pulumi.Input[str]] = None,
+                 role: Optional[pulumi.Input[str]] = None,
                  verified: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering User resources.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if email is not None:
@@ -105,14 +118,16 @@
             pulumi.set(__self__, "last_updated", last_updated)
         if logged_in_at is not None:
             pulumi.set(__self__, "logged_in_at", logged_in_at)
         if phone is not None:
             pulumi.set(__self__, "phone", phone)
         if picture is not None:
             pulumi.set(__self__, "picture", picture)
+        if role is not None:
+            pulumi.set(__self__, "role", role)
         if verified is not None:
             pulumi.set(__self__, "verified", verified)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "created_at")
@@ -191,14 +206,23 @@
 
     @picture.setter
     def picture(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "picture", value)
 
     @property
     @pulumi.getter
+    def role(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role")
+
+    @role.setter
+    def role(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role", value)
+
+    @property
+    @pulumi.getter
     def verified(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "verified")
 
     @verified.setter
     def verified(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "verified", value)
 
@@ -209,14 +233,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  family_name: Optional[pulumi.Input[str]] = None,
                  given_name: Optional[pulumi.Input[str]] = None,
                  phone: Optional[pulumi.Input[str]] = None,
                  picture: Optional[pulumi.Input[str]] = None,
+                 role: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Create a User resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -243,14 +268,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  email: Optional[pulumi.Input[str]] = None,
                  family_name: Optional[pulumi.Input[str]] = None,
                  given_name: Optional[pulumi.Input[str]] = None,
                  phone: Optional[pulumi.Input[str]] = None,
                  picture: Optional[pulumi.Input[str]] = None,
+                 role: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
@@ -266,14 +292,15 @@
                 raise TypeError("Missing required property 'family_name'")
             __props__.__dict__["family_name"] = family_name
             if given_name is None and not opts.urn:
                 raise TypeError("Missing required property 'given_name'")
             __props__.__dict__["given_name"] = given_name
             __props__.__dict__["phone"] = phone
             __props__.__dict__["picture"] = picture
+            __props__.__dict__["role"] = role
             __props__.__dict__["created_at"] = None
             __props__.__dict__["invited"] = None
             __props__.__dict__["last_updated"] = None
             __props__.__dict__["logged_in_at"] = None
             __props__.__dict__["verified"] = None
         super(User, __self__).__init__(
             'fivetran:index/user:User',
@@ -290,14 +317,15 @@
             family_name: Optional[pulumi.Input[str]] = None,
             given_name: Optional[pulumi.Input[str]] = None,
             invited: Optional[pulumi.Input[bool]] = None,
             last_updated: Optional[pulumi.Input[str]] = None,
             logged_in_at: Optional[pulumi.Input[str]] = None,
             phone: Optional[pulumi.Input[str]] = None,
             picture: Optional[pulumi.Input[str]] = None,
+            role: Optional[pulumi.Input[str]] = None,
             verified: Optional[pulumi.Input[bool]] = None) -> 'User':
         """
         Get an existing User resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
@@ -312,14 +340,15 @@
         __props__.__dict__["family_name"] = family_name
         __props__.__dict__["given_name"] = given_name
         __props__.__dict__["invited"] = invited
         __props__.__dict__["last_updated"] = last_updated
         __props__.__dict__["logged_in_at"] = logged_in_at
         __props__.__dict__["phone"] = phone
         __props__.__dict__["picture"] = picture
+        __props__.__dict__["role"] = role
         __props__.__dict__["verified"] = verified
         return User(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[str]:
         return pulumi.get(self, "created_at")
@@ -362,10 +391,15 @@
     @property
     @pulumi.getter
     def picture(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "picture")
 
     @property
     @pulumi.getter
+    def role(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "role")
+
+    @property
+    @pulumi.getter
     def verified(self) -> pulumi.Output[bool]:
         return pulumi.get(self, "verified")
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/PKG-INFO` & `pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fivetran
-Version: 0.1.6
+Version: 0.1.8
 Summary: A Pulumi package for creating and managing Fivetran resources.
 Home-page: https://github.com/benesch/pulumi-fivetran
 License: Apache-2.0
 Project-URL: Repository, https://github.com/benesch/pulumi-fivetran
 Description: # Fivetran Pulumi Provider
         
         A [Pulumi](https://pulumi.com) provider for the [Fivetran] ETL platform.
```

### Comparing `pulumi_fivetran-0.1.6/pulumi_fivetran.egg-info/SOURCES.txt` & `pulumi_fivetran-0.1.8/pulumi_fivetran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fivetran-0.1.6/setup.py` & `pulumi_fivetran-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.6"
-PLUGIN_VERSION = "0.1.6"
+VERSION = "0.1.8"
+PLUGIN_VERSION = "0.1.8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'fivetran', PLUGIN_VERSION, '--server', 'https://github.com/benesch/pulumi-fivetran/releases/download/v0.1.6/'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'fivetran', PLUGIN_VERSION, '--server', 'https://github.com/benesch/pulumi-fivetran/releases/download/v0.1.8/'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the fivetran resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
```

