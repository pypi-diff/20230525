# Comparing `tmp/alvin_api_client-1.3.0rc2.tar.gz` & `tmp/alvin_api_client-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alvin_api_client-1.3.0rc2.tar", last modified: Tue Dec  6 15:05:25 2022, max compression
+gzip compressed data, was "alvin_api_client-1.4.0rc1.tar", last modified: Thu May 25 19:42:10 2023, max compression
```

## Comparing `alvin_api_client-1.3.0rc2.tar` & `alvin_api_client-1.4.0rc1.tar`

### file list

```diff
@@ -1,402 +1,500 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.598294 alvin_api_client-1.3.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.602294 alvin_api_client-1.3.0rc2/src/alvin_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.602294 alvin_api_client-1.3.0rc2/src/alvin_api_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   927873 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37082 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.606294 alvin_api_client-1.3.0rc2/src/alvin_api_client/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/accept_invite_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/admin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/airflow_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11764 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/alter_parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/alter_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/alvin_description_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/api_key_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/api_key_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/api_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_query_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_query_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15638 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/auth_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/bi_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/big_query_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/big_query_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/big_query_entity_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/body_download_search_as_file_api_v2_search_file_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/body_get_manual_entities_api_v1_manual_entities_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11680 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/bulk_search_v2_response_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12402 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/classification_match_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/classification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/client_auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/client_config_post_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11682 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/column_alter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/column_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/comparison_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/connection_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/connection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/connection_usage_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_asset_count_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_connection_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14343 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_connection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_delete_tag_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_dependency_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_dependency_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_dependency_get_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15692 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    20929 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_iddto.py
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_job_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_job_run_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    17799 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_job_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_children_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_children_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_children_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_graph_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22278 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_v2_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    22702 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_v2_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_file_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_generic_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_topic_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_numerical_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_numerical_stat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_numerical_stat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_facet_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    14329 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_job_mapping_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_job_step_mapping_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_save_tag_connection_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stat_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stats_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stats_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13002 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_manual_entity_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_aggregated_job_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_airflow_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_big_query_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_created_in.py
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_databricks_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_dbt_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    18244 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_full.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_hightouch_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12532 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_hive_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_hive_glue_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    14268 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_entity_aggregated_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_execution_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15354 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_aggregated_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_execution_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_report_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12033 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12298 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_looker_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_azure_blob_storage_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_file_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12125 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_gcs_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_generic_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_google_drive_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_kafka_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_s3_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_mode_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_mssql_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_my_sql_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_postgres_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12653 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_power_bi_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_redshift_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_snowflake_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_tableau_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_treasure_data_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    15081 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_bulk_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_bulk_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_classification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_connection_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_created_in.py
--rw-r--r--   0 runner    (1001) docker     (123)    16933 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_request_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_request_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14627 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rules_request_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14568 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_taxonomy_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_transformation_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/databricks_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/databricks_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/datadog_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/dbt_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/delete_parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/drop_parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/drop_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/element_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/email_login_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_graph_connector_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_graph_node_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_usage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/environment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/exchange_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience.py
--rw-r--r--   0 runner    (1001) docker     (123)    14171 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experiences_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/extracted_simple_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    12361 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/extracted_simple_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_data_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_match.py
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filters_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/firebase_auth_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/firebase_auth_ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/group_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/healthcheck_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hightouch_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hightouch_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_glue_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_glue_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/html_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_entity_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_platform_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_row_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_node_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_node_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_platform_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_query_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_query_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11629 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11811 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_response_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_sidebar_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_entity_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_job_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    14419 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_response_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_validation_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    11985 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_entity_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_entity_usage_stats_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    16890 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_query_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_steps_agg_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/kirby_failed_batches_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/kirby_ingest_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/known_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    14923 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/known_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/known_table_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_api_keys_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_numerical_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_run_facet_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_run_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_run_job_mapping_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stat_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stats_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_platform_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_platform_job_entity_aggregated_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_tag_connection_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_tag_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12207 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_tag_rule_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_manual_lineage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_tag_entity_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/lineage_connection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11787 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/lineage_expanding_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/lineage_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/links_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/looker_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/looker_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/looker_query_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/manual_lineage_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/manual_lineage_data_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/manual_lineage_entity_type_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/map_entity_to_url_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mode_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mode_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mssql_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mssql_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/my_sql_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/my_sql_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/onboarding_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/operator_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/organization_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/organization_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/page_data_entity_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/page_search_display_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/page_view_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_asset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_build_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_build_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11757 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/popularity_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/position.py
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/postgres_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/postgres_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/power_bi_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/power_bi_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/predefined_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/processed_lineage_graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11682 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/product_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11589 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_create_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    19119 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_lineage_parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    15318 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/redshift_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/redshift_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_element_value_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/save_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/save_search_string_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_csv_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    12901 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_display_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    13234 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13101 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_filter_label_association.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13875 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    12408 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_usage_stat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_v2_response_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_validation_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/seen_table_at_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/sheet_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/snowflake_account_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13066 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/snowflake_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/sql_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/stat_data_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/strings_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_alter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_existence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13582 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge_match_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge_match_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tableau_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tableau_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_entity_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_entity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11168 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/taxonomy_classification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tiny_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11494 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/treasure_data_additional_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/treasure_data_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tree_result_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11290 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/truncate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_activity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_activity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_activity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_invite_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_name_usage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_name_usage_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_organization_api_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_organization_api_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_persona.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/valid_data_manual_entity_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12510 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_save_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12732 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_upsert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model/views_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)    81910 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/src/alvin_api_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    27732 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.602294 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2022-12-06 15:05:25.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20554 2022-12-06 15:05:25.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 15:05:25.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 15:05:25.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-06 15:05:25.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-06 15:05:25.000000 alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/tests/integration/test_current_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:05:25.666294 alvin_api_client-1.3.0rc2/tests/request_model/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/tests/request_model/test_data_entity_usage_stats_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/tests/sqlutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2022-12-06 15:04:44.000000 alvin_api_client-1.3.0rc2/tests/test_default_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.490806 alvin_api_client-1.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 19:42:10.490806 alvin_api_client-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-25 19:42:10.490806 alvin_api_client-1.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.418805 alvin_api_client-1.4.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.422805 alvin_api_client-1.4.0rc1/src/alvin_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.422805 alvin_api_client-1.4.0rc1/src/alvin_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1067378 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37083 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.422805 alvin_api_client-1.4.0rc1/src/alvin_api_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.486806 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/accept_invite_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/admin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/aggregated_search_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/aggregated_search_orchestration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/airflow_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11764 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/alter_parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/alter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/alvin_description_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/api_key_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/api_key_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/api_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_api_lineage_models_entity_graph_connector_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_api_lineage_models_entity_graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_notifications_models_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14965 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_core_data_entity_lineage_entity_graph_connector_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_core_data_entity_lineage_entity_graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_core_data_platform_events_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_query_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_query_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/auth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/bi_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/big_query_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/big_query_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/big_query_entity_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_download_search_as_file_api_v2_search_file_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_get_dashboard_costs_api_insights_v1_dashboards_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_get_dashboard_costs_api_insights_v2_dashboards_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_get_manual_entities_api_v1_manual_entities_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/bulk_search_v2_response_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/classification_match_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/classification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/client_auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/client_config_post_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/column_alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/column_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/comparison_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/connection_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/connection_usage_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/costs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dashboard_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dashboard_costs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11884 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dashboard_costs_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dashboard_user_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dashboard_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_asset_count_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connect_nodes_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connection_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_delete_tag_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_dependency_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_dependency_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_dependency_get_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_iddto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_job_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_job_run_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17799 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_job_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_children_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_children_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_children_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_explorer_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_graph_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v2_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v2_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v3_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v3_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_file_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_generic_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_topic_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_numerical_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_numerical_stat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_numerical_stat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_facet_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_job_mapping_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_job_step_mapping_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_save_tag_connection_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_simple_lineage_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_grouped.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stat_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stats_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_user_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_user_usage_grouped.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_manual_entity_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_aggregated_job_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_airflow_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_big_query_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_created_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_databricks_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_dbt_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_hightouch_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_hive_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_hive_glue_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_costs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_entity_aggregated_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_execution_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_aggregated_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_execution_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_report_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_looker_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_azure_blob_storage_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_file_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_gcs_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_generic_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_google_drive_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_kafka_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_s3_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_mode_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_mssql_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_my_sql_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_postgres_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_power_bi_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_redshift_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_snowflake_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_tableau_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_treasure_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_bulk_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_bulk_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_classification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_connection_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_created_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16933 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_request_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_request_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rules_request_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14568 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_taxonomy_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_transformation_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/databricks_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/databricks_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/datadog_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dbt_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/delete_parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/direction_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/drop_parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/drop_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/element_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/email_login_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_events_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_graph_connector_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_graph_node_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_usage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/environment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_chart_x_asis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_chart_y_asis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_group_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_metric_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_metric_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_metric_group_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12756 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_metric_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_metric_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response_costs_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response_group_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response_group_item_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22070 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response_row_stats_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_timeline_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_type_values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_values_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_stats_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_stats_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_stats_request_stat_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/exchange_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experiences_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/extracted_simple_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/extracted_simple_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_data_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filters_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/firebase_auth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/firebase_auth_ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/get_table_num_rows_chart_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/group_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/healthcheck_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hightouch_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hightouch_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_glue_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_glue_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/html_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_entity_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15701 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_row_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_node_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_node_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_platform_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_query_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_query_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_query_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11811 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_response_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_sidebar_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_entity_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_job_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_response_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_validation_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_validation_payload_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insight_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insight_usage_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_chart_series_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_chart_x_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_chart_x_axis_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_delta_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_metric_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_request_stat_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_stats_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_entity_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_entity_usage_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16890 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_query_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_query_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_steps_agg_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/kirby_failed_batches_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/kirby_ingest_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/known_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14923 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/known_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/known_table_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_api_keys_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_numerical_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_run_facet_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_run_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_run_job_mapping_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stat_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12328 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_platform_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_platform_job_entity_aggregated_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_tag_connection_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_tag_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_tag_rule_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12276 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_insights_usage_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_manual_lineage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_organization_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_pipeline_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_tag_entity_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_connection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_expanding_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_field_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/links_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/list_event_databases_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/list_event_databases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/list_event_users_by_period_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/list_event_users_by_period_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/list_platform_databases_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/list_platform_databases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/looker_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/looker_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/looker_query_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/manual_lineage_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/manual_lineage_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/manual_lineage_entity_type_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/map_entity_to_url_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mode_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mode_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mssql_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mssql_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/my_sql_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/my_sql_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/onboarding_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/operator_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/organization_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/organization_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/organization_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/page_data_entity_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/page_search_display_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/page_view_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/pipeline_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/pipeline_run_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/pipeline_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/pipeline_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_asset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_build_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_build_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/popularity_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/postgres_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/postgres_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/power_bi_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/power_bi_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/predefined_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/processed_lineage_graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/product_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_create_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19119 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_lineage_parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15318 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/recommendation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/redshift_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/redshift_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_element_value_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/save_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/save_search_string_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_display_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_filter_label_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_usage_stat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13283 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_v2_response_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_validation_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/seen_table_at_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sheet_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/snowflake_account_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13066 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/snowflake_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sort_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/source_entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sql_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/stat_data_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/stats_agreggation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/strings_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_existence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13582 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge_match_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge_match_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tableau_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tableau_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_entity_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11168 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/taxonomy_classification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tiny_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/treasure_data_additional_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/treasure_data_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tree_result_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11290 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/truncate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/usage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_activity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_activity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_invite_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_name_usage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_name_usage_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_organization_api_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_organization_api_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/valid_data_manual_entity_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_save_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_upsert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model/views_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81910 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.486806 alvin_api_client-1.4.0rc1/src/alvin_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.422805 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 19:42:10.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-05-25 19:42:10.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:42:10.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:42:10.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 19:42:10.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 19:42:10.000000 alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.486806 alvin_api_client-1.4.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.490806 alvin_api_client-1.4.0rc1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/tests/integration/test_current_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:42:10.490806 alvin_api_client-1.4.0rc1/tests/request_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/tests/request_model/test_data_entity_usage_stats_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/tests/sqlutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-25 19:41:42.000000 alvin_api_client-1.4.0rc1/tests/test_default_api.py
```

### Comparing `alvin_api_client-1.3.0rc2/LICENSE` & `alvin_api_client-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/PKG-INFO` & `alvin_api_client-1.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alvin_api_client
-Version: 1.3.0rc2
+Version: 1.4.0rc1
 Summary: Python SDK implementing a Client of the Alvin API
 Home-page: https://github.com/alvindotai/alvin/tree/master/alvin_api_client
 Author: Alvin
 Author-email: tech@alvin.ai
 License: AGPLv3
 Project-URL: Bug Tracker, https://github.com/alvindotai/alvin/issues
 Project-URL: Source Code, https://github.com/alvindotai/alvin/tree/master/alvin_api_client
```

### Comparing `alvin_api_client-1.3.0rc2/setup.cfg` & `alvin_api_client-1.4.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = alvin_api_client
-version = 1.3.0rc2
+version = 1.4.0rc1
 description = Python SDK implementing a Client of the Alvin API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = AGPLv3
 license_files = LICENSE
 platforms = All
 author = Alvin
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/__init__.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/api/default_api.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/api/default_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,46 +20,55 @@
     file_type,
     none_type,
     validate_and_convert_types
 )
 from alvin_api_client.model.accept_invite_request import AcceptInviteRequest
 from alvin_api_client.model.admin_config import AdminConfig
 from alvin_api_client.model.alvin_description_request import AlvinDescriptionRequest
-from alvin_api_client.model.app_schemas_impact_analysis_response_impact_analysis_response import AppSchemasImpactAnalysisResponseImpactAnalysisResponse
-from alvin_api_client.model.app_schemas_impact_analysis_v3_response_impact_analysis_response import AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponse
 from alvin_api_client.model.auth_provider import AuthProvider
 from alvin_api_client.model.body_download_search_as_file_api_v2_search_file_post import BodyDownloadSearchAsFileApiV2SearchFilePost
+from alvin_api_client.model.body_get_dashboard_costs_api_insights_v1_dashboards_post import BodyGetDashboardCostsApiInsightsV1DashboardsPost
+from alvin_api_client.model.body_get_dashboard_costs_api_insights_v2_dashboards_post import BodyGetDashboardCostsApiInsightsV2DashboardsPost
+from alvin_api_client.model.body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post import BodyGetDashboardUsersCostApiInsightsV1DashboardsDashboardIdUsersPost
 from alvin_api_client.model.body_get_manual_entities_api_v1_manual_entities_post import BodyGetManualEntitiesApiV1ManualEntitiesPost
 from alvin_api_client.model.bulk_search_v2_response_payload import BulkSearchV2ResponsePayload
 from alvin_api_client.model.client_config import ClientConfig
 from alvin_api_client.model.client_config_post_auth import ClientConfigPostAuth
 from alvin_api_client.model.connection_direction import ConnectionDirection
 from alvin_api_client.model.connection_type import ConnectionType
 from alvin_api_client.model.connection_usage_classification import ConnectionUsageClassification
+from alvin_api_client.model.dashboard_costs_response import DashboardCostsResponse
+from alvin_api_client.model.dashboard_costs_v2_response import DashboardCostsV2Response
+from alvin_api_client.model.dashboard_users_response import DashboardUsersResponse
 from alvin_api_client.model.data_entity_asset_count_get import DataEntityAssetCountGet
+from alvin_api_client.model.data_entity_connect_nodes_request import DataEntityConnectNodesRequest
 from alvin_api_client.model.data_entity_delete_tag_connection_request import DataEntityDeleteTagConnectionRequest
 from alvin_api_client.model.data_entity_dependency_get import DataEntityDependencyGet
 from alvin_api_client.model.data_entity_dependency_get_list import DataEntityDependencyGetList
 from alvin_api_client.model.data_entity_get import DataEntityGet
 from alvin_api_client.model.data_entity_id import DataEntityID
 from alvin_api_client.model.data_entity_iddto import DataEntityIDDTO
 from alvin_api_client.model.data_entity_lineage_children_request import DataEntityLineageChildrenRequest
 from alvin_api_client.model.data_entity_lineage_children_response import DataEntityLineageChildrenResponse
+from alvin_api_client.model.data_entity_lineage_explorer_response import DataEntityLineageExplorerResponse
 from alvin_api_client.model.data_entity_lineage_list_request import DataEntityLineageListRequest
 from alvin_api_client.model.data_entity_lineage_list_response import DataEntityLineageListResponse
 from alvin_api_client.model.data_entity_lineage_v2_request_dto import DataEntityLineageV2RequestDTO
 from alvin_api_client.model.data_entity_lineage_v2_response import DataEntityLineageV2Response
+from alvin_api_client.model.data_entity_lineage_v3_request import DataEntityLineageV3Request
+from alvin_api_client.model.data_entity_lineage_v3_response import DataEntityLineageV3Response
 from alvin_api_client.model.data_entity_manual_file_create import DataEntityManualFileCreate
 from alvin_api_client.model.data_entity_manual_generic_create import DataEntityManualGenericCreate
 from alvin_api_client.model.data_entity_manual_topic_create import DataEntityManualTopicCreate
 from alvin_api_client.model.data_entity_manual_update import DataEntityManualUpdate
 from alvin_api_client.model.data_entity_numerical_stat_response import DataEntityNumericalStatResponse
 from alvin_api_client.model.data_entity_run_get import DataEntityRunGet
 from alvin_api_client.model.data_entity_run_job_step_mapping_get import DataEntityRunJobStepMappingGet
 from alvin_api_client.model.data_entity_save_tag_connection_request import DataEntitySaveTagConnectionRequest
+from alvin_api_client.model.data_entity_simple_lineage_response import DataEntitySimpleLineageResponse
 from alvin_api_client.model.data_entity_type import DataEntityType
 from alvin_api_client.model.data_entity_usage_stats_report import DataEntityUsageStatsReport
 from alvin_api_client.model.data_entity_usage_stats_request import DataEntityUsageStatsRequest
 from alvin_api_client.model.data_platform_airflow_create import DataPlatformAirflowCreate
 from alvin_api_client.model.data_platform_big_query_create import DataPlatformBigQueryCreate
 from alvin_api_client.model.data_platform_dbt_create import DataPlatformDBTCreate
 from alvin_api_client.model.data_platform_databricks_create import DataPlatformDatabricksCreate
@@ -96,25 +105,38 @@
 from alvin_api_client.model.data_tag_request import DataTagRequest
 from alvin_api_client.model.data_tag_request_delete import DataTagRequestDelete
 from alvin_api_client.model.data_tag_request_v2 import DataTagRequestV2
 from alvin_api_client.model.data_tag_rules_request_delete import DataTagRulesRequestDelete
 from alvin_api_client.model.data_tag_type import DataTagType
 from alvin_api_client.model.data_taxonomy_classification import DataTaxonomyClassification
 from alvin_api_client.model.email_login_request import EmailLoginRequest
+from alvin_api_client.model.event_request_filter import EventRequestFilter
+from alvin_api_client.model.event_search_request import EventSearchRequest
+from alvin_api_client.model.event_search_response import EventSearchResponse
+from alvin_api_client.model.event_search_timeline_response import EventSearchTimelineResponse
+from alvin_api_client.model.event_stats_report import EventStatsReport
+from alvin_api_client.model.event_stats_request import EventStatsRequest
+from alvin_api_client.model.event_users_response import EventUsersResponse
 from alvin_api_client.model.exchange_token_request import ExchangeTokenRequest
 from alvin_api_client.model.experience import Experience
 from alvin_api_client.model.experience_data import ExperienceData
 from alvin_api_client.model.filter_options import FilterOptions
 from alvin_api_client.model.filters_response import FiltersResponse
+from alvin_api_client.model.get_table_num_rows_chart_response import GetTableNumRowsChartResponse
 from alvin_api_client.model.http_validation_error import HTTPValidationError
 from alvin_api_client.model.healthcheck_response import HealthcheckResponse
 from alvin_api_client.model.impact_analysis_node_list_response import ImpactAnalysisNodeListResponse
 from alvin_api_client.model.impact_analysis_query_validation import ImpactAnalysisQueryValidation
 from alvin_api_client.model.impact_analysis_request import ImpactAnalysisRequest
+from alvin_api_client.model.impact_analysis_response import ImpactAnalysisResponse
 from alvin_api_client.model.impact_analysis_validation_payload import ImpactAnalysisValidationPayload
+from alvin_api_client.model.impact_analysis_validation_payload_v2 import ImpactAnalysisValidationPayloadV2
+from alvin_api_client.model.insights_delta_response import InsightsDeltaResponse
+from alvin_api_client.model.insights_request import InsightsRequest
+from alvin_api_client.model.insights_usage_request import InsightsUsageRequest
 from alvin_api_client.model.job_entity_usage_stats_report import JobEntityUsageStatsReport
 from alvin_api_client.model.job_query_request import JobQueryRequest
 from alvin_api_client.model.job_query_v1_response import JobQueryV1Response
 from alvin_api_client.model.kirby_failed_batches_response import KirbyFailedBatchesResponse
 from alvin_api_client.model.kirby_ingest_request import KirbyIngestRequest
 from alvin_api_client.model.limit_offset_page_api_keys_response import LimitOffsetPageAPIKeysResponse
 from alvin_api_client.model.limit_offset_page_data_entity_get import LimitOffsetPageDataEntityGet
@@ -125,26 +147,39 @@
 from alvin_api_client.model.limit_offset_page_data_entity_usage_stat_raw import LimitOffsetPageDataEntityUsageStatRaw
 from alvin_api_client.model.limit_offset_page_data_entity_usage_stats_report import LimitOffsetPageDataEntityUsageStatsReport
 from alvin_api_client.model.limit_offset_page_data_platform_job import LimitOffsetPageDataPlatformJob
 from alvin_api_client.model.limit_offset_page_data_platform_job_entity_aggregated_report import LimitOffsetPageDataPlatformJobEntityAggregatedReport
 from alvin_api_client.model.limit_offset_page_data_tag_connection_get import LimitOffsetPageDataTagConnectionGet
 from alvin_api_client.model.limit_offset_page_data_tag_get import LimitOffsetPageDataTagGet
 from alvin_api_client.model.limit_offset_page_data_tag_rule_get import LimitOffsetPageDataTagRuleGet
+from alvin_api_client.model.limit_offset_page_insights_usage_response import LimitOffsetPageInsightsUsageResponse
 from alvin_api_client.model.limit_offset_page_manual_lineage_data import LimitOffsetPageManualLineageData
+from alvin_api_client.model.limit_offset_page_organization_get import LimitOffsetPageOrganizationGet
+from alvin_api_client.model.limit_offset_page_pipeline_get import LimitOffsetPagePipelineGet
+from alvin_api_client.model.lineage_graph_request import LineageGraphRequest
 from alvin_api_client.model.links_request import LinksRequest
+from alvin_api_client.model.list_event_databases_request import ListEventDatabasesRequest
+from alvin_api_client.model.list_event_databases_response import ListEventDatabasesResponse
+from alvin_api_client.model.list_event_users_by_period_request import ListEventUsersByPeriodRequest
+from alvin_api_client.model.list_event_users_by_period_response import ListEventUsersByPeriodResponse
+from alvin_api_client.model.list_platform_databases_request import ListPlatformDatabasesRequest
+from alvin_api_client.model.list_platform_databases_response import ListPlatformDatabasesResponse
 from alvin_api_client.model.manual_lineage_data_request import ManualLineageDataRequest
 from alvin_api_client.model.map_entity_to_url_request import MapEntityToUrlRequest
 from alvin_api_client.model.notification import Notification
+from alvin_api_client.model.organization_create import OrganizationCreate
 from alvin_api_client.model.organization_get import OrganizationGet
 from alvin_api_client.model.organization_status import OrganizationStatus
+from alvin_api_client.model.organization_update import OrganizationUpdate
 from alvin_api_client.model.page_data_entity_get import PageDataEntityGet
 from alvin_api_client.model.page_view_get import PageViewGet
 from alvin_api_client.model.platform_asset_type import PlatformAssetType
 from alvin_api_client.model.platform_classification import PlatformClassification
 from alvin_api_client.model.processed_lineage_graph_data import ProcessedLineageGraphData
+from alvin_api_client.model.search_entities_response import SearchEntitiesResponse
 from alvin_api_client.model.search_filter_label_association import SearchFilterLabelAssociation
 from alvin_api_client.model.search_node import SearchNode
 from alvin_api_client.model.search_v2_response import SearchV2Response
 from alvin_api_client.model.search_v2_response_payload import SearchV2ResponsePayload
 from alvin_api_client.model.strings_response import StringsResponse
 from alvin_api_client.model.tiny_url_response import TinyURLResponse
 from alvin_api_client.model.token import Token
@@ -330,17 +365,19 @@
                 'endpoint_path': '/api/v2/users',
                 'operation_id': 'add_users_to_org_api_v2_users_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'org_id',
                     'user_create_request',
                 ],
                 'required': [
+                    'org_id',
                     'user_create_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -348,20 +385,24 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'org_id':
+                        (str,),
                     'user_create_request':
                         (UserCreateRequest,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
                 },
                 'location_map': {
+                    'org_id': 'query',
                     'user_create_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -469,14 +510,56 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.callback_api_auth_v1_sso_callback_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (Token,),
+                'auth': [],
+                'endpoint_path': '/api/auth/v1/sso-callback',
+                'operation_id': 'callback_api_auth_v1_sso_callback_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.clear_platform_api_v1_platforms_platform_id_clear_post_endpoint = _Endpoint(
             settings={
                 'response_type': (DataPlatformDelete,),
                 'auth': [],
                 'endpoint_path': '/api/v1/platforms/{platform_id}/clear',
                 'operation_id': 'clear_platform_api_v1_platforms_platform_id_clear_post',
                 'http_method': 'POST',
@@ -1670,14 +1753,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.create_org_api_v1_organization_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (OrganizationGet,),
+                'auth': [],
+                'endpoint_path': '/api/v1/organization',
+                'operation_id': 'create_org_api_v1_organization_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'organization_create',
+                ],
+                'required': [
+                    'organization_create',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'organization_create':
+                        (OrganizationCreate,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'organization_create': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.create_postgres_platform_api_v1_platforms_postgres_post_endpoint = _Endpoint(
             settings={
                 'response_type': (DataPlatformGet,),
                 'auth': [],
                 'endpoint_path': '/api/v1/platforms/postgres',
                 'operation_id': 'create_postgres_platform_api_v1_platforms_postgres_post',
                 'http_method': 'POST',
@@ -2794,14 +2927,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.expand_children_lineage2_api_v2_lineage_expand_children2_post_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/expand-children2',
+                'operation_id': 'expand_children_lineage2_api_v2_lineage_expand_children2_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'required': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_lineage_v3_request':
+                        (DataEntityLineageV3Request,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_lineage_v3_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.expand_children_lineage_api_v2_lineage_expand_children_post_endpoint = _Endpoint(
             settings={
                 'response_type': (DataEntityLineageV2Response,),
                 'auth': [],
                 'endpoint_path': '/api/v2/lineage/expand-children',
                 'operation_id': 'expand_children_lineage_api_v2_lineage_expand_children_post',
                 'http_method': 'POST',
@@ -3178,14 +3361,72 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_all_organizations_info_api_v1_organizations_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (LimitOffsetPageOrganizationGet,),
+                'auth': [],
+                'endpoint_path': '/api/v1/organizations',
+                'operation_id': 'get_all_organizations_info_api_v1_organizations_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'limit',
+                    'offset',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'limit',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('limit',): {
+
+                        'inclusive_maximum': 10000,
+                        'inclusive_minimum': 1,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'limit':
+                        (int,),
+                    'offset':
+                        (int,),
+                },
+                'attribute_map': {
+                    'limit': 'limit',
+                    'offset': 'offset',
+                },
+                'location_map': {
+                    'limit': 'query',
+                    'offset': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_all_taxonomy_classifications_api_v1_taxonomy_all_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([DataTaxonomyClassification],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/taxonomy/all',
@@ -3450,14 +3691,215 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_connected_entities_api_v2_lineage_connecting_entities_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DataEntityLineageV3Response,),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/connecting-entities',
+                'operation_id': 'get_connected_entities_api_v2_lineage_connecting_entities_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_connect_nodes_request',
+                ],
+                'required': [
+                    'data_entity_connect_nodes_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_connect_nodes_request':
+                        (DataEntityConnectNodesRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_connect_nodes_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_dashboard_costs_api_insights_v1_dashboards_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DashboardCostsResponse,),
+                'auth': [],
+                'endpoint_path': '/api/insights/v1/dashboards',
+                'operation_id': 'get_dashboard_costs_api_insights_v1_dashboards_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'body_get_dashboard_costs_api_insights_v1_dashboards_post',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'body_get_dashboard_costs_api_insights_v1_dashboards_post':
+                        (BodyGetDashboardCostsApiInsightsV1DashboardsPost,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'body_get_dashboard_costs_api_insights_v1_dashboards_post': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_dashboard_costs_api_insights_v2_dashboards_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DashboardCostsV2Response,),
+                'auth': [],
+                'endpoint_path': '/api/insights/v2/dashboards',
+                'operation_id': 'get_dashboard_costs_api_insights_v2_dashboards_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'body_get_dashboard_costs_api_insights_v2_dashboards_post',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'body_get_dashboard_costs_api_insights_v2_dashboards_post':
+                        (BodyGetDashboardCostsApiInsightsV2DashboardsPost,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'body_get_dashboard_costs_api_insights_v2_dashboards_post': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DashboardUsersResponse,),
+                'auth': [],
+                'endpoint_path': '/api/insights/v1/dashboards/{dashboard_id}/users',
+                'operation_id': 'get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'dashboard_id',
+                    'body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post',
+                ],
+                'required': [
+                    'dashboard_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'dashboard_id':
+                        (str,),
+                    'body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post':
+                        (BodyGetDashboardUsersCostApiInsightsV1DashboardsDashboardIdUsersPost,),
+                },
+                'attribute_map': {
+                    'dashboard_id': 'dashboard_id',
+                },
+                'location_map': {
+                    'dashboard_id': 'path',
+                    'body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_data_entity_run_facets_api_v1_entity_runs_run_id_facets_get_endpoint = _Endpoint(
             settings={
                 'response_type': (LimitOffsetPageDataEntityRunFacetGet,),
                 'auth': [],
                 'endpoint_path': '/api/v1/entity/runs/{runId}/facets',
                 'operation_id': 'get_data_entity_run_facets_api_v1_entity_runs_run_id_facets_get',
                 'http_method': 'GET',
@@ -3486,15 +3928,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'run_id':
@@ -3569,15 +4011,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'run_id':
@@ -3717,15 +4159,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -4243,15 +4685,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -4324,15 +4766,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -4523,15 +4965,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -4616,14 +5058,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.get_entity_lineage_children2_api_v2_lineage_children2_post_endpoint = _Endpoint(
+            settings={
+                'response_type': ([str],),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/children2',
+                'operation_id': 'get_entity_lineage_children2_api_v2_lineage_children2_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'required': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_lineage_v3_request':
+                        (DataEntityLineageV3Request,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_lineage_v3_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_entity_lineage_children_api_v2_lineage_children_post_endpoint = _Endpoint(
             settings={
                 'response_type': (DataEntityLineageChildrenResponse,),
                 'auth': [],
                 'endpoint_path': '/api/v2/lineage/children',
                 'operation_id': 'get_entity_lineage_children_api_v2_lineage_children_post',
                 'http_method': 'POST',
@@ -4666,14 +5158,114 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.get_entity_lineage_explorer2_api_v2_lineage_explorer2_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DataEntityLineageV3Response,),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/explorer2',
+                'operation_id': 'get_entity_lineage_explorer2_api_v2_lineage_explorer2_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'required': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_lineage_v3_request':
+                        (DataEntityLineageV3Request,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_lineage_v3_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_entity_lineage_explorer_api_v2_lineage_explorer_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DataEntityLineageExplorerResponse,),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/explorer',
+                'operation_id': 'get_entity_lineage_explorer_api_v2_lineage_explorer_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_lineage_v2_request_dto',
+                ],
+                'required': [
+                    'data_entity_lineage_v2_request_dto',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_lineage_v2_request_dto':
+                        (DataEntityLineageV2RequestDTO,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_lineage_v2_request_dto': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_entity_lineage_explorer_link_api_entity_v1_lineage_explorer_link_post_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [],
                 'endpoint_path': '/api/entity/v1/lineage-explorer-link',
                 'operation_id': 'get_entity_lineage_explorer_link_api_entity_v1_lineage_explorer_link_post',
                 'http_method': 'POST',
@@ -4716,14 +5308,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.get_entity_lineage_list2_api_v2_lineage_list2_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DataEntityLineageV3Response,),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/list2',
+                'operation_id': 'get_entity_lineage_list2_api_v2_lineage_list2_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'required': [
+                    'data_entity_lineage_v3_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_lineage_v3_request':
+                        (DataEntityLineageV3Request,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_lineage_v3_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_entity_lineage_list_api_v2_lineage_list_post_endpoint = _Endpoint(
             settings={
                 'response_type': (DataEntityLineageListResponse,),
                 'auth': [],
                 'endpoint_path': '/api/v2/lineage/list',
                 'operation_id': 'get_entity_lineage_list_api_v2_lineage_list_post',
                 'http_method': 'POST',
@@ -4997,15 +5639,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -5082,15 +5724,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -5346,15 +5988,15 @@
                     'entity_id',
                     'entity_type',
                     'start_timestamp',
                     'end_timestamp',
                     'connection_type',
                     'connection_direction',
                     'connection_usage_classification',
-                    'usage_type',
+                    'usage_types',
                     'user_name',
                     'sort',
                     'limit',
                     'offset',
                 ],
                 'required': [
                     'platform_id',
@@ -5376,38 +6018,38 @@
 
                         'regex': {
                             'pattern': r'^[\w: ]*$',  # noqa: E501
                         },
                     },
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
                         (str,),
                     'entity_id':
                         (str,),
                     'entity_type':
-                        (str,),
+                        (DataEntityType,),
                     'start_timestamp':
                         (datetime,),
                     'end_timestamp':
                         (datetime,),
                     'connection_type':
                         (ConnectionType,),
                     'connection_direction':
                         (ConnectionDirection,),
                     'connection_usage_classification':
                         (ConnectionUsageClassification,),
-                    'usage_type':
+                    'usage_types':
                         ([str],),
                     'user_name':
                         ([str],),
                     'sort':
                         ([str],),
                     'limit':
                         (int,),
@@ -5419,49 +6061,199 @@
                     'entity_id': 'entityId',
                     'entity_type': 'entityType',
                     'start_timestamp': 'startTimestamp',
                     'end_timestamp': 'endTimestamp',
                     'connection_type': 'connectionType',
                     'connection_direction': 'connectionDirection',
                     'connection_usage_classification': 'connectionUsageClassification',
-                    'usage_type': 'usageType',
+                    'usage_types': 'usageTypes',
                     'user_name': 'userName',
                     'sort': 'sort',
                     'limit': 'limit',
                     'offset': 'offset',
                 },
                 'location_map': {
                     'platform_id': 'query',
                     'entity_id': 'query',
                     'entity_type': 'query',
                     'start_timestamp': 'query',
                     'end_timestamp': 'query',
                     'connection_type': 'query',
                     'connection_direction': 'query',
                     'connection_usage_classification': 'query',
-                    'usage_type': 'query',
+                    'usage_types': 'query',
                     'user_name': 'query',
                     'sort': 'query',
                     'limit': 'query',
                     'offset': 'query',
                 },
                 'collection_format_map': {
-                    'usage_type': 'multi',
+                    'usage_types': 'multi',
                     'user_name': 'multi',
                     'sort': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_event_users_api_events_v1_users_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (EventUsersResponse,),
+                'auth': [],
+                'endpoint_path': '/api/events/v1/users',
+                'operation_id': 'get_event_users_api_events_v1_users_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'event_request_filter',
+                ],
+                'required': [
+                    'event_request_filter',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'event_request_filter':
+                        (EventRequestFilter,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'event_request_filter': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_event_users_by_period_api_events_v1_users_by_period_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (ListEventUsersByPeriodResponse,),
+                'auth': [],
+                'endpoint_path': '/api/events/v1/users-by-period',
+                'operation_id': 'get_event_users_by_period_api_events_v1_users_by_period_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'list_event_users_by_period_request',
+                ],
+                'required': [
+                    'list_event_users_by_period_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'list_event_users_by_period_request':
+                        (ListEventUsersByPeriodRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'list_event_users_by_period_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.get_events_stats_api_events_v1_stats_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (EventStatsReport,),
+                'auth': [],
+                'endpoint_path': '/api/events/v1/stats',
+                'operation_id': 'get_events_stats_api_events_v1_stats_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'event_stats_request',
+                ],
+                'required': [
+                    'event_stats_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'event_stats_request':
+                        (EventStatsRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'event_stats_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_experiences_api_v1_experience_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([Experience],),
                 'auth': [],
                 'endpoint_path': '/api/v1/experience',
                 'operation_id': 'get_experiences_api_v1_experience_get',
                 'http_method': 'GET',
@@ -5832,56 +6624,14 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_impact_analysis_platforms_api_impact_analysis_v3_platforms_get_endpoint = _Endpoint(
-            settings={
-                'response_type': ([DataPlatformGet],),
-                'auth': [],
-                'endpoint_path': '/api/impact-analysis/v3/platforms',
-                'operation_id': 'get_impact_analysis_platforms_api_impact_analysis_v3_platforms_get',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                ],
-                'required': [],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
         self.get_impact_analysis_platforms_api_v2_impact_analysis_platforms_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([DataPlatformGet],),
                 'auth': [],
                 'endpoint_path': '/api/v2/impact-analysis/platforms',
                 'operation_id': 'get_impact_analysis_platforms_api_v2_impact_analysis_platforms_get',
                 'http_method': 'GET',
@@ -5916,20 +6666,20 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_impact_by_query_api_impact_analysis_v3_query_post_endpoint = _Endpoint(
+        self.get_impact_by_query_api_v2_impact_analysis_query_post_endpoint = _Endpoint(
             settings={
-                'response_type': (AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponse,),
+                'response_type': (ImpactAnalysisResponse,),
                 'auth': [],
-                'endpoint_path': '/api/impact-analysis/v3/query',
-                'operation_id': 'get_impact_by_query_api_impact_analysis_v3_query_post',
+                'endpoint_path': '/api/v2/impact-analysis/query',
+                'operation_id': 'get_impact_by_query_api_v2_impact_analysis_query_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'impact_analysis_request',
                 ],
@@ -5966,70 +6716,70 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.get_impact_by_query_api_v2_impact_analysis_query_post_endpoint = _Endpoint(
+        self.get_impact_from_validation_payload2_api_v2_impact_analysis_query_entities2_post_endpoint = _Endpoint(
             settings={
-                'response_type': (AppSchemasImpactAnalysisResponseImpactAnalysisResponse,),
+                'response_type': (ImpactAnalysisResponse,),
                 'auth': [],
-                'endpoint_path': '/api/v2/impact-analysis/query',
-                'operation_id': 'get_impact_by_query_api_v2_impact_analysis_query_post',
+                'endpoint_path': '/api/v2/impact-analysis/query-entities2',
+                'operation_id': 'get_impact_from_validation_payload2_api_v2_impact_analysis_query_entities2_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'impact_analysis_request',
+                    'impact_analysis_validation_payload_v2',
                 ],
                 'required': [
-                    'impact_analysis_request',
+                    'impact_analysis_validation_payload_v2',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'impact_analysis_request':
-                        (ImpactAnalysisRequest,),
+                    'impact_analysis_validation_payload_v2':
+                        (ImpactAnalysisValidationPayloadV2,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'impact_analysis_request': 'body',
+                    'impact_analysis_validation_payload_v2': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.get_impact_from_validation_payload_api_impact_analysis_v3_query_entities_post_endpoint = _Endpoint(
+        self.get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post_endpoint = _Endpoint(
             settings={
-                'response_type': (AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponse,),
+                'response_type': (ImpactAnalysisResponse,),
                 'auth': [],
-                'endpoint_path': '/api/impact-analysis/v3/query-entities',
-                'operation_id': 'get_impact_from_validation_payload_api_impact_analysis_v3_query_entities_post',
+                'endpoint_path': '/api/v2/impact-analysis/query-entities',
+                'operation_id': 'get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'impact_analysis_validation_payload',
                 ],
@@ -6066,50 +6816,50 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post_endpoint = _Endpoint(
+        self.get_insights_period_report_api_insights_v1_post_endpoint = _Endpoint(
             settings={
-                'response_type': (AppSchemasImpactAnalysisResponseImpactAnalysisResponse,),
+                'response_type': (InsightsDeltaResponse,),
                 'auth': [],
-                'endpoint_path': '/api/v2/impact-analysis/query-entities',
-                'operation_id': 'get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post',
+                'endpoint_path': '/api/insights/v1/',
+                'operation_id': 'get_insights_period_report_api_insights_v1_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'impact_analysis_validation_payload',
+                    'insights_request',
                 ],
                 'required': [
-                    'impact_analysis_validation_payload',
+                    'insights_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'impact_analysis_validation_payload':
-                        (ImpactAnalysisValidationPayload,),
+                    'insights_request':
+                        (InsightsRequest,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'impact_analysis_validation_payload': 'body',
+                    'insights_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -6129,33 +6879,40 @@
                 'endpoint_path': '/api/v2/users/invite',
                 'operation_id': 'get_invited_users_to_org_api_v2_users_invite_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'org_id',
+                ],
+                'required': [
+                    'org_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'org_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
                 },
                 'location_map': {
+                    'org_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -6389,15 +7146,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'entity_id':
@@ -6594,14 +7351,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.get_lineage_graph_api_v2_lineage_graph_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (DataEntityLineageV3Response,),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/graph',
+                'operation_id': 'get_lineage_graph_api_v2_lineage_graph_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'lineage_graph_request',
+                ],
+                'required': [
+                    'lineage_graph_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'lineage_graph_request':
+                        (LineageGraphRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'lineage_graph_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_lineage_job_steps_api_v1_lineage_jobs_steps_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([DataPlatformJobStep],),
                 'auth': [],
                 'endpoint_path': '/api/v1/lineage/jobs/steps',
                 'operation_id': 'get_lineage_job_steps_api_v1_lineage_jobs_steps_get',
                 'http_method': 'GET',
@@ -7171,14 +7978,105 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_organization_info_api_v1_organization_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (OrganizationGet,),
+                'auth': [],
+                'endpoint_path': '/api/v1/organization',
+                'operation_id': 'get_organization_info_api_v1_organization_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_organization_info_from_org_id_api_v1_organization_org_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (OrganizationGet,),
+                'auth': [],
+                'endpoint_path': '/api/v1/organization/{org_id}',
+                'operation_id': 'get_organization_info_from_org_id_api_v1_organization_org_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                ],
+                'required': [
+                    'org_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_parent_taxonomy_classifications_api_v1_taxonomy_parents_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([DataTaxonomyClassification],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/taxonomy/parents',
@@ -7215,14 +8113,115 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_pipeline_by_id_api_v1_pipeline_pipeline_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/api/v1/pipeline/{pipeline_id}',
+                'operation_id': 'get_pipeline_by_id_api_v1_pipeline_pipeline_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'pipeline_id',
+                ],
+                'required': [
+                    'pipeline_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'pipeline_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'pipeline_id': 'pipeline_id',
+                },
+                'location_map': {
+                    'pipeline_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.get_pipelines_api_v1_pipelines_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (LimitOffsetPagePipelineGet,),
+                'auth': [],
+                'endpoint_path': '/api/v1/pipelines',
+                'operation_id': 'get_pipelines_api_v1_pipelines_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'page',
+                    'size',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
+                },
+                'attribute_map': {
+                    'page': 'page',
+                    'size': 'size',
+                },
+                'location_map': {
+                    'page': 'query',
+                    'size': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_platform_api_v1_platforms_platform_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (DataPlatformGet,),
                 'auth': [],
                 'endpoint_path': '/api/v1/platforms/{platform_id}',
                 'operation_id': 'get_platform_api_v1_platforms_platform_id_get',
                 'http_method': 'GET',
@@ -7637,14 +8636,78 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_simple_lineage_api_v2_simple_lineage_entity_fqn_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (DataEntitySimpleLineageResponse,),
+                'auth': [],
+                'endpoint_path': '/api/v2/simple-lineage/{entity_fqn}',
+                'operation_id': 'get_simple_lineage_api_v2_simple_lineage_entity_fqn_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'entity_fqn',
+                    'upstream',
+                    'get_parent_enriched',
+                    'group_by_parent',
+                ],
+                'required': [
+                    'entity_fqn',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'entity_fqn':
+                        (str,),
+                    'upstream':
+                        (bool,),
+                    'get_parent_enriched':
+                        (bool,),
+                    'group_by_parent':
+                        (bool,),
+                },
+                'attribute_map': {
+                    'entity_fqn': 'entity_fqn',
+                    'upstream': 'upstream',
+                    'get_parent_enriched': 'get_parent_enriched',
+                    'group_by_parent': 'group_by_parent',
+                },
+                'location_map': {
+                    'entity_fqn': 'path',
+                    'upstream': 'query',
+                    'get_parent_enriched': 'query',
+                    'group_by_parent': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_snowflake_platform_api_v1_platforms_snowflake_platform_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (DataPlatformGet,),
                 'auth': [],
                 'endpoint_path': '/api/v1/platforms/snowflake/{platform_id}',
                 'operation_id': 'get_snowflake_platform_api_v1_platforms_snowflake_platform_id_get',
                 'http_method': 'GET',
@@ -7686,14 +8749,61 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_table_num_rows_api_entity_v1_num_rows_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (GetTableNumRowsChartResponse,),
+                'auth': [],
+                'endpoint_path': '/api/entity/v1/num-rows',
+                'operation_id': 'get_table_num_rows_api_entity_v1_num_rows_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'fqn',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'fqn':
+                        (str,),
+                },
+                'attribute_map': {
+                    'fqn': 'fqn',
+                },
+                'location_map': {
+                    'fqn': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.get_tableau_platform_api_v1_platforms_tableau_platform_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (DataPlatformGet,),
                 'auth': [],
                 'endpoint_path': '/api/v1/platforms/tableau/{platform_id}',
                 'operation_id': 'get_tableau_platform_api_v1_platforms_tableau_platform_id_get',
                 'http_method': 'GET',
@@ -7918,15 +9028,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'platform_id':
@@ -8051,14 +9161,80 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_usage_api_insights_v1_usage_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (LimitOffsetPageInsightsUsageResponse,),
+                'auth': [],
+                'endpoint_path': '/api/insights/v1/usage',
+                'operation_id': 'get_usage_api_insights_v1_usage_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'insights_usage_request',
+                    'limit',
+                    'offset',
+                ],
+                'required': [
+                    'insights_usage_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                    'limit',
+                ]
+            },
+            root_map={
+                'validations': {
+                    ('limit',): {
+
+                        'inclusive_maximum': 10000,
+                        'inclusive_minimum': 1,
+                    },
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'insights_usage_request':
+                        (InsightsUsageRequest,),
+                    'limit':
+                        (int,),
+                    'offset':
+                        (int,),
+                },
+                'attribute_map': {
+                    'limit': 'limit',
+                    'offset': 'offset',
+                },
+                'location_map': {
+                    'insights_usage_request': 'body',
+                    'limit': 'query',
+                    'offset': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_user_id_api_v1_user_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [],
                 'endpoint_path': '/api/v1/user/id',
                 'operation_id': 'get_user_id_api_v1_user_id_get',
                 'http_method': 'GET',
@@ -8142,64 +9318,69 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_user_info_api_v1_organization_get_endpoint = _Endpoint(
+        self.get_user_invite_by_link_id_api_v2_users_invite_link_id_get_endpoint = _Endpoint(
             settings={
-                'response_type': (OrganizationGet,),
-                'auth': [
-                    'HTTPBearer'
-                ],
-                'endpoint_path': '/api/v1/organization',
-                'operation_id': 'get_user_info_api_v1_organization_get',
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/api/v2/users/invite/{link_id}',
+                'operation_id': 'get_user_invite_by_link_id_api_v2_users_invite_link_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'link_id',
+                ],
+                'required': [
+                    'link_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'link_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'link_id': 'link_id',
                 },
                 'location_map': {
+                    'link_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_user_invite_by_link_id_api_v2_users_invite_link_id_get_endpoint = _Endpoint(
+        self.get_user_invite_object_api_v2_user_invite_link_id_get_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (UserInviteCreate,),
                 'auth': [],
-                'endpoint_path': '/api/v2/users/invite/{link_id}',
-                'operation_id': 'get_user_invite_by_link_id_api_v2_users_invite_link_id_get',
+                'endpoint_path': '/api/v2/user_invite/{link_id}',
+                'operation_id': 'get_user_invite_object_api_v2_user_invite_link_id_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'link_id',
                 ],
@@ -8651,17 +9832,19 @@
                 'endpoint_path': '/api/v2/users/invite',
                 'operation_id': 'invite_user_to_org_api_v2_users_invite_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'org_id',
                     'user_create_request',
                 ],
                 'required': [
+                    'org_id',
                     'user_create_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -8669,20 +9852,24 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'org_id':
+                        (str,),
                     'user_create_request':
                         (UserCreateRequest,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
                 },
                 'location_map': {
+                    'org_id': 'query',
                     'user_create_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -8741,14 +9928,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.lineage_has_temp_entity_api_v2_lineage_has_temp_entity_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/api/v2/lineage/has-temp-entity',
+                'operation_id': 'lineage_has_temp_entity_api_v2_lineage_has_temp_entity_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_lineage_v2_request_dto',
+                ],
+                'required': [
+                    'data_entity_lineage_v2_request_dto',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_lineage_v2_request_dto':
+                        (DataEntityLineageV2RequestDTO,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_lineage_v2_request_dto': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.lineage_spark_api_v1_lineage_spark_post_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [],
                 'endpoint_path': '/api/v1/lineage/spark',
                 'operation_id': 'lineage_spark_api_v1_lineage_spark_post',
                 'http_method': 'POST',
@@ -8792,14 +10029,64 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.list_databases_api_events_v1_list_databases_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (ListEventDatabasesResponse,),
+                'auth': [],
+                'endpoint_path': '/api/events/v1/list-databases',
+                'operation_id': 'list_databases_api_events_v1_list_databases_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'list_event_databases_request',
+                ],
+                'required': [
+                    'list_event_databases_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'list_event_databases_request':
+                        (ListEventDatabasesRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'list_event_databases_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.list_manual_lineage_api_v1_lineage_manual_get_endpoint = _Endpoint(
             settings={
                 'response_type': (LimitOffsetPageManualLineageData,),
                 'auth': [],
                 'endpoint_path': '/api/v1/lineage/manual',
                 'operation_id': 'list_manual_lineage_api_v1_lineage_manual_get',
                 'http_method': 'GET',
@@ -8819,15 +10106,15 @@
                     'limit',
                 ]
             },
             root_map={
                 'validations': {
                     ('limit',): {
 
-                        'inclusive_maximum': 1000,
+                        'inclusive_maximum': 10000,
                         'inclusive_minimum': 1,
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'limit':
@@ -8917,27 +10204,170 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.list_platform_databases_api_v2_search_list_databases_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (ListPlatformDatabasesResponse,),
+                'auth': [
+                    'HTTPBearer'
+                ],
+                'endpoint_path': '/api/v2/search/list-databases',
+                'operation_id': 'list_platform_databases_api_v2_search_list_databases_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'list_platform_databases_request',
+                ],
+                'required': [
+                    'list_platform_databases_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'list_platform_databases_request':
+                        (ListPlatformDatabasesRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'list_platform_databases_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.list_users_in_org_api_v2_users_get_endpoint = _Endpoint(
             settings={
                 'response_type': ([UserGet],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v2/users',
                 'operation_id': 'list_users_in_org_api_v2_users_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'org_id',
+                ],
+                'required': [
+                    'org_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                },
+                'location_map': {
+                    'org_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.load_api_graph_v1_load_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/api/graph/v1/load',
+                'operation_id': 'load_api_graph_v1_load_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.login_api_auth_v1_sso_login_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/api/auth/v1/sso-login',
+                'operation_id': 'login_api_auth_v1_sso_login_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -8961,14 +10391,65 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.metadata_api_dbt_v1_metadata_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [],
+                'endpoint_path': '/api/dbt/v1/metadata',
+                'operation_id': 'metadata_api_dbt_v1_metadata_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'unknown_base_type',
+                ],
+                'required': [
+                    'unknown_base_type',
+                ],
+                'nullable': [
+                    'unknown_base_type',
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'unknown_base_type':
+                        (),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'unknown_base_type': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.metadata_api_v1_metadata_post_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [],
                 'endpoint_path': '/api/v1/metadata',
                 'operation_id': 'metadata_api_v1_metadata_post',
                 'http_method': 'POST',
@@ -9126,17 +10607,19 @@
                 'endpoint_path': '/api/v2/user',
                 'operation_id': 'remove_user_from_org_api_v2_user_delete',
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'org_id',
                     'user_id',
                 ],
                 'required': [
+                    'org_id',
                     'user_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -9144,21 +10627,25 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'org_id':
+                        (str,),
                     'user_id':
                         (str,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
                     'user_id': 'user_id',
                 },
                 'location_map': {
+                    'org_id': 'query',
                     'user_id': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -9536,14 +11023,16 @@
                 'operation_id': 'search_api_v2_search_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'search_string',
+                    'generate_filter_count_data',
+                    'generate_downstream_usage',
                     'page',
                     'size',
                     'search_node',
                 ],
                 'required': [],
                 'nullable': [
                 ],
@@ -9567,28 +11056,36 @@
                     },
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'search_string':
                         (str,),
+                    'generate_filter_count_data':
+                        (bool,),
+                    'generate_downstream_usage':
+                        (bool,),
                     'page':
                         (int,),
                     'size':
                         (int,),
                     'search_node':
                         ([SearchNode],),
                 },
                 'attribute_map': {
                     'search_string': 'searchString',
+                    'generate_filter_count_data': 'generateFilterCountData',
+                    'generate_downstream_usage': 'generateDownstreamUsage',
                     'page': 'page',
                     'size': 'size',
                 },
                 'location_map': {
                     'search_string': 'query',
+                    'generate_filter_count_data': 'query',
+                    'generate_downstream_usage': 'query',
                     'page': 'query',
                     'size': 'query',
                     'search_node': 'body',
                 },
                 'collection_format_map': {
                 }
             },
@@ -9598,14 +11095,66 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.search_entities_api_v2_search_entities_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (SearchEntitiesResponse,),
+                'auth': [
+                    'HTTPBearer'
+                ],
+                'endpoint_path': '/api/v2/search/entities',
+                'operation_id': 'search_entities_api_v2_search_entities_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'data_entity_id',
+                ],
+                'required': [
+                    'data_entity_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'data_entity_id':
+                        ([DataEntityID],),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'data_entity_id': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.search_entities_stats_post_api_v1_search_entities_usage_stats_post_endpoint = _Endpoint(
             settings={
                 'response_type': (LimitOffsetPageDataEntityUsageStatsReport,),
                 'auth': [],
                 'endpoint_path': '/api/v1/search/entities/usage-stats',
                 'operation_id': 'search_entities_stats_post_api_v1_search_entities_usage_stats_post',
                 'http_method': 'POST',
@@ -9706,17 +11255,15 @@
                 ]
             },
             api_client=api_client
         )
         self.search_entity_by_id_api_v2_search_find_entity_post_endpoint = _Endpoint(
             settings={
                 'response_type': (SearchV2ResponsePayload,),
-                'auth': [
-                    'HTTPBearer'
-                ],
+                'auth': [],
                 'endpoint_path': '/api/v2/search/find-entity',
                 'operation_id': 'search_entity_by_id_api_v2_search_find_entity_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
@@ -9766,14 +11313,114 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.search_events_api_events_v1_search_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (EventSearchResponse,),
+                'auth': [],
+                'endpoint_path': '/api/events/v1/search',
+                'operation_id': 'search_events_api_events_v1_search_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'event_search_request',
+                ],
+                'required': [
+                    'event_search_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'event_search_request':
+                        (EventSearchRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'event_search_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.search_events_timeline_api_events_v1_search_timeline_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (EventSearchTimelineResponse,),
+                'auth': [],
+                'endpoint_path': '/api/events/v1/search/timeline',
+                'operation_id': 'search_events_timeline_api_events_v1_search_timeline_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'event_search_request',
+                ],
+                'required': [
+                    'event_search_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'event_search_request':
+                        (EventSearchRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'event_search_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.set_org_status_api_v1_organization_status_post_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [],
                 'endpoint_path': '/api/v1/organization/status',
                 'operation_id': 'set_org_status_api_v1_organization_status_post',
                 'http_method': 'POST',
@@ -10820,18 +12467,20 @@
                 'endpoint_path': '/api/v2/users/invite',
                 'operation_id': 'update_invite_to_organization_status_api_v2_users_invite_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'org_id',
                     'invite_id',
                     'status',
                 ],
                 'required': [
+                    'org_id',
                     'invite_id',
                     'status',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
@@ -10840,57 +12489,59 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'org_id':
+                        (str,),
                     'invite_id':
                         (str,),
                     'status':
                         (str,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
                     'invite_id': 'invite_id',
                     'status': 'status',
                 },
                 'location_map': {
+                    'org_id': 'query',
                     'invite_id': 'query',
                     'status': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.update_org_status_api_v2_organizations_org_id_post_endpoint = _Endpoint(
+        self.update_org_api_v1_organization_update_post_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [
-                    'HTTPBearer'
-                ],
-                'endpoint_path': '/api/v2/organizations/{org_id}',
-                'operation_id': 'update_org_status_api_v2_organizations_org_id_post',
+                'auth': [],
+                'endpoint_path': '/api/v1/organization/update',
+                'operation_id': 'update_org_api_v1_organization_update_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'org_id',
-                    'status',
+                    'organization_update',
                 ],
                 'required': [
                     'org_id',
-                    'status',
+                    'organization_update',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -10899,176 +12550,190 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'org_id':
                         (str,),
-                    'status':
-                        (OrganizationStatus,),
+                    'organization_update':
+                        (OrganizationUpdate,),
                 },
                 'attribute_map': {
                     'org_id': 'org_id',
-                    'status': 'status',
                 },
                 'location_map': {
-                    'org_id': 'path',
-                    'status': 'query',
+                    'org_id': 'query',
+                    'organization_update': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
-        self.update_user_in_org_api_v2_user_put_endpoint = _Endpoint(
+        self.update_org_status_api_v2_organizations_org_id_post_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
-                'endpoint_path': '/api/v2/user',
-                'operation_id': 'update_user_in_org_api_v2_user_put',
-                'http_method': 'PUT',
+                'endpoint_path': '/api/v2/organizations/{org_id}',
+                'operation_id': 'update_org_status_api_v2_organizations_org_id_post',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'user_create_request',
+                    'org_id',
+                    'status',
                 ],
                 'required': [
-                    'user_create_request',
+                    'org_id',
+                    'status',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'user_create_request':
-                        (UserCreateRequest,),
+                    'org_id':
+                        (str,),
+                    'status':
+                        (OrganizationStatus,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
+                    'status': 'status',
                 },
                 'location_map': {
-                    'user_create_request': 'body',
+                    'org_id': 'path',
+                    'status': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.update_view_api_v2_views_update_put_endpoint = _Endpoint(
+        self.update_user_in_org_api_v2_user_put_endpoint = _Endpoint(
             settings={
-                'response_type': (ViewSaveResponse,),
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
-                'endpoint_path': '/api/v2/views/update',
-                'operation_id': 'update_view_api_v2_views_update_put',
+                'endpoint_path': '/api/v2/user',
+                'operation_id': 'update_user_in_org_api_v2_user_put',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'view_get',
+                    'org_id',
+                    'user_create_request',
                 ],
                 'required': [
-                    'view_get',
+                    'org_id',
+                    'user_create_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'view_get':
-                        (ViewGet,),
+                    'org_id':
+                        (str,),
+                    'user_create_request':
+                        (UserCreateRequest,),
                 },
                 'attribute_map': {
+                    'org_id': 'org_id',
                 },
                 'location_map': {
-                    'view_get': 'body',
+                    'org_id': 'query',
+                    'user_create_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.validate_impact_analysis_query_api_impact_analysis_v3_validate_query_post_endpoint = _Endpoint(
+        self.update_view_api_v2_views_update_put_endpoint = _Endpoint(
             settings={
-                'response_type': (ImpactAnalysisQueryValidation,),
-                'auth': [],
-                'endpoint_path': '/api/impact-analysis/v3/validate-query',
-                'operation_id': 'validate_impact_analysis_query_api_impact_analysis_v3_validate_query_post',
-                'http_method': 'POST',
+                'response_type': (ViewSaveResponse,),
+                'auth': [
+                    'HTTPBearer'
+                ],
+                'endpoint_path': '/api/v2/views/update',
+                'operation_id': 'update_view_api_v2_views_update_put',
+                'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'impact_analysis_request',
+                    'view_get',
                 ],
                 'required': [
-                    'impact_analysis_request',
+                    'view_get',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'impact_analysis_request':
-                        (ImpactAnalysisRequest,),
+                    'view_get':
+                        (ViewGet,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'impact_analysis_request': 'body',
+                    'view_get': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -11371,26 +13036,28 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.add_user_stat_api_v2_user_analytics_add_post_endpoint.call_with_http_info(**kwargs)
 
     def add_users_to_org_api_v2_users_post(
         self,
+        org_id,
         user_create_request,
         **kwargs
     ):
         """Add Users To Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.add_users_to_org_api_v2_users_post(user_create_request, async_req=True)
+        >>> thread = api.add_users_to_org_api_v2_users_post(org_id, user_create_request, async_req=True)
         >>> result = thread.get()
 
         Args:
+            org_id (str):
             user_create_request (UserCreateRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -11430,14 +13097,16 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
         kwargs['user_create_request'] = \
             user_create_request
         return self.add_users_to_org_api_v2_users_post_endpoint.call_with_http_info(**kwargs)
 
     def bulk_apply_api_v1_tags_bulk_apply_post(
         self,
         data_tag_bulk_apply,
@@ -11566,14 +13235,74 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['data_tag_bulk_delete'] = \
             data_tag_bulk_delete
         return self.bulk_delete_api_v1_tags_bulk_delete_delete_endpoint.call_with_http_info(**kwargs)
 
+    def callback_api_auth_v1_sso_callback_get(
+        self,
+        **kwargs
+    ):
+        """Callback  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.callback_api_auth_v1_sso_callback_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Token
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.callback_api_auth_v1_sso_callback_get_endpoint.call_with_http_info(**kwargs)
+
     def clear_platform_api_v1_platforms_platform_id_clear_post(
         self,
         platform_id,
         **kwargs
     ):
         """Clear Platform  # noqa: E501
 
@@ -13136,14 +14865,79 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['data_entity_iddto'] = \
             data_entity_iddto
         return self.create_node_api_v1_lineage_node_create_node_post_endpoint.call_with_http_info(**kwargs)
 
+    def create_org_api_v1_organization_post(
+        self,
+        organization_create,
+        **kwargs
+    ):
+        """Create Org  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_org_api_v1_organization_post(organization_create, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            organization_create (OrganizationCreate):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            OrganizationGet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['organization_create'] = \
+            organization_create
+        return self.create_org_api_v1_organization_post_endpoint.call_with_http_info(**kwargs)
+
     def create_postgres_platform_api_v1_platforms_postgres_post(
         self,
         data_platform_postgres_create,
         **kwargs
     ):
         """Create Postgres Platform  # noqa: E501
 
@@ -14574,14 +16368,79 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['provider_id'] = \
             provider_id
         kwargs['exchange_token_request'] = \
             exchange_token_request
         return self.exchange_token_api_v1_auth_exchange_token_post_endpoint.call_with_http_info(**kwargs)
 
+    def expand_children_lineage2_api_v2_lineage_expand_children2_post(
+        self,
+        data_entity_lineage_v3_request,
+        **kwargs
+    ):
+        """Expand Children Lineage2  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.expand_children_lineage2_api_v2_lineage_expand_children2_post(data_entity_lineage_v3_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_lineage_v3_request (DataEntityLineageV3Request):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_lineage_v3_request'] = \
+            data_entity_lineage_v3_request
+        return self.expand_children_lineage2_api_v2_lineage_expand_children2_post_endpoint.call_with_http_info(**kwargs)
+
     def expand_children_lineage_api_v2_lineage_expand_children_post(
         self,
         data_entity_lineage_v2_request_dto,
         **kwargs
     ):
         """Expand Children Lineage  # noqa: E501
 
@@ -15083,14 +16942,76 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['platform_id'] = \
             platform_id
         return self.get_airflow_platform_api_v1_platforms_airflow_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
+    def get_all_organizations_info_api_v1_organizations_get(
+        self,
+        **kwargs
+    ):
+        """Get All Organizations Info  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_all_organizations_info_api_v1_organizations_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            limit (int): [optional] if omitted the server will use the default value of 50
+            offset (int): [optional] if omitted the server will use the default value of 0
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            LimitOffsetPageOrganizationGet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_all_organizations_info_api_v1_organizations_get_endpoint.call_with_http_info(**kwargs)
+
     def get_all_taxonomy_classifications_api_v1_taxonomy_all_get(
         self,
         **kwargs
     ):
         """Get All Taxonomy Classifications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15453,14 +17374,267 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.get_client_config_post_auth_api_v1_client_config_post_auth_get_endpoint.call_with_http_info(**kwargs)
 
+    def get_connected_entities_api_v2_lineage_connecting_entities_post(
+        self,
+        data_entity_connect_nodes_request,
+        **kwargs
+    ):
+        """Get Connected Entities  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_connected_entities_api_v2_lineage_connecting_entities_post(data_entity_connect_nodes_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_connect_nodes_request (DataEntityConnectNodesRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DataEntityLineageV3Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_connect_nodes_request'] = \
+            data_entity_connect_nodes_request
+        return self.get_connected_entities_api_v2_lineage_connecting_entities_post_endpoint.call_with_http_info(**kwargs)
+
+    def get_dashboard_costs_api_insights_v1_dashboards_post(
+        self,
+        **kwargs
+    ):
+        """Get Dashboard Costs  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_dashboard_costs_api_insights_v1_dashboards_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            body_get_dashboard_costs_api_insights_v1_dashboards_post (BodyGetDashboardCostsApiInsightsV1DashboardsPost): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DashboardCostsResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_dashboard_costs_api_insights_v1_dashboards_post_endpoint.call_with_http_info(**kwargs)
+
+    def get_dashboard_costs_api_insights_v2_dashboards_post(
+        self,
+        **kwargs
+    ):
+        """Get Dashboard Costs  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_dashboard_costs_api_insights_v2_dashboards_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            body_get_dashboard_costs_api_insights_v2_dashboards_post (BodyGetDashboardCostsApiInsightsV2DashboardsPost): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DashboardCostsV2Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_dashboard_costs_api_insights_v2_dashboards_post_endpoint.call_with_http_info(**kwargs)
+
+    def get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post(
+        self,
+        dashboard_id,
+        **kwargs
+    ):
+        """Get Dashboard Users Cost  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post(dashboard_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            dashboard_id (str):
+
+        Keyword Args:
+            body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post (BodyGetDashboardUsersCostApiInsightsV1DashboardsDashboardIdUsersPost): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DashboardUsersResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['dashboard_id'] = \
+            dashboard_id
+        return self.get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post_endpoint.call_with_http_info(**kwargs)
+
     def get_data_entity_run_facets_api_v1_entity_runs_run_id_facets_get(
         self,
         run_id,
         platform_id,
         entity_id,
         entity_type,
         **kwargs
@@ -16710,14 +18884,79 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['data_entity_lineage_v2_request_dto'] = \
             data_entity_lineage_v2_request_dto
         return self.get_entity_lineage_api_v2_lineage_post_endpoint.call_with_http_info(**kwargs)
 
+    def get_entity_lineage_children2_api_v2_lineage_children2_post(
+        self,
+        data_entity_lineage_v3_request,
+        **kwargs
+    ):
+        """Get Entity Lineage Children2  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_entity_lineage_children2_api_v2_lineage_children2_post(data_entity_lineage_v3_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_lineage_v3_request (DataEntityLineageV3Request):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            [str]
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_lineage_v3_request'] = \
+            data_entity_lineage_v3_request
+        return self.get_entity_lineage_children2_api_v2_lineage_children2_post_endpoint.call_with_http_info(**kwargs)
+
     def get_entity_lineage_children_api_v2_lineage_children_post(
         self,
         data_entity_lineage_children_request,
         **kwargs
     ):
         """Get Entity Lineage Children  # noqa: E501
 
@@ -16775,14 +19014,144 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['data_entity_lineage_children_request'] = \
             data_entity_lineage_children_request
         return self.get_entity_lineage_children_api_v2_lineage_children_post_endpoint.call_with_http_info(**kwargs)
 
+    def get_entity_lineage_explorer2_api_v2_lineage_explorer2_post(
+        self,
+        data_entity_lineage_v3_request,
+        **kwargs
+    ):
+        """Get Entity Lineage Explorer2  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_entity_lineage_explorer2_api_v2_lineage_explorer2_post(data_entity_lineage_v3_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_lineage_v3_request (DataEntityLineageV3Request):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DataEntityLineageV3Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_lineage_v3_request'] = \
+            data_entity_lineage_v3_request
+        return self.get_entity_lineage_explorer2_api_v2_lineage_explorer2_post_endpoint.call_with_http_info(**kwargs)
+
+    def get_entity_lineage_explorer_api_v2_lineage_explorer_post(
+        self,
+        data_entity_lineage_v2_request_dto,
+        **kwargs
+    ):
+        """Get Entity Lineage Explorer  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_entity_lineage_explorer_api_v2_lineage_explorer_post(data_entity_lineage_v2_request_dto, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_lineage_v2_request_dto (DataEntityLineageV2RequestDTO):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DataEntityLineageExplorerResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_lineage_v2_request_dto'] = \
+            data_entity_lineage_v2_request_dto
+        return self.get_entity_lineage_explorer_api_v2_lineage_explorer_post_endpoint.call_with_http_info(**kwargs)
+
     def get_entity_lineage_explorer_link_api_entity_v1_lineage_explorer_link_post(
         self,
         map_entity_to_url_request,
         **kwargs
     ):
         """Get Entity Lineage Explorer Link  # noqa: E501
 
@@ -16840,14 +19209,79 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['map_entity_to_url_request'] = \
             map_entity_to_url_request
         return self.get_entity_lineage_explorer_link_api_entity_v1_lineage_explorer_link_post_endpoint.call_with_http_info(**kwargs)
 
+    def get_entity_lineage_list2_api_v2_lineage_list2_post(
+        self,
+        data_entity_lineage_v3_request,
+        **kwargs
+    ):
+        """Get Entity Lineage List2  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_entity_lineage_list2_api_v2_lineage_list2_post(data_entity_lineage_v3_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_lineage_v3_request (DataEntityLineageV3Request):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DataEntityLineageV3Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_lineage_v3_request'] = \
+            data_entity_lineage_v3_request
+        return self.get_entity_lineage_list2_api_v2_lineage_list2_post_endpoint.call_with_http_info(**kwargs)
+
     def get_entity_lineage_list_api_v2_lineage_list_post(
         self,
         data_entity_lineage_list_request,
         **kwargs
     ):
         """Get Entity Lineage List  # noqa: E501
 
@@ -17524,23 +19958,23 @@
 
         >>> thread = api.get_entity_usage_stats_raw_api_v1_entity_usage_stats_raw_get(platform_id, entity_id, entity_type, async_req=True)
         >>> result = thread.get()
 
         Args:
             platform_id (str):
             entity_id (str):
-            entity_type (str):
+            entity_type (DataEntityType):
 
         Keyword Args:
             start_timestamp (datetime): [optional]
             end_timestamp (datetime): [optional]
             connection_type (ConnectionType): [optional]
             connection_direction (ConnectionDirection): [optional]
             connection_usage_classification (ConnectionUsageClassification): [optional]
-            usage_type ([str]): [optional]
+            usage_types ([str]): [optional]
             user_name ([str]): [optional]
             sort ([str]): [optional] if omitted the server will use the default value of ["start:desc"]
             limit (int): [optional] if omitted the server will use the default value of 50
             offset (int): [optional] if omitted the server will use the default value of 0
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -17589,30 +20023,31 @@
             platform_id
         kwargs['entity_id'] = \
             entity_id
         kwargs['entity_type'] = \
             entity_type
         return self.get_entity_usage_stats_raw_api_v1_entity_usage_stats_raw_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_experiences_api_v1_experience_get(
+    def get_event_users_api_events_v1_users_post(
         self,
+        event_request_filter,
         **kwargs
     ):
-        """Get Experiences  # noqa: E501
+        """Get Event Users  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_experiences_api_v1_experience_get(async_req=True)
+        >>> thread = api.get_event_users_api_events_v1_users_post(event_request_filter, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            event_request_filter (EventRequestFilter):
 
         Keyword Args:
-            lead_user_email (str): [optional]
-            user_persona (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -17626,15 +20061,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [Experience]
+            EventUsersResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -17649,28 +20084,33 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_experiences_api_v1_experience_get_endpoint.call_with_http_info(**kwargs)
+        kwargs['event_request_filter'] = \
+            event_request_filter
+        return self.get_event_users_api_events_v1_users_post_endpoint.call_with_http_info(**kwargs)
 
-    def get_failed_batches_api_kirby_v1_failed_get(
+    def get_event_users_by_period_api_events_v1_users_by_period_post(
         self,
+        list_event_users_by_period_request,
         **kwargs
     ):
-        """Get Failed Batches  # noqa: E501
+        """Get Event Users By Period  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_failed_batches_api_kirby_v1_failed_get(async_req=True)
+        >>> thread = api.get_event_users_by_period_api_events_v1_users_by_period_post(list_event_users_by_period_request, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            list_event_users_by_period_request (ListEventUsersByPeriodRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -17686,15 +20126,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            KirbyFailedBatchesResponse
+            ListEventUsersByPeriodResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -17709,28 +20149,33 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_failed_batches_api_kirby_v1_failed_get_endpoint.call_with_http_info(**kwargs)
+        kwargs['list_event_users_by_period_request'] = \
+            list_event_users_by_period_request
+        return self.get_event_users_by_period_api_events_v1_users_by_period_post_endpoint.call_with_http_info(**kwargs)
 
-    def get_filter_api_v2_filters_get(
+    def get_events_stats_api_events_v1_stats_post(
         self,
+        event_stats_request,
         **kwargs
     ):
-        """Get Filter  # noqa: E501
+        """Get Events Stats  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_filter_api_v2_filters_get(async_req=True)
+        >>> thread = api.get_events_stats_api_events_v1_stats_post(event_stats_request, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            event_stats_request (EventStatsRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -17746,15 +20191,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [FilterOptions]
+            EventStatsReport
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -17769,30 +20214,34 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_filter_api_v2_filters_get_endpoint.call_with_http_info(**kwargs)
+        kwargs['event_stats_request'] = \
+            event_stats_request
+        return self.get_events_stats_api_events_v1_stats_post_endpoint.call_with_http_info(**kwargs)
 
-    def get_filter_labels_api_v2_filter_labels_get(
+    def get_experiences_api_v1_experience_get(
         self,
         **kwargs
     ):
-        """Get Filter Labels  # noqa: E501
+        """Get Experiences  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_filter_labels_api_v2_filter_labels_get(async_req=True)
+        >>> thread = api.get_experiences_api_v1_experience_get(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
+            lead_user_email (str): [optional]
+            user_persona (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -17806,15 +20255,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            {str: (SearchFilterLabelAssociation,)}
+            [Experience]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -17829,31 +20278,30 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_filter_labels_api_v2_filter_labels_get_endpoint.call_with_http_info(**kwargs)
+        return self.get_experiences_api_v1_experience_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_filters_config_api_v1_filters_config_get(
+    def get_failed_batches_api_kirby_v1_failed_get(
         self,
         **kwargs
     ):
-        """Get Filters Config  # noqa: E501
+        """Get Failed Batches  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_filters_config_api_v1_filters_config_get(async_req=True)
+        >>> thread = api.get_failed_batches_api_kirby_v1_failed_get(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            filter_view (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -17867,15 +20315,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            FiltersResponse
+            KirbyFailedBatchesResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -17890,31 +20338,28 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_filters_config_api_v1_filters_config_get_endpoint.call_with_http_info(**kwargs)
+        return self.get_failed_batches_api_kirby_v1_failed_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_hightouch_platform_api_v1_platforms_hightouch_platform_id_get(
+    def get_filter_api_v2_filters_get(
         self,
-        platform_id,
         **kwargs
     ):
-        """Get Hightouch Platform  # noqa: E501
+        """Get Filter  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_hightouch_platform_api_v1_platforms_hightouch_platform_id_get(platform_id, async_req=True)
+        >>> thread = api.get_filter_api_v2_filters_get(async_req=True)
         >>> result = thread.get()
 
-        Args:
-            platform_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -17930,15 +20375,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            DataPlatformGet
+            [FilterOptions]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -17953,29 +20398,148 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['platform_id'] = \
-            platform_id
-        return self.get_hightouch_platform_api_v1_platforms_hightouch_platform_id_get_endpoint.call_with_http_info(**kwargs)
+        return self.get_filter_api_v2_filters_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_hive_platform_api_v1_platforms_hive_platform_id_get(
+    def get_filter_labels_api_v2_filter_labels_get(
+        self,
+        **kwargs
+    ):
+        """Get Filter Labels  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_filter_labels_api_v2_filter_labels_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            {str: (SearchFilterLabelAssociation,)}
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_filter_labels_api_v2_filter_labels_get_endpoint.call_with_http_info(**kwargs)
+
+    def get_filters_config_api_v1_filters_config_get(
+        self,
+        **kwargs
+    ):
+        """Get Filters Config  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_filters_config_api_v1_filters_config_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            filter_view (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            FiltersResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_filters_config_api_v1_filters_config_get_endpoint.call_with_http_info(**kwargs)
+
+    def get_hightouch_platform_api_v1_platforms_hightouch_platform_id_get(
         self,
         platform_id,
         **kwargs
     ):
-        """Get Hive Platform  # noqa: E501
+        """Get Hightouch Platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_hive_platform_api_v1_platforms_hive_platform_id_get(platform_id, async_req=True)
+        >>> thread = api.get_hightouch_platform_api_v1_platforms_hightouch_platform_id_get(platform_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             platform_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -18020,27 +20584,27 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['platform_id'] = \
             platform_id
-        return self.get_hive_platform_api_v1_platforms_hive_platform_id_get_endpoint.call_with_http_info(**kwargs)
+        return self.get_hightouch_platform_api_v1_platforms_hightouch_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_hiveglue_platform_api_v1_platforms_hiveglue_platform_id_get(
+    def get_hive_platform_api_v1_platforms_hive_platform_id_get(
         self,
         platform_id,
         **kwargs
     ):
-        """Get Hiveglue Platform  # noqa: E501
+        """Get Hive Platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_hiveglue_platform_api_v1_platforms_hiveglue_platform_id_get(platform_id, async_req=True)
+        >>> thread = api.get_hive_platform_api_v1_platforms_hive_platform_id_get(platform_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             platform_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -18085,28 +20649,31 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['platform_id'] = \
             platform_id
-        return self.get_hiveglue_platform_api_v1_platforms_hiveglue_platform_id_get_endpoint.call_with_http_info(**kwargs)
+        return self.get_hive_platform_api_v1_platforms_hive_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_impact_analysis_platforms_api_impact_analysis_v3_platforms_get(
+    def get_hiveglue_platform_api_v1_platforms_hiveglue_platform_id_get(
         self,
+        platform_id,
         **kwargs
     ):
-        """Get Impact Analysis Platforms  # noqa: E501
+        """Get Hiveglue Platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_impact_analysis_platforms_api_impact_analysis_v3_platforms_get(async_req=True)
+        >>> thread = api.get_hiveglue_platform_api_v1_platforms_hiveglue_platform_id_get(platform_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            platform_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -18122,15 +20689,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            [DataPlatformGet]
+            DataPlatformGet
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -18145,15 +20712,17 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_impact_analysis_platforms_api_impact_analysis_v3_platforms_get_endpoint.call_with_http_info(**kwargs)
+        kwargs['platform_id'] = \
+            platform_id
+        return self.get_hiveglue_platform_api_v1_platforms_hiveglue_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
     def get_impact_analysis_platforms_api_v2_impact_analysis_platforms_get(
         self,
         **kwargs
     ):
         """Get Impact Analysis Platforms  # noqa: E501
 
@@ -18207,25 +20776,25 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.get_impact_analysis_platforms_api_v2_impact_analysis_platforms_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_impact_by_query_api_impact_analysis_v3_query_post(
+    def get_impact_by_query_api_v2_impact_analysis_query_post(
         self,
         impact_analysis_request,
         **kwargs
     ):
         """Get Impact By Query  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_impact_by_query_api_impact_analysis_v3_query_post(impact_analysis_request, async_req=True)
+        >>> thread = api.get_impact_by_query_api_v2_impact_analysis_query_post(impact_analysis_request, async_req=True)
         >>> result = thread.get()
 
         Args:
             impact_analysis_request (ImpactAnalysisRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -18245,15 +20814,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponse
+            ImpactAnalysisResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -18270,31 +20839,31 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['impact_analysis_request'] = \
             impact_analysis_request
-        return self.get_impact_by_query_api_impact_analysis_v3_query_post_endpoint.call_with_http_info(**kwargs)
+        return self.get_impact_by_query_api_v2_impact_analysis_query_post_endpoint.call_with_http_info(**kwargs)
 
-    def get_impact_by_query_api_v2_impact_analysis_query_post(
+    def get_impact_from_validation_payload2_api_v2_impact_analysis_query_entities2_post(
         self,
-        impact_analysis_request,
+        impact_analysis_validation_payload_v2,
         **kwargs
     ):
-        """Get Impact By Query  # noqa: E501
+        """Get Impact From Validation Payload 2  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_impact_by_query_api_v2_impact_analysis_query_post(impact_analysis_request, async_req=True)
+        >>> thread = api.get_impact_from_validation_payload2_api_v2_impact_analysis_query_entities2_post(impact_analysis_validation_payload_v2, async_req=True)
         >>> result = thread.get()
 
         Args:
-            impact_analysis_request (ImpactAnalysisRequest):
+            impact_analysis_validation_payload_v2 (ImpactAnalysisValidationPayloadV2):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -18310,15 +20879,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            AppSchemasImpactAnalysisResponseImpactAnalysisResponse
+            ImpactAnalysisResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -18333,29 +20902,29 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['impact_analysis_request'] = \
-            impact_analysis_request
-        return self.get_impact_by_query_api_v2_impact_analysis_query_post_endpoint.call_with_http_info(**kwargs)
+        kwargs['impact_analysis_validation_payload_v2'] = \
+            impact_analysis_validation_payload_v2
+        return self.get_impact_from_validation_payload2_api_v2_impact_analysis_query_entities2_post_endpoint.call_with_http_info(**kwargs)
 
-    def get_impact_from_validation_payload_api_impact_analysis_v3_query_entities_post(
+    def get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post(
         self,
         impact_analysis_validation_payload,
         **kwargs
     ):
         """Get Impact From Validation Payload  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_impact_from_validation_payload_api_impact_analysis_v3_query_entities_post(impact_analysis_validation_payload, async_req=True)
+        >>> thread = api.get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post(impact_analysis_validation_payload, async_req=True)
         >>> result = thread.get()
 
         Args:
             impact_analysis_validation_payload (ImpactAnalysisValidationPayload):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -18375,15 +20944,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponse
+            ImpactAnalysisResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -18400,31 +20969,31 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['impact_analysis_validation_payload'] = \
             impact_analysis_validation_payload
-        return self.get_impact_from_validation_payload_api_impact_analysis_v3_query_entities_post_endpoint.call_with_http_info(**kwargs)
+        return self.get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post_endpoint.call_with_http_info(**kwargs)
 
-    def get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post(
+    def get_insights_period_report_api_insights_v1_post(
         self,
-        impact_analysis_validation_payload,
+        insights_request,
         **kwargs
     ):
-        """Get Impact From Validation Payload  # noqa: E501
+        """Get Insights Period Report  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post(impact_analysis_validation_payload, async_req=True)
+        >>> thread = api.get_insights_period_report_api_insights_v1_post(insights_request, async_req=True)
         >>> result = thread.get()
 
         Args:
-            impact_analysis_validation_payload (ImpactAnalysisValidationPayload):
+            insights_request (InsightsRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -18440,15 +21009,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            AppSchemasImpactAnalysisResponseImpactAnalysisResponse
+            InsightsDeltaResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -18463,30 +21032,33 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['impact_analysis_validation_payload'] = \
-            impact_analysis_validation_payload
-        return self.get_impact_from_validation_payload_api_v2_impact_analysis_query_entities_post_endpoint.call_with_http_info(**kwargs)
+        kwargs['insights_request'] = \
+            insights_request
+        return self.get_insights_period_report_api_insights_v1_post_endpoint.call_with_http_info(**kwargs)
 
     def get_invited_users_to_org_api_v2_users_invite_get(
         self,
+        org_id,
         **kwargs
     ):
         """Get Invited Users To Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_invited_users_to_org_api_v2_users_invite_get(async_req=True)
+        >>> thread = api.get_invited_users_to_org_api_v2_users_invite_get(org_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            org_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -18525,14 +21097,16 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
         return self.get_invited_users_to_org_api_v2_users_invite_get_endpoint.call_with_http_info(**kwargs)
 
     def get_job_entity_usage_stats_report_api_v1_job_usage_stats_get(
         self,
         job_hash,
         platform_id,
         start_timestamp,
@@ -18978,14 +21552,79 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['job_query_request'] = \
             job_query_request
         return self.get_last_job_query_api_v1_job_query_post_endpoint.call_with_http_info(**kwargs)
 
+    def get_lineage_graph_api_v2_lineage_graph_post(
+        self,
+        lineage_graph_request,
+        **kwargs
+    ):
+        """Get Lineage Graph  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_lineage_graph_api_v2_lineage_graph_post(lineage_graph_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            lineage_graph_request (LineageGraphRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DataEntityLineageV3Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['lineage_graph_request'] = \
+            lineage_graph_request
+        return self.get_lineage_graph_api_v2_lineage_graph_post_endpoint.call_with_http_info(**kwargs)
+
     def get_lineage_job_steps_api_v1_lineage_jobs_steps_get(
         self,
         from_entity_id,
         from_entity_type,
         from_entity_platform_id,
         to_entity_id,
         to_entity_type,
@@ -19699,14 +22338,139 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.get_org_platform_asset_types_api_v2_org_platform_asset_types_post_endpoint.call_with_http_info(**kwargs)
 
+    def get_organization_info_api_v1_organization_get(
+        self,
+        **kwargs
+    ):
+        """Get Organization Info  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_organization_info_api_v1_organization_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            OrganizationGet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_organization_info_api_v1_organization_get_endpoint.call_with_http_info(**kwargs)
+
+    def get_organization_info_from_org_id_api_v1_organization_org_id_get(
+        self,
+        org_id,
+        **kwargs
+    ):
+        """Get Organization Info From Org Id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_organization_info_from_org_id_api_v1_organization_org_id_get(org_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            OrganizationGet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        return self.get_organization_info_from_org_id_api_v1_organization_org_id_get_endpoint.call_with_http_info(**kwargs)
+
     def get_parent_taxonomy_classifications_api_v1_taxonomy_parents_get(
         self,
         **kwargs
     ):
         """Get Parent Taxonomy Classifications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19759,14 +22523,141 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.get_parent_taxonomy_classifications_api_v1_taxonomy_parents_get_endpoint.call_with_http_info(**kwargs)
 
+    def get_pipeline_by_id_api_v1_pipeline_pipeline_id_get(
+        self,
+        pipeline_id,
+        **kwargs
+    ):
+        """Get Pipeline By Id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_pipeline_by_id_api_v1_pipeline_pipeline_id_get(pipeline_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            pipeline_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['pipeline_id'] = \
+            pipeline_id
+        return self.get_pipeline_by_id_api_v1_pipeline_pipeline_id_get_endpoint.call_with_http_info(**kwargs)
+
+    def get_pipelines_api_v1_pipelines_get(
+        self,
+        **kwargs
+    ):
+        """Get Pipelines  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_pipelines_api_v1_pipelines_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            page (int): [optional] if omitted the server will use the default value of 1
+            size (int): [optional] if omitted the server will use the default value of 50
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            LimitOffsetPagePipelineGet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_pipelines_api_v1_pipelines_get_endpoint.call_with_http_info(**kwargs)
+
     def get_platform_api_v1_platforms_platform_id_get(
         self,
         platform_id,
         **kwargs
     ):
         """Get Platform  # noqa: E501
 
@@ -20327,14 +23218,82 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['platform_id'] = \
             platform_id
         return self.get_redshift_platform_api_v1_platforms_redshift_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
+    def get_simple_lineage_api_v2_simple_lineage_entity_fqn_get(
+        self,
+        entity_fqn,
+        **kwargs
+    ):
+        """Get Simple Lineage  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_simple_lineage_api_v2_simple_lineage_entity_fqn_get(entity_fqn, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            entity_fqn (str):
+
+        Keyword Args:
+            upstream (bool): [optional] if omitted the server will use the default value of False
+            get_parent_enriched (bool): [optional] if omitted the server will use the default value of False
+            group_by_parent (bool): [optional] if omitted the server will use the default value of False
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            DataEntitySimpleLineageResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['entity_fqn'] = \
+            entity_fqn
+        return self.get_simple_lineage_api_v2_simple_lineage_entity_fqn_get_endpoint.call_with_http_info(**kwargs)
+
     def get_snowflake_platform_api_v1_platforms_snowflake_platform_id_get(
         self,
         platform_id,
         **kwargs
     ):
         """Get Snowflake Platform  # noqa: E501
 
@@ -20392,14 +23351,75 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['platform_id'] = \
             platform_id
         return self.get_snowflake_platform_api_v1_platforms_snowflake_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
+    def get_table_num_rows_api_entity_v1_num_rows_get(
+        self,
+        **kwargs
+    ):
+        """Get Table Num Rows  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_table_num_rows_api_entity_v1_num_rows_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            fqn (str): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            GetTableNumRowsChartResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.get_table_num_rows_api_entity_v1_num_rows_get_endpoint.call_with_http_info(**kwargs)
+
     def get_tableau_platform_api_v1_platforms_tableau_platform_id_get(
         self,
         platform_id,
         **kwargs
     ):
         """Get Tableau Platform  # noqa: E501
 
@@ -20841,14 +23861,81 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['platform_id'] = \
             platform_id
         return self.get_treasuredata_platform_api_v1_platforms_treasuredata_platform_id_get_endpoint.call_with_http_info(**kwargs)
 
+    def get_usage_api_insights_v1_usage_post(
+        self,
+        insights_usage_request,
+        **kwargs
+    ):
+        """Get Usage  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_usage_api_insights_v1_usage_post(insights_usage_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            insights_usage_request (InsightsUsageRequest):
+
+        Keyword Args:
+            limit (int): [optional] if omitted the server will use the default value of 50
+            offset (int): [optional] if omitted the server will use the default value of 0
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            LimitOffsetPageInsightsUsageResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['insights_usage_request'] = \
+            insights_usage_request
+        return self.get_usage_api_insights_v1_usage_post_endpoint.call_with_http_info(**kwargs)
+
     def get_user_id_api_v1_user_id_get(
         self,
         user_email,
         **kwargs
     ):
         """Get User Id  # noqa: E501
 
@@ -20966,26 +24053,29 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.get_user_info_api_v1_me_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_user_info_api_v1_organization_get(
+    def get_user_invite_by_link_id_api_v2_users_invite_link_id_get(
         self,
+        link_id,
         **kwargs
     ):
-        """Get User Info  # noqa: E501
+        """Get User Invite By Link Id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_user_info_api_v1_organization_get(async_req=True)
+        >>> thread = api.get_user_invite_by_link_id_api_v2_users_invite_link_id_get(link_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            link_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -21001,15 +24091,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            OrganizationGet
+            bool, date, datetime, dict, float, int, list, str, none_type
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -21024,27 +24114,29 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.get_user_info_api_v1_organization_get_endpoint.call_with_http_info(**kwargs)
+        kwargs['link_id'] = \
+            link_id
+        return self.get_user_invite_by_link_id_api_v2_users_invite_link_id_get_endpoint.call_with_http_info(**kwargs)
 
-    def get_user_invite_by_link_id_api_v2_users_invite_link_id_get(
+    def get_user_invite_object_api_v2_user_invite_link_id_get(
         self,
         link_id,
         **kwargs
     ):
-        """Get User Invite By Link Id  # noqa: E501
+        """Get User Invite Object  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_user_invite_by_link_id_api_v2_users_invite_link_id_get(link_id, async_req=True)
+        >>> thread = api.get_user_invite_object_api_v2_user_invite_link_id_get(link_id, async_req=True)
         >>> result = thread.get()
 
         Args:
             link_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
@@ -21064,15 +24156,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            UserInviteCreate
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -21089,15 +24181,15 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['link_id'] = \
             link_id
-        return self.get_user_invite_by_link_id_api_v2_users_invite_link_id_get_endpoint.call_with_http_info(**kwargs)
+        return self.get_user_invite_object_api_v2_user_invite_link_id_get_endpoint.call_with_http_info(**kwargs)
 
     def get_user_popular_searches_api_v2_user_search_popular_get(
         self,
         **kwargs
     ):
         """Get User Popular Searches  # noqa: E501
 
@@ -21589,26 +24681,28 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['kirby_ingest_request'] = \
             kirby_ingest_request
         return self.ingest_file_api_kirby_v1_ingest_failed_post_endpoint.call_with_http_info(**kwargs)
 
     def invite_user_to_org_api_v2_users_invite_post(
         self,
+        org_id,
         user_create_request,
         **kwargs
     ):
         """Invite User To Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.invite_user_to_org_api_v2_users_invite_post(user_create_request, async_req=True)
+        >>> thread = api.invite_user_to_org_api_v2_users_invite_post(org_id, user_create_request, async_req=True)
         >>> result = thread.get()
 
         Args:
+            org_id (str):
             user_create_request (UserCreateRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -21648,14 +24742,16 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
         kwargs['user_create_request'] = \
             user_create_request
         return self.invite_user_to_org_api_v2_users_invite_post_endpoint.call_with_http_info(**kwargs)
 
     def lineage_api_v1_lineage_post(
         self,
         unknown_base_type,
@@ -21717,14 +24813,79 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['unknown_base_type'] = \
             unknown_base_type
         return self.lineage_api_v1_lineage_post_endpoint.call_with_http_info(**kwargs)
 
+    def lineage_has_temp_entity_api_v2_lineage_has_temp_entity_post(
+        self,
+        data_entity_lineage_v2_request_dto,
+        **kwargs
+    ):
+        """Lineage Has Temp Entity  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.lineage_has_temp_entity_api_v2_lineage_has_temp_entity_post(data_entity_lineage_v2_request_dto, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_lineage_v2_request_dto (DataEntityLineageV2RequestDTO):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_lineage_v2_request_dto'] = \
+            data_entity_lineage_v2_request_dto
+        return self.lineage_has_temp_entity_api_v2_lineage_has_temp_entity_post_endpoint.call_with_http_info(**kwargs)
+
     def lineage_spark_api_v1_lineage_spark_post(
         self,
         unknown_base_type,
         **kwargs
     ):
         """Lineage Spark  # noqa: E501
 
@@ -21782,14 +24943,79 @@
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['unknown_base_type'] = \
             unknown_base_type
         return self.lineage_spark_api_v1_lineage_spark_post_endpoint.call_with_http_info(**kwargs)
 
+    def list_databases_api_events_v1_list_databases_post(
+        self,
+        list_event_databases_request,
+        **kwargs
+    ):
+        """List Databases  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_databases_api_events_v1_list_databases_post(list_event_databases_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            list_event_databases_request (ListEventDatabasesRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ListEventDatabasesResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['list_event_databases_request'] = \
+            list_event_databases_request
+        return self.list_databases_api_events_v1_list_databases_post_endpoint.call_with_http_info(**kwargs)
+
     def list_manual_lineage_api_v1_lineage_manual_get(
         self,
         **kwargs
     ):
         """List Manual Lineage  # noqa: E501
 
         Return paginated result of Manual Lineage Data  # noqa: E501
@@ -21923,26 +25149,94 @@
             entity_type
         kwargs['entity_id'] = \
             entity_id
         kwargs['platform_id'] = \
             platform_id
         return self.list_manual_lineage_valid_entity_types_api_v1_lineage_manual_valid_entity_types_get_endpoint.call_with_http_info(**kwargs)
 
+    def list_platform_databases_api_v2_search_list_databases_post(
+        self,
+        list_platform_databases_request,
+        **kwargs
+    ):
+        """List Platform Databases  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_platform_databases_api_v2_search_list_databases_post(list_platform_databases_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            list_platform_databases_request (ListPlatformDatabasesRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ListPlatformDatabasesResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['list_platform_databases_request'] = \
+            list_platform_databases_request
+        return self.list_platform_databases_api_v2_search_list_databases_post_endpoint.call_with_http_info(**kwargs)
+
     def list_users_in_org_api_v2_users_get(
         self,
+        org_id,
         **kwargs
     ):
         """List Users In Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_users_in_org_api_v2_users_get(async_req=True)
+        >>> thread = api.list_users_in_org_api_v2_users_get(org_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            org_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -21981,16 +25275,203 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
         return self.list_users_in_org_api_v2_users_get_endpoint.call_with_http_info(**kwargs)
 
+    def load_api_graph_v1_load_get(
+        self,
+        **kwargs
+    ):
+        """Load  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.load_api_graph_v1_load_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.load_api_graph_v1_load_get_endpoint.call_with_http_info(**kwargs)
+
+    def login_api_auth_v1_sso_login_get(
+        self,
+        **kwargs
+    ):
+        """Login  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.login_api_auth_v1_sso_login_get(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.login_api_auth_v1_sso_login_get_endpoint.call_with_http_info(**kwargs)
+
+    def metadata_api_dbt_v1_metadata_post(
+        self,
+        unknown_base_type,
+        **kwargs
+    ):
+        """Metadata  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.metadata_api_dbt_v1_metadata_post(unknown_base_type, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            unknown_base_type (UNKNOWN_BASE_TYPE):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['unknown_base_type'] = \
+            unknown_base_type
+        return self.metadata_api_dbt_v1_metadata_post_endpoint.call_with_http_info(**kwargs)
+
     def metadata_api_v1_metadata_post(
         self,
         unknown_base_type,
         **kwargs
     ):
         """Metadata  # noqa: E501
 
@@ -22176,26 +25657,28 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['experience_data'] = \
             experience_data
         return self.register_interest_api_v1_experiences_register_interest_post_endpoint.call_with_http_info(**kwargs)
 
     def remove_user_from_org_api_v2_user_delete(
         self,
+        org_id,
         user_id,
         **kwargs
     ):
         """Remove User From Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.remove_user_from_org_api_v2_user_delete(user_id, async_req=True)
+        >>> thread = api.remove_user_from_org_api_v2_user_delete(org_id, user_id, async_req=True)
         >>> result = thread.get()
 
         Args:
+            org_id (str):
             user_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -22235,14 +25718,16 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
         kwargs['user_id'] = \
             user_id
         return self.remove_user_from_org_api_v2_user_delete_endpoint.call_with_http_info(**kwargs)
 
     def request_access_api_v1_experiences_request_access_post(
         self,
         experience_data,
@@ -22709,14 +26194,16 @@
 
         >>> thread = api.search_api_v2_search_post(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             search_string (str): [optional] if omitted the server will use the default value of ""
+            generate_filter_count_data (bool): [optional] if omitted the server will use the default value of True
+            generate_downstream_usage (bool): [optional] if omitted the server will use the default value of False
             page (int): [optional] if omitted the server will use the default value of 1
             size (int): [optional] if omitted the server will use the default value of 50
             search_node ([SearchNode]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -22758,14 +26245,79 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.search_api_v2_search_post_endpoint.call_with_http_info(**kwargs)
 
+    def search_entities_api_v2_search_entities_post(
+        self,
+        data_entity_id,
+        **kwargs
+    ):
+        """Search Entities  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_entities_api_v2_search_entities_post(data_entity_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            data_entity_id ([DataEntityID]):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SearchEntitiesResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['data_entity_id'] = \
+            data_entity_id
+        return self.search_entities_api_v2_search_entities_post_endpoint.call_with_http_info(**kwargs)
+
     def search_entities_stats_post_api_v1_search_entities_usage_stats_post(
         self,
         platform_id,
         entity_type,
         start_timestamp,
         end_timestamp,
         data_entity_usage_stats_request,
@@ -22915,14 +26467,144 @@
             platform_id
         kwargs['entity_id'] = \
             entity_id
         kwargs['entity_type'] = \
             entity_type
         return self.search_entity_by_id_api_v2_search_find_entity_post_endpoint.call_with_http_info(**kwargs)
 
+    def search_events_api_events_v1_search_post(
+        self,
+        event_search_request,
+        **kwargs
+    ):
+        """Search Events  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_events_api_events_v1_search_post(event_search_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            event_search_request (EventSearchRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            EventSearchResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['event_search_request'] = \
+            event_search_request
+        return self.search_events_api_events_v1_search_post_endpoint.call_with_http_info(**kwargs)
+
+    def search_events_timeline_api_events_v1_search_timeline_post(
+        self,
+        event_search_request,
+        **kwargs
+    ):
+        """Search Events Timeline  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_events_timeline_api_events_v1_search_timeline_post(event_search_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            event_search_request (EventSearchRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            EventSearchTimelineResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['event_search_request'] = \
+            event_search_request
+        return self.search_events_timeline_api_events_v1_search_timeline_post_endpoint.call_with_http_info(**kwargs)
+
     def set_org_status_api_v1_organization_status_post(
         self,
         status,
         **kwargs
     ):
         """Set Org Status  # noqa: E501
 
@@ -24277,27 +27959,29 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['code'] = \
             code
         return self.tinyurl_api_v1_tinyurl_get_endpoint.call_with_http_info(**kwargs)
 
     def update_invite_to_organization_status_api_v2_users_invite_put(
         self,
+        org_id,
         invite_id,
         status,
         **kwargs
     ):
         """Update Invite To Organization Status  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_invite_to_organization_status_api_v2_users_invite_put(invite_id, status, async_req=True)
+        >>> thread = api.update_invite_to_organization_status_api_v2_users_invite_put(org_id, invite_id, status, async_req=True)
         >>> result = thread.get()
 
         Args:
+            org_id (str):
             invite_id (str):
             status (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -24338,37 +28022,39 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
         kwargs['invite_id'] = \
             invite_id
         kwargs['status'] = \
             status
         return self.update_invite_to_organization_status_api_v2_users_invite_put_endpoint.call_with_http_info(**kwargs)
 
-    def update_org_status_api_v2_organizations_org_id_post(
+    def update_org_api_v1_organization_update_post(
         self,
         org_id,
-        status,
+        organization_update,
         **kwargs
     ):
-        """Update Org Status  # noqa: E501
+        """Update Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_org_status_api_v2_organizations_org_id_post(org_id, status, async_req=True)
+        >>> thread = api.update_org_api_v1_organization_update_post(org_id, organization_update, async_req=True)
         >>> result = thread.get()
 
         Args:
             org_id (str):
-            status (OrganizationStatus):
+            organization_update (OrganizationUpdate):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -24409,33 +28095,35 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['org_id'] = \
             org_id
-        kwargs['status'] = \
-            status
-        return self.update_org_status_api_v2_organizations_org_id_post_endpoint.call_with_http_info(**kwargs)
+        kwargs['organization_update'] = \
+            organization_update
+        return self.update_org_api_v1_organization_update_post_endpoint.call_with_http_info(**kwargs)
 
-    def update_user_in_org_api_v2_user_put(
+    def update_org_status_api_v2_organizations_org_id_post(
         self,
-        user_create_request,
+        org_id,
+        status,
         **kwargs
     ):
-        """Update User In Org  # noqa: E501
+        """Update Org Status  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_user_in_org_api_v2_user_put(user_create_request, async_req=True)
+        >>> thread = api.update_org_status_api_v2_organizations_org_id_post(org_id, status, async_req=True)
         >>> result = thread.get()
 
         Args:
-            user_create_request (UserCreateRequest):
+            org_id (str):
+            status (OrganizationStatus):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -24474,33 +28162,37 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['user_create_request'] = \
-            user_create_request
-        return self.update_user_in_org_api_v2_user_put_endpoint.call_with_http_info(**kwargs)
+        kwargs['org_id'] = \
+            org_id
+        kwargs['status'] = \
+            status
+        return self.update_org_status_api_v2_organizations_org_id_post_endpoint.call_with_http_info(**kwargs)
 
-    def update_view_api_v2_views_update_put(
+    def update_user_in_org_api_v2_user_put(
         self,
-        view_get,
+        org_id,
+        user_create_request,
         **kwargs
     ):
-        """Update View  # noqa: E501
+        """Update User In Org  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_view_api_v2_views_update_put(view_get, async_req=True)
+        >>> thread = api.update_user_in_org_api_v2_user_put(org_id, user_create_request, async_req=True)
         >>> result = thread.get()
 
         Args:
-            view_get (ViewGet):
+            org_id (str):
+            user_create_request (UserCreateRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -24516,15 +28208,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            ViewSaveResponse
+            bool, date, datetime, dict, float, int, list, str, none_type
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -24539,33 +28231,35 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['view_get'] = \
-            view_get
-        return self.update_view_api_v2_views_update_put_endpoint.call_with_http_info(**kwargs)
+        kwargs['org_id'] = \
+            org_id
+        kwargs['user_create_request'] = \
+            user_create_request
+        return self.update_user_in_org_api_v2_user_put_endpoint.call_with_http_info(**kwargs)
 
-    def validate_impact_analysis_query_api_impact_analysis_v3_validate_query_post(
+    def update_view_api_v2_views_update_put(
         self,
-        impact_analysis_request,
+        view_get,
         **kwargs
     ):
-        """Validate Impact Analysis Query  # noqa: E501
+        """Update View  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.validate_impact_analysis_query_api_impact_analysis_v3_validate_query_post(impact_analysis_request, async_req=True)
+        >>> thread = api.update_view_api_v2_views_update_put(view_get, async_req=True)
         >>> result = thread.get()
 
         Args:
-            impact_analysis_request (ImpactAnalysisRequest):
+            view_get (ViewGet):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -24581,15 +28275,15 @@
                 Default is True.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            ImpactAnalysisQueryValidation
+            ViewSaveResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -24604,17 +28298,17 @@
         kwargs['_check_input_type'] = kwargs.get(
             '_check_input_type', True
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['impact_analysis_request'] = \
-            impact_analysis_request
-        return self.validate_impact_analysis_query_api_impact_analysis_v3_validate_query_post_endpoint.call_with_http_info(**kwargs)
+        kwargs['view_get'] = \
+            view_get
+        return self.update_view_api_v2_views_update_put_endpoint.call_with_http_info(**kwargs)
 
     def validate_impact_analysis_query_api_v2_impact_analysis_validate_query_post(
         self,
         impact_analysis_request,
         **kwargs
     ):
         """Validate Impact Analysis Query  # noqa: E501
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/api_client.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
     Alvin
 
+
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/configuration.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/exceptions.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/accept_invite_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/accept_invite_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/admin_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/admin_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/airflow_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/airflow_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/alter_parse_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/alter_parse_result.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/alter_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/alter_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/alvin_description_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/alvin_description_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/api_key_scope.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/api_key_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
             'USER_INHERITED': "USER_INHERITED",
             'IMPACT_ANALYSIS_API': "IMPACT_ANALYSIS_API",
+            'EMBEDDED_LINEAGE': "EMBEDDED_LINEAGE",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -101,18 +102,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """APIKeyScope - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", "EMBEDDED_LINEAGE", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", "EMBEDDED_LINEAGE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -191,18 +192,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """APIKeyScope - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", "EMBEDDED_LINEAGE", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["USER_INHERITED", "IMPACT_ANALYSIS_API", "EMBEDDED_LINEAGE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/api_key_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/api_key_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/api_keys_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/api_keys_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_query_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_query_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_query_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_query_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/auth_provider.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/auth_provider.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/bi_platform.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/bi_platform.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/big_query_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/big_query_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/big_query_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/big_query_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/big_query_entity_map.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/big_query_entity_map.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/body_download_search_as_file_api_v2_search_file_post.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_download_search_as_file_api_v2_search_file_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             search_nodes ([SearchNode]): [optional] if omitted the server will use the default value of []  # noqa: E501
-            columns ([SearchCSVColumn]): [optional] if omitted the server will use the default value of ["Parent","Platform Name","Platform Type","Name","Description","Terms","Tags","Data Type","Asset Type"]  # noqa: E501
+            columns ([SearchCSVColumn]): [optional] if omitted the server will use the default value of ["Parent","Platform Name","Platform Type","Name","Description","Terms","Tags","Data Type","Asset Type","Last Used","7d Usage","30d Usage","Users","30d Cost","30d Upstream Cost","30d Downstream Usage","Downstream Users","Orchestration"]  # noqa: E501
             group_by ([SearchCSVColumn]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -227,15 +227,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             search_nodes ([SearchNode]): [optional] if omitted the server will use the default value of []  # noqa: E501
-            columns ([SearchCSVColumn]): [optional] if omitted the server will use the default value of ["Parent","Platform Name","Platform Type","Name","Description","Terms","Tags","Data Type","Asset Type"]  # noqa: E501
+            columns ([SearchCSVColumn]): [optional] if omitted the server will use the default value of ["Parent","Platform Name","Platform Type","Name","Description","Terms","Tags","Data Type","Asset Type","Last Used","7d Usage","30d Usage","Users","30d Cost","30d Upstream Cost","30d Downstream Usage","Downstream Users","Orchestration"]  # noqa: E501
             group_by ([SearchCSVColumn]): [optional] if omitted the server will use the default value of []  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/body_get_manual_entities_api_v1_manual_entities_post.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/body_get_manual_entities_api_v1_manual_entities_post.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/bulk_search_v2_response_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/bulk_search_v2_response_payload.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/classification_match_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/classification_match_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/classification_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/classification_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/client_auth_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/client_auth_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/client_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/client_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/client_config_post_auth.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/client_config_post_auth.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/column_alter.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/column_alter.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/column_target.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/column_target.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/comparison_operator.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/comparison_operator.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,17 +53,20 @@
     allowed_values = {
         ('value',): {
             'IS': "IS",
             'NOT': "NOT",
             'IS_NOT': "IS_NOT",
             'CONTAINS': "CONTAINS",
             'GREATER_THAN': "GREATER_THAN",
+            'EQUAL_OR_GREATER_THAN': "EQUAL_OR_GREATER_THAN",
             'MORE_THAN': "MORE_THAN",
             'LESS_THAN': "LESS_THAN",
+            'EQUAL_OR_LESS_THAN': "EQUAL_OR_LESS_THAN",
             'EXACTLY': "EXACTLY",
+            'EXACT_TERM': "EXACT_TERM",
             'BETWEEN': "BETWEEN",
             'STARTS_WITH': "STARTS_WITH",
             'ENDS_WITH': "ENDS_WITH",
         },
     }
 
     validations = {
@@ -110,18 +113,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """ComparisonOperator - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "MORE_THAN", "LESS_THAN", "EXACTLY", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "EQUAL_OR_GREATER_THAN", "MORE_THAN", "LESS_THAN", "EQUAL_OR_LESS_THAN", "EXACTLY", "EXACT_TERM", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "MORE_THAN", "LESS_THAN", "EXACTLY", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "EQUAL_OR_GREATER_THAN", "MORE_THAN", "LESS_THAN", "EQUAL_OR_LESS_THAN", "EXACTLY", "EXACT_TERM", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -200,18 +203,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """ComparisonOperator - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "MORE_THAN", "LESS_THAN", "EXACTLY", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "EQUAL_OR_GREATER_THAN", "MORE_THAN", "LESS_THAN", "EQUAL_OR_LESS_THAN", "EXACTLY", "EXACT_TERM", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "MORE_THAN", "LESS_THAN", "EXACTLY", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["IS", "NOT", "IS_NOT", "CONTAINS", "GREATER_THAN", "EQUAL_OR_GREATER_THAN", "MORE_THAN", "LESS_THAN", "EQUAL_OR_LESS_THAN", "EXACTLY", "EXACT_TERM", "BETWEEN", "STARTS_WITH", "ENDS_WITH", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/config_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/config_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/connection_direction.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/connection_direction.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/connection_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/connection_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/connection_usage_classification.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/connection_usage_classification.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_asset_count_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_asset_count_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_connection.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connection.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_connection_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connection_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_connection_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_connection_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_delete_tag_connection_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_delete_tag_connection_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_dependency_direction.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_dependency_direction.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_dependency_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_dependency_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_dependency_get_list.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_dependency_get_list.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_detail.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_detail.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_id.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     allowed_values = {
     }
 
     validations = {
         ('platform_id',): {
             'min_length': 3,
             'regex': {
-                'pattern': r'^[a-z][a-z0-9_]*$',  # noqa: E501
+                'pattern': r'^[aA-zZ][aA-zZ0-9_]*$',  # noqa: E501
             },
         },
         ('org_id',): {
             'min_length': 3,
             'regex': {
                 'pattern': r'^[a-z][a-z0-9_]*$',  # noqa: E501
             },
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_iddto.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_iddto.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_job_run.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_job_run.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_job_run_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_job_run_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_job_step.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_job_step.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_children_item.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_children_item.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_children_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_children_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_children_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_children_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_data.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_graph_edge.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_graph_edge.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_graph_node.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_graph_node.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list_item.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from alvin_api_client.model.data_entity_lineage_data import DataEntityLineageData
+    from alvin_api_client.model.entity_usage_context import EntityUsageContext
     from alvin_api_client.model.popularity_values import PopularityValues
     globals()['DataEntityLineageData'] = DataEntityLineageData
+    globals()['EntityUsageContext'] = EntityUsageContext
     globals()['PopularityValues'] = PopularityValues
 
 
 class DataEntityLineageListItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -86,46 +88,47 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'entity': (DataEntityLineageData,),  # noqa: E501
-            'popularity_values': (PopularityValues,),  # noqa: E501
             'level': (int,),  # noqa: E501
             'maximum_depth_found': (int,),  # noqa: E501
+            'entity_usage_context': (EntityUsageContext,),  # noqa: E501
+            'popularity_values': (PopularityValues,),  # noqa: E501
             'last_seen': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'entity': 'entity',  # noqa: E501
-        'popularity_values': 'popularityValues',  # noqa: E501
         'level': 'level',  # noqa: E501
         'maximum_depth_found': 'maximumDepthFound',  # noqa: E501
+        'entity_usage_context': 'entityUsageContext',  # noqa: E501
+        'popularity_values': 'popularityValues',  # noqa: E501
         'last_seen': 'lastSeen',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, entity, popularity_values, level, maximum_depth_found, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, entity, level, maximum_depth_found, *args, **kwargs):  # noqa: E501
         """DataEntityLineageListItem - a model defined in OpenAPI
 
         Args:
             entity (DataEntityLineageData):
-            popularity_values (PopularityValues):
             level (int):
             maximum_depth_found (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -152,14 +155,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
+            popularity_values (PopularityValues): [optional]  # noqa: E501
             last_seen (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -181,15 +186,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.entity = entity
-        self.popularity_values = popularity_values
         self.level = level
         self.maximum_depth_found = maximum_depth_found
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -204,20 +208,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, entity, popularity_values, level, maximum_depth_found, *args, **kwargs):  # noqa: E501
+    def __init__(self, entity, level, maximum_depth_found, *args, **kwargs):  # noqa: E501
         """DataEntityLineageListItem - a model defined in OpenAPI
 
         Args:
             entity (DataEntityLineageData):
-            popularity_values (PopularityValues):
             level (int):
             maximum_depth_found (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -244,14 +247,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
+            popularity_values (PopularityValues): [optional]  # noqa: E501
             last_seen (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -271,15 +276,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.entity = entity
-        self.popularity_values = popularity_values
         self.level = level
         self.maximum_depth_found = maximum_depth_found
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_list_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_list_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_node.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_node.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from alvin_api_client.model.data_entity_lineage import DataEntityLineage
+    from alvin_api_client.model.data_entity_lineage_graph_edge import DataEntityLineageGraphEdge
     globals()['DataEntityLineage'] = DataEntityLineage
+    globals()['DataEntityLineageGraphEdge'] = DataEntityLineageGraphEdge
 
 
 class DataEntityLineageResult(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -85,24 +87,26 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'lineage': (DataEntityLineage,),  # noqa: E501
             'level': (int,),  # noqa: E501
+            'edge': (DataEntityLineageGraphEdge,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'lineage': 'lineage',  # noqa: E501
         'level': 'level',  # noqa: E501
+        'edge': 'edge',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -142,14 +146,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            edge (DataEntityLineageGraphEdge): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -229,14 +234,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            edge (DataEntityLineageGraphEdge): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_v2_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v2_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_v2_request_dto.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v2_request_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             'load_children_lineage': (bool,),  # noqa: E501
             'expand_transformations': (bool,),  # noqa: E501
             'expand_dw_transformations': (bool,),  # noqa: E501
             'fetch_entity_run_lineage': (bool,),  # noqa: E501
             'fetch_jobs': (bool,),  # noqa: E501
             'fetch_latest_job': (bool,),  # noqa: E501
             'invalidate_cache_count': (int,),  # noqa: E501
+            'force_graph_calculation': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -159,14 +160,15 @@
         'load_children_lineage': 'loadChildrenLineage',  # noqa: E501
         'expand_transformations': 'expandTransformations',  # noqa: E501
         'expand_dw_transformations': 'expandDwTransformations',  # noqa: E501
         'fetch_entity_run_lineage': 'fetchEntityRunLineage',  # noqa: E501
         'fetch_jobs': 'fetchJobs',  # noqa: E501
         'fetch_latest_job': 'fetchLatestJob',  # noqa: E501
         'invalidate_cache_count': 'invalidateCacheCount',  # noqa: E501
+        'force_graph_calculation': 'forceGraphCalculation',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -233,14 +235,15 @@
             load_children_lineage (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             expand_transformations (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             expand_dw_transformations (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             fetch_entity_run_lineage (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             fetch_jobs (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
             fetch_latest_job (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
             invalidate_cache_count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+            force_graph_calculation (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -346,14 +349,15 @@
             load_children_lineage (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             expand_transformations (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             expand_dw_transformations (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             fetch_entity_run_lineage (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
             fetch_jobs (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
             fetch_latest_job (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
             invalidate_cache_count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
+            force_graph_calculation (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_lineage_v2_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_lineage_v2_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_file_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_file_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_generic_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_generic_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_topic_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_topic_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_manual_update.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_manual_update.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_numerical_stat.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_numerical_stat.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_numerical_stat_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_numerical_stat_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_numerical_stat_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_numerical_stat_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_facet_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_facet_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_id.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_id.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_job_mapping_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_job_mapping_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_job_step_mapping_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_job_step_mapping_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_run_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_run_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_save_tag_connection_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_save_tag_connection_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_sub_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_sub_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             'TABLE': "TABLE",
             'EXTERNAL_TABLE': "EXTERNAL_TABLE",
             'TEMP_ENTITY': "TEMP_ENTITY",
             'LOOKER_PDT': "LOOKER_PDT",
             'DIMENSION_FIELD': "DIMENSION_FIELD",
             'MEASURE_FIELD': "MEASURE_FIELD",
             'FILTER_FIELD': "FILTER_FIELD",
+            'LIMITED_PERMISSION': "LIMITED_PERMISSION",
             'SALESFORCE': "SALESFORCE",
             'BIGQUERY': "BIGQUERY",
             'SNOWFLAKE': "SNOWFLAKE",
             'REDSHIFT': "REDSHIFT",
             'POSTGRES': "POSTGRES",
             'QUERY_EXPORT': "QUERY_EXPORT",
             'JSON': "JSON",
@@ -119,18 +120,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """DataEntitySubType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "LIMITED_PERMISSION", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "LIMITED_PERMISSION", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -209,18 +210,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """DataEntitySubType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "LIMITED_PERMISSION", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["VIEW", "MATERIALIZED_VIEW", "TABLE", "EXTERNAL_TABLE", "TEMP_ENTITY", "LOOKER_PDT", "DIMENSION_FIELD", "MEASURE_FIELD", "FILTER_FIELD", "LIMITED_PERMISSION", "SALESFORCE", "BIGQUERY", "SNOWFLAKE", "REDSHIFT", "POSTGRES", "QUERY_EXPORT", "JSON", "CSV", "PARQUET", "SPREADSHEET", "GENERIC", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_transformation.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_transformation.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
             'QUERY': "QUERY",
             'DESTINATION_OBJECT': "DESTINATION_OBJECT",
             'DESTINATION_OBJECT_MAPPING': "DESTINATION_OBJECT_MAPPING",
             'SYNC': "SYNC",
             'MODEL_FIELD': "MODEL_FIELD",
             'SALESFORCE_OBJECT': "SALESFORCE_OBJECT",
             'SALESFORCE_OBJECT_FIELD': "SALESFORCE_OBJECT_FIELD",
+            'PIPELINE': "PIPELINE",
             'NONE': "NONE",
             'DBT_FOLDER': "DBT_FOLDER",
             'DBT_MODEL': "DBT_MODEL",
             'DBT_PROJECT': "DBT_PROJECT",
             'DBT_RUN': "DBT_RUN",
         },
     }
@@ -151,18 +152,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """DataEntityType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "PIPELINE", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "PIPELINE", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -241,18 +242,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """DataEntityType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "PIPELINE", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["SOURCE", "DESTINATION", "TOP_LEVEL_PLATFORM_ENTITY", "DATABASE", "SCHEMA", "TABLE", "COLUMN", "FILESET", "FOLDER", "DASHBOARD", "DASHBOARD_ELEMENT", "DASHBOARD_ELEMENT_FIELD", "MODEL", "EXPLORE", "EXPLORE_FIELD", "LOOK", "LOOK_FIELD", "JOB", "QUERY_RESULT", "QUERY_RESULT_COLUMN", "SITE", "PROJECT", "WORKBOOK", "SHEET", "FIELD", "CUSTOM_SQL_QUERY", "REPORT", "SPACE", "CHART", "REPORT_CHART_FIELD", "WORKSPACE", "DATASET", "TILE", "REPORT_PAGE", "MEASURE", "DAG", "TASK", "TOPIC", "FILE", "GENERIC", "QUERY", "DESTINATION_OBJECT", "DESTINATION_OBJECT_MAPPING", "SYNC", "MODEL_FIELD", "SALESFORCE_OBJECT", "SALESFORCE_OBJECT_FIELD", "PIPELINE", "NONE", "DBT_FOLDER", "DBT_MODEL", "DBT_PROJECT", "DBT_RUN", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stat.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stat.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stat_raw.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stat_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 
 
 def lazy_import():
     from alvin_api_client.model.connection_direction import ConnectionDirection
     from alvin_api_client.model.connection_type import ConnectionType
     from alvin_api_client.model.connection_usage_classification import ConnectionUsageClassification
     from alvin_api_client.model.data_entity_usage_type import DataEntityUsageType
+    from alvin_api_client.model.data_platform_job_costs import DataPlatformJobCosts
     from alvin_api_client.model.data_platform_type import DataPlatformType
     globals()['ConnectionDirection'] = ConnectionDirection
     globals()['ConnectionType'] = ConnectionType
     globals()['ConnectionUsageClassification'] = ConnectionUsageClassification
     globals()['DataEntityUsageType'] = DataEntityUsageType
+    globals()['DataPlatformJobCosts'] = DataPlatformJobCosts
     globals()['DataPlatformType'] = DataPlatformType
 
 
 class DataEntityUsageStatRaw(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -112,14 +114,15 @@
             'job_step_status': (str,),  # noqa: E501
             'sync_id': (str,),  # noqa: E501
             'connection_type': (ConnectionType,),  # noqa: E501
             'connection_direction': (ConnectionDirection,),  # noqa: E501
             'connection_usage_classification': (ConnectionUsageClassification,),  # noqa: E501
             'start': (datetime,),  # noqa: E501
             'end': (datetime,),  # noqa: E501
+            'costs_data': (DataPlatformJobCosts,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -141,14 +144,15 @@
         'job_step_status': 'jobStepStatus',  # noqa: E501
         'sync_id': 'syncId',  # noqa: E501
         'connection_type': 'connectionType',  # noqa: E501
         'connection_direction': 'connectionDirection',  # noqa: E501
         'connection_usage_classification': 'connectionUsageClassification',  # noqa: E501
         'start': 'start',  # noqa: E501
         'end': 'end',  # noqa: E501
+        'costs_data': 'costsData',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -207,14 +211,15 @@
             job_step_status (str): [optional]  # noqa: E501
             sync_id (str): [optional]  # noqa: E501
             connection_type (ConnectionType): [optional]  # noqa: E501
             connection_direction (ConnectionDirection): [optional]  # noqa: E501
             connection_usage_classification (ConnectionUsageClassification): [optional]  # noqa: E501
             start (datetime): [optional]  # noqa: E501
             end (datetime): [optional]  # noqa: E501
+            costs_data (DataPlatformJobCosts): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -319,14 +324,15 @@
             job_step_status (str): [optional]  # noqa: E501
             sync_id (str): [optional]  # noqa: E501
             connection_type (ConnectionType): [optional]  # noqa: E501
             connection_direction (ConnectionDirection): [optional]  # noqa: E501
             connection_usage_classification (ConnectionUsageClassification): [optional]  # noqa: E501
             start (datetime): [optional]  # noqa: E501
             end (datetime): [optional]  # noqa: E501
+            costs_data (DataPlatformJobCosts): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stats_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stats_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_stats_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_stats_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_entity_usage_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_entity_usage_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_manual_entity_sub_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_manual_entity_sub_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_aggregated_job_stat.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_aggregated_job_stat.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_airflow_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_airflow_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_big_query_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_big_query_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_created_in.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_created_in.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_databricks_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_databricks_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_dbt_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_dbt_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_delete.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_delete.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_full.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     from alvin_api_client.model.data_platform_status import DataPlatformStatus
     from alvin_api_client.model.data_platform_type import DataPlatformType
     globals()['DataPlatformCreatedIn'] = DataPlatformCreatedIn
     globals()['DataPlatformStatus'] = DataPlatformStatus
     globals()['DataPlatformType'] = DataPlatformType
 
 
-class DataPlatformFull(ModelNormal):
+class DataPlatformGet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,19 +93,14 @@
         return {
             'id': (str,),  # noqa: E501
             'org_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'platform_type': (DataPlatformType,),  # noqa: E501
             'status': (DataPlatformStatus,),  # noqa: E501
-            'has_jobs': (bool,),  # noqa: E501
-            'sync_jobs': (bool,),  # noqa: E501
-            'has_metadata': (bool,),  # noqa: E501
-            'sync_metadata': (bool,),  # noqa: E501
-            'connection_data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'status_message': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'created': (datetime,),  # noqa: E501
             'last_updated': (datetime,),  # noqa: E501
             'is_syncing_jobs': (bool,),  # noqa: E501
             'is_syncing_metadata': (bool,),  # noqa: E501
             'is_syncing': (bool,),  # noqa: E501
@@ -113,33 +108,29 @@
             'job_sync_heartbeat': (datetime,),  # noqa: E501
             'sync_heartbeat': (datetime,),  # noqa: E501
             'last_metadata_sync_time': (datetime,),  # noqa: E501
             'last_job_sync_time': (datetime,),  # noqa: E501
             'last_sync_time': (datetime,),  # noqa: E501
             'additional_config': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'created_in': (DataPlatformCreatedIn,),  # noqa: E501
+            'first_sync_start_time': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'org_id': 'orgId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'platform_type': 'platformType',  # noqa: E501
         'status': 'status',  # noqa: E501
-        'has_jobs': 'hasJobs',  # noqa: E501
-        'sync_jobs': 'syncJobs',  # noqa: E501
-        'has_metadata': 'hasMetadata',  # noqa: E501
-        'sync_metadata': 'syncMetadata',  # noqa: E501
-        'connection_data': 'connectionData',  # noqa: E501
         'status_message': 'statusMessage',  # noqa: E501
         'description': 'description',  # noqa: E501
         'created': 'created',  # noqa: E501
         'last_updated': 'lastUpdated',  # noqa: E501
         'is_syncing_jobs': 'isSyncingJobs',  # noqa: E501
         'is_syncing_metadata': 'isSyncingMetadata',  # noqa: E501
         'is_syncing': 'isSyncing',  # noqa: E501
@@ -147,38 +138,34 @@
         'job_sync_heartbeat': 'jobSyncHeartbeat',  # noqa: E501
         'sync_heartbeat': 'syncHeartbeat',  # noqa: E501
         'last_metadata_sync_time': 'lastMetadataSyncTime',  # noqa: E501
         'last_job_sync_time': 'lastJobSyncTime',  # noqa: E501
         'last_sync_time': 'lastSyncTime',  # noqa: E501
         'additional_config': 'additionalConfig',  # noqa: E501
         'created_in': 'createdIn',  # noqa: E501
+        'first_sync_start_time': 'firstSyncStartTime',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, org_id, name, display_name, platform_type, status, has_jobs, sync_jobs, has_metadata, sync_metadata, connection_data, *args, **kwargs):  # noqa: E501
-        """DataPlatformFull - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, org_id, name, display_name, platform_type, status, *args, **kwargs):  # noqa: E501
+        """DataPlatformGet - a model defined in OpenAPI
 
         Args:
             id (str):
             org_id (str):
             name (str):
             display_name (str):
             platform_type (DataPlatformType):
             status (DataPlatformStatus):
-            has_jobs (bool):
-            sync_jobs (bool):
-            has_metadata (bool):
-            sync_metadata (bool):
-            connection_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,14 +205,15 @@
             job_sync_heartbeat (datetime): [optional]  # noqa: E501
             sync_heartbeat (datetime): [optional]  # noqa: E501
             last_metadata_sync_time (datetime): [optional]  # noqa: E501
             last_job_sync_time (datetime): [optional]  # noqa: E501
             last_sync_time (datetime): [optional]  # noqa: E501
             additional_config ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             created_in (DataPlatformCreatedIn): [optional]  # noqa: E501
+            first_sync_start_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,19 +239,14 @@
 
         self.id = id
         self.org_id = org_id
         self.name = name
         self.display_name = display_name
         self.platform_type = platform_type
         self.status = status
-        self.has_jobs = has_jobs
-        self.sync_jobs = sync_jobs
-        self.has_metadata = has_metadata
-        self.sync_metadata = sync_metadata
-        self.connection_data = connection_data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -276,29 +259,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, org_id, name, display_name, platform_type, status, has_jobs, sync_jobs, has_metadata, sync_metadata, connection_data, *args, **kwargs):  # noqa: E501
-        """DataPlatformFull - a model defined in OpenAPI
+    def __init__(self, id, org_id, name, display_name, platform_type, status, *args, **kwargs):  # noqa: E501
+        """DataPlatformGet - a model defined in OpenAPI
 
         Args:
             id (str):
             org_id (str):
             name (str):
             display_name (str):
             platform_type (DataPlatformType):
             status (DataPlatformStatus):
-            has_jobs (bool):
-            sync_jobs (bool):
-            has_metadata (bool):
-            sync_metadata (bool):
-            connection_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -338,14 +316,15 @@
             job_sync_heartbeat (datetime): [optional]  # noqa: E501
             sync_heartbeat (datetime): [optional]  # noqa: E501
             last_metadata_sync_time (datetime): [optional]  # noqa: E501
             last_job_sync_time (datetime): [optional]  # noqa: E501
             last_sync_time (datetime): [optional]  # noqa: E501
             additional_config ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             created_in (DataPlatformCreatedIn): [optional]  # noqa: E501
+            first_sync_start_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -369,19 +348,14 @@
 
         self.id = id
         self.org_id = org_id
         self.name = name
         self.display_name = display_name
         self.platform_type = platform_type
         self.status = status
-        self.has_jobs = has_jobs
-        self.sync_jobs = sync_jobs
-        self.has_metadata = has_metadata
-        self.sync_metadata = sync_metadata
-        self.connection_data = connection_data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_full.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     from alvin_api_client.model.data_platform_status import DataPlatformStatus
     from alvin_api_client.model.data_platform_type import DataPlatformType
     globals()['DataPlatformCreatedIn'] = DataPlatformCreatedIn
     globals()['DataPlatformStatus'] = DataPlatformStatus
     globals()['DataPlatformType'] = DataPlatformType
 
 
-class DataPlatformGet(ModelNormal):
+class DataPlatformFull(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,14 +93,19 @@
         return {
             'id': (str,),  # noqa: E501
             'org_id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'platform_type': (DataPlatformType,),  # noqa: E501
             'status': (DataPlatformStatus,),  # noqa: E501
+            'has_jobs': (bool,),  # noqa: E501
+            'sync_jobs': (bool,),  # noqa: E501
+            'has_metadata': (bool,),  # noqa: E501
+            'sync_metadata': (bool,),  # noqa: E501
+            'connection_data': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'status_message': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'created': (datetime,),  # noqa: E501
             'last_updated': (datetime,),  # noqa: E501
             'is_syncing_jobs': (bool,),  # noqa: E501
             'is_syncing_metadata': (bool,),  # noqa: E501
             'is_syncing': (bool,),  # noqa: E501
@@ -108,28 +113,34 @@
             'job_sync_heartbeat': (datetime,),  # noqa: E501
             'sync_heartbeat': (datetime,),  # noqa: E501
             'last_metadata_sync_time': (datetime,),  # noqa: E501
             'last_job_sync_time': (datetime,),  # noqa: E501
             'last_sync_time': (datetime,),  # noqa: E501
             'additional_config': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'created_in': (DataPlatformCreatedIn,),  # noqa: E501
+            'first_sync_start_time': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'org_id': 'orgId',  # noqa: E501
         'name': 'name',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'platform_type': 'platformType',  # noqa: E501
         'status': 'status',  # noqa: E501
+        'has_jobs': 'hasJobs',  # noqa: E501
+        'sync_jobs': 'syncJobs',  # noqa: E501
+        'has_metadata': 'hasMetadata',  # noqa: E501
+        'sync_metadata': 'syncMetadata',  # noqa: E501
+        'connection_data': 'connectionData',  # noqa: E501
         'status_message': 'statusMessage',  # noqa: E501
         'description': 'description',  # noqa: E501
         'created': 'created',  # noqa: E501
         'last_updated': 'lastUpdated',  # noqa: E501
         'is_syncing_jobs': 'isSyncingJobs',  # noqa: E501
         'is_syncing_metadata': 'isSyncingMetadata',  # noqa: E501
         'is_syncing': 'isSyncing',  # noqa: E501
@@ -137,33 +148,39 @@
         'job_sync_heartbeat': 'jobSyncHeartbeat',  # noqa: E501
         'sync_heartbeat': 'syncHeartbeat',  # noqa: E501
         'last_metadata_sync_time': 'lastMetadataSyncTime',  # noqa: E501
         'last_job_sync_time': 'lastJobSyncTime',  # noqa: E501
         'last_sync_time': 'lastSyncTime',  # noqa: E501
         'additional_config': 'additionalConfig',  # noqa: E501
         'created_in': 'createdIn',  # noqa: E501
+        'first_sync_start_time': 'firstSyncStartTime',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, org_id, name, display_name, platform_type, status, *args, **kwargs):  # noqa: E501
-        """DataPlatformGet - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, org_id, name, display_name, platform_type, status, has_jobs, sync_jobs, has_metadata, sync_metadata, connection_data, *args, **kwargs):  # noqa: E501
+        """DataPlatformFull - a model defined in OpenAPI
 
         Args:
             id (str):
             org_id (str):
             name (str):
             display_name (str):
             platform_type (DataPlatformType):
             status (DataPlatformStatus):
+            has_jobs (bool):
+            sync_jobs (bool):
+            has_metadata (bool):
+            sync_metadata (bool):
+            connection_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -203,14 +220,15 @@
             job_sync_heartbeat (datetime): [optional]  # noqa: E501
             sync_heartbeat (datetime): [optional]  # noqa: E501
             last_metadata_sync_time (datetime): [optional]  # noqa: E501
             last_job_sync_time (datetime): [optional]  # noqa: E501
             last_sync_time (datetime): [optional]  # noqa: E501
             additional_config ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             created_in (DataPlatformCreatedIn): [optional]  # noqa: E501
+            first_sync_start_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -236,14 +254,19 @@
 
         self.id = id
         self.org_id = org_id
         self.name = name
         self.display_name = display_name
         self.platform_type = platform_type
         self.status = status
+        self.has_jobs = has_jobs
+        self.sync_jobs = sync_jobs
+        self.has_metadata = has_metadata
+        self.sync_metadata = sync_metadata
+        self.connection_data = connection_data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -256,24 +279,29 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, org_id, name, display_name, platform_type, status, *args, **kwargs):  # noqa: E501
-        """DataPlatformGet - a model defined in OpenAPI
+    def __init__(self, id, org_id, name, display_name, platform_type, status, has_jobs, sync_jobs, has_metadata, sync_metadata, connection_data, *args, **kwargs):  # noqa: E501
+        """DataPlatformFull - a model defined in OpenAPI
 
         Args:
             id (str):
             org_id (str):
             name (str):
             display_name (str):
             platform_type (DataPlatformType):
             status (DataPlatformStatus):
+            has_jobs (bool):
+            sync_jobs (bool):
+            has_metadata (bool):
+            sync_metadata (bool):
+            connection_data ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -313,14 +341,15 @@
             job_sync_heartbeat (datetime): [optional]  # noqa: E501
             sync_heartbeat (datetime): [optional]  # noqa: E501
             last_metadata_sync_time (datetime): [optional]  # noqa: E501
             last_job_sync_time (datetime): [optional]  # noqa: E501
             last_sync_time (datetime): [optional]  # noqa: E501
             additional_config ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             created_in (DataPlatformCreatedIn): [optional]  # noqa: E501
+            first_sync_start_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -344,14 +373,19 @@
 
         self.id = id
         self.org_id = org_id
         self.name = name
         self.display_name = display_name
         self.platform_type = platform_type
         self.status = status
+        self.has_jobs = has_jobs
+        self.sync_jobs = sync_jobs
+        self.has_metadata = has_metadata
+        self.sync_metadata = sync_metadata
+        self.connection_data = connection_data
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_hightouch_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_hightouch_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_hive_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_hive_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_hive_glue_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_hive_glue_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_entity_aggregated_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_entity_aggregated_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_execution_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_execution_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_stat.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_stat.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_aggregated_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_aggregated_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_execution_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_execution_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_id.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_id.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_report_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_report_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_sub_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_sub_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_step_user.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_step_user.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_job_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_job_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_looker_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_looker_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_azure_blob_storage_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_azure_blob_storage_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_file_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_file_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_gcs_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_gcs_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_generic_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_generic_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_google_drive_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_google_drive_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_kafka_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_kafka_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_manual_s3_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_manual_s3_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_mode_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_mode_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_mssql_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_mssql_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_my_sql_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_my_sql_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_postgres_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_postgres_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_power_bi_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_power_bi_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_redshift_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_redshift_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_snowflake_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_snowflake_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_tableau_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_tableau_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_treasure_data_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_treasure_data_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_platform_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_platform_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_bulk_apply.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_bulk_apply.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_bulk_delete.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_classification_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_classification_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_connection_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_connection_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_created_in.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_created_in.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_request_delete.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_request_delete.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_request_v2.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_request_v2.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_entity_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_entity_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_propagation.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_propagation.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rule_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rule_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_rules_request_delete.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_rules_request_delete.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_search_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_search_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_tag_v2.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_tag_v2.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_taxonomy_classification.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_taxonomy_classification.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/data_transformation_lineage.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/data_transformation_lineage.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/databricks_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/databricks_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/databricks_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/databricks_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/datadog_settings.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/datadog_settings.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/dbt_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/dbt_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/delete_parse_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/delete_parse_result.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/drop_parse_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/drop_parse_result.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/drop_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/drop_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/element_position.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/element_position.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/email_login_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/email_login_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_graph_connector_edge.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_graph_connector_edge.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_graph_node.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_graph_node.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_graph_node_connector.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/entity_graph_node_connector.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/entity_usage_context.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from alvin_api_client.model.popularity_values import PopularityValues
-    from alvin_api_client.model.user_name_usage_context import UserNameUsageContext
-    globals()['PopularityValues'] = PopularityValues
-    globals()['UserNameUsageContext'] = UserNameUsageContext
 
-
-class EntityUsageContext(ModelNormal):
+class UserCreate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -68,58 +62,66 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'user_names': ([UserNameUsageContext],),  # noqa: E501
-            'user_popularity_values': (PopularityValues,),  # noqa: E501
-            'popularity_values': (PopularityValues,),  # noqa: E501
-            'last_seen': (datetime,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'sha_id': (str,),  # noqa: E501
+            'created_time': (datetime,),  # noqa: E501
+            'first_name': (str,),  # noqa: E501
+            'last_name': (str,),  # noqa: E501
+            'avatar_url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'user_names': 'userNames',  # noqa: E501
-        'user_popularity_values': 'userPopularityValues',  # noqa: E501
-        'popularity_values': 'popularityValues',  # noqa: E501
-        'last_seen': 'lastSeen',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'sha_id': 'shaId',  # noqa: E501
+        'created_time': 'createdTime',  # noqa: E501
+        'first_name': 'firstName',  # noqa: E501
+        'last_name': 'lastName',  # noqa: E501
+        'avatar_url': 'avatarUrl',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """EntityUsageContext - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, email, *args, **kwargs):  # noqa: E501
+        """UserCreate - a model defined in OpenAPI
+
+        Args:
+            id (str):
+            email (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,18 +146,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_names ([UserNameUsageContext]): [optional]  # noqa: E501
-            user_popularity_values (PopularityValues): [optional]  # noqa: E501
-            popularity_values (PopularityValues): [optional]  # noqa: E501
-            last_seen (datetime): [optional]  # noqa: E501
+            sha_id (str): [optional]  # noqa: E501
+            created_time (datetime): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            avatar_url (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -175,14 +178,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -195,16 +200,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """EntityUsageContext - a model defined in OpenAPI
+    def __init__(self, id, email, *args, **kwargs):  # noqa: E501
+        """UserCreate - a model defined in OpenAPI
+
+        Args:
+            id (str):
+            email (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,18 +238,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            user_names ([UserNameUsageContext]): [optional]  # noqa: E501
-            user_popularity_values (PopularityValues): [optional]  # noqa: E501
-            popularity_values (PopularityValues): [optional]  # noqa: E501
-            last_seen (datetime): [optional]  # noqa: E501
+            sha_id (str): [optional]  # noqa: E501
+            created_time (datetime): [optional]  # noqa: E501
+            first_name (str): [optional]  # noqa: E501
+            last_name (str): [optional]  # noqa: E501
+            avatar_url (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,14 +268,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/environment_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/environment_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/event_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/exchange_token_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/exchange_token_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience_data.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experience_user.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experience_user.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/experiences_settings.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/experiences_settings.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/extracted_simple_column.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/extracted_simple_column.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/extracted_simple_table.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/extracted_simple_table.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_data_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_data_payload.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_match.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_match.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_options.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_options.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insight_usage_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 
-class FilterType(ModelSimple):
+class InsightUsageGroup(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -48,20 +48,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'TEXT_INPUT': "TEXT_INPUT",
-            'NUM_RANGE': "NUM_RANGE",
-            'DROPDOWN': "DROPDOWN",
-            'TAG': "TAG",
-            'BOOL': "BOOL",
-            'ENTITY_TYPE': "ENTITY_TYPE",
+            'USER': "USER",
+            'TABLE': "TABLE",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -100,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """FilterType - a model defined in OpenAPI
+        """InsightUsageGroup - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["TEXT_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["USER", "TABLE", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["TEXT_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["USER", "TABLE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -190,23 +186,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """FilterType - a model defined in OpenAPI
+        """InsightUsageGroup - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["TEXT_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["USER", "TABLE", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["TEXT_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["USER", "TABLE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filter_view.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_view.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/filters_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filters_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/firebase_auth_provider.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/firebase_auth_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             'GOOGLE.COM': "google.com",
             'FACEBOOK.COM': "facebook.com",
             'TWITTER.COM': "twitter.com",
             'GITHUB.COM': "github.com",
             'APPLE.COM': "apple.com",
             'YAHOO.COM': "yahoo.com",
             'MICROSOFT.COM': "microsoft.com",
+            'SSO': "sso",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -108,18 +109,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """FirebaseAuthProvider - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", "sso", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", "sso", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -198,18 +199,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """FirebaseAuthProvider - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", "sso", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["password", "phone", "google.com", "facebook.com", "twitter.com", "github.com", "apple.com", "yahoo.com", "microsoft.com", "sso", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/firebase_auth_ui_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/firebase_auth_ui_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/group_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/group_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/healthcheck_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/healthcheck_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hightouch_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hightouch_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hightouch_credentials.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hightouch_credentials.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_glue_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_glue_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/hive_glue_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/hive_glue_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/html_values.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/html_values.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/http_validation_error.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_entity_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_entity_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from alvin_api_client.model.data_entity_get import DataEntityGet
     from alvin_api_client.model.data_entity_id import DataEntityID
+    from alvin_api_client.model.entity_usage_context import EntityUsageContext
     globals()['DataEntityGet'] = DataEntityGet
     globals()['DataEntityID'] = DataEntityID
+    globals()['EntityUsageContext'] = EntityUsageContext
 
 
 class IAEntityData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -94,14 +96,15 @@
             'org_id': (str,),  # noqa: E501
             'comparison_key': (str,),  # noqa: E501
             'depth': (int,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'entity_id': (DataEntityID,),  # noqa: E501
             'impact_status': ({str: (int,)},),  # noqa: E501
             'impacted_users': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
+            'entity_usage_context': (EntityUsageContext,),  # noqa: E501
             'usage_stats': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'user_usage_stats': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'last_used': (datetime,),  # noqa: E501
             'source_entities': ([str],),  # noqa: E501
             'row_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'entity_detail': (DataEntityGet,),  # noqa: E501
             'parent_entity': (DataEntityID,),  # noqa: E501
@@ -117,14 +120,15 @@
         'org_id': 'orgId',  # noqa: E501
         'comparison_key': 'comparisonKey',  # noqa: E501
         'depth': 'depth',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'entity_id': 'entityId',  # noqa: E501
         'impact_status': 'impactStatus',  # noqa: E501
         'impacted_users': 'impactedUsers',  # noqa: E501
+        'entity_usage_context': 'entityUsageContext',  # noqa: E501
         'usage_stats': 'usageStats',  # noqa: E501
         'user_usage_stats': 'userUsageStats',  # noqa: E501
         'last_used': 'lastUsed',  # noqa: E501
         'source_entities': 'sourceEntities',  # noqa: E501
         'row_type': 'rowType',  # noqa: E501
         'entity_detail': 'entityDetail',  # noqa: E501
         'parent_entity': 'parentEntity',  # noqa: E501
@@ -177,14 +181,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             impact_status ({str: (int,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
             impacted_users ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
             usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             user_usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             last_used (datetime): [optional]  # noqa: E501
             source_entities ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
             row_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             entity_detail (DataEntityGet): [optional]  # noqa: E501
             parent_entity (DataEntityID): [optional]  # noqa: E501
@@ -280,14 +285,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             impact_status ({str: (int,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
             impacted_users ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
             usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             user_usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             last_used (datetime): [optional]  # noqa: E501
             source_entities ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
             row_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             entity_detail (DataEntityGet): [optional]  # noqa: E501
             parent_entity (DataEntityID): [optional]  # noqa: E501
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_job_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_job_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from alvin_api_client.model.data_entity_job_step import DataEntityJobStep
+    from alvin_api_client.model.entity_usage_context import EntityUsageContext
     from alvin_api_client.model.job_entity_usage_stats_report import JobEntityUsageStatsReport
     globals()['DataEntityJobStep'] = DataEntityJobStep
+    globals()['EntityUsageContext'] = EntityUsageContext
     globals()['JobEntityUsageStatsReport'] = JobEntityUsageStatsReport
 
 
 class IAJobData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -94,14 +96,15 @@
             'org_id': (str,),  # noqa: E501
             'comparison_key': (str,),  # noqa: E501
             'depth': (int,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'job_data': (DataEntityJobStep,),  # noqa: E501
             'impact_status': ({str: (int,)},),  # noqa: E501
             'impacted_users': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
+            'entity_usage_context': (EntityUsageContext,),  # noqa: E501
             'usage_stats': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'user_usage_stats': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'last_used': (datetime,),  # noqa: E501
             'source_entities': ([str],),  # noqa: E501
             'row_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'job_stats': (JobEntityUsageStatsReport,),  # noqa: E501
         }
@@ -115,14 +118,15 @@
         'org_id': 'orgId',  # noqa: E501
         'comparison_key': 'comparisonKey',  # noqa: E501
         'depth': 'depth',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'job_data': 'jobData',  # noqa: E501
         'impact_status': 'impactStatus',  # noqa: E501
         'impacted_users': 'impactedUsers',  # noqa: E501
+        'entity_usage_context': 'entityUsageContext',  # noqa: E501
         'usage_stats': 'usageStats',  # noqa: E501
         'user_usage_stats': 'userUsageStats',  # noqa: E501
         'last_used': 'lastUsed',  # noqa: E501
         'source_entities': 'sourceEntities',  # noqa: E501
         'row_type': 'rowType',  # noqa: E501
         'job_stats': 'jobStats',  # noqa: E501
     }
@@ -173,14 +177,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             impact_status ({str: (int,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
             impacted_users ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
             usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             user_usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             last_used (datetime): [optional]  # noqa: E501
             source_entities ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
             row_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             job_stats (JobEntityUsageStatsReport): [optional]  # noqa: E501
         """
@@ -274,14 +279,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             impact_status ({str: (int,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
             impacted_users ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
             usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             user_usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             last_used (datetime): [optional]  # noqa: E501
             source_entities ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
             row_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             job_stats (JobEntityUsageStatsReport): [optional]  # noqa: E501
         """
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_platform_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_platform_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from alvin_api_client.model.data_platform_type import DataPlatformType
+    from alvin_api_client.model.entity_usage_context import EntityUsageContext
     globals()['DataPlatformType'] = DataPlatformType
+    globals()['EntityUsageContext'] = EntityUsageContext
 
 
 class IAPlatformData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -92,14 +94,15 @@
             'org_id': (str,),  # noqa: E501
             'comparison_key': (str,),  # noqa: E501
             'depth': (int,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'platform_id': (str,),  # noqa: E501
             'impact_status': ({str: (int,)},),  # noqa: E501
             'impacted_users': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
+            'entity_usage_context': (EntityUsageContext,),  # noqa: E501
             'usage_stats': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'user_usage_stats': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'last_used': (datetime,),  # noqa: E501
             'source_entities': ([str],),  # noqa: E501
             'row_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'platform_type': (DataPlatformType,),  # noqa: E501
         }
@@ -113,14 +116,15 @@
         'org_id': 'orgId',  # noqa: E501
         'comparison_key': 'comparisonKey',  # noqa: E501
         'depth': 'depth',  # noqa: E501
         'display_name': 'displayName',  # noqa: E501
         'platform_id': 'platformId',  # noqa: E501
         'impact_status': 'impactStatus',  # noqa: E501
         'impacted_users': 'impactedUsers',  # noqa: E501
+        'entity_usage_context': 'entityUsageContext',  # noqa: E501
         'usage_stats': 'usageStats',  # noqa: E501
         'user_usage_stats': 'userUsageStats',  # noqa: E501
         'last_used': 'lastUsed',  # noqa: E501
         'source_entities': 'sourceEntities',  # noqa: E501
         'row_type': 'rowType',  # noqa: E501
         'platform_type': 'platformType',  # noqa: E501
     }
@@ -171,14 +175,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             impact_status ({str: (int,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
             impacted_users ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
             usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             user_usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             last_used (datetime): [optional]  # noqa: E501
             source_entities ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
             row_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             platform_type (DataPlatformType): [optional]  # noqa: E501
         """
@@ -272,14 +277,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             impact_status ({str: (int,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
             impacted_users ([bool, date, datetime, dict, float, int, list, str, none_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            entity_usage_context (EntityUsageContext): [optional]  # noqa: E501
             usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             user_usage_stats (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             last_used (datetime): [optional]  # noqa: E501
             source_entities ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
             row_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             platform_type (DataPlatformType): [optional]  # noqa: E501
         """
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_row.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_row.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,28 +89,30 @@
         return {
             'data': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'platform_id': (str,),  # noqa: E501
             'entity_type': (DataEntityType,),  # noqa: E501
             'entity_key': (str,),  # noqa: E501
             'parent_key': (str,),  # noqa: E501
             'children': ({str: (IARow,)},),  # noqa: E501
+            'min_depth': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'data': 'data',  # noqa: E501
         'platform_id': 'platformId',  # noqa: E501
         'entity_type': 'entityType',  # noqa: E501
         'entity_key': 'entityKey',  # noqa: E501
         'parent_key': 'parentKey',  # noqa: E501
         'children': 'children',  # noqa: E501
+        'min_depth': 'minDepth',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -154,14 +156,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             parent_key (str): [optional]  # noqa: E501
             children ({str: (IARow,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            min_depth (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +250,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             parent_key (str): [optional]  # noqa: E501
             children ({str: (IARow,)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            min_depth (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/ia_row_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/ia_row_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_node_list_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_node_list_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alvin_api_client.model.app_schemas_impact_analysis_response_impact_analysis_response import AppSchemasImpactAnalysisResponseImpactAnalysisResponse
     from alvin_api_client.model.ia_row import IARow
     from alvin_api_client.model.impact_analysis_node_stats import ImpactAnalysisNodeStats
-    globals()['AppSchemasImpactAnalysisResponseImpactAnalysisResponse'] = AppSchemasImpactAnalysisResponseImpactAnalysisResponse
+    from alvin_api_client.model.impact_analysis_response import ImpactAnalysisResponse
     globals()['IARow'] = IARow
     globals()['ImpactAnalysisNodeStats'] = ImpactAnalysisNodeStats
+    globals()['ImpactAnalysisResponse'] = ImpactAnalysisResponse
 
 
 class ImpactAnalysisNodeListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -87,15 +87,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'impact_analysis_response': (AppSchemasImpactAnalysisResponseImpactAnalysisResponse,),  # noqa: E501
+            'impact_analysis_response': (ImpactAnalysisResponse,),  # noqa: E501
             'node_list': ([IARow],),  # noqa: E501
             'node_stats': (ImpactAnalysisNodeStats,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -114,15 +114,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, impact_analysis_response, node_list, *args, **kwargs):  # noqa: E501
         """ImpactAnalysisNodeListResponse - a model defined in OpenAPI
 
         Args:
-            impact_analysis_response (AppSchemasImpactAnalysisResponseImpactAnalysisResponse):
+            impact_analysis_response (ImpactAnalysisResponse):
             node_list ([IARow]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -202,15 +202,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, impact_analysis_response, node_list, *args, **kwargs):  # noqa: E501
         """ImpactAnalysisNodeListResponse - a model defined in OpenAPI
 
         Args:
-            impact_analysis_response (AppSchemasImpactAnalysisResponseImpactAnalysisResponse):
+            impact_analysis_response (ImpactAnalysisResponse):
             node_list ([IARow]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_node_stats.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_node_stats.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_platform_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_platform_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_query_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_query_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_query_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_query_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_query_validation.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_query_validation.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_response_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_response_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_sidebar_data_node.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_sidebar_data_node.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_entity_row.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_entity_row.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_job_row.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_job_row.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_v2_response_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_v2_response_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_analysis_validation_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_analysis_validation_payload.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/impact_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/impact_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_entity_id.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_entity_id.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_entity_usage_stats_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_entity_usage_stats_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_integration_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_integration_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_query_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_query_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_query_v1_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_query_v1_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/job_steps_agg_response_model.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/job_steps_agg_response_model.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/kirby_failed_batches_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/kirby_failed_batches_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/kirby_ingest_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/kirby_ingest_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/known_column.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/known_column.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/known_table.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/known_table.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/known_table_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/known_table_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_api_keys_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_numerical_stat.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_numerical_stat.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_run_facet_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_run_facet_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_run_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_run_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_run_job_mapping_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_run_job_mapping_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stat_raw.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stat_raw.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stats_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_entity_usage_stats_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_platform_job.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_platform_job.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_platform_job_entity_aggregated_report.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_platform_job_entity_aggregated_report.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_tag_connection_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_tag_connection_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_tag_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_tag_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_data_tag_rule_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_data_tag_rule_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_manual_lineage_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_manual_lineage_data.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/limit_offset_page_tag_entity_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/limit_offset_page_tag_entity_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/lineage_connection_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_connection_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/lineage_expanding_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_expanding_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/lineage_scope.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/lineage_scope.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/links_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/links_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/looker_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/looker_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/looker_credentials.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/looker_credentials.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/looker_query_comment.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/looker_query_comment.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/manual_lineage_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/manual_lineage_data.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/manual_lineage_data_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/manual_lineage_data_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/manual_lineage_entity_type_validation.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/manual_lineage_entity_type_validation.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/map_entity_to_url_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/map_entity_to_url_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mode_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mode_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mode_credentials.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mode_credentials.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mssql_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mssql_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/mssql_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/mssql_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/my_sql_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/my_sql_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/my_sql_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/my_sql_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification_provider.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification_provider.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/notification_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/notification_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/onboarding_level.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/onboarding_level.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/operator_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/operator_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/organization_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_stats_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from alvin_api_client.model.organization_status import OrganizationStatus
-    globals()['OrganizationStatus'] = OrganizationStatus
 
-
-class OrganizationGet(ModelNormal):
+class InsightsUsageStatsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,65 +62,62 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'id': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'display_name': (str,),  # noqa: E501
-            'plan': (str,),  # noqa: E501
-            'status': (OrganizationStatus,),  # noqa: E501
+            'usage_count': (int,),  # noqa: E501
+            'cost': (float,),  # noqa: E501
+            'avg_cost': (float,),  # noqa: E501
+            'user_count': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'display_name': 'displayName',  # noqa: E501
-        'plan': 'plan',  # noqa: E501
-        'status': 'status',  # noqa: E501
+        'usage_count': 'usageCount',  # noqa: E501
+        'cost': 'cost',  # noqa: E501
+        'avg_cost': 'avgCost',  # noqa: E501
+        'user_count': 'userCount',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, display_name, *args, **kwargs):  # noqa: E501
-        """OrganizationGet - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, usage_count, *args, **kwargs):  # noqa: E501
+        """InsightsUsageStatsResponse - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
-            display_name (str):
+            usage_count (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,16 +142,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            plan (str): [optional]  # noqa: E501
-            status (OrganizationStatus): [optional]  # noqa: E501
+            cost (float): [optional]  # noqa: E501
+            avg_cost (float): [optional]  # noqa: E501
+            user_count (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,17 +172,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
-        self.display_name = display_name
+        self.usage_count = usage_count
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -201,21 +194,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, display_name, *args, **kwargs):  # noqa: E501
-        """OrganizationGet - a model defined in OpenAPI
+    def __init__(self, name, usage_count, *args, **kwargs):  # noqa: E501
+        """InsightsUsageStatsResponse - a model defined in OpenAPI
 
         Args:
-            id (str):
             name (str):
-            display_name (str):
+            usage_count (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -240,16 +232,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            plan (str): [optional]  # noqa: E501
-            status (OrganizationStatus): [optional]  # noqa: E501
+            cost (float): [optional]  # noqa: E501
+            avg_cost (float): [optional]  # noqa: E501
+            user_count (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,17 +260,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         self.name = name
-        self.display_name = display_name
+        self.usage_count = usage_count
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/organization_status.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/organization_status.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/page_data_entity_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/page_data_entity_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/page_search_display_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/page_search_display_payload.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/page_view_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/page_view_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_asset_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_asset_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_build_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_build_data.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_build_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_build_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/platform_classification.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/platform_classification.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/popularity_values.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/popularity_values.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/position.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/position.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/postgres_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/postgres_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/postgres_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/postgres_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/power_bi_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/power_bi_additional_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,25 +80,27 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'ignore_private_workspaces': (bool,),  # noqa: E501
             'toggles': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'ignored_workspaces_names': ([str],),  # noqa: E501
+            'included_workspaces_names': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'ignore_private_workspaces': 'ignorePrivateWorkspaces',  # noqa: E501
         'toggles': 'toggles',  # noqa: E501
         'ignored_workspaces_names': 'ignoredWorkspacesNames',  # noqa: E501
+        'included_workspaces_names': 'includedWorkspacesNames',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -139,14 +141,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             toggles ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             ignored_workspaces_names ([str]): [optional]  # noqa: E501
+            included_workspaces_names ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -226,14 +229,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             toggles ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             ignored_workspaces_names ([str]): [optional]  # noqa: E501
+            included_workspaces_names ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/power_bi_credentials.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/power_bi_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,39 +79,42 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'client_id': (str,),  # noqa: E501
             'client_secret': (str,),  # noqa: E501
+            'tenant': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'client_id': 'clientId',  # noqa: E501
         'client_secret': 'clientSecret',  # noqa: E501
+        'tenant': 'tenant',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, client_id, client_secret, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, client_id, client_secret, tenant, *args, **kwargs):  # noqa: E501
         """PowerBICredentials - a model defined in OpenAPI
 
         Args:
             client_id (str):
             client_secret (str):
+            tenant (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,14 +168,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.client_id = client_id
         self.client_secret = client_secret
+        self.tenant = tenant
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,20 +189,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, client_id, client_secret, *args, **kwargs):  # noqa: E501
+    def __init__(self, client_id, client_secret, tenant, *args, **kwargs):  # noqa: E501
         """PowerBICredentials - a model defined in OpenAPI
 
         Args:
             client_id (str):
             client_secret (str):
+            tenant (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,14 +255,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.client_id = client_id
         self.client_secret = client_secret
+        self.tenant = tenant
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/predefined_filter.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/predefined_filter.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/processed_lineage_graph_data.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/processed_lineage_graph_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from alvin_api_client.model.app_schemas_core_data_entity_lineage_entity_graph_connector_edge import AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge
+    from alvin_api_client.model.app_schemas_core_data_entity_lineage_entity_graph_node import AppSchemasCoreDataEntityLineageEntityGraphNode
     from alvin_api_client.model.data_entity_type import DataEntityType
-    from alvin_api_client.model.entity_graph_connector_edge import EntityGraphConnectorEdge
-    from alvin_api_client.model.entity_graph_node import EntityGraphNode
+    globals()['AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge'] = AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge
+    globals()['AppSchemasCoreDataEntityLineageEntityGraphNode'] = AppSchemasCoreDataEntityLineageEntityGraphNode
     globals()['DataEntityType'] = DataEntityType
-    globals()['EntityGraphConnectorEdge'] = EntityGraphConnectorEdge
-    globals()['EntityGraphNode'] = EntityGraphNode
 
 
 class ProcessedLineageGraphData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -89,19 +89,19 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'grouping_entities': ([DataEntityType],),  # noqa: E501
             'has_groupings': (bool,),  # noqa: E501
-            'all_nodes': ([EntityGraphNode],),  # noqa: E501
-            'nodes_grouped': ([EntityGraphNode],),  # noqa: E501
-            'all_nodes_grouped': ([EntityGraphNode],),  # noqa: E501
-            'all_edges': ([EntityGraphConnectorEdge],),  # noqa: E501
-            'all_edges_grouped': ([EntityGraphConnectorEdge],),  # noqa: E501
+            'all_nodes': ([AppSchemasCoreDataEntityLineageEntityGraphNode],),  # noqa: E501
+            'nodes_grouped': ([AppSchemasCoreDataEntityLineageEntityGraphNode],),  # noqa: E501
+            'all_nodes_grouped': ([AppSchemasCoreDataEntityLineageEntityGraphNode],),  # noqa: E501
+            'all_edges': ([AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge],),  # noqa: E501
+            'all_edges_grouped': ([AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge],),  # noqa: E501
             'node_id_separator': (str,),  # noqa: E501
             'node_child_separator': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -128,19 +128,19 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, grouping_entities, has_groupings, all_nodes, nodes_grouped, all_nodes_grouped, all_edges, all_edges_grouped, *args, **kwargs):  # noqa: E501
         """ProcessedLineageGraphData - a model defined in OpenAPI
 
         Args:
             grouping_entities ([DataEntityType]):
             has_groupings (bool):
-            all_nodes ([EntityGraphNode]):
-            nodes_grouped ([EntityGraphNode]):
-            all_nodes_grouped ([EntityGraphNode]):
-            all_edges ([EntityGraphConnectorEdge]):
-            all_edges_grouped ([EntityGraphConnectorEdge]):
+            all_nodes ([AppSchemasCoreDataEntityLineageEntityGraphNode]):
+            nodes_grouped ([AppSchemasCoreDataEntityLineageEntityGraphNode]):
+            all_nodes_grouped ([AppSchemasCoreDataEntityLineageEntityGraphNode]):
+            all_edges ([AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge]):
+            all_edges_grouped ([AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,19 +227,19 @@
     @convert_js_args_to_python_args
     def __init__(self, grouping_entities, has_groupings, all_nodes, nodes_grouped, all_nodes_grouped, all_edges, all_edges_grouped, *args, **kwargs):  # noqa: E501
         """ProcessedLineageGraphData - a model defined in OpenAPI
 
         Args:
             grouping_entities ([DataEntityType]):
             has_groupings (bool):
-            all_nodes ([EntityGraphNode]):
-            nodes_grouped ([EntityGraphNode]):
-            all_nodes_grouped ([EntityGraphNode]):
-            all_edges ([EntityGraphConnectorEdge]):
-            all_edges_grouped ([EntityGraphConnectorEdge]):
+            all_nodes ([AppSchemasCoreDataEntityLineageEntityGraphNode]):
+            nodes_grouped ([AppSchemasCoreDataEntityLineageEntityGraphNode]):
+            all_nodes_grouped ([AppSchemasCoreDataEntityLineageEntityGraphNode]):
+            all_edges ([AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge]):
+            all_edges_grouped ([AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/product_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/product_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_builder.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_builder.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_comment.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_comment.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_create_mode.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_create_mode.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_fingerprint.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_fingerprint.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_lineage_parse_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_lineage_parse_result.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_parse_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_parse_result.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/query_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/query_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/redshift_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/redshift_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/redshift_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/redshift_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_element.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_element.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_element_value_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_element_value_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/rule_value.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/rule_value.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/save_search_filter.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/save_search_filter.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/save_search_string_filter.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/save_search_string_filter.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_csv_column.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/filter_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 
-class SearchCSVColumn(ModelSimple):
+class FilterType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -48,23 +48,21 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'PARENT': "Parent",
-            'PLATFORM_NAME': "Platform Name",
-            'PLATFORM_TYPE': "Platform Type",
-            'NAME': "Name",
-            'DESCRIPTION': "Description",
-            'TERMS': "Terms",
-            'TAGS': "Tags",
-            'DATA_TYPE': "Data Type",
-            'ASSET_TYPE': "Asset Type",
+            'TEXT_INPUT': "TEXT_INPUT",
+            'TERM_INPUT': "TERM_INPUT",
+            'NUM_RANGE': "NUM_RANGE",
+            'DROPDOWN': "DROPDOWN",
+            'TAG': "TAG",
+            'BOOL': "BOOL",
+            'ENTITY_TYPE': "ENTITY_TYPE",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -103,23 +101,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """SearchCSVColumn - a model defined in OpenAPI
+        """FilterType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["Parent", "Platform Name", "Platform Type", "Name", "Description", "Terms", "Tags", "Data Type", "Asset Type", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["TEXT_INPUT", "TERM_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["Parent", "Platform Name", "Platform Type", "Name", "Description", "Terms", "Tags", "Data Type", "Asset Type", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["TEXT_INPUT", "TERM_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -193,23 +191,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """SearchCSVColumn - a model defined in OpenAPI
+        """FilterType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["Parent", "Platform Name", "Platform Type", "Name", "Description", "Terms", "Tags", "Data Type", "Asset Type", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["TEXT_INPUT", "TERM_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["Parent", "Platform Name", "Platform Type", "Name", "Description", "Terms", "Tags", "Data Type", "Asset Type", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["TEXT_INPUT", "TERM_INPUT", "NUM_RANGE", "DROPDOWN", "TAG", "BOOL", "ENTITY_TYPE", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_display_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/insights_usage_metric_aggregation.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,21 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alvin_api_client.model.data_entity_get import DataEntityGet
-    from alvin_api_client.model.data_tag_search_response import DataTagSearchResponse
-    from alvin_api_client.model.html_values import HTMLValues
-    from alvin_api_client.model.popularity_values import PopularityValues
-    globals()['DataEntityGet'] = DataEntityGet
-    globals()['DataTagSearchResponse'] = DataTagSearchResponse
-    globals()['HTMLValues'] = HTMLValues
-    globals()['PopularityValues'] = PopularityValues
+    from alvin_api_client.model.event_metric_type import EventMetricType
+    from alvin_api_client.model.insights_usage_request_stat_group import InsightsUsageRequestStatGroup
+    globals()['EventMetricType'] = EventMetricType
+    globals()['InsightsUsageRequestStatGroup'] = InsightsUsageRequestStatGroup
 
 
-class SearchDisplayPayload(ModelNormal):
+class InsightsUsageMetricAggregation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -89,46 +85,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'entity': (DataEntityGet,),  # noqa: E501
-            'tags': ([DataTagSearchResponse],),  # noqa: E501
-            'html_values': (HTMLValues,),  # noqa: E501
-            'popularity_values': (PopularityValues,),  # noqa: E501
-            'user_popularity_values': (PopularityValues,),  # noqa: E501
+            'metric': ([InsightsUsageRequestStatGroup],),  # noqa: E501
+            'metric_function': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sorting': (EventMetricType,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'entity': 'entity',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
-        'html_values': 'htmlValues',  # noqa: E501
-        'popularity_values': 'popularityValues',  # noqa: E501
-        'user_popularity_values': 'userPopularityValues',  # noqa: E501
+        'metric': 'metric',  # noqa: E501
+        'metric_function': 'metricFunction',  # noqa: E501
+        'sorting': 'sorting',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, entity, *args, **kwargs):  # noqa: E501
-        """SearchDisplayPayload - a model defined in OpenAPI
+    def _from_openapi_data(cls, metric, metric_function, *args, **kwargs):  # noqa: E501
+        """InsightsUsageMetricAggregation - a model defined in OpenAPI
 
         Args:
-            entity (DataEntityGet):
+            metric ([InsightsUsageRequestStatGroup]):
+            metric_function (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,18 +146,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tags ([DataTagSearchResponse]): [optional] if omitted the server will use the default value of []  # noqa: E501
-            html_values (HTMLValues): [optional]  # noqa: E501
-            popularity_values (PopularityValues): [optional]  # noqa: E501
-            user_popularity_values (PopularityValues): [optional]  # noqa: E501
+            sorting (EventMetricType): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +174,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.entity = entity
+        self.metric = metric
+        self.metric_function = metric_function
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -205,19 +196,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, entity, *args, **kwargs):  # noqa: E501
-        """SearchDisplayPayload - a model defined in OpenAPI
+    def __init__(self, metric, metric_function, *args, **kwargs):  # noqa: E501
+        """InsightsUsageMetricAggregation - a model defined in OpenAPI
 
         Args:
-            entity (DataEntityGet):
+            metric ([InsightsUsageRequestStatGroup]):
+            metric_function (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -242,18 +234,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            tags ([DataTagSearchResponse]): [optional] if omitted the server will use the default value of []  # noqa: E501
-            html_values (HTMLValues): [optional]  # noqa: E501
-            popularity_values (PopularityValues): [optional]  # noqa: E501
-            user_popularity_values (PopularityValues): [optional]  # noqa: E501
+            sorting (EventMetricType): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -271,15 +260,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.entity = entity
+        self.metric = metric
+        self.metric_function = metric_function
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_filter.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_filter.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_filter_label_association.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_filter_label_association.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_node.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_node.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_prefix.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_prefix.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     """
 
     allowed_values = {
         ('value',): {
             'NAME': "name",
             'ENTITY': "entity",
             'ENTITY_ID': "entity_id",
+            'DATABASE_NAME': "database_name",
             'PLATFORM_ID': "platform_id",
             'PLATFORM_TYPE': "platform_type",
             'OWNERS': "owners",
             'USAGE': "usage",
             'MAX_USAGE': "max_usage",
             'MIN_USAGE': "min_usage",
             'TEXT': "text",
@@ -74,14 +75,24 @@
             'TAG_NAME': "tag_name",
             'TAG_TYPE': "tag_type",
             'TAG_DOMAIN': "tag_domain",
             'CLASSIFICATION_TYPE': "classification_type",
             'SORT': "sort",
             'SHOW_DELETED': "show_deleted",
             'CREATED_ON': "created_on",
+            'ASSET_USERS': "asset_users",
+            'EVENT_TYPE': "event_type",
+            'EVENT_GROUP': "event_group",
+            'EVENT_USERS': "event_users",
+            'JOB_ID': "job_id",
+            'IS_NATIVE_EVENT': "is_native_event",
+            'FETCH_UPSTREAM_EVENTS': "fetch_upstream_events",
+            'COSTS30D': "costs30d",
+            'UPSTREAM_COSTS30D': "upstream_costs30d",
+            'DOWNSTREAM_USAGE30D': "downstream_usage30d",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -125,18 +136,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """SearchPrefix - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["name", "entity", "entity_id", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["name", "entity", "entity_id", "database_name", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", "asset_users", "event_type", "event_group", "event_users", "job_id", "is_native_event", "fetch_upstream_events", "costs30d", "upstream_costs30d", "downstream_usage30d", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["name", "entity", "entity_id", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["name", "entity", "entity_id", "database_name", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", "asset_users", "event_type", "event_group", "event_users", "job_id", "is_native_event", "fetch_upstream_events", "costs30d", "upstream_costs30d", "downstream_usage30d", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -215,18 +226,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """SearchPrefix - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): An enumeration.., must be one of ["name", "entity", "entity_id", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", ]  # noqa: E501
+            args[0] (str): An enumeration.., must be one of ["name", "entity", "entity_id", "database_name", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", "asset_users", "event_type", "event_group", "event_users", "job_id", "is_native_event", "fetch_upstream_events", "costs30d", "upstream_costs30d", "downstream_usage30d", ]  # noqa: E501
 
         Keyword Args:
-            value (str): An enumeration.., must be one of ["name", "entity", "entity_id", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", ]  # noqa: E501
+            value (str): An enumeration.., must be one of ["name", "entity", "entity_id", "database_name", "platform_id", "platform_type", "owners", "usage", "max_usage", "min_usage", "text", "last_used", "last_used_before", "last_used_after", "last_used_between", "parent", "term", "tags", "tag_data_type", "tag_value", "tag_name", "tag_type", "tag_domain", "classification_type", "sort", "show_deleted", "created_on", "asset_users", "event_type", "event_group", "event_users", "job_id", "is_native_event", "fetch_upstream_events", "costs30d", "upstream_costs30d", "downstream_usage30d", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_usage_stat_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_usage_stat_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_v2_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_v2_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_v2_response_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_v2_response_payload.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,19 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from alvin_api_client.model.costs_data import CostsData
     from alvin_api_client.model.filter_data_payload import FilterDataPayload
     from alvin_api_client.model.page_search_display_payload import PageSearchDisplayPayload
     from alvin_api_client.model.stat_data_payload import StatDataPayload
+    globals()['CostsData'] = CostsData
     globals()['FilterDataPayload'] = FilterDataPayload
     globals()['PageSearchDisplayPayload'] = PageSearchDisplayPayload
     globals()['StatDataPayload'] = StatDataPayload
 
 
 class SearchV2ResponsePayload(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
@@ -92,27 +94,29 @@
         lazy_import()
         return {
             'results': (PageSearchDisplayPayload,),  # noqa: E501
             'stat_data': ([StatDataPayload],),  # noqa: E501
             'total': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'completed_in': (int,),  # noqa: E501
             'num_remaining_data': (FilterDataPayload,),  # noqa: E501
+            'costs_data': (CostsData,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'results': 'results',  # noqa: E501
         'stat_data': 'statData',  # noqa: E501
         'total': 'total',  # noqa: E501
         'completed_in': 'completedIn',  # noqa: E501
         'num_remaining_data': 'numRemainingData',  # noqa: E501
+        'costs_data': 'costsData',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -155,14 +159,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             num_remaining_data (FilterDataPayload): [optional]  # noqa: E501
+            costs_data (CostsData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +252,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             num_remaining_data (FilterDataPayload): [optional]  # noqa: E501
+            costs_data (CostsData): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/search_validation_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/search_validation_payload.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/seen_table_at_level.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/seen_table_at_level.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/sheet_settings.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sheet_settings.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/snowflake_account_details.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/snowflake_account_details.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/snowflake_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/snowflake_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/sort_order.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/sql_table.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/sql_table.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/stat_data_payload.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/stat_data_payload.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/strings_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/strings_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_alter.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_alter.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_existence.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_existence.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_insert.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_insert.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge_action.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge_action.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge_match_action_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge_match_action_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_merge_match_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_merge_match_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/table_update.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/table_update.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tableau_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tableau_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tableau_credentials.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tableau_credentials.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_data_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_data_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_entity_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_entity_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_entity_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_entity_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tag_values.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tag_values.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/taxonomy_classification_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/taxonomy_classification_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tiny_url_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tiny_url_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/token.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/token.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/treasure_data_additional_config.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/treasure_data_additional_config.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/treasure_data_credentials.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/treasure_data_credentials.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/tree_result_classification.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/tree_result_classification.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/truncate_result.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/truncate_result.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_activity_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_activity_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_activity_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_activity_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,28 +89,30 @@
         return {
             'event_type': (UserActivityType,),  # noqa: E501
             'event_payload': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'org_id': (str,),  # noqa: E501
             'user_email': (str,),  # noqa: E501
             'view_date': (datetime,),  # noqa: E501
             'view_count': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'event_type': 'eventType',  # noqa: E501
         'event_payload': 'eventPayload',  # noqa: E501
         'org_id': 'orgId',  # noqa: E501
         'user_email': 'userEmail',  # noqa: E501
         'view_date': 'viewDate',  # noqa: E501
         'view_count': 'viewCount',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -154,14 +156,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             view_date (datetime): [optional]  # noqa: E501
             view_count (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +250,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             view_date (datetime): [optional]  # noqa: E501
             view_count (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_activity_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_activity_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/event_search_response_costs_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from alvin_api_client.exceptions import ApiAttributeError
 
 
 
-class UserCreate(ModelNormal):
+class EventSearchResponseCostsItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,51 +77,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'email': (str,),  # noqa: E501
-            'sha_id': (str,),  # noqa: E501
-            'created_time': (datetime,),  # noqa: E501
-            'first_name': (str,),  # noqa: E501
-            'last_name': (str,),  # noqa: E501
-            'avatar_url': (str,),  # noqa: E501
+            'total_billed': (float,),  # noqa: E501
+            'total_processed': (float,),  # noqa: E501
+            'slot_millis': (float,),  # noqa: E501
+            'billing_tier': (int,),  # noqa: E501
+            'cost': (int,),  # noqa: E501
+            'avg_slot_usage': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'email': 'email',  # noqa: E501
-        'sha_id': 'shaId',  # noqa: E501
-        'created_time': 'createdTime',  # noqa: E501
-        'first_name': 'firstName',  # noqa: E501
-        'last_name': 'lastName',  # noqa: E501
-        'avatar_url': 'avatarUrl',  # noqa: E501
+        'total_billed': 'totalBilled',  # noqa: E501
+        'total_processed': 'totalProcessed',  # noqa: E501
+        'slot_millis': 'slotMillis',  # noqa: E501
+        'billing_tier': 'billingTier',  # noqa: E501
+        'cost': 'cost',  # noqa: E501
+        'avg_slot_usage': 'avgSlotUsage',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, email, *args, **kwargs):  # noqa: E501
-        """UserCreate - a model defined in OpenAPI
-
-        Args:
-            id (str):
-            email (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """EventSearchResponseCostsItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,19 +140,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sha_id (str): [optional]  # noqa: E501
-            created_time (datetime): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            avatar_url (str): [optional]  # noqa: E501
+            total_billed (float): [optional]  # noqa: E501
+            total_processed (float): [optional]  # noqa: E501
+            slot_millis (float): [optional]  # noqa: E501
+            billing_tier (int): [optional]  # noqa: E501
+            cost (int): [optional]  # noqa: E501
+            avg_slot_usage (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -178,16 +173,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -200,20 +193,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, email, *args, **kwargs):  # noqa: E501
-        """UserCreate - a model defined in OpenAPI
-
-        Args:
-            id (str):
-            email (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """EventSearchResponseCostsItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,19 +227,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sha_id (str): [optional]  # noqa: E501
-            created_time (datetime): [optional]  # noqa: E501
-            first_name (str): [optional]  # noqa: E501
-            last_name (str): [optional]  # noqa: E501
-            avatar_url (str): [optional]  # noqa: E501
+            total_billed (float): [optional]  # noqa: E501
+            total_processed (float): [optional]  # noqa: E501
+            slot_millis (float): [optional]  # noqa: E501
+            billing_tier (int): [optional]  # noqa: E501
+            cost (int): [optional]  # noqa: E501
+            avg_slot_usage (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -268,16 +258,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_create_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_create_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_invite_create.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_invite_create.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_name_usage_context.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_name_usage_context.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_name_usage_stat.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_name_usage_stat.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_organization_api_key_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_organization_api_key_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_organization_api_key_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_persona.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_persona.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/user_role.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/user_role.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/valid_data_manual_entity_sub_type.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/valid_data_manual_entity_sub_type.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/validation_error.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_classification.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_classification.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_create_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_create_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_get.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_get.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_save_response.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_save_response.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/view_upsert_request.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/view_upsert_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model/views_sort.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model/views_sort.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/model_utils.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/models/__init__.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,109 +10,131 @@
 # sys.setrecursionlimit(n)
 
 from alvin_api_client.model.api_key_scope import APIKeyScope
 from alvin_api_client.model.api_key_status import APIKeyStatus
 from alvin_api_client.model.api_keys_response import APIKeysResponse
 from alvin_api_client.model.accept_invite_request import AcceptInviteRequest
 from alvin_api_client.model.admin_config import AdminConfig
+from alvin_api_client.model.aggregated_search_cost import AggregatedSearchCost
+from alvin_api_client.model.aggregated_search_orchestration_info import AggregatedSearchOrchestrationInfo
 from alvin_api_client.model.airflow_additional_config import AirflowAdditionalConfig
 from alvin_api_client.model.alter_parse_result import AlterParseResult
 from alvin_api_client.model.alter_type import AlterType
 from alvin_api_client.model.alvin_description_request import AlvinDescriptionRequest
-from alvin_api_client.model.app_schemas_impact_analysis_response_impact_analysis_query_report import AppSchemasImpactAnalysisResponseImpactAnalysisQueryReport
-from alvin_api_client.model.app_schemas_impact_analysis_response_impact_analysis_response import AppSchemasImpactAnalysisResponseImpactAnalysisResponse
-from alvin_api_client.model.app_schemas_impact_analysis_response_impact_analysis_response_status import AppSchemasImpactAnalysisResponseImpactAnalysisResponseStatus
-from alvin_api_client.model.app_schemas_impact_analysis_v3_response_impact_analysis_query_report import AppSchemasImpactAnalysisV3ResponseImpactAnalysisQueryReport
-from alvin_api_client.model.app_schemas_impact_analysis_v3_response_impact_analysis_response import AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponse
-from alvin_api_client.model.app_schemas_impact_analysis_v3_response_impact_analysis_response_status import AppSchemasImpactAnalysisV3ResponseImpactAnalysisResponseStatus
+from alvin_api_client.model.app_api_lineage_models_entity_graph_connector_edge import AppApiLineageModelsEntityGraphConnectorEdge
+from alvin_api_client.model.app_api_lineage_models_entity_graph_node import AppApiLineageModelsEntityGraphNode
+from alvin_api_client.model.app_notifications_models_event_type import AppNotificationsModelsEventType
+from alvin_api_client.model.app_schemas_core_data_entity_lineage_entity_graph_connector_edge import AppSchemasCoreDataEntityLineageEntityGraphConnectorEdge
+from alvin_api_client.model.app_schemas_core_data_entity_lineage_entity_graph_node import AppSchemasCoreDataEntityLineageEntityGraphNode
+from alvin_api_client.model.app_schemas_core_data_platform_events_event_type import AppSchemasCoreDataPlatformEventsEventType
 from alvin_api_client.model.auth_provider import AuthProvider
 from alvin_api_client.model.bi_platform import BiPlatform
 from alvin_api_client.model.big_query_account_details import BigQueryAccountDetails
 from alvin_api_client.model.big_query_additional_config import BigQueryAdditionalConfig
 from alvin_api_client.model.big_query_entity_map import BigQueryEntityMap
 from alvin_api_client.model.body_download_search_as_file_api_v2_search_file_post import BodyDownloadSearchAsFileApiV2SearchFilePost
+from alvin_api_client.model.body_get_dashboard_costs_api_insights_v1_dashboards_post import BodyGetDashboardCostsApiInsightsV1DashboardsPost
+from alvin_api_client.model.body_get_dashboard_costs_api_insights_v2_dashboards_post import BodyGetDashboardCostsApiInsightsV2DashboardsPost
+from alvin_api_client.model.body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post import BodyGetDashboardUsersCostApiInsightsV1DashboardsDashboardIdUsersPost
 from alvin_api_client.model.body_get_manual_entities_api_v1_manual_entities_post import BodyGetManualEntitiesApiV1ManualEntitiesPost
 from alvin_api_client.model.bulk_search_v2_response_payload import BulkSearchV2ResponsePayload
 from alvin_api_client.model.classification_match_type import ClassificationMatchType
 from alvin_api_client.model.classification_type import ClassificationType
 from alvin_api_client.model.client_auth_config import ClientAuthConfig
 from alvin_api_client.model.client_config import ClientConfig
 from alvin_api_client.model.client_config_post_auth import ClientConfigPostAuth
 from alvin_api_client.model.column_alter import ColumnAlter
 from alvin_api_client.model.column_target import ColumnTarget
 from alvin_api_client.model.comparison_operator import ComparisonOperator
 from alvin_api_client.model.config_type import ConfigType
 from alvin_api_client.model.connection_direction import ConnectionDirection
 from alvin_api_client.model.connection_type import ConnectionType
 from alvin_api_client.model.connection_usage_classification import ConnectionUsageClassification
+from alvin_api_client.model.costs_data import CostsData
 from alvin_api_client.model.dbt_additional_config import DBTAdditionalConfig
+from alvin_api_client.model.dashboard_cost import DashboardCost
+from alvin_api_client.model.dashboard_costs_response import DashboardCostsResponse
+from alvin_api_client.model.dashboard_costs_v2_response import DashboardCostsV2Response
+from alvin_api_client.model.dashboard_user_cost import DashboardUserCost
+from alvin_api_client.model.dashboard_users_response import DashboardUsersResponse
 from alvin_api_client.model.data_entity_asset_count_get import DataEntityAssetCountGet
+from alvin_api_client.model.data_entity_connect_nodes_request import DataEntityConnectNodesRequest
 from alvin_api_client.model.data_entity_connection import DataEntityConnection
 from alvin_api_client.model.data_entity_connection_get import DataEntityConnectionGet
 from alvin_api_client.model.data_entity_connection_type import DataEntityConnectionType
 from alvin_api_client.model.data_entity_delete_tag_connection_request import DataEntityDeleteTagConnectionRequest
 from alvin_api_client.model.data_entity_dependency_direction import DataEntityDependencyDirection
 from alvin_api_client.model.data_entity_dependency_get import DataEntityDependencyGet
 from alvin_api_client.model.data_entity_dependency_get_list import DataEntityDependencyGetList
+from alvin_api_client.model.data_entity_enriched import DataEntityEnriched
 from alvin_api_client.model.data_entity_get import DataEntityGet
 from alvin_api_client.model.data_entity_id import DataEntityID
 from alvin_api_client.model.data_entity_iddto import DataEntityIDDTO
 from alvin_api_client.model.data_entity_job_run import DataEntityJobRun
 from alvin_api_client.model.data_entity_job_run_type import DataEntityJobRunType
 from alvin_api_client.model.data_entity_job_step import DataEntityJobStep
 from alvin_api_client.model.data_entity_lineage import DataEntityLineage
 from alvin_api_client.model.data_entity_lineage_children_item import DataEntityLineageChildrenItem
 from alvin_api_client.model.data_entity_lineage_children_request import DataEntityLineageChildrenRequest
 from alvin_api_client.model.data_entity_lineage_children_response import DataEntityLineageChildrenResponse
 from alvin_api_client.model.data_entity_lineage_data import DataEntityLineageData
+from alvin_api_client.model.data_entity_lineage_explorer_response import DataEntityLineageExplorerResponse
 from alvin_api_client.model.data_entity_lineage_graph_edge import DataEntityLineageGraphEdge
 from alvin_api_client.model.data_entity_lineage_graph_node import DataEntityLineageGraphNode
 from alvin_api_client.model.data_entity_lineage_list import DataEntityLineageList
 from alvin_api_client.model.data_entity_lineage_list_item import DataEntityLineageListItem
 from alvin_api_client.model.data_entity_lineage_list_request import DataEntityLineageListRequest
 from alvin_api_client.model.data_entity_lineage_list_response import DataEntityLineageListResponse
 from alvin_api_client.model.data_entity_lineage_node import DataEntityLineageNode
 from alvin_api_client.model.data_entity_lineage_result import DataEntityLineageResult
 from alvin_api_client.model.data_entity_lineage_v2_request_dto import DataEntityLineageV2RequestDTO
 from alvin_api_client.model.data_entity_lineage_v2_response import DataEntityLineageV2Response
+from alvin_api_client.model.data_entity_lineage_v3_request import DataEntityLineageV3Request
+from alvin_api_client.model.data_entity_lineage_v3_response import DataEntityLineageV3Response
 from alvin_api_client.model.data_entity_manual_file_create import DataEntityManualFileCreate
 from alvin_api_client.model.data_entity_manual_generic_create import DataEntityManualGenericCreate
 from alvin_api_client.model.data_entity_manual_topic_create import DataEntityManualTopicCreate
 from alvin_api_client.model.data_entity_manual_update import DataEntityManualUpdate
 from alvin_api_client.model.data_entity_numerical_stat import DataEntityNumericalStat
 from alvin_api_client.model.data_entity_numerical_stat_response import DataEntityNumericalStatResponse
 from alvin_api_client.model.data_entity_numerical_stat_type import DataEntityNumericalStatType
 from alvin_api_client.model.data_entity_run_facet_get import DataEntityRunFacetGet
 from alvin_api_client.model.data_entity_run_get import DataEntityRunGet
 from alvin_api_client.model.data_entity_run_id import DataEntityRunID
 from alvin_api_client.model.data_entity_run_job_mapping_get import DataEntityRunJobMappingGet
 from alvin_api_client.model.data_entity_run_job_step_mapping_get import DataEntityRunJobStepMappingGet
 from alvin_api_client.model.data_entity_run_status import DataEntityRunStatus
 from alvin_api_client.model.data_entity_save_tag_connection_request import DataEntitySaveTagConnectionRequest
+from alvin_api_client.model.data_entity_simple_lineage_response import DataEntitySimpleLineageResponse
 from alvin_api_client.model.data_entity_sub_type import DataEntitySubType
 from alvin_api_client.model.data_entity_transformation import DataEntityTransformation
 from alvin_api_client.model.data_entity_type import DataEntityType
+from alvin_api_client.model.data_entity_usage import DataEntityUsage
+from alvin_api_client.model.data_entity_usage_grouped import DataEntityUsageGrouped
 from alvin_api_client.model.data_entity_usage_stat import DataEntityUsageStat
 from alvin_api_client.model.data_entity_usage_stat_raw import DataEntityUsageStatRaw
 from alvin_api_client.model.data_entity_usage_stats_report import DataEntityUsageStatsReport
 from alvin_api_client.model.data_entity_usage_stats_request import DataEntityUsageStatsRequest
 from alvin_api_client.model.data_entity_usage_type import DataEntityUsageType
+from alvin_api_client.model.data_entity_user_usage import DataEntityUserUsage
+from alvin_api_client.model.data_entity_user_usage_grouped import DataEntityUserUsageGrouped
 from alvin_api_client.model.data_platform_aggregated_job_stat import DataPlatformAggregatedJobStat
 from alvin_api_client.model.data_platform_airflow_create import DataPlatformAirflowCreate
 from alvin_api_client.model.data_platform_big_query_create import DataPlatformBigQueryCreate
 from alvin_api_client.model.data_platform_created_in import DataPlatformCreatedIn
 from alvin_api_client.model.data_platform_dbt_create import DataPlatformDBTCreate
 from alvin_api_client.model.data_platform_databricks_create import DataPlatformDatabricksCreate
 from alvin_api_client.model.data_platform_delete import DataPlatformDelete
 from alvin_api_client.model.data_platform_full import DataPlatformFull
 from alvin_api_client.model.data_platform_get import DataPlatformGet
 from alvin_api_client.model.data_platform_hightouch_create import DataPlatformHightouchCreate
 from alvin_api_client.model.data_platform_hive_create import DataPlatformHiveCreate
 from alvin_api_client.model.data_platform_hive_glue_create import DataPlatformHiveGlueCreate
 from alvin_api_client.model.data_platform_job import DataPlatformJob
+from alvin_api_client.model.data_platform_job_costs import DataPlatformJobCosts
 from alvin_api_client.model.data_platform_job_entity_aggregated_report import DataPlatformJobEntityAggregatedReport
 from alvin_api_client.model.data_platform_job_execution_status import DataPlatformJobExecutionStatus
 from alvin_api_client.model.data_platform_job_stat import DataPlatformJobStat
 from alvin_api_client.model.data_platform_job_step import DataPlatformJobStep
 from alvin_api_client.model.data_platform_job_step_aggregated_report import DataPlatformJobStepAggregatedReport
 from alvin_api_client.model.data_platform_job_step_execution_status import DataPlatformJobStepExecutionStatus
 from alvin_api_client.model.data_platform_job_step_id import DataPlatformJobStepId
@@ -162,24 +184,51 @@
 from alvin_api_client.model.data_tag_v2 import DataTagV2
 from alvin_api_client.model.data_taxonomy_classification import DataTaxonomyClassification
 from alvin_api_client.model.data_transformation_lineage import DataTransformationLineage
 from alvin_api_client.model.databricks_account_details import DatabricksAccountDetails
 from alvin_api_client.model.databricks_additional_config import DatabricksAdditionalConfig
 from alvin_api_client.model.datadog_settings import DatadogSettings
 from alvin_api_client.model.delete_parse_result import DeleteParseResult
+from alvin_api_client.model.direction_enum import DirectionEnum
 from alvin_api_client.model.drop_parse_result import DropParseResult
 from alvin_api_client.model.drop_type import DropType
 from alvin_api_client.model.element_position import ElementPosition
 from alvin_api_client.model.email_login_request import EmailLoginRequest
-from alvin_api_client.model.entity_graph_connector_edge import EntityGraphConnectorEdge
-from alvin_api_client.model.entity_graph_node import EntityGraphNode
+from alvin_api_client.model.entity_events_context import EntityEventsContext
 from alvin_api_client.model.entity_graph_node_connector import EntityGraphNodeConnector
 from alvin_api_client.model.entity_usage_context import EntityUsageContext
 from alvin_api_client.model.environment_config import EnvironmentConfig
-from alvin_api_client.model.event_type import EventType
+from alvin_api_client.model.event_chart_data import EventChartData
+from alvin_api_client.model.event_chart_x_asis_data import EventChartXAsisData
+from alvin_api_client.model.event_chart_y_asis_data import EventChartYAsisData
+from alvin_api_client.model.event_group import EventGroup
+from alvin_api_client.model.event_group_value import EventGroupValue
+from alvin_api_client.model.event_metric import EventMetric
+from alvin_api_client.model.event_metric_aggregation import EventMetricAggregation
+from alvin_api_client.model.event_metric_function import EventMetricFunction
+from alvin_api_client.model.event_metric_group_type import EventMetricGroupType
+from alvin_api_client.model.event_metric_type import EventMetricType
+from alvin_api_client.model.event_metric_value import EventMetricValue
+from alvin_api_client.model.event_request_filter import EventRequestFilter
+from alvin_api_client.model.event_search_pagination import EventSearchPagination
+from alvin_api_client.model.event_search_request import EventSearchRequest
+from alvin_api_client.model.event_search_response import EventSearchResponse
+from alvin_api_client.model.event_search_response_costs_item import EventSearchResponseCostsItem
+from alvin_api_client.model.event_search_response_group_item import EventSearchResponseGroupItem
+from alvin_api_client.model.event_search_response_group_item_value import EventSearchResponseGroupItemValue
+from alvin_api_client.model.event_search_response_item import EventSearchResponseItem
+from alvin_api_client.model.event_search_response_row_stats_item import EventSearchResponseRowStatsItem
+from alvin_api_client.model.event_search_timeline_response import EventSearchTimelineResponse
+from alvin_api_client.model.event_search_type_values_response import EventSearchTypeValuesResponse
+from alvin_api_client.model.event_search_values_count_response import EventSearchValuesCountResponse
+from alvin_api_client.model.event_stats_group import EventStatsGroup
+from alvin_api_client.model.event_stats_report import EventStatsReport
+from alvin_api_client.model.event_stats_request import EventStatsRequest
+from alvin_api_client.model.event_stats_request_stat_group import EventStatsRequestStatGroup
+from alvin_api_client.model.event_users_response import EventUsersResponse
 from alvin_api_client.model.exchange_token_request import ExchangeTokenRequest
 from alvin_api_client.model.experience import Experience
 from alvin_api_client.model.experience_data import ExperienceData
 from alvin_api_client.model.experience_status import ExperienceStatus
 from alvin_api_client.model.experience_user import ExperienceUser
 from alvin_api_client.model.experiences_settings import ExperiencesSettings
 from alvin_api_client.model.extracted_simple_column import ExtractedSimpleColumn
@@ -188,14 +237,15 @@
 from alvin_api_client.model.filter_match import FilterMatch
 from alvin_api_client.model.filter_options import FilterOptions
 from alvin_api_client.model.filter_type import FilterType
 from alvin_api_client.model.filter_view import FilterView
 from alvin_api_client.model.filters_response import FiltersResponse
 from alvin_api_client.model.firebase_auth_provider import FirebaseAuthProvider
 from alvin_api_client.model.firebase_auth_ui_config import FirebaseAuthUIConfig
+from alvin_api_client.model.get_table_num_rows_chart_response import GetTableNumRowsChartResponse
 from alvin_api_client.model.group_type import GroupType
 from alvin_api_client.model.html_values import HTMLValues
 from alvin_api_client.model.http_validation_error import HTTPValidationError
 from alvin_api_client.model.healthcheck_response import HealthcheckResponse
 from alvin_api_client.model.hightouch_additional_config import HightouchAdditionalConfig
 from alvin_api_client.model.hightouch_credentials import HightouchCredentials
 from alvin_api_client.model.hive_account_details import HiveAccountDetails
@@ -206,19 +256,37 @@
 from alvin_api_client.model.ia_job_data import IAJobData
 from alvin_api_client.model.ia_platform_data import IAPlatformData
 from alvin_api_client.model.ia_row import IARow
 from alvin_api_client.model.ia_row_type import IARowType
 from alvin_api_client.model.impact_analysis_node_list_response import ImpactAnalysisNodeListResponse
 from alvin_api_client.model.impact_analysis_node_stats import ImpactAnalysisNodeStats
 from alvin_api_client.model.impact_analysis_platform_request import ImpactAnalysisPlatformRequest
+from alvin_api_client.model.impact_analysis_query_report import ImpactAnalysisQueryReport
 from alvin_api_client.model.impact_analysis_query_request import ImpactAnalysisQueryRequest
 from alvin_api_client.model.impact_analysis_query_validation import ImpactAnalysisQueryValidation
 from alvin_api_client.model.impact_analysis_request import ImpactAnalysisRequest
+from alvin_api_client.model.impact_analysis_response import ImpactAnalysisResponse
+from alvin_api_client.model.impact_analysis_response_status import ImpactAnalysisResponseStatus
 from alvin_api_client.model.impact_analysis_validation_payload import ImpactAnalysisValidationPayload
+from alvin_api_client.model.impact_analysis_validation_payload_v2 import ImpactAnalysisValidationPayloadV2
 from alvin_api_client.model.impact_status import ImpactStatus
+from alvin_api_client.model.impact_type import ImpactType
+from alvin_api_client.model.insight_metric import InsightMetric
+from alvin_api_client.model.insight_usage_group import InsightUsageGroup
+from alvin_api_client.model.insights_chart_series_data import InsightsChartSeriesData
+from alvin_api_client.model.insights_chart_x_axis import InsightsChartXAxis
+from alvin_api_client.model.insights_chart_x_axis_type import InsightsChartXAxisType
+from alvin_api_client.model.insights_delta_response import InsightsDeltaResponse
+from alvin_api_client.model.insights_request import InsightsRequest
+from alvin_api_client.model.insights_response import InsightsResponse
+from alvin_api_client.model.insights_usage_metric_aggregation import InsightsUsageMetricAggregation
+from alvin_api_client.model.insights_usage_request import InsightsUsageRequest
+from alvin_api_client.model.insights_usage_request_stat_group import InsightsUsageRequestStatGroup
+from alvin_api_client.model.insights_usage_response import InsightsUsageResponse
+from alvin_api_client.model.insights_usage_stats_response import InsightsUsageStatsResponse
 from alvin_api_client.model.job_entity_id import JobEntityID
 from alvin_api_client.model.job_entity_usage_stats_report import JobEntityUsageStatsReport
 from alvin_api_client.model.job_query_request import JobQueryRequest
 from alvin_api_client.model.job_query_v1_response import JobQueryV1Response
 from alvin_api_client.model.job_steps_agg_response_model import JobStepsAggResponseModel
 from alvin_api_client.model.kirby_failed_batches_response import KirbyFailedBatchesResponse
 from alvin_api_client.model.kirby_ingest_request import KirbyIngestRequest
@@ -234,19 +302,30 @@
 from alvin_api_client.model.limit_offset_page_data_entity_usage_stat_raw import LimitOffsetPageDataEntityUsageStatRaw
 from alvin_api_client.model.limit_offset_page_data_entity_usage_stats_report import LimitOffsetPageDataEntityUsageStatsReport
 from alvin_api_client.model.limit_offset_page_data_platform_job import LimitOffsetPageDataPlatformJob
 from alvin_api_client.model.limit_offset_page_data_platform_job_entity_aggregated_report import LimitOffsetPageDataPlatformJobEntityAggregatedReport
 from alvin_api_client.model.limit_offset_page_data_tag_connection_get import LimitOffsetPageDataTagConnectionGet
 from alvin_api_client.model.limit_offset_page_data_tag_get import LimitOffsetPageDataTagGet
 from alvin_api_client.model.limit_offset_page_data_tag_rule_get import LimitOffsetPageDataTagRuleGet
+from alvin_api_client.model.limit_offset_page_insights_usage_response import LimitOffsetPageInsightsUsageResponse
 from alvin_api_client.model.limit_offset_page_manual_lineage_data import LimitOffsetPageManualLineageData
+from alvin_api_client.model.limit_offset_page_organization_get import LimitOffsetPageOrganizationGet
+from alvin_api_client.model.limit_offset_page_pipeline_get import LimitOffsetPagePipelineGet
 from alvin_api_client.model.lineage_connection_type import LineageConnectionType
 from alvin_api_client.model.lineage_expanding_type import LineageExpandingType
+from alvin_api_client.model.lineage_field_enum import LineageFieldEnum
+from alvin_api_client.model.lineage_graph_request import LineageGraphRequest
 from alvin_api_client.model.lineage_scope import LineageScope
 from alvin_api_client.model.links_request import LinksRequest
+from alvin_api_client.model.list_event_databases_request import ListEventDatabasesRequest
+from alvin_api_client.model.list_event_databases_response import ListEventDatabasesResponse
+from alvin_api_client.model.list_event_users_by_period_request import ListEventUsersByPeriodRequest
+from alvin_api_client.model.list_event_users_by_period_response import ListEventUsersByPeriodResponse
+from alvin_api_client.model.list_platform_databases_request import ListPlatformDatabasesRequest
+from alvin_api_client.model.list_platform_databases_response import ListPlatformDatabasesResponse
 from alvin_api_client.model.looker_additional_config import LookerAdditionalConfig
 from alvin_api_client.model.looker_credentials import LookerCredentials
 from alvin_api_client.model.looker_query_comment import LookerQueryComment
 from alvin_api_client.model.mssql_account_details import MSSQLAccountDetails
 from alvin_api_client.model.mssql_additional_config import MSSQLAdditionalConfig
 from alvin_api_client.model.manual_lineage_data import ManualLineageData
 from alvin_api_client.model.manual_lineage_data_request import ManualLineageDataRequest
@@ -257,19 +336,25 @@
 from alvin_api_client.model.my_sql_additional_config import MySQLAdditionalConfig
 from alvin_api_client.model.notification import Notification
 from alvin_api_client.model.notification_config import NotificationConfig
 from alvin_api_client.model.notification_provider import NotificationProvider
 from alvin_api_client.model.notification_type import NotificationType
 from alvin_api_client.model.onboarding_level import OnboardingLevel
 from alvin_api_client.model.operator_type import OperatorType
+from alvin_api_client.model.organization_create import OrganizationCreate
 from alvin_api_client.model.organization_get import OrganizationGet
 from alvin_api_client.model.organization_status import OrganizationStatus
+from alvin_api_client.model.organization_update import OrganizationUpdate
 from alvin_api_client.model.page_data_entity_get import PageDataEntityGet
 from alvin_api_client.model.page_search_display_payload import PageSearchDisplayPayload
 from alvin_api_client.model.page_view_get import PageViewGet
+from alvin_api_client.model.pipeline_get import PipelineGet
+from alvin_api_client.model.pipeline_run_get import PipelineRunGet
+from alvin_api_client.model.pipeline_run_metrics import PipelineRunMetrics
+from alvin_api_client.model.pipeline_step import PipelineStep
 from alvin_api_client.model.platform_asset_type import PlatformAssetType
 from alvin_api_client.model.platform_build_data import PlatformBuildData
 from alvin_api_client.model.platform_build_type import PlatformBuildType
 from alvin_api_client.model.platform_classification import PlatformClassification
 from alvin_api_client.model.popularity_values import PopularityValues
 from alvin_api_client.model.position import Position
 from alvin_api_client.model.postgres_account_details import PostgresAccountDetails
@@ -282,35 +367,41 @@
 from alvin_api_client.model.query_builder import QueryBuilder
 from alvin_api_client.model.query_comment import QueryComment
 from alvin_api_client.model.query_create_mode import QueryCreateMode
 from alvin_api_client.model.query_fingerprint import QueryFingerprint
 from alvin_api_client.model.query_lineage_parse_result import QueryLineageParseResult
 from alvin_api_client.model.query_parse_result import QueryParseResult
 from alvin_api_client.model.query_type import QueryType
+from alvin_api_client.model.recommendation_actions import RecommendationActions
 from alvin_api_client.model.redshift_account_details import RedshiftAccountDetails
 from alvin_api_client.model.redshift_additional_config import RedshiftAdditionalConfig
 from alvin_api_client.model.rule_element import RuleElement
 from alvin_api_client.model.rule_element_value_type import RuleElementValueType
 from alvin_api_client.model.rule_type import RuleType
 from alvin_api_client.model.rule_value import RuleValue
 from alvin_api_client.model.search_csv_column import SearchCSVColumn
 from alvin_api_client.model.search_display_payload import SearchDisplayPayload
+from alvin_api_client.model.search_entities_response import SearchEntitiesResponse
+from alvin_api_client.model.search_entity import SearchEntity
 from alvin_api_client.model.search_filter_label_association import SearchFilterLabelAssociation
 from alvin_api_client.model.search_node import SearchNode
 from alvin_api_client.model.search_prefix import SearchPrefix
 from alvin_api_client.model.search_usage_stat_type import SearchUsageStatType
 from alvin_api_client.model.search_v2_response import SearchV2Response
 from alvin_api_client.model.search_v2_response_payload import SearchV2ResponsePayload
 from alvin_api_client.model.seen_table_at_level import SeenTableAtLevel
 from alvin_api_client.model.sheet_settings import SheetSettings
 from alvin_api_client.model.snowflake_account_details import SnowflakeAccountDetails
 from alvin_api_client.model.snowflake_additional_config import SnowflakeAdditionalConfig
+from alvin_api_client.model.sort_field import SortField
 from alvin_api_client.model.sort_order import SortOrder
+from alvin_api_client.model.source_entity_request import SourceEntityRequest
 from alvin_api_client.model.sql_table import SqlTable
 from alvin_api_client.model.stat_data_payload import StatDataPayload
+from alvin_api_client.model.stats_agreggation_data import StatsAgreggationData
 from alvin_api_client.model.strings_response import StringsResponse
 from alvin_api_client.model.table_alter import TableAlter
 from alvin_api_client.model.table_existence import TableExistence
 from alvin_api_client.model.table_insert import TableInsert
 from alvin_api_client.model.table_merge import TableMerge
 from alvin_api_client.model.table_merge_action import TableMergeAction
 from alvin_api_client.model.table_merge_match_action_type import TableMergeMatchActionType
@@ -322,14 +413,15 @@
 from alvin_api_client.model.taxonomy_classification_config import TaxonomyClassificationConfig
 from alvin_api_client.model.tiny_url_response import TinyURLResponse
 from alvin_api_client.model.token import Token
 from alvin_api_client.model.treasure_data_additional_config import TreasureDataAdditionalConfig
 from alvin_api_client.model.treasure_data_credentials import TreasureDataCredentials
 from alvin_api_client.model.tree_result_classification import TreeResultClassification
 from alvin_api_client.model.truncate_result import TruncateResult
+from alvin_api_client.model.usage_context import UsageContext
 from alvin_api_client.model.user_activity_request import UserActivityRequest
 from alvin_api_client.model.user_activity_response import UserActivityResponse
 from alvin_api_client.model.user_activity_type import UserActivityType
 from alvin_api_client.model.user_create import UserCreate
 from alvin_api_client.model.user_create_request import UserCreateRequest
 from alvin_api_client.model.user_get import UserGet
 from alvin_api_client.model.user_invite_create import UserInviteCreate
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client/rest.py` & `alvin_api_client-1.4.0rc1/src/alvin_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/PKG-INFO` & `alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alvin-api-client
-Version: 1.3.0rc2
+Version: 1.4.0rc1
 Summary: Python SDK implementing a Client of the Alvin API
 Home-page: https://github.com/alvindotai/alvin/tree/master/alvin_api_client
 Author: Alvin
 Author-email: tech@alvin.ai
 License: AGPLv3
 Project-URL: Bug Tracker, https://github.com/alvindotai/alvin/issues
 Project-URL: Source Code, https://github.com/alvindotai/alvin/tree/master/alvin_api_client
```

### Comparing `alvin_api_client-1.3.0rc2/src/alvin_api_client.egg-info/SOURCES.txt` & `alvin_api_client-1.4.0rc1/src/alvin_api_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,78 +18,100 @@
 src/alvin_api_client.egg-info/top_level.txt
 src/alvin_api_client/api/__init__.py
 src/alvin_api_client/api/default_api.py
 src/alvin_api_client/apis/__init__.py
 src/alvin_api_client/model/__init__.py
 src/alvin_api_client/model/accept_invite_request.py
 src/alvin_api_client/model/admin_config.py
+src/alvin_api_client/model/aggregated_search_cost.py
+src/alvin_api_client/model/aggregated_search_orchestration_info.py
 src/alvin_api_client/model/airflow_additional_config.py
 src/alvin_api_client/model/alter_parse_result.py
 src/alvin_api_client/model/alter_type.py
 src/alvin_api_client/model/alvin_description_request.py
 src/alvin_api_client/model/api_key_scope.py
 src/alvin_api_client/model/api_key_status.py
 src/alvin_api_client/model/api_keys_response.py
+src/alvin_api_client/model/app_api_lineage_models_entity_graph_connector_edge.py
+src/alvin_api_client/model/app_api_lineage_models_entity_graph_node.py
+src/alvin_api_client/model/app_notifications_models_event_type.py
+src/alvin_api_client/model/app_schemas_core_data_entity_lineage_entity_graph_connector_edge.py
+src/alvin_api_client/model/app_schemas_core_data_entity_lineage_entity_graph_node.py
+src/alvin_api_client/model/app_schemas_core_data_platform_events_event_type.py
 src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_query_report.py
 src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response.py
 src/alvin_api_client/model/app_schemas_impact_analysis_response_impact_analysis_response_status.py
 src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_query_report.py
 src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response.py
 src/alvin_api_client/model/app_schemas_impact_analysis_v3_response_impact_analysis_response_status.py
 src/alvin_api_client/model/auth_provider.py
 src/alvin_api_client/model/bi_platform.py
 src/alvin_api_client/model/big_query_account_details.py
 src/alvin_api_client/model/big_query_additional_config.py
 src/alvin_api_client/model/big_query_entity_map.py
 src/alvin_api_client/model/body_download_search_as_file_api_v2_search_file_post.py
+src/alvin_api_client/model/body_get_dashboard_costs_api_insights_v1_dashboards_post.py
+src/alvin_api_client/model/body_get_dashboard_costs_api_insights_v2_dashboards_post.py
+src/alvin_api_client/model/body_get_dashboard_users_cost_api_insights_v1_dashboards_dashboard_id_users_post.py
 src/alvin_api_client/model/body_get_manual_entities_api_v1_manual_entities_post.py
 src/alvin_api_client/model/bulk_search_v2_response_payload.py
 src/alvin_api_client/model/classification_match_type.py
 src/alvin_api_client/model/classification_type.py
 src/alvin_api_client/model/client_auth_config.py
 src/alvin_api_client/model/client_config.py
 src/alvin_api_client/model/client_config_post_auth.py
 src/alvin_api_client/model/column_alter.py
 src/alvin_api_client/model/column_target.py
 src/alvin_api_client/model/comparison_operator.py
 src/alvin_api_client/model/config_type.py
 src/alvin_api_client/model/connection_direction.py
 src/alvin_api_client/model/connection_type.py
 src/alvin_api_client/model/connection_usage_classification.py
+src/alvin_api_client/model/costs_data.py
+src/alvin_api_client/model/dashboard_cost.py
+src/alvin_api_client/model/dashboard_costs_response.py
+src/alvin_api_client/model/dashboard_costs_v2_response.py
+src/alvin_api_client/model/dashboard_user_cost.py
+src/alvin_api_client/model/dashboard_users_response.py
 src/alvin_api_client/model/data_entity_asset_count_get.py
+src/alvin_api_client/model/data_entity_connect_nodes_request.py
 src/alvin_api_client/model/data_entity_connection.py
 src/alvin_api_client/model/data_entity_connection_get.py
 src/alvin_api_client/model/data_entity_connection_type.py
 src/alvin_api_client/model/data_entity_delete_tag_connection_request.py
 src/alvin_api_client/model/data_entity_dependency_direction.py
 src/alvin_api_client/model/data_entity_dependency_get.py
 src/alvin_api_client/model/data_entity_dependency_get_list.py
 src/alvin_api_client/model/data_entity_detail.py
+src/alvin_api_client/model/data_entity_enriched.py
 src/alvin_api_client/model/data_entity_get.py
 src/alvin_api_client/model/data_entity_id.py
 src/alvin_api_client/model/data_entity_iddto.py
 src/alvin_api_client/model/data_entity_job_run.py
 src/alvin_api_client/model/data_entity_job_run_type.py
 src/alvin_api_client/model/data_entity_job_step.py
 src/alvin_api_client/model/data_entity_lineage.py
 src/alvin_api_client/model/data_entity_lineage_children_item.py
 src/alvin_api_client/model/data_entity_lineage_children_request.py
 src/alvin_api_client/model/data_entity_lineage_children_response.py
 src/alvin_api_client/model/data_entity_lineage_data.py
+src/alvin_api_client/model/data_entity_lineage_explorer_response.py
 src/alvin_api_client/model/data_entity_lineage_graph_edge.py
 src/alvin_api_client/model/data_entity_lineage_graph_node.py
 src/alvin_api_client/model/data_entity_lineage_list.py
 src/alvin_api_client/model/data_entity_lineage_list_item.py
 src/alvin_api_client/model/data_entity_lineage_list_request.py
 src/alvin_api_client/model/data_entity_lineage_list_response.py
 src/alvin_api_client/model/data_entity_lineage_node.py
 src/alvin_api_client/model/data_entity_lineage_result.py
 src/alvin_api_client/model/data_entity_lineage_v2_request.py
 src/alvin_api_client/model/data_entity_lineage_v2_request_dto.py
 src/alvin_api_client/model/data_entity_lineage_v2_response.py
+src/alvin_api_client/model/data_entity_lineage_v3_request.py
+src/alvin_api_client/model/data_entity_lineage_v3_response.py
 src/alvin_api_client/model/data_entity_manual_file_create.py
 src/alvin_api_client/model/data_entity_manual_generic_create.py
 src/alvin_api_client/model/data_entity_manual_topic_create.py
 src/alvin_api_client/model/data_entity_manual_update.py
 src/alvin_api_client/model/data_entity_numerical_stat.py
 src/alvin_api_client/model/data_entity_numerical_stat_response.py
 src/alvin_api_client/model/data_entity_numerical_stat_type.py
@@ -97,36 +119,42 @@
 src/alvin_api_client/model/data_entity_run_facet_get.py
 src/alvin_api_client/model/data_entity_run_get.py
 src/alvin_api_client/model/data_entity_run_id.py
 src/alvin_api_client/model/data_entity_run_job_mapping_get.py
 src/alvin_api_client/model/data_entity_run_job_step_mapping_get.py
 src/alvin_api_client/model/data_entity_run_status.py
 src/alvin_api_client/model/data_entity_save_tag_connection_request.py
+src/alvin_api_client/model/data_entity_simple_lineage_response.py
 src/alvin_api_client/model/data_entity_sub_type.py
 src/alvin_api_client/model/data_entity_transformation.py
 src/alvin_api_client/model/data_entity_type.py
+src/alvin_api_client/model/data_entity_usage.py
+src/alvin_api_client/model/data_entity_usage_grouped.py
 src/alvin_api_client/model/data_entity_usage_stat.py
 src/alvin_api_client/model/data_entity_usage_stat_raw.py
 src/alvin_api_client/model/data_entity_usage_stats_report.py
 src/alvin_api_client/model/data_entity_usage_stats_request.py
 src/alvin_api_client/model/data_entity_usage_type.py
+src/alvin_api_client/model/data_entity_user_usage.py
+src/alvin_api_client/model/data_entity_user_usage_grouped.py
 src/alvin_api_client/model/data_manual_entity_sub_type.py
 src/alvin_api_client/model/data_platform_aggregated_job_stat.py
 src/alvin_api_client/model/data_platform_airflow_create.py
 src/alvin_api_client/model/data_platform_big_query_create.py
 src/alvin_api_client/model/data_platform_created_in.py
 src/alvin_api_client/model/data_platform_databricks_create.py
 src/alvin_api_client/model/data_platform_dbt_create.py
 src/alvin_api_client/model/data_platform_delete.py
 src/alvin_api_client/model/data_platform_full.py
 src/alvin_api_client/model/data_platform_get.py
 src/alvin_api_client/model/data_platform_hightouch_create.py
 src/alvin_api_client/model/data_platform_hive_create.py
 src/alvin_api_client/model/data_platform_hive_glue_create.py
 src/alvin_api_client/model/data_platform_job.py
+src/alvin_api_client/model/data_platform_job_costs.py
 src/alvin_api_client/model/data_platform_job_entity_aggregated_report.py
 src/alvin_api_client/model/data_platform_job_execution_status.py
 src/alvin_api_client/model/data_platform_job_stat.py
 src/alvin_api_client/model/data_platform_job_step.py
 src/alvin_api_client/model/data_platform_job_step_aggregated_report.py
 src/alvin_api_client/model/data_platform_job_step_execution_status.py
 src/alvin_api_client/model/data_platform_job_step_id.py
@@ -177,24 +205,54 @@
 src/alvin_api_client/model/data_taxonomy_classification.py
 src/alvin_api_client/model/data_transformation_lineage.py
 src/alvin_api_client/model/databricks_account_details.py
 src/alvin_api_client/model/databricks_additional_config.py
 src/alvin_api_client/model/datadog_settings.py
 src/alvin_api_client/model/dbt_additional_config.py
 src/alvin_api_client/model/delete_parse_result.py
+src/alvin_api_client/model/direction_enum.py
 src/alvin_api_client/model/drop_parse_result.py
 src/alvin_api_client/model/drop_type.py
 src/alvin_api_client/model/element_position.py
 src/alvin_api_client/model/email_login_request.py
+src/alvin_api_client/model/entity_events_context.py
 src/alvin_api_client/model/entity_graph_connector_edge.py
 src/alvin_api_client/model/entity_graph_node.py
 src/alvin_api_client/model/entity_graph_node_connector.py
 src/alvin_api_client/model/entity_usage_context.py
 src/alvin_api_client/model/environment_config.py
+src/alvin_api_client/model/event_chart_data.py
+src/alvin_api_client/model/event_chart_x_asis_data.py
+src/alvin_api_client/model/event_chart_y_asis_data.py
+src/alvin_api_client/model/event_group.py
+src/alvin_api_client/model/event_group_value.py
+src/alvin_api_client/model/event_metric.py
+src/alvin_api_client/model/event_metric_aggregation.py
+src/alvin_api_client/model/event_metric_function.py
+src/alvin_api_client/model/event_metric_group_type.py
+src/alvin_api_client/model/event_metric_type.py
+src/alvin_api_client/model/event_metric_value.py
+src/alvin_api_client/model/event_request_filter.py
+src/alvin_api_client/model/event_search_pagination.py
+src/alvin_api_client/model/event_search_request.py
+src/alvin_api_client/model/event_search_response.py
+src/alvin_api_client/model/event_search_response_costs_item.py
+src/alvin_api_client/model/event_search_response_group_item.py
+src/alvin_api_client/model/event_search_response_group_item_value.py
+src/alvin_api_client/model/event_search_response_item.py
+src/alvin_api_client/model/event_search_response_row_stats_item.py
+src/alvin_api_client/model/event_search_timeline_response.py
+src/alvin_api_client/model/event_search_type_values_response.py
+src/alvin_api_client/model/event_search_values_count_response.py
+src/alvin_api_client/model/event_stats_group.py
+src/alvin_api_client/model/event_stats_report.py
+src/alvin_api_client/model/event_stats_request.py
+src/alvin_api_client/model/event_stats_request_stat_group.py
 src/alvin_api_client/model/event_type.py
+src/alvin_api_client/model/event_users_response.py
 src/alvin_api_client/model/exchange_token_request.py
 src/alvin_api_client/model/experience.py
 src/alvin_api_client/model/experience_data.py
 src/alvin_api_client/model/experience_status.py
 src/alvin_api_client/model/experience_user.py
 src/alvin_api_client/model/experiences_settings.py
 src/alvin_api_client/model/extracted_simple_column.py
@@ -203,14 +261,15 @@
 src/alvin_api_client/model/filter_match.py
 src/alvin_api_client/model/filter_options.py
 src/alvin_api_client/model/filter_type.py
 src/alvin_api_client/model/filter_view.py
 src/alvin_api_client/model/filters_response.py
 src/alvin_api_client/model/firebase_auth_provider.py
 src/alvin_api_client/model/firebase_auth_ui_config.py
+src/alvin_api_client/model/get_table_num_rows_chart_response.py
 src/alvin_api_client/model/group_type.py
 src/alvin_api_client/model/healthcheck_response.py
 src/alvin_api_client/model/hightouch_additional_config.py
 src/alvin_api_client/model/hightouch_credentials.py
 src/alvin_api_client/model/hive_account_details.py
 src/alvin_api_client/model/hive_additional_config.py
 src/alvin_api_client/model/hive_glue_account_details.py
@@ -233,15 +292,30 @@
 src/alvin_api_client/model/impact_analysis_response_status.py
 src/alvin_api_client/model/impact_analysis_sidebar_data_node.py
 src/alvin_api_client/model/impact_analysis_v2_entity_row.py
 src/alvin_api_client/model/impact_analysis_v2_job_row.py
 src/alvin_api_client/model/impact_analysis_v2_response.py
 src/alvin_api_client/model/impact_analysis_v2_response_status.py
 src/alvin_api_client/model/impact_analysis_validation_payload.py
+src/alvin_api_client/model/impact_analysis_validation_payload_v2.py
 src/alvin_api_client/model/impact_status.py
+src/alvin_api_client/model/impact_type.py
+src/alvin_api_client/model/insight_metric.py
+src/alvin_api_client/model/insight_usage_group.py
+src/alvin_api_client/model/insights_chart_series_data.py
+src/alvin_api_client/model/insights_chart_x_axis.py
+src/alvin_api_client/model/insights_chart_x_axis_type.py
+src/alvin_api_client/model/insights_delta_response.py
+src/alvin_api_client/model/insights_request.py
+src/alvin_api_client/model/insights_response.py
+src/alvin_api_client/model/insights_usage_metric_aggregation.py
+src/alvin_api_client/model/insights_usage_request.py
+src/alvin_api_client/model/insights_usage_request_stat_group.py
+src/alvin_api_client/model/insights_usage_response.py
+src/alvin_api_client/model/insights_usage_stats_response.py
 src/alvin_api_client/model/job_entity_id.py
 src/alvin_api_client/model/job_entity_usage_stats_report.py
 src/alvin_api_client/model/job_integration_request.py
 src/alvin_api_client/model/job_query_request.py
 src/alvin_api_client/model/job_query_v1_response.py
 src/alvin_api_client/model/job_steps_agg_response_model.py
 src/alvin_api_client/model/kirby_failed_batches_response.py
@@ -258,20 +332,31 @@
 src/alvin_api_client/model/limit_offset_page_data_entity_usage_stat_raw.py
 src/alvin_api_client/model/limit_offset_page_data_entity_usage_stats_report.py
 src/alvin_api_client/model/limit_offset_page_data_platform_job.py
 src/alvin_api_client/model/limit_offset_page_data_platform_job_entity_aggregated_report.py
 src/alvin_api_client/model/limit_offset_page_data_tag_connection_get.py
 src/alvin_api_client/model/limit_offset_page_data_tag_get.py
 src/alvin_api_client/model/limit_offset_page_data_tag_rule_get.py
+src/alvin_api_client/model/limit_offset_page_insights_usage_response.py
 src/alvin_api_client/model/limit_offset_page_manual_lineage_data.py
+src/alvin_api_client/model/limit_offset_page_organization_get.py
+src/alvin_api_client/model/limit_offset_page_pipeline_get.py
 src/alvin_api_client/model/limit_offset_page_tag_entity_get.py
 src/alvin_api_client/model/lineage_connection_type.py
 src/alvin_api_client/model/lineage_expanding_type.py
+src/alvin_api_client/model/lineage_field_enum.py
+src/alvin_api_client/model/lineage_graph_request.py
 src/alvin_api_client/model/lineage_scope.py
 src/alvin_api_client/model/links_request.py
+src/alvin_api_client/model/list_event_databases_request.py
+src/alvin_api_client/model/list_event_databases_response.py
+src/alvin_api_client/model/list_event_users_by_period_request.py
+src/alvin_api_client/model/list_event_users_by_period_response.py
+src/alvin_api_client/model/list_platform_databases_request.py
+src/alvin_api_client/model/list_platform_databases_response.py
 src/alvin_api_client/model/looker_additional_config.py
 src/alvin_api_client/model/looker_credentials.py
 src/alvin_api_client/model/looker_query_comment.py
 src/alvin_api_client/model/manual_lineage_data.py
 src/alvin_api_client/model/manual_lineage_data_request.py
 src/alvin_api_client/model/manual_lineage_entity_type_validation.py
 src/alvin_api_client/model/map_entity_to_url_request.py
@@ -283,19 +368,25 @@
 src/alvin_api_client/model/my_sql_additional_config.py
 src/alvin_api_client/model/notification.py
 src/alvin_api_client/model/notification_config.py
 src/alvin_api_client/model/notification_provider.py
 src/alvin_api_client/model/notification_type.py
 src/alvin_api_client/model/onboarding_level.py
 src/alvin_api_client/model/operator_type.py
+src/alvin_api_client/model/organization_create.py
 src/alvin_api_client/model/organization_get.py
 src/alvin_api_client/model/organization_status.py
+src/alvin_api_client/model/organization_update.py
 src/alvin_api_client/model/page_data_entity_get.py
 src/alvin_api_client/model/page_search_display_payload.py
 src/alvin_api_client/model/page_view_get.py
+src/alvin_api_client/model/pipeline_get.py
+src/alvin_api_client/model/pipeline_run_get.py
+src/alvin_api_client/model/pipeline_run_metrics.py
+src/alvin_api_client/model/pipeline_step.py
 src/alvin_api_client/model/platform_asset_type.py
 src/alvin_api_client/model/platform_build_data.py
 src/alvin_api_client/model/platform_build_type.py
 src/alvin_api_client/model/platform_classification.py
 src/alvin_api_client/model/popularity_values.py
 src/alvin_api_client/model/position.py
 src/alvin_api_client/model/postgres_account_details.py
@@ -308,39 +399,45 @@
 src/alvin_api_client/model/query_builder.py
 src/alvin_api_client/model/query_comment.py
 src/alvin_api_client/model/query_create_mode.py
 src/alvin_api_client/model/query_fingerprint.py
 src/alvin_api_client/model/query_lineage_parse_result.py
 src/alvin_api_client/model/query_parse_result.py
 src/alvin_api_client/model/query_type.py
+src/alvin_api_client/model/recommendation_actions.py
 src/alvin_api_client/model/redshift_account_details.py
 src/alvin_api_client/model/redshift_additional_config.py
 src/alvin_api_client/model/rule_element.py
 src/alvin_api_client/model/rule_element_value_type.py
 src/alvin_api_client/model/rule_type.py
 src/alvin_api_client/model/rule_value.py
 src/alvin_api_client/model/save_search_filter.py
 src/alvin_api_client/model/save_search_string_filter.py
 src/alvin_api_client/model/search_csv_column.py
 src/alvin_api_client/model/search_display_payload.py
+src/alvin_api_client/model/search_entities_response.py
+src/alvin_api_client/model/search_entity.py
 src/alvin_api_client/model/search_filter.py
 src/alvin_api_client/model/search_filter_label_association.py
 src/alvin_api_client/model/search_node.py
 src/alvin_api_client/model/search_prefix.py
 src/alvin_api_client/model/search_usage_stat_type.py
 src/alvin_api_client/model/search_v2_response.py
 src/alvin_api_client/model/search_v2_response_payload.py
 src/alvin_api_client/model/search_validation_payload.py
 src/alvin_api_client/model/seen_table_at_level.py
 src/alvin_api_client/model/sheet_settings.py
 src/alvin_api_client/model/snowflake_account_details.py
 src/alvin_api_client/model/snowflake_additional_config.py
+src/alvin_api_client/model/sort_field.py
 src/alvin_api_client/model/sort_order.py
+src/alvin_api_client/model/source_entity_request.py
 src/alvin_api_client/model/sql_table.py
 src/alvin_api_client/model/stat_data_payload.py
+src/alvin_api_client/model/stats_agreggation_data.py
 src/alvin_api_client/model/strings_response.py
 src/alvin_api_client/model/table_alter.py
 src/alvin_api_client/model/table_existence.py
 src/alvin_api_client/model/table_insert.py
 src/alvin_api_client/model/table_merge.py
 src/alvin_api_client/model/table_merge_action.py
 src/alvin_api_client/model/table_merge_match_action_type.py
@@ -356,14 +453,15 @@
 src/alvin_api_client/model/taxonomy_classification_config.py
 src/alvin_api_client/model/tiny_url_response.py
 src/alvin_api_client/model/token.py
 src/alvin_api_client/model/treasure_data_additional_config.py
 src/alvin_api_client/model/treasure_data_credentials.py
 src/alvin_api_client/model/tree_result_classification.py
 src/alvin_api_client/model/truncate_result.py
+src/alvin_api_client/model/usage_context.py
 src/alvin_api_client/model/user_activity_request.py
 src/alvin_api_client/model/user_activity_response.py
 src/alvin_api_client/model/user_activity_type.py
 src/alvin_api_client/model/user_create.py
 src/alvin_api_client/model/user_create_request.py
 src/alvin_api_client/model/user_get.py
 src/alvin_api_client/model/user_invite_create.py
```

### Comparing `alvin_api_client-1.3.0rc2/tests/conftest.py` & `alvin_api_client-1.4.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/tests/integration/test_current_user.py` & `alvin_api_client-1.4.0rc1/tests/integration/test_current_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import configparser
 from pathlib import Path
 
 from alvin_api_client import ApiClient, Configuration
 from alvin_api_client.api.default_api import DefaultApi
+from sqlalchemy import text
+
 from tests.sqlutil import db_engine
 
 config = configparser.ConfigParser()
 home = Path.home()
 config.read(f"{home}/.alvin/alvin.cfg")
 api_token = config.get("ALVIN", "alvin_api_token")
 
@@ -28,26 +30,26 @@
 add_entity = f.read()
 f.close()
 f = open("tests/integration/delete_entity.sql", "r")
 delete_entity = f.read()
 f.close()
 
 with db_engine.connect() as c:
-    c.execute(add_entity)
+    c.execute(text(add_entity))
     try:
         # Test here
         from alvin_api_client.model.data_entity_type import DataEntityType
 
         res = api.get_entity_api_v1_entity_get(
-            platform_id="dvdrental",
-            entity_id="dvdrental.public.film_actor__test",
+            platform_id="bigquery",
+            entity_id="alvinai.analytics_demo_v1_safe.employees_us",
             entity_type=DataEntityType("TABLE"),
             _check_return_type=False,
             _return_http_data_only=True,
         )
         assert res["id"] == "dvdrental.public.film_actor__test"
         assert res["entity_type"] == "TABLE"
         assert res["name"] == "film_actor"
     finally:
-        c.execute(delete_entity)
+        c.execute(text(delete_entity))
 
 # TODO: move other tests elsewhere
```

### Comparing `alvin_api_client-1.3.0rc2/tests/request_model/test_data_entity_usage_stats_request.py` & `alvin_api_client-1.4.0rc1/tests/request_model/test_data_entity_usage_stats_request.py`

 * *Files identical despite different names*

### Comparing `alvin_api_client-1.3.0rc2/tests/test_default_api.py` & `alvin_api_client-1.4.0rc1/tests/test_default_api.py`

 * *Files identical despite different names*

