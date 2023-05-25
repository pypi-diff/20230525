# Comparing `tmp/kensu-datagalaxy-client-1.0.0.tar.gz` & `tmp/kensu-datagalaxy-client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kensu-datagalaxy-client-1.0.0.tar", last modified: Thu May 25 10:55:26 2023, max compression
+gzip compressed data, was "kensu-datagalaxy-client-1.0.1.tar", last modified: Thu May 25 11:11:21 2023, max compression
```

## Comparing `kensu-datagalaxy-client-1.0.0.tar` & `kensu-datagalaxy-client-1.0.1.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 10:55:26.518150 kensu-datagalaxy-client-1.0.0/
--rw-r--r--   0 andy       (501) staff       (20)      242 2023-05-25 10:55:26.517979 kensu-datagalaxy-client-1.0.0/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)    44813 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 10:55:26.436463 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/
--rw-r--r--   0 andy       (501) staff       (20)    23669 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/__init__.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 10:55:26.445260 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/
--rw-r--r--   0 andy       (501) staff       (20)     1466 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    64974 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/attributes_api.py
--rw-r--r--   0 andy       (501) staff       (20)    13435 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/authentication_api.py
--rw-r--r--   0 andy       (501) staff       (20)    24764 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/comments_api.py
--rw-r--r--   0 andy       (501) staff       (20)    48467 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/containers_api.py
--rw-r--r--   0 andy       (501) staff       (20)    44107 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/data_processing_api.py
--rw-r--r--   0 andy       (501) staff       (20)    36544 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/data_processing_item_api.py
--rw-r--r--   0 andy       (501) staff       (20)    48107 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/fields_api.py
--rw-r--r--   0 andy       (501) staff       (20)     9361 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/filtered_views_api.py
--rw-r--r--   0 andy       (501) staff       (20)    61740 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/glossary_api.py
--rw-r--r--   0 andy       (501) staff       (20)    14271 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/history_api.py
--rw-r--r--   0 andy       (501) staff       (20)    16448 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/image_api.py
--rw-r--r--   0 andy       (501) staff       (20)    10370 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/licenses_api.py
--rw-r--r--   0 andy       (501) staff       (20)    29452 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/links_api.py
--rw-r--r--   0 andy       (501) staff       (20)    27503 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/scim_users_api.py
--rw-r--r--   0 andy       (501) staff       (20)    38423 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/screens_api.py
--rw-r--r--   0 andy       (501) staff       (20)    15667 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/search_api.py
--rw-r--r--   0 andy       (501) staff       (20)    79769 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/sources_api.py
--rw-r--r--   0 andy       (501) staff       (20)    48787 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/structures_api.py
--rw-r--r--   0 andy       (501) staff       (20)    29117 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/tasks_api.py
--rw-r--r--   0 andy       (501) staff       (20)    27546 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/teams_api.py
--rw-r--r--   0 andy       (501) staff       (20)    23181 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/technologies_api.py
--rw-r--r--   0 andy       (501) staff       (20)    42895 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/usage_api.py
--rw-r--r--   0 andy       (501) staff       (20)    41516 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/users_api.py
--rw-r--r--   0 andy       (501) staff       (20)    12866 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/workspaces_api.py
--rw-r--r--   0 andy       (501) staff       (20)    29513 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api_client.py
--rw-r--r--   0 andy       (501) staff       (20)    12419 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/configuration.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 10:55:26.516731 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/
--rw-r--r--   0 andy       (501) staff       (20)    22138 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)    19323 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/access_data.py
--rw-r--r--   0 andy       (501) staff       (20)     6984 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/access_type.py
--rw-r--r--   0 andy       (501) staff       (20)     6937 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/additional_custom_attribute.py
--rw-r--r--   0 andy       (501) staff       (20)     6953 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/additional_custom_attribute_bulk.py
--rw-r--r--   0 andy       (501) staff       (20)     8010 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/all_types.py
--rw-r--r--   0 andy       (501) staff       (20)     8030 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/all_types_lower.py
--rw-r--r--   0 andy       (501) staff       (20)     7005 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_bulk_creation_body_default_value.py
--rw-r--r--   0 andy       (501) staff       (20)     6997 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_bulk_update_body_default_value.py
--rw-r--r--   0 andy       (501) staff       (20)     6989 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_creation_body_default_value.py
--rw-r--r--   0 andy       (501) staff       (20)     6941 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_default_value.py
--rw-r--r--   0 andy       (501) staff       (20)     6981 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_update_body_default_value.py
--rw-r--r--   0 andy       (501) staff       (20)     6933 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_category_attribute_id.py
--rw-r--r--   0 andy       (501) staff       (20)     6965 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_category_body_attribute_name_id.py
--rw-r--r--   0 andy       (501) staff       (20)     7017 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_scim_patch_operation_payload_operations_value.py
--rw-r--r--   0 andy       (501) staff       (20)     6929 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_search_filter_values.py
--rw-r--r--   0 andy       (501) staff       (20)     6909 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_tags_body_color.py
--rw-r--r--   0 andy       (501) staff       (20)     7617 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/api_error_model.py
--rw-r--r--   0 andy       (501) staff       (20)     8300 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/api_error_model_error.py
--rw-r--r--   0 andy       (501) staff       (20)    16597 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute.py
--rw-r--r--   0 andy       (501) staff       (20)    14095 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_bulk_creation_body.py
--rw-r--r--   0 andy       (501) staff       (20)    13146 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_bulk_update_body.py
--rw-r--r--   0 andy       (501) staff       (20)    13115 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_creation_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6921 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_data_type_enum.py
--rw-r--r--   0 andy       (501) staff       (20)     7328 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_formats.py
--rw-r--r--   0 andy       (501) staff       (20)     6885 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_key.py
--rw-r--r--   0 andy       (501) staff       (20)     6889 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_name.py
--rw-r--r--   0 andy       (501) staff       (20)    11287 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_update_body.py
--rw-r--r--   0 andy       (501) staff       (20)     8227 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_value.py
--rw-r--r--   0 andy       (501) staff       (20)    10161 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_layout.py
--rw-r--r--   0 andy       (501) staff       (20)     9378 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_response_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6917 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_values_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6921 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_values_body1.py
--rw-r--r--   0 andy       (501) staff       (20)     7844 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/authorizations.py
--rw-r--r--   0 andy       (501) staff       (20)     8689 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/authorizations_authorizations.py
--rw-r--r--   0 andy       (501) staff       (20)     7891 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_delete_response.py
--rw-r--r--   0 andy       (501) staff       (20)     8417 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_input.py
--rw-r--r--   0 andy       (501) staff       (20)     9051 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_links_payload.py
--rw-r--r--   0 andy       (501) staff       (20)    10155 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_links_result.py
--rw-r--r--   0 andy       (501) staff       (20)    10480 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_result.py
--rw-r--r--   0 andy       (501) staff       (20)     7165 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_tree_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)    11464 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/category_attribute_.py
--rw-r--r--   0 andy       (501) staff       (20)     9871 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/category_body_attribute_name_.py
--rw-r--r--   0 andy       (501) staff       (20)     7129 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/child_container.py
--rw-r--r--   0 andy       (501) staff       (20)     7129 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/child_structure.py
--rw-r--r--   0 andy       (501) staff       (20)     7214 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/color.py
--rw-r--r--   0 andy       (501) staff       (20)     7242 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/column_data_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7637 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/comment_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     9345 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/compatibility_definition.py
--rw-r--r--   0 andy       (501) staff       (20)     8308 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/compatible_link.py
--rw-r--r--   0 andy       (501) staff       (20)    13284 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_bulk_creation.py
--rw-r--r--   0 andy       (501) staff       (20)    13214 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_bulk_update.py
--rw-r--r--   0 andy       (501) staff       (20)     7169 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7006 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_type.py
--rw-r--r--   0 andy       (501) staff       (20)    10495 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/create_technology_body.py
--rw-r--r--   0 andy       (501) staff       (20)     7702 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/credentials.py
--rw-r--r--   0 andy       (501) staff       (20)     6913 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/custom_attribute_name.py
--rw-r--r--   0 andy       (501) staff       (20)     7177 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_creation.py
--rw-r--r--   0 andy       (501) staff       (20)    11733 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_response.py
--rw-r--r--   0 andy       (501) staff       (20)    11242 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_response_details.py
--rw-r--r--   0 andy       (501) staff       (20)    11488 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_response_details_data_processing_items.py
--rw-r--r--   0 andy       (501) staff       (20)    16234 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_entity.py
--rw-r--r--   0 andy       (501) staff       (20)     7346 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_item_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7014 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7096 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_types.py
--rw-r--r--   0 andy       (501) staff       (20)     7216 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_types_client_mapping.py
--rw-r--r--   0 andy       (501) staff       (20)     6865 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/date_iso.py
--rw-r--r--   0 andy       (501) staff       (20)    10524 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/default_user.py
--rw-r--r--   0 andy       (501) staff       (20)     6877 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/double_uuid.py
--rw-r--r--   0 andy       (501) staff       (20)     7141 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dp_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7133 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dp_update_request.py
--rw-r--r--   0 andy       (501) staff       (20)    11899 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_bulk_model.py
--rw-r--r--   0 andy       (501) staff       (20)    11776 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_creation_body.py
--rw-r--r--   0 andy       (501) staff       (20)    14435 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_data.py
--rw-r--r--   0 andy       (501) staff       (20)     7448 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_id.py
--rw-r--r--   0 andy       (501) staff       (20)    11023 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_input.py
--rw-r--r--   0 andy       (501) staff       (20)    13363 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_update_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6857 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/email.py
--rw-r--r--   0 andy       (501) staff       (20)    14900 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity.py
--rw-r--r--   0 andy       (501) staff       (20)     7137 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_attributes.py
--rw-r--r--   0 andy       (501) staff       (20)    10656 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_base.py
--rw-r--r--   0 andy       (501) staff       (20)    11438 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_descriptor.py
--rw-r--r--   0 andy       (501) staff       (20)     8290 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_location.py
--rw-r--r--   0 andy       (501) staff       (20)    20227 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_search_result.py
--rw-r--r--   0 andy       (501) staff       (20)     7070 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_status.py
--rw-r--r--   0 andy       (501) staff       (20)    18668 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_summary.py
--rw-r--r--   0 andy       (501) staff       (20)     8388 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/exact_match.py
--rw-r--r--   0 andy       (501) staff       (20)     7502 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/exclude_typeof_attribute_data_type_enum_at_keyoftypeof_attribute_data_type_enum_typeof_data_type_enum_dataprocessingitem_.py
--rw-r--r--   0 andy       (501) staff       (20)    13205 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/field_bulk_creation.py
--rw-r--r--   0 andy       (501) staff       (20)    13032 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/field_bulk_update.py
--rw-r--r--   0 andy       (501) staff       (20)     6956 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/field_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/fields_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7149 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/fields_update_request.py
--rw-r--r--   0 andy       (501) staff       (20)    15069 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/filtered_view.py
--rw-r--r--   0 andy       (501) staff       (20)     9898 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/filtered_view_summary.py
--rw-r--r--   0 andy       (501) staff       (20)     8343 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/fk_column.py
--rw-r--r--   0 andy       (501) staff       (20)    12738 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/foreign_key.py
--rw-r--r--   0 andy       (501) staff       (20)    13881 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/foreign_key_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     8727 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/get_technologies_result.py
--rw-r--r--   0 andy       (501) staff       (20)    10755 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/governance_users.py
--rw-r--r--   0 andy       (501) staff       (20)     8146 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/hyper_link.py
--rw-r--r--   0 andy       (501) staff       (20)    11538 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/i_attributes.py
--rw-r--r--   0 andy       (501) staff       (20)     6857 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/i_date.py
--rw-r--r--   0 andy       (501) staff       (20)    11100 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6873 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_hash.py
--rw-r--r--   0 andy       (501) staff       (20)     6889 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_mime_type.py
--rw-r--r--   0 andy       (501) staff       (20)     8388 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_result.py
--rw-r--r--   0 andy       (501) staff       (20)     7742 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_upload_response.py
--rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/include_access_data.py
--rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/include_attributes.py
--rw-r--r--   0 andy       (501) staff       (20)     6885 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/include_links.py
--rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/inline_response200.py
--rw-r--r--   0 andy       (501) staff       (20)    10663 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/inline_response201.py
--rw-r--r--   0 andy       (501) staff       (20)     8007 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/integration_token_regeneration_response.py
--rw-r--r--   0 andy       (501) staff       (20)    15828 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license.py
--rw-r--r--   0 andy       (501) staff       (20)     6979 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license_level.py
--rw-r--r--   0 andy       (501) staff       (20)    10642 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license_list.py
--rw-r--r--   0 andy       (501) staff       (20)     9107 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license_report.py
--rw-r--r--   0 andy       (501) staff       (20)     7129 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/linked_entities.py
--rw-r--r--   0 andy       (501) staff       (20)    11340 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/linked_entity.py
--rw-r--r--   0 andy       (501) staff       (20)    10202 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/links.py
--rw-r--r--   0 andy       (501) staff       (20)    10811 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/links_bulktree_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     8340 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/links_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     8878 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/local_synonym.py
--rw-r--r--   0 andy       (501) staff       (20)     8404 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/local_synonym_creation_body.py
--rw-r--r--   0 andy       (501) staff       (20)     8297 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/local_synonym_update_body.py
--rw-r--r--   0 andy       (501) staff       (20)     8046 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/lower_case_all_types.py
--rw-r--r--   0 andy       (501) staff       (20)     8441 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/mapping_path.py
--rw-r--r--   0 andy       (501) staff       (20)     6869 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/max_depth.py
--rw-r--r--   0 andy       (501) staff       (20)     7008 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module.py
--rw-r--r--   0 andy       (501) staff       (20)    10593 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_authorizations.py
--rw-r--r--   0 andy       (501) staff       (20)     9471 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_authorizations_update.py
--rw-r--r--   0 andy       (501) staff       (20)     7126 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_names.py
--rw-r--r--   0 andy       (501) staff       (20)     6992 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_role.py
--rw-r--r--   0 andy       (501) staff       (20)     6909 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/object_history_entry.py
--rw-r--r--   0 andy       (501) staff       (20)     6893 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/object_location.py
--rw-r--r--   0 andy       (501) staff       (20)     8726 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/objects_history_result.py
--rw-r--r--   0 andy       (501) staff       (20)     7085 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/omit_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
--rw-r--r--   0 andy       (501) staff       (20)     7045 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/omit_search_body_included_attributes_or_include_access_data_.py
--rw-r--r--   0 andy       (501) staff       (20)     6977 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/omit_team_id_or_icon_hash_or_members_count_.py
--rw-r--r--   0 andy       (501) staff       (20)    11775 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_attributes_response_body_.py
--rw-r--r--   0 andy       (501) staff       (20)    11370 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_dpi_data_.py
--rw-r--r--   0 andy       (501) staff       (20)    11646 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_entity_summary_.py
--rw-r--r--   0 andy       (501) staff       (20)    11613 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_tags_response_body_.py
--rw-r--r--   0 andy       (501) staff       (20)    11289 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_user_.py
--rw-r--r--   0 andy       (501) staff       (20)    11667 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_user_authorizations_.py
--rw-r--r--   0 andy       (501) staff       (20)    11370 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_version_.py
--rw-r--r--   0 andy       (501) staff       (20)    11695 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/partial_team_creation_payload_.py
--rw-r--r--   0 andy       (501) staff       (20)    19173 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_entity_summary_exclude_keyof_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
--rw-r--r--   0 andy       (501) staff       (20)    20134 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_entity_summary_exclude_keyof_entity_summary_links_.py
--rw-r--r--   0 andy       (501) staff       (20)    12780 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_search_body_exclude_keyof_search_body_included_attributes_or_include_access_data_.py
--rw-r--r--   0 andy       (501) staff       (20)    12620 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_team_exclude_keyof_team_id_or_icon_hash_or_members_count_.py
--rw-r--r--   0 andy       (501) staff       (20)     9076 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pk_column.py
--rw-r--r--   0 andy       (501) staff       (20)    10744 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/primary_key.py
--rw-r--r--   0 andy       (501) staff       (20)    10045 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/primary_key_payload.py
--rw-r--r--   0 andy       (501) staff       (20)    14411 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/properties_bulk_tree_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7165 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/property_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7310 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/property_type.py
--rw-r--r--   0 andy       (501) staff       (20)     8840 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/queries_history_result.py
--rw-r--r--   0 andy       (501) staff       (20)     8385 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/quick_filter.py
--rw-r--r--   0 andy       (501) staff       (20)     9099 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/reference_object.py
--rw-r--r--   0 andy       (501) staff       (20)     8488 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/reference_parents.py
--rw-r--r--   0 andy       (501) staff       (20)     6869 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/rich_text.py
--rw-r--r--   0 andy       (501) staff       (20)     7014 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/roles.py
--rw-r--r--   0 andy       (501) staff       (20)     9022 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/saved_query.py
--rw-r--r--   0 andy       (501) staff       (20)    10263 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_error.py
--rw-r--r--   0 andy       (501) staff       (20)    11148 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_list_response_user_.py
--rw-r--r--   0 andy       (501) staff       (20)     8972 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_patch_operation_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     9336 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_patch_operation_payload_operations.py
--rw-r--r--   0 andy       (501) staff       (20)    12411 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user.py
--rw-r--r--   0 andy       (501) staff       (20)     8254 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_emails.py
--rw-r--r--   0 andy       (501) staff       (20)     7926 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_meta.py
--rw-r--r--   0 andy       (501) staff       (20)     9239 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_name.py
--rw-r--r--   0 andy       (501) staff       (20)     8248 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_photos.py
--rw-r--r--   0 andy       (501) staff       (20)     7166 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/screen_data_types.py
--rw-r--r--   0 andy       (501) staff       (20)    13714 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_body.py
--rw-r--r--   0 andy       (501) staff       (20)    10156 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_filter.py
--rw-r--r--   0 andy       (501) staff       (20)     7814 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_filter_operator.py
--rw-r--r--   0 andy       (501) staff       (20)     6881 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_query.py
--rw-r--r--   0 andy       (501) staff       (20)    10430 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_response.py
--rw-r--r--   0 andy       (501) staff       (20)     8721 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_response_result.py
--rw-r--r--   0 andy       (501) staff       (20)    12057 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/social_comment.py
--rw-r--r--   0 andy       (501) staff       (20)    13155 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_bulk_creation.py
--rw-r--r--   0 andy       (501) staff       (20)    13085 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_bulk_update.py
--rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7028 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7149 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_update_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_bulk_creation.py
--rw-r--r--   0 andy       (501) staff       (20)    13204 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_bulk_update.py
--rw-r--r--   0 andy       (501) staff       (20)     7169 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7062 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7161 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_update_request.py
--rw-r--r--   0 andy       (501) staff       (20)    11880 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/system_attribute.py
--rw-r--r--   0 andy       (501) staff       (20)    11182 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/tags_body.py
--rw-r--r--   0 andy       (501) staff       (20)    12421 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/tags_response_body.py
--rw-r--r--   0 andy       (501) staff       (20)    12771 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task.py
--rw-r--r--   0 andy       (501) staff       (20)    11845 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_creation_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     7026 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_status.py
--rw-r--r--   0 andy       (501) staff       (20)     7212 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_type.py
--rw-r--r--   0 andy       (501) staff       (20)    11444 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_update_payload.py
--rw-r--r--   0 andy       (501) staff       (20)    13989 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team.py
--rw-r--r--   0 andy       (501) staff       (20)     6913 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_creation_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     6861 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_id.py
--rw-r--r--   0 andy       (501) staff       (20)     8221 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_member.py
--rw-r--r--   0 andy       (501) staff       (20)     6952 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_role.py
--rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_update_payload.py
--rw-r--r--   0 andy       (501) staff       (20)     8477 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/teams_result.py
--rw-r--r--   0 andy       (501) staff       (20)    18948 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/technology.py
--rw-r--r--   0 andy       (501) staff       (20)     7016 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/technology_module.py
--rw-r--r--   0 andy       (501) staff       (20)     7048 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_color_rule.py
--rw-r--r--   0 andy       (501) staff       (20)     8292 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_entry.py
--rw-r--r--   0 andy       (501) staff       (20)     7020 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_frequency.py
--rw-r--r--   0 andy       (501) staff       (20)     6897 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_value.py
--rw-r--r--   0 andy       (501) staff       (20)     7125 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/update_request.py
--rw-r--r--   0 andy       (501) staff       (20)     9158 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/update_technology_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6849 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/url.py
--rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_bulktree_creation.py
--rw-r--r--   0 andy       (501) staff       (20)     7153 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_creation_request.py
--rw-r--r--   0 andy       (501) staff       (20)     7238 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_type.py
--rw-r--r--   0 andy       (501) staff       (20)     7145 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_update_request.py
--rw-r--r--   0 andy       (501) staff       (20)    13656 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user.py
--rw-r--r--   0 andy       (501) staff       (20)     8175 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_authorizations.py
--rw-r--r--   0 andy       (501) staff       (20)    11720 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_creation_body.py
--rw-r--r--   0 andy       (501) staff       (20)     8715 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_update_authorizations.py
--rw-r--r--   0 andy       (501) staff       (20)     8605 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_update_authorizations_definition.py
--rw-r--r--   0 andy       (501) staff       (20)    12121 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_update_body.py
--rw-r--r--   0 andy       (501) staff       (20)     8652 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/users_update_authorizations_body.py
--rw-r--r--   0 andy       (501) staff       (20)     6853 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/uuid.py
--rw-r--r--   0 andy       (501) staff       (20)    12119 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/version.py
--rw-r--r--   0 andy       (501) staff       (20)     6873 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/version_id.py
--rw-r--r--   0 andy       (501) staff       (20)    16109 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/workspace.py
--rw-r--r--   0 andy       (501) staff       (20)     7034 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/workspace_authorization.py
--rw-r--r--   0 andy       (501) staff       (20)     8524 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/workspaces.py
--rw-r--r--   0 andy       (501) staff       (20)    17465 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/rest.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 10:55:26.517707 kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)      242 2023-05-25 10:55:26.000000 kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)    14410 2023-05-25 10:55:26.000000 kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2023-05-25 10:55:26.000000 kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       48 2023-05-25 10:55:26.000000 kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       24 2023-05-25 10:55:26.000000 kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       38 2023-05-25 10:55:26.518191 kensu-datagalaxy-client-1.0.0/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     5414 2023-05-25 10:55:17.000000 kensu-datagalaxy-client-1.0.0/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 11:11:21.938860 kensu-datagalaxy-client-1.0.1/
+-rw-r--r--   0 andy       (501) staff       (20)      242 2023-05-25 11:11:21.938666 kensu-datagalaxy-client-1.0.1/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)    44813 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 11:11:21.830924 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/
+-rw-r--r--   0 andy       (501) staff       (20)    23669 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/__init__.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 11:11:21.840545 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/
+-rw-r--r--   0 andy       (501) staff       (20)     1466 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    64974 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/attributes_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    13435 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/authentication_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    24764 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/comments_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    48467 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/containers_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    44107 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/data_processing_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    36544 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/data_processing_item_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    48107 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/fields_api.py
+-rw-r--r--   0 andy       (501) staff       (20)     9361 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/filtered_views_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    61740 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/glossary_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    14271 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/history_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    16448 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/image_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    10370 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/licenses_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    29452 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/links_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    27503 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/scim_users_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    38423 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/screens_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    15667 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/search_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    79769 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/sources_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    48787 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/structures_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    29117 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/tasks_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    27546 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/teams_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    23181 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/technologies_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    42895 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/usage_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    41516 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/users_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    12866 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/workspaces_api.py
+-rw-r--r--   0 andy       (501) staff       (20)    29513 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api_client.py
+-rw-r--r--   0 andy       (501) staff       (20)    12419 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/configuration.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 11:11:21.938388 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/
+-rw-r--r--   0 andy       (501) staff       (20)    22138 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    19323 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/access_data.py
+-rw-r--r--   0 andy       (501) staff       (20)     6984 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/access_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     6937 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/additional_custom_attribute.py
+-rw-r--r--   0 andy       (501) staff       (20)     6953 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/additional_custom_attribute_bulk.py
+-rw-r--r--   0 andy       (501) staff       (20)     8010 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/all_types.py
+-rw-r--r--   0 andy       (501) staff       (20)     8030 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/all_types_lower.py
+-rw-r--r--   0 andy       (501) staff       (20)     7005 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_bulk_creation_body_default_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     6997 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_bulk_update_body_default_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     6989 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_creation_body_default_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     6941 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_default_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     6981 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_update_body_default_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     6933 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_category_attribute_id.py
+-rw-r--r--   0 andy       (501) staff       (20)     6965 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_category_body_attribute_name_id.py
+-rw-r--r--   0 andy       (501) staff       (20)     7017 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_scim_patch_operation_payload_operations_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     6929 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_search_filter_values.py
+-rw-r--r--   0 andy       (501) staff       (20)     6909 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_tags_body_color.py
+-rw-r--r--   0 andy       (501) staff       (20)     7617 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/api_error_model.py
+-rw-r--r--   0 andy       (501) staff       (20)     8300 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/api_error_model_error.py
+-rw-r--r--   0 andy       (501) staff       (20)    16597 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute.py
+-rw-r--r--   0 andy       (501) staff       (20)    14095 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_bulk_creation_body.py
+-rw-r--r--   0 andy       (501) staff       (20)    13146 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_bulk_update_body.py
+-rw-r--r--   0 andy       (501) staff       (20)    13115 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_creation_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6921 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_data_type_enum.py
+-rw-r--r--   0 andy       (501) staff       (20)     7328 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_formats.py
+-rw-r--r--   0 andy       (501) staff       (20)     6885 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_key.py
+-rw-r--r--   0 andy       (501) staff       (20)     6889 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_name.py
+-rw-r--r--   0 andy       (501) staff       (20)    11287 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_update_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     8227 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_value.py
+-rw-r--r--   0 andy       (501) staff       (20)    10161 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_layout.py
+-rw-r--r--   0 andy       (501) staff       (20)     9378 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_response_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6917 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_values_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6921 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_values_body1.py
+-rw-r--r--   0 andy       (501) staff       (20)     7844 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/authorizations.py
+-rw-r--r--   0 andy       (501) staff       (20)     8689 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/authorizations_authorizations.py
+-rw-r--r--   0 andy       (501) staff       (20)     7891 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_delete_response.py
+-rw-r--r--   0 andy       (501) staff       (20)     8417 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_input.py
+-rw-r--r--   0 andy       (501) staff       (20)     9051 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_links_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)    10155 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_links_result.py
+-rw-r--r--   0 andy       (501) staff       (20)    10480 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_result.py
+-rw-r--r--   0 andy       (501) staff       (20)     7165 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_tree_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)    11464 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/category_attribute_.py
+-rw-r--r--   0 andy       (501) staff       (20)     9871 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/category_body_attribute_name_.py
+-rw-r--r--   0 andy       (501) staff       (20)     7129 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/child_container.py
+-rw-r--r--   0 andy       (501) staff       (20)     7129 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/child_structure.py
+-rw-r--r--   0 andy       (501) staff       (20)     7214 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/color.py
+-rw-r--r--   0 andy       (501) staff       (20)     7242 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/column_data_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7637 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/comment_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     9345 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/compatibility_definition.py
+-rw-r--r--   0 andy       (501) staff       (20)     8308 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/compatible_link.py
+-rw-r--r--   0 andy       (501) staff       (20)    13284 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_bulk_creation.py
+-rw-r--r--   0 andy       (501) staff       (20)    13214 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_bulk_update.py
+-rw-r--r--   0 andy       (501) staff       (20)     7169 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7006 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_type.py
+-rw-r--r--   0 andy       (501) staff       (20)    10495 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/create_technology_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     7702 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/credentials.py
+-rw-r--r--   0 andy       (501) staff       (20)     6913 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/custom_attribute_name.py
+-rw-r--r--   0 andy       (501) staff       (20)     7177 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_creation.py
+-rw-r--r--   0 andy       (501) staff       (20)    11733 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_response.py
+-rw-r--r--   0 andy       (501) staff       (20)    11242 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_response_details.py
+-rw-r--r--   0 andy       (501) staff       (20)    11488 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_response_details_data_processing_items.py
+-rw-r--r--   0 andy       (501) staff       (20)    16234 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_entity.py
+-rw-r--r--   0 andy       (501) staff       (20)     7346 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_item_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7014 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7096 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_types.py
+-rw-r--r--   0 andy       (501) staff       (20)     7216 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_types_client_mapping.py
+-rw-r--r--   0 andy       (501) staff       (20)     6865 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/date_iso.py
+-rw-r--r--   0 andy       (501) staff       (20)    10524 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/default_user.py
+-rw-r--r--   0 andy       (501) staff       (20)     6877 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/double_uuid.py
+-rw-r--r--   0 andy       (501) staff       (20)     7141 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dp_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7133 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dp_update_request.py
+-rw-r--r--   0 andy       (501) staff       (20)    11899 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_bulk_model.py
+-rw-r--r--   0 andy       (501) staff       (20)    11776 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_creation_body.py
+-rw-r--r--   0 andy       (501) staff       (20)    14435 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_data.py
+-rw-r--r--   0 andy       (501) staff       (20)     7448 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_id.py
+-rw-r--r--   0 andy       (501) staff       (20)    11023 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_input.py
+-rw-r--r--   0 andy       (501) staff       (20)    13363 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_update_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6857 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/email.py
+-rw-r--r--   0 andy       (501) staff       (20)    14900 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity.py
+-rw-r--r--   0 andy       (501) staff       (20)     7137 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_attributes.py
+-rw-r--r--   0 andy       (501) staff       (20)    10656 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_base.py
+-rw-r--r--   0 andy       (501) staff       (20)    11438 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_descriptor.py
+-rw-r--r--   0 andy       (501) staff       (20)     8290 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_location.py
+-rw-r--r--   0 andy       (501) staff       (20)    20227 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_search_result.py
+-rw-r--r--   0 andy       (501) staff       (20)     7070 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_status.py
+-rw-r--r--   0 andy       (501) staff       (20)    18668 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_summary.py
+-rw-r--r--   0 andy       (501) staff       (20)     8388 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/exact_match.py
+-rw-r--r--   0 andy       (501) staff       (20)     7502 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/exclude_typeof_attribute_data_type_enum_at_keyoftypeof_attribute_data_type_enum_typeof_data_type_enum_dataprocessingitem_.py
+-rw-r--r--   0 andy       (501) staff       (20)    13205 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/field_bulk_creation.py
+-rw-r--r--   0 andy       (501) staff       (20)    13032 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/field_bulk_update.py
+-rw-r--r--   0 andy       (501) staff       (20)     6956 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/field_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/fields_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7149 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/fields_update_request.py
+-rw-r--r--   0 andy       (501) staff       (20)    15069 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/filtered_view.py
+-rw-r--r--   0 andy       (501) staff       (20)     9898 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/filtered_view_summary.py
+-rw-r--r--   0 andy       (501) staff       (20)     8343 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/fk_column.py
+-rw-r--r--   0 andy       (501) staff       (20)    12738 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/foreign_key.py
+-rw-r--r--   0 andy       (501) staff       (20)    13881 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/foreign_key_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     8727 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/get_technologies_result.py
+-rw-r--r--   0 andy       (501) staff       (20)    10755 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/governance_users.py
+-rw-r--r--   0 andy       (501) staff       (20)     8146 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/hyper_link.py
+-rw-r--r--   0 andy       (501) staff       (20)    11538 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/i_attributes.py
+-rw-r--r--   0 andy       (501) staff       (20)     6857 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/i_date.py
+-rw-r--r--   0 andy       (501) staff       (20)    11100 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6873 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_hash.py
+-rw-r--r--   0 andy       (501) staff       (20)     6889 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_mime_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     8388 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_result.py
+-rw-r--r--   0 andy       (501) staff       (20)     7742 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_upload_response.py
+-rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/include_access_data.py
+-rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/include_attributes.py
+-rw-r--r--   0 andy       (501) staff       (20)     6885 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/include_links.py
+-rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/inline_response200.py
+-rw-r--r--   0 andy       (501) staff       (20)    10663 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/inline_response201.py
+-rw-r--r--   0 andy       (501) staff       (20)     8007 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/integration_token_regeneration_response.py
+-rw-r--r--   0 andy       (501) staff       (20)    15828 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license.py
+-rw-r--r--   0 andy       (501) staff       (20)     6979 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license_level.py
+-rw-r--r--   0 andy       (501) staff       (20)    10642 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license_list.py
+-rw-r--r--   0 andy       (501) staff       (20)     9107 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license_report.py
+-rw-r--r--   0 andy       (501) staff       (20)     7129 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/linked_entities.py
+-rw-r--r--   0 andy       (501) staff       (20)    11340 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/linked_entity.py
+-rw-r--r--   0 andy       (501) staff       (20)    10202 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/links.py
+-rw-r--r--   0 andy       (501) staff       (20)    10811 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/links_bulktree_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     8340 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/links_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     8878 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/local_synonym.py
+-rw-r--r--   0 andy       (501) staff       (20)     8404 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/local_synonym_creation_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     8297 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/local_synonym_update_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     8046 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/lower_case_all_types.py
+-rw-r--r--   0 andy       (501) staff       (20)     8441 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/mapping_path.py
+-rw-r--r--   0 andy       (501) staff       (20)     6869 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/max_depth.py
+-rw-r--r--   0 andy       (501) staff       (20)     7008 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module.py
+-rw-r--r--   0 andy       (501) staff       (20)    10593 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_authorizations.py
+-rw-r--r--   0 andy       (501) staff       (20)     9471 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_authorizations_update.py
+-rw-r--r--   0 andy       (501) staff       (20)     7126 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_names.py
+-rw-r--r--   0 andy       (501) staff       (20)     6992 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_role.py
+-rw-r--r--   0 andy       (501) staff       (20)     6909 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/object_history_entry.py
+-rw-r--r--   0 andy       (501) staff       (20)     6893 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/object_location.py
+-rw-r--r--   0 andy       (501) staff       (20)     8726 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/objects_history_result.py
+-rw-r--r--   0 andy       (501) staff       (20)     7085 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/omit_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
+-rw-r--r--   0 andy       (501) staff       (20)     7045 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/omit_search_body_included_attributes_or_include_access_data_.py
+-rw-r--r--   0 andy       (501) staff       (20)     6977 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/omit_team_id_or_icon_hash_or_members_count_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11775 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_attributes_response_body_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11370 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_dpi_data_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11646 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_entity_summary_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11613 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_tags_response_body_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11289 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_user_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11667 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_user_authorizations_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11370 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_version_.py
+-rw-r--r--   0 andy       (501) staff       (20)    11695 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/partial_team_creation_payload_.py
+-rw-r--r--   0 andy       (501) staff       (20)    19173 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_entity_summary_exclude_keyof_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
+-rw-r--r--   0 andy       (501) staff       (20)    20134 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_entity_summary_exclude_keyof_entity_summary_links_.py
+-rw-r--r--   0 andy       (501) staff       (20)    12780 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_search_body_exclude_keyof_search_body_included_attributes_or_include_access_data_.py
+-rw-r--r--   0 andy       (501) staff       (20)    12620 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_team_exclude_keyof_team_id_or_icon_hash_or_members_count_.py
+-rw-r--r--   0 andy       (501) staff       (20)     9076 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pk_column.py
+-rw-r--r--   0 andy       (501) staff       (20)    10744 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/primary_key.py
+-rw-r--r--   0 andy       (501) staff       (20)    10045 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/primary_key_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)    14411 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/properties_bulk_tree_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7165 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/property_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7310 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/property_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     8840 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/queries_history_result.py
+-rw-r--r--   0 andy       (501) staff       (20)     8385 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/quick_filter.py
+-rw-r--r--   0 andy       (501) staff       (20)     9099 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/reference_object.py
+-rw-r--r--   0 andy       (501) staff       (20)     8488 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/reference_parents.py
+-rw-r--r--   0 andy       (501) staff       (20)     6869 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/rich_text.py
+-rw-r--r--   0 andy       (501) staff       (20)     7014 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/roles.py
+-rw-r--r--   0 andy       (501) staff       (20)     9022 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/saved_query.py
+-rw-r--r--   0 andy       (501) staff       (20)    10263 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_error.py
+-rw-r--r--   0 andy       (501) staff       (20)    11148 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_list_response_user_.py
+-rw-r--r--   0 andy       (501) staff       (20)     8972 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_patch_operation_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     9336 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_patch_operation_payload_operations.py
+-rw-r--r--   0 andy       (501) staff       (20)    12411 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user.py
+-rw-r--r--   0 andy       (501) staff       (20)     8254 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_emails.py
+-rw-r--r--   0 andy       (501) staff       (20)     7926 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_meta.py
+-rw-r--r--   0 andy       (501) staff       (20)     9239 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_name.py
+-rw-r--r--   0 andy       (501) staff       (20)     8248 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_photos.py
+-rw-r--r--   0 andy       (501) staff       (20)     7166 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/screen_data_types.py
+-rw-r--r--   0 andy       (501) staff       (20)    13714 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_body.py
+-rw-r--r--   0 andy       (501) staff       (20)    10156 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_filter.py
+-rw-r--r--   0 andy       (501) staff       (20)     7814 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_filter_operator.py
+-rw-r--r--   0 andy       (501) staff       (20)     6881 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_query.py
+-rw-r--r--   0 andy       (501) staff       (20)    10430 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_response.py
+-rw-r--r--   0 andy       (501) staff       (20)     8721 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_response_result.py
+-rw-r--r--   0 andy       (501) staff       (20)    12057 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/social_comment.py
+-rw-r--r--   0 andy       (501) staff       (20)    13155 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_bulk_creation.py
+-rw-r--r--   0 andy       (501) staff       (20)    13085 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_bulk_update.py
+-rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7028 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7149 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_update_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_bulk_creation.py
+-rw-r--r--   0 andy       (501) staff       (20)    13204 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_bulk_update.py
+-rw-r--r--   0 andy       (501) staff       (20)     7169 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7062 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7161 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_update_request.py
+-rw-r--r--   0 andy       (501) staff       (20)    11880 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/system_attribute.py
+-rw-r--r--   0 andy       (501) staff       (20)    11182 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/tags_body.py
+-rw-r--r--   0 andy       (501) staff       (20)    12421 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/tags_response_body.py
+-rw-r--r--   0 andy       (501) staff       (20)    12771 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task.py
+-rw-r--r--   0 andy       (501) staff       (20)    11845 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_creation_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     7026 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_status.py
+-rw-r--r--   0 andy       (501) staff       (20)     7212 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_type.py
+-rw-r--r--   0 andy       (501) staff       (20)    11444 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_update_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)    13989 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team.py
+-rw-r--r--   0 andy       (501) staff       (20)     6913 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_creation_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     6861 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_id.py
+-rw-r--r--   0 andy       (501) staff       (20)     8221 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_member.py
+-rw-r--r--   0 andy       (501) staff       (20)     6952 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_role.py
+-rw-r--r--   0 andy       (501) staff       (20)     6905 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_update_payload.py
+-rw-r--r--   0 andy       (501) staff       (20)     8477 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/teams_result.py
+-rw-r--r--   0 andy       (501) staff       (20)    18948 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/technology.py
+-rw-r--r--   0 andy       (501) staff       (20)     7016 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/technology_module.py
+-rw-r--r--   0 andy       (501) staff       (20)     7048 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_color_rule.py
+-rw-r--r--   0 andy       (501) staff       (20)     8292 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_entry.py
+-rw-r--r--   0 andy       (501) staff       (20)     7020 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_frequency.py
+-rw-r--r--   0 andy       (501) staff       (20)     6897 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_value.py
+-rw-r--r--   0 andy       (501) staff       (20)     7125 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/update_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     9158 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/update_technology_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6849 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/url.py
+-rw-r--r--   0 andy       (501) staff       (20)     7157 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_bulktree_creation.py
+-rw-r--r--   0 andy       (501) staff       (20)     7153 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_creation_request.py
+-rw-r--r--   0 andy       (501) staff       (20)     7238 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_type.py
+-rw-r--r--   0 andy       (501) staff       (20)     7145 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_update_request.py
+-rw-r--r--   0 andy       (501) staff       (20)    13656 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user.py
+-rw-r--r--   0 andy       (501) staff       (20)     8175 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_authorizations.py
+-rw-r--r--   0 andy       (501) staff       (20)    11720 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_creation_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     8715 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_update_authorizations.py
+-rw-r--r--   0 andy       (501) staff       (20)     8605 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_update_authorizations_definition.py
+-rw-r--r--   0 andy       (501) staff       (20)    12121 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_update_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     8652 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/users_update_authorizations_body.py
+-rw-r--r--   0 andy       (501) staff       (20)     6853 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/uuid.py
+-rw-r--r--   0 andy       (501) staff       (20)    12119 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/version.py
+-rw-r--r--   0 andy       (501) staff       (20)     6873 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/version_id.py
+-rw-r--r--   0 andy       (501) staff       (20)    16109 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/workspace.py
+-rw-r--r--   0 andy       (501) staff       (20)     7034 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/workspace_authorization.py
+-rw-r--r--   0 andy       (501) staff       (20)     8524 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/workspaces.py
+-rw-r--r--   0 andy       (501) staff       (20)    17465 2023-05-25 10:39:39.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/rest.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2023-05-25 11:11:21.832831 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)      242 2023-05-25 11:11:21.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)    14410 2023-05-25 11:11:21.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2023-05-25 11:11:21.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       48 2023-05-25 11:11:21.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       24 2023-05-25 11:11:21.000000 kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       38 2023-05-25 11:11:21.938910 kensu-datagalaxy-client-1.0.1/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     5414 2023-05-25 11:10:40.000000 kensu-datagalaxy-client-1.0.1/setup.py
```

### Comparing `kensu-datagalaxy-client-1.0.0/README.md` & `kensu-datagalaxy-client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/__init__.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/__init__.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/attributes_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/attributes_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/authentication_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/comments_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/comments_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/containers_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/containers_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/data_processing_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/data_processing_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/data_processing_item_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/data_processing_item_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/fields_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/fields_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/filtered_views_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/filtered_views_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/glossary_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/glossary_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/history_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/history_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/image_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/image_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/licenses_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/licenses_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/links_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/links_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/scim_users_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/scim_users_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/screens_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/screens_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/search_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/sources_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/structures_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/structures_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/tasks_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/teams_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/technologies_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/technologies_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/usage_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/usage_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/users_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/users_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api/workspaces_api.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/api_client.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/api_client.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/configuration.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/configuration.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/__init__.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/access_data.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/access_data.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/access_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/access_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/additional_custom_attribute.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/additional_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/additional_custom_attribute_bulk.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/additional_custom_attribute_bulk.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/all_types.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/all_types.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/all_types_lower.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/all_types_lower.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_bulk_creation_body_default_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_bulk_creation_body_default_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_bulk_update_body_default_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_bulk_update_body_default_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_creation_body_default_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_creation_body_default_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_default_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_default_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_attribute_update_body_default_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_attribute_update_body_default_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_category_attribute_id.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_category_attribute_id.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_category_body_attribute_name_id.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_category_body_attribute_name_id.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_scim_patch_operation_payload_operations_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_scim_patch_operation_payload_operations_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_search_filter_values.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_search_filter_values.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/any_of_tags_body_color.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/any_of_tags_body_color.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/api_error_model.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/api_error_model.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/api_error_model_error.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/api_error_model_error.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_bulk_creation_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_bulk_creation_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_bulk_update_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_bulk_update_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_creation_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_creation_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_data_type_enum.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_data_type_enum.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_formats.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_formats.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_key.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_key.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_name.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_name.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_update_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_update_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attribute_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attribute_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_layout.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_layout.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_response_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_response_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_values_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_values_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/attributes_values_body1.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/attributes_values_body1.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/authorizations.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/authorizations.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/authorizations_authorizations.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/authorizations_authorizations.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_delete_response.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_delete_response.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_input.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_input.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_links_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_links_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_links_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_links_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/bulk_tree_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/bulk_tree_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/category_attribute_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/category_attribute_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/category_body_attribute_name_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/category_body_attribute_name_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/child_container.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/child_container.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/child_structure.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/child_structure.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/color.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/color.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/column_data_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/column_data_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/comment_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/comment_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/compatibility_definition.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/compatibility_definition.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/compatible_link.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/compatible_link.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_bulk_creation.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_bulk_update.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_bulk_update.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/container_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/container_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/create_technology_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/create_technology_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/credentials.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/credentials.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/custom_attribute_name.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/custom_attribute_name.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_creation.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_response.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_response.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_response_details.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_response_details.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_bulk_response_details_data_processing_items.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_bulk_response_details_data_processing_items.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_entity.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_entity.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_item_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_item_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_processing_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_processing_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_types.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_types.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/data_types_client_mapping.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/data_types_client_mapping.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/date_iso.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/date_iso.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/default_user.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/default_user.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/double_uuid.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/double_uuid.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dp_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dp_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dp_update_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dp_update_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_bulk_model.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_bulk_model.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_creation_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_creation_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_data.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_data.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_id.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_id.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_input.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_input.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/dpi_update_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/dpi_update_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/email.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/email.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_attributes.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_attributes.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_base.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_base.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_descriptor.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_descriptor.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_location.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_location.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_search_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_search_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_status.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_status.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/entity_summary.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/entity_summary.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/exact_match.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/exact_match.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/exclude_typeof_attribute_data_type_enum_at_keyoftypeof_attribute_data_type_enum_typeof_data_type_enum_dataprocessingitem_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/exclude_typeof_attribute_data_type_enum_at_keyoftypeof_attribute_data_type_enum_typeof_data_type_enum_dataprocessingitem_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/field_bulk_creation.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/field_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/field_bulk_update.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/field_bulk_update.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/field_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/field_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/fields_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/fields_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/fields_update_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/fields_update_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/filtered_view.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/filtered_view.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/filtered_view_summary.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/filtered_view_summary.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/fk_column.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/fk_column.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/foreign_key.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/foreign_key.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/foreign_key_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/foreign_key_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/get_technologies_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/get_technologies_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/governance_users.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/governance_users.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/hyper_link.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/hyper_link.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/i_attributes.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/i_attributes.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/i_date.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/i_date.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_hash.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_hash.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_mime_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_mime_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/image_upload_response.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/image_upload_response.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/include_access_data.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/include_access_data.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/include_attributes.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/include_attributes.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/include_links.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/include_links.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/inline_response200.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/inline_response201.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/inline_response201.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/integration_token_regeneration_response.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/integration_token_regeneration_response.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license_level.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license_level.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license_list.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license_list.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/license_report.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/license_report.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/linked_entities.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/linked_entities.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/linked_entity.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/linked_entity.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/links.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/links.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/links_bulktree_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/links_bulktree_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/links_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/links_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/local_synonym.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/local_synonym.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/local_synonym_creation_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/local_synonym_creation_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/local_synonym_update_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/local_synonym_update_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/lower_case_all_types.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/lower_case_all_types.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/mapping_path.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/mapping_path.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/max_depth.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/max_depth.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_authorizations.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_authorizations.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_authorizations_update.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_authorizations_update.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_names.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_names.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/module_role.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/module_role.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/object_history_entry.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/object_history_entry.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/object_location.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/object_location.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/objects_history_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/objects_history_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/omit_entity_summary_access_data_or_attributes_or_links_or_children_count_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/omit_entity_summary_access_data_or_attributes_or_links_or_children_count_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/omit_search_body_included_attributes_or_include_access_data_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/omit_search_body_included_attributes_or_include_access_data_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/omit_team_id_or_icon_hash_or_members_count_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/omit_team_id_or_icon_hash_or_members_count_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_attributes_response_body_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_attributes_response_body_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_dpi_data_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_dpi_data_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_entity_summary_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_entity_summary_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_tags_response_body_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_tags_response_body_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_user_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_user_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_user_authorizations_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_user_authorizations_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/paginated_response_version_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/paginated_response_version_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/partial_team_creation_payload_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/partial_team_creation_payload_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_entity_summary_exclude_keyof_entity_summary_access_data_or_attributes_or_links_or_children_count_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_entity_summary_exclude_keyof_entity_summary_access_data_or_attributes_or_links_or_children_count_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_entity_summary_exclude_keyof_entity_summary_links_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_entity_summary_exclude_keyof_entity_summary_links_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_search_body_exclude_keyof_search_body_included_attributes_or_include_access_data_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_search_body_exclude_keyof_search_body_included_attributes_or_include_access_data_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pick_team_exclude_keyof_team_id_or_icon_hash_or_members_count_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pick_team_exclude_keyof_team_id_or_icon_hash_or_members_count_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/pk_column.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/pk_column.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/primary_key.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/primary_key.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/primary_key_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/primary_key_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/properties_bulk_tree_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/properties_bulk_tree_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/property_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/property_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/property_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/property_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/queries_history_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/queries_history_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/quick_filter.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/quick_filter.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/reference_object.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/reference_object.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/reference_parents.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/reference_parents.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/rich_text.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/rich_text.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/roles.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/roles.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/saved_query.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/saved_query.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_error.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_error.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_list_response_user_.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_list_response_user_.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_patch_operation_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_patch_operation_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_patch_operation_payload_operations.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_patch_operation_payload_operations.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_emails.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_emails.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_meta.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_meta.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_name.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_name.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/scim_user_photos.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/scim_user_photos.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/screen_data_types.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/screen_data_types.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_filter.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_filter.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_filter_operator.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_filter_operator.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_query.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_query.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_response.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_response.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/search_response_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/search_response_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/social_comment.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/social_comment.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_bulk_creation.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_bulk_update.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_bulk_update.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/source_update_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/source_update_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_bulk_creation.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_bulk_update.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_bulk_update.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/structure_update_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/structure_update_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/system_attribute.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/system_attribute.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/tags_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/tags_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/tags_response_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/tags_response_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_creation_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_creation_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_status.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_status.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/task_update_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/task_update_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_creation_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_creation_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_id.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_id.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_member.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_member.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_role.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/team_update_payload.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/team_update_payload.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/teams_result.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/teams_result.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/technology.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/technology.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/technology_module.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/technology_module.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_color_rule.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_color_rule.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_entry.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_entry.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_frequency.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_frequency.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/time_series_value.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/time_series_value.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/update_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/update_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/update_technology_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/update_technology_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/url.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/url.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_bulktree_creation.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_bulktree_creation.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_creation_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_creation_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_type.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_type.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/usage_update_request.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/usage_update_request.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_authorizations.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_authorizations.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_creation_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_creation_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_update_authorizations.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_update_authorizations.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_update_authorizations_definition.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_update_authorizations_definition.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/user_update_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/user_update_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/users_update_authorizations_body.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/users_update_authorizations_body.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/uuid.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/uuid.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/version.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/version.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/version_id.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/version_id.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/workspace.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/workspace.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/workspace_authorization.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/workspace_authorization.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/models/workspaces.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/models/workspaces.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu-datagalaxy-client/rest.py` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client/rest.py`

 * *Files identical despite different names*

### Comparing `kensu-datagalaxy-client-1.0.0/kensu_datagalaxy_client.egg-info/SOURCES.txt` & `kensu-datagalaxy-client-1.0.1/kensu_datagalaxy_client.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,269 +1,269 @@
 README.md
 setup.py
-kensu-datagalaxy-client/__init__.py
-kensu-datagalaxy-client/api_client.py
-kensu-datagalaxy-client/configuration.py
-kensu-datagalaxy-client/rest.py
-kensu-datagalaxy-client/api/__init__.py
-kensu-datagalaxy-client/api/attributes_api.py
-kensu-datagalaxy-client/api/authentication_api.py
-kensu-datagalaxy-client/api/comments_api.py
-kensu-datagalaxy-client/api/containers_api.py
-kensu-datagalaxy-client/api/data_processing_api.py
-kensu-datagalaxy-client/api/data_processing_item_api.py
-kensu-datagalaxy-client/api/fields_api.py
-kensu-datagalaxy-client/api/filtered_views_api.py
-kensu-datagalaxy-client/api/glossary_api.py
-kensu-datagalaxy-client/api/history_api.py
-kensu-datagalaxy-client/api/image_api.py
-kensu-datagalaxy-client/api/licenses_api.py
-kensu-datagalaxy-client/api/links_api.py
-kensu-datagalaxy-client/api/scim_users_api.py
-kensu-datagalaxy-client/api/screens_api.py
-kensu-datagalaxy-client/api/search_api.py
-kensu-datagalaxy-client/api/sources_api.py
-kensu-datagalaxy-client/api/structures_api.py
-kensu-datagalaxy-client/api/tasks_api.py
-kensu-datagalaxy-client/api/teams_api.py
-kensu-datagalaxy-client/api/technologies_api.py
-kensu-datagalaxy-client/api/usage_api.py
-kensu-datagalaxy-client/api/users_api.py
-kensu-datagalaxy-client/api/workspaces_api.py
-kensu-datagalaxy-client/models/__init__.py
-kensu-datagalaxy-client/models/access_data.py
-kensu-datagalaxy-client/models/access_type.py
-kensu-datagalaxy-client/models/additional_custom_attribute.py
-kensu-datagalaxy-client/models/additional_custom_attribute_bulk.py
-kensu-datagalaxy-client/models/all_types.py
-kensu-datagalaxy-client/models/all_types_lower.py
-kensu-datagalaxy-client/models/any_of_attribute_bulk_creation_body_default_value.py
-kensu-datagalaxy-client/models/any_of_attribute_bulk_update_body_default_value.py
-kensu-datagalaxy-client/models/any_of_attribute_creation_body_default_value.py
-kensu-datagalaxy-client/models/any_of_attribute_default_value.py
-kensu-datagalaxy-client/models/any_of_attribute_update_body_default_value.py
-kensu-datagalaxy-client/models/any_of_category_attribute_id.py
-kensu-datagalaxy-client/models/any_of_category_body_attribute_name_id.py
-kensu-datagalaxy-client/models/any_of_scim_patch_operation_payload_operations_value.py
-kensu-datagalaxy-client/models/any_of_search_filter_values.py
-kensu-datagalaxy-client/models/any_of_tags_body_color.py
-kensu-datagalaxy-client/models/api_error_model.py
-kensu-datagalaxy-client/models/api_error_model_error.py
-kensu-datagalaxy-client/models/attribute.py
-kensu-datagalaxy-client/models/attribute_bulk_creation_body.py
-kensu-datagalaxy-client/models/attribute_bulk_update_body.py
-kensu-datagalaxy-client/models/attribute_creation_body.py
-kensu-datagalaxy-client/models/attribute_data_type_enum.py
-kensu-datagalaxy-client/models/attribute_formats.py
-kensu-datagalaxy-client/models/attribute_key.py
-kensu-datagalaxy-client/models/attribute_name.py
-kensu-datagalaxy-client/models/attribute_update_body.py
-kensu-datagalaxy-client/models/attribute_value.py
-kensu-datagalaxy-client/models/attributes_layout.py
-kensu-datagalaxy-client/models/attributes_response_body.py
-kensu-datagalaxy-client/models/attributes_values_body.py
-kensu-datagalaxy-client/models/attributes_values_body1.py
-kensu-datagalaxy-client/models/authorizations.py
-kensu-datagalaxy-client/models/authorizations_authorizations.py
-kensu-datagalaxy-client/models/bulk_delete_response.py
-kensu-datagalaxy-client/models/bulk_input.py
-kensu-datagalaxy-client/models/bulk_links_payload.py
-kensu-datagalaxy-client/models/bulk_links_result.py
-kensu-datagalaxy-client/models/bulk_result.py
-kensu-datagalaxy-client/models/bulk_tree_creation_request.py
-kensu-datagalaxy-client/models/category_attribute_.py
-kensu-datagalaxy-client/models/category_body_attribute_name_.py
-kensu-datagalaxy-client/models/child_container.py
-kensu-datagalaxy-client/models/child_structure.py
-kensu-datagalaxy-client/models/color.py
-kensu-datagalaxy-client/models/column_data_type.py
-kensu-datagalaxy-client/models/comment_payload.py
-kensu-datagalaxy-client/models/compatibility_definition.py
-kensu-datagalaxy-client/models/compatible_link.py
-kensu-datagalaxy-client/models/container_bulk_creation.py
-kensu-datagalaxy-client/models/container_bulk_update.py
-kensu-datagalaxy-client/models/container_creation_request.py
-kensu-datagalaxy-client/models/container_type.py
-kensu-datagalaxy-client/models/create_technology_body.py
-kensu-datagalaxy-client/models/credentials.py
-kensu-datagalaxy-client/models/custom_attribute_name.py
-kensu-datagalaxy-client/models/data_processing_bulk_creation.py
-kensu-datagalaxy-client/models/data_processing_bulk_response.py
-kensu-datagalaxy-client/models/data_processing_bulk_response_details.py
-kensu-datagalaxy-client/models/data_processing_bulk_response_details_data_processing_items.py
-kensu-datagalaxy-client/models/data_processing_entity.py
-kensu-datagalaxy-client/models/data_processing_item_type.py
-kensu-datagalaxy-client/models/data_processing_type.py
-kensu-datagalaxy-client/models/data_types.py
-kensu-datagalaxy-client/models/data_types_client_mapping.py
-kensu-datagalaxy-client/models/date_iso.py
-kensu-datagalaxy-client/models/default_user.py
-kensu-datagalaxy-client/models/double_uuid.py
-kensu-datagalaxy-client/models/dp_creation_request.py
-kensu-datagalaxy-client/models/dp_update_request.py
-kensu-datagalaxy-client/models/dpi_bulk_model.py
-kensu-datagalaxy-client/models/dpi_creation_body.py
-kensu-datagalaxy-client/models/dpi_data.py
-kensu-datagalaxy-client/models/dpi_id.py
-kensu-datagalaxy-client/models/dpi_input.py
-kensu-datagalaxy-client/models/dpi_update_body.py
-kensu-datagalaxy-client/models/email.py
-kensu-datagalaxy-client/models/entity.py
-kensu-datagalaxy-client/models/entity_attributes.py
-kensu-datagalaxy-client/models/entity_base.py
-kensu-datagalaxy-client/models/entity_descriptor.py
-kensu-datagalaxy-client/models/entity_location.py
-kensu-datagalaxy-client/models/entity_search_result.py
-kensu-datagalaxy-client/models/entity_status.py
-kensu-datagalaxy-client/models/entity_summary.py
-kensu-datagalaxy-client/models/exact_match.py
-kensu-datagalaxy-client/models/exclude_typeof_attribute_data_type_enum_at_keyoftypeof_attribute_data_type_enum_typeof_data_type_enum_dataprocessingitem_.py
-kensu-datagalaxy-client/models/field_bulk_creation.py
-kensu-datagalaxy-client/models/field_bulk_update.py
-kensu-datagalaxy-client/models/field_type.py
-kensu-datagalaxy-client/models/fields_creation_request.py
-kensu-datagalaxy-client/models/fields_update_request.py
-kensu-datagalaxy-client/models/filtered_view.py
-kensu-datagalaxy-client/models/filtered_view_summary.py
-kensu-datagalaxy-client/models/fk_column.py
-kensu-datagalaxy-client/models/foreign_key.py
-kensu-datagalaxy-client/models/foreign_key_payload.py
-kensu-datagalaxy-client/models/get_technologies_result.py
-kensu-datagalaxy-client/models/governance_users.py
-kensu-datagalaxy-client/models/hyper_link.py
-kensu-datagalaxy-client/models/i_attributes.py
-kensu-datagalaxy-client/models/i_date.py
-kensu-datagalaxy-client/models/image_body.py
-kensu-datagalaxy-client/models/image_hash.py
-kensu-datagalaxy-client/models/image_mime_type.py
-kensu-datagalaxy-client/models/image_result.py
-kensu-datagalaxy-client/models/image_upload_response.py
-kensu-datagalaxy-client/models/include_access_data.py
-kensu-datagalaxy-client/models/include_attributes.py
-kensu-datagalaxy-client/models/include_links.py
-kensu-datagalaxy-client/models/inline_response200.py
-kensu-datagalaxy-client/models/inline_response201.py
-kensu-datagalaxy-client/models/integration_token_regeneration_response.py
-kensu-datagalaxy-client/models/license.py
-kensu-datagalaxy-client/models/license_level.py
-kensu-datagalaxy-client/models/license_list.py
-kensu-datagalaxy-client/models/license_report.py
-kensu-datagalaxy-client/models/linked_entities.py
-kensu-datagalaxy-client/models/linked_entity.py
-kensu-datagalaxy-client/models/links.py
-kensu-datagalaxy-client/models/links_bulktree_payload.py
-kensu-datagalaxy-client/models/links_creation_request.py
-kensu-datagalaxy-client/models/local_synonym.py
-kensu-datagalaxy-client/models/local_synonym_creation_body.py
-kensu-datagalaxy-client/models/local_synonym_update_body.py
-kensu-datagalaxy-client/models/lower_case_all_types.py
-kensu-datagalaxy-client/models/mapping_path.py
-kensu-datagalaxy-client/models/max_depth.py
-kensu-datagalaxy-client/models/module.py
-kensu-datagalaxy-client/models/module_authorizations.py
-kensu-datagalaxy-client/models/module_authorizations_update.py
-kensu-datagalaxy-client/models/module_names.py
-kensu-datagalaxy-client/models/module_role.py
-kensu-datagalaxy-client/models/object_history_entry.py
-kensu-datagalaxy-client/models/object_location.py
-kensu-datagalaxy-client/models/objects_history_result.py
-kensu-datagalaxy-client/models/omit_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
-kensu-datagalaxy-client/models/omit_search_body_included_attributes_or_include_access_data_.py
-kensu-datagalaxy-client/models/omit_team_id_or_icon_hash_or_members_count_.py
-kensu-datagalaxy-client/models/paginated_response_attributes_response_body_.py
-kensu-datagalaxy-client/models/paginated_response_dpi_data_.py
-kensu-datagalaxy-client/models/paginated_response_entity_summary_.py
-kensu-datagalaxy-client/models/paginated_response_tags_response_body_.py
-kensu-datagalaxy-client/models/paginated_response_user_.py
-kensu-datagalaxy-client/models/paginated_response_user_authorizations_.py
-kensu-datagalaxy-client/models/paginated_response_version_.py
-kensu-datagalaxy-client/models/partial_team_creation_payload_.py
-kensu-datagalaxy-client/models/pick_entity_summary_exclude_keyof_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
-kensu-datagalaxy-client/models/pick_entity_summary_exclude_keyof_entity_summary_links_.py
-kensu-datagalaxy-client/models/pick_search_body_exclude_keyof_search_body_included_attributes_or_include_access_data_.py
-kensu-datagalaxy-client/models/pick_team_exclude_keyof_team_id_or_icon_hash_or_members_count_.py
-kensu-datagalaxy-client/models/pk_column.py
-kensu-datagalaxy-client/models/primary_key.py
-kensu-datagalaxy-client/models/primary_key_payload.py
-kensu-datagalaxy-client/models/properties_bulk_tree_creation_request.py
-kensu-datagalaxy-client/models/property_creation_request.py
-kensu-datagalaxy-client/models/property_type.py
-kensu-datagalaxy-client/models/queries_history_result.py
-kensu-datagalaxy-client/models/quick_filter.py
-kensu-datagalaxy-client/models/reference_object.py
-kensu-datagalaxy-client/models/reference_parents.py
-kensu-datagalaxy-client/models/rich_text.py
-kensu-datagalaxy-client/models/roles.py
-kensu-datagalaxy-client/models/saved_query.py
-kensu-datagalaxy-client/models/scim_error.py
-kensu-datagalaxy-client/models/scim_list_response_user_.py
-kensu-datagalaxy-client/models/scim_patch_operation_payload.py
-kensu-datagalaxy-client/models/scim_patch_operation_payload_operations.py
-kensu-datagalaxy-client/models/scim_user.py
-kensu-datagalaxy-client/models/scim_user_emails.py
-kensu-datagalaxy-client/models/scim_user_meta.py
-kensu-datagalaxy-client/models/scim_user_name.py
-kensu-datagalaxy-client/models/scim_user_photos.py
-kensu-datagalaxy-client/models/screen_data_types.py
-kensu-datagalaxy-client/models/search_body.py
-kensu-datagalaxy-client/models/search_filter.py
-kensu-datagalaxy-client/models/search_filter_operator.py
-kensu-datagalaxy-client/models/search_query.py
-kensu-datagalaxy-client/models/search_response.py
-kensu-datagalaxy-client/models/search_response_result.py
-kensu-datagalaxy-client/models/social_comment.py
-kensu-datagalaxy-client/models/source_bulk_creation.py
-kensu-datagalaxy-client/models/source_bulk_update.py
-kensu-datagalaxy-client/models/source_creation_request.py
-kensu-datagalaxy-client/models/source_type.py
-kensu-datagalaxy-client/models/source_update_request.py
-kensu-datagalaxy-client/models/structure_bulk_creation.py
-kensu-datagalaxy-client/models/structure_bulk_update.py
-kensu-datagalaxy-client/models/structure_creation_request.py
-kensu-datagalaxy-client/models/structure_type.py
-kensu-datagalaxy-client/models/structure_update_request.py
-kensu-datagalaxy-client/models/system_attribute.py
-kensu-datagalaxy-client/models/tags_body.py
-kensu-datagalaxy-client/models/tags_response_body.py
-kensu-datagalaxy-client/models/task.py
-kensu-datagalaxy-client/models/task_creation_payload.py
-kensu-datagalaxy-client/models/task_status.py
-kensu-datagalaxy-client/models/task_type.py
-kensu-datagalaxy-client/models/task_update_payload.py
-kensu-datagalaxy-client/models/team.py
-kensu-datagalaxy-client/models/team_creation_payload.py
-kensu-datagalaxy-client/models/team_id.py
-kensu-datagalaxy-client/models/team_member.py
-kensu-datagalaxy-client/models/team_role.py
-kensu-datagalaxy-client/models/team_update_payload.py
-kensu-datagalaxy-client/models/teams_result.py
-kensu-datagalaxy-client/models/technology.py
-kensu-datagalaxy-client/models/technology_module.py
-kensu-datagalaxy-client/models/time_series_color_rule.py
-kensu-datagalaxy-client/models/time_series_entry.py
-kensu-datagalaxy-client/models/time_series_frequency.py
-kensu-datagalaxy-client/models/time_series_value.py
-kensu-datagalaxy-client/models/update_request.py
-kensu-datagalaxy-client/models/update_technology_body.py
-kensu-datagalaxy-client/models/url.py
-kensu-datagalaxy-client/models/usage_bulktree_creation.py
-kensu-datagalaxy-client/models/usage_creation_request.py
-kensu-datagalaxy-client/models/usage_type.py
-kensu-datagalaxy-client/models/usage_update_request.py
-kensu-datagalaxy-client/models/user.py
-kensu-datagalaxy-client/models/user_authorizations.py
-kensu-datagalaxy-client/models/user_creation_body.py
-kensu-datagalaxy-client/models/user_update_authorizations.py
-kensu-datagalaxy-client/models/user_update_authorizations_definition.py
-kensu-datagalaxy-client/models/user_update_body.py
-kensu-datagalaxy-client/models/users_update_authorizations_body.py
-kensu-datagalaxy-client/models/uuid.py
-kensu-datagalaxy-client/models/version.py
-kensu-datagalaxy-client/models/version_id.py
-kensu-datagalaxy-client/models/workspace.py
-kensu-datagalaxy-client/models/workspace_authorization.py
-kensu-datagalaxy-client/models/workspaces.py
+kensu_datagalaxy_client/__init__.py
+kensu_datagalaxy_client/api_client.py
+kensu_datagalaxy_client/configuration.py
+kensu_datagalaxy_client/rest.py
 kensu_datagalaxy_client.egg-info/PKG-INFO
 kensu_datagalaxy_client.egg-info/SOURCES.txt
 kensu_datagalaxy_client.egg-info/dependency_links.txt
 kensu_datagalaxy_client.egg-info/requires.txt
-kensu_datagalaxy_client.egg-info/top_level.txt
+kensu_datagalaxy_client.egg-info/top_level.txt
+kensu_datagalaxy_client/api/__init__.py
+kensu_datagalaxy_client/api/attributes_api.py
+kensu_datagalaxy_client/api/authentication_api.py
+kensu_datagalaxy_client/api/comments_api.py
+kensu_datagalaxy_client/api/containers_api.py
+kensu_datagalaxy_client/api/data_processing_api.py
+kensu_datagalaxy_client/api/data_processing_item_api.py
+kensu_datagalaxy_client/api/fields_api.py
+kensu_datagalaxy_client/api/filtered_views_api.py
+kensu_datagalaxy_client/api/glossary_api.py
+kensu_datagalaxy_client/api/history_api.py
+kensu_datagalaxy_client/api/image_api.py
+kensu_datagalaxy_client/api/licenses_api.py
+kensu_datagalaxy_client/api/links_api.py
+kensu_datagalaxy_client/api/scim_users_api.py
+kensu_datagalaxy_client/api/screens_api.py
+kensu_datagalaxy_client/api/search_api.py
+kensu_datagalaxy_client/api/sources_api.py
+kensu_datagalaxy_client/api/structures_api.py
+kensu_datagalaxy_client/api/tasks_api.py
+kensu_datagalaxy_client/api/teams_api.py
+kensu_datagalaxy_client/api/technologies_api.py
+kensu_datagalaxy_client/api/usage_api.py
+kensu_datagalaxy_client/api/users_api.py
+kensu_datagalaxy_client/api/workspaces_api.py
+kensu_datagalaxy_client/models/__init__.py
+kensu_datagalaxy_client/models/access_data.py
+kensu_datagalaxy_client/models/access_type.py
+kensu_datagalaxy_client/models/additional_custom_attribute.py
+kensu_datagalaxy_client/models/additional_custom_attribute_bulk.py
+kensu_datagalaxy_client/models/all_types.py
+kensu_datagalaxy_client/models/all_types_lower.py
+kensu_datagalaxy_client/models/any_of_attribute_bulk_creation_body_default_value.py
+kensu_datagalaxy_client/models/any_of_attribute_bulk_update_body_default_value.py
+kensu_datagalaxy_client/models/any_of_attribute_creation_body_default_value.py
+kensu_datagalaxy_client/models/any_of_attribute_default_value.py
+kensu_datagalaxy_client/models/any_of_attribute_update_body_default_value.py
+kensu_datagalaxy_client/models/any_of_category_attribute_id.py
+kensu_datagalaxy_client/models/any_of_category_body_attribute_name_id.py
+kensu_datagalaxy_client/models/any_of_scim_patch_operation_payload_operations_value.py
+kensu_datagalaxy_client/models/any_of_search_filter_values.py
+kensu_datagalaxy_client/models/any_of_tags_body_color.py
+kensu_datagalaxy_client/models/api_error_model.py
+kensu_datagalaxy_client/models/api_error_model_error.py
+kensu_datagalaxy_client/models/attribute.py
+kensu_datagalaxy_client/models/attribute_bulk_creation_body.py
+kensu_datagalaxy_client/models/attribute_bulk_update_body.py
+kensu_datagalaxy_client/models/attribute_creation_body.py
+kensu_datagalaxy_client/models/attribute_data_type_enum.py
+kensu_datagalaxy_client/models/attribute_formats.py
+kensu_datagalaxy_client/models/attribute_key.py
+kensu_datagalaxy_client/models/attribute_name.py
+kensu_datagalaxy_client/models/attribute_update_body.py
+kensu_datagalaxy_client/models/attribute_value.py
+kensu_datagalaxy_client/models/attributes_layout.py
+kensu_datagalaxy_client/models/attributes_response_body.py
+kensu_datagalaxy_client/models/attributes_values_body.py
+kensu_datagalaxy_client/models/attributes_values_body1.py
+kensu_datagalaxy_client/models/authorizations.py
+kensu_datagalaxy_client/models/authorizations_authorizations.py
+kensu_datagalaxy_client/models/bulk_delete_response.py
+kensu_datagalaxy_client/models/bulk_input.py
+kensu_datagalaxy_client/models/bulk_links_payload.py
+kensu_datagalaxy_client/models/bulk_links_result.py
+kensu_datagalaxy_client/models/bulk_result.py
+kensu_datagalaxy_client/models/bulk_tree_creation_request.py
+kensu_datagalaxy_client/models/category_attribute_.py
+kensu_datagalaxy_client/models/category_body_attribute_name_.py
+kensu_datagalaxy_client/models/child_container.py
+kensu_datagalaxy_client/models/child_structure.py
+kensu_datagalaxy_client/models/color.py
+kensu_datagalaxy_client/models/column_data_type.py
+kensu_datagalaxy_client/models/comment_payload.py
+kensu_datagalaxy_client/models/compatibility_definition.py
+kensu_datagalaxy_client/models/compatible_link.py
+kensu_datagalaxy_client/models/container_bulk_creation.py
+kensu_datagalaxy_client/models/container_bulk_update.py
+kensu_datagalaxy_client/models/container_creation_request.py
+kensu_datagalaxy_client/models/container_type.py
+kensu_datagalaxy_client/models/create_technology_body.py
+kensu_datagalaxy_client/models/credentials.py
+kensu_datagalaxy_client/models/custom_attribute_name.py
+kensu_datagalaxy_client/models/data_processing_bulk_creation.py
+kensu_datagalaxy_client/models/data_processing_bulk_response.py
+kensu_datagalaxy_client/models/data_processing_bulk_response_details.py
+kensu_datagalaxy_client/models/data_processing_bulk_response_details_data_processing_items.py
+kensu_datagalaxy_client/models/data_processing_entity.py
+kensu_datagalaxy_client/models/data_processing_item_type.py
+kensu_datagalaxy_client/models/data_processing_type.py
+kensu_datagalaxy_client/models/data_types.py
+kensu_datagalaxy_client/models/data_types_client_mapping.py
+kensu_datagalaxy_client/models/date_iso.py
+kensu_datagalaxy_client/models/default_user.py
+kensu_datagalaxy_client/models/double_uuid.py
+kensu_datagalaxy_client/models/dp_creation_request.py
+kensu_datagalaxy_client/models/dp_update_request.py
+kensu_datagalaxy_client/models/dpi_bulk_model.py
+kensu_datagalaxy_client/models/dpi_creation_body.py
+kensu_datagalaxy_client/models/dpi_data.py
+kensu_datagalaxy_client/models/dpi_id.py
+kensu_datagalaxy_client/models/dpi_input.py
+kensu_datagalaxy_client/models/dpi_update_body.py
+kensu_datagalaxy_client/models/email.py
+kensu_datagalaxy_client/models/entity.py
+kensu_datagalaxy_client/models/entity_attributes.py
+kensu_datagalaxy_client/models/entity_base.py
+kensu_datagalaxy_client/models/entity_descriptor.py
+kensu_datagalaxy_client/models/entity_location.py
+kensu_datagalaxy_client/models/entity_search_result.py
+kensu_datagalaxy_client/models/entity_status.py
+kensu_datagalaxy_client/models/entity_summary.py
+kensu_datagalaxy_client/models/exact_match.py
+kensu_datagalaxy_client/models/exclude_typeof_attribute_data_type_enum_at_keyoftypeof_attribute_data_type_enum_typeof_data_type_enum_dataprocessingitem_.py
+kensu_datagalaxy_client/models/field_bulk_creation.py
+kensu_datagalaxy_client/models/field_bulk_update.py
+kensu_datagalaxy_client/models/field_type.py
+kensu_datagalaxy_client/models/fields_creation_request.py
+kensu_datagalaxy_client/models/fields_update_request.py
+kensu_datagalaxy_client/models/filtered_view.py
+kensu_datagalaxy_client/models/filtered_view_summary.py
+kensu_datagalaxy_client/models/fk_column.py
+kensu_datagalaxy_client/models/foreign_key.py
+kensu_datagalaxy_client/models/foreign_key_payload.py
+kensu_datagalaxy_client/models/get_technologies_result.py
+kensu_datagalaxy_client/models/governance_users.py
+kensu_datagalaxy_client/models/hyper_link.py
+kensu_datagalaxy_client/models/i_attributes.py
+kensu_datagalaxy_client/models/i_date.py
+kensu_datagalaxy_client/models/image_body.py
+kensu_datagalaxy_client/models/image_hash.py
+kensu_datagalaxy_client/models/image_mime_type.py
+kensu_datagalaxy_client/models/image_result.py
+kensu_datagalaxy_client/models/image_upload_response.py
+kensu_datagalaxy_client/models/include_access_data.py
+kensu_datagalaxy_client/models/include_attributes.py
+kensu_datagalaxy_client/models/include_links.py
+kensu_datagalaxy_client/models/inline_response200.py
+kensu_datagalaxy_client/models/inline_response201.py
+kensu_datagalaxy_client/models/integration_token_regeneration_response.py
+kensu_datagalaxy_client/models/license.py
+kensu_datagalaxy_client/models/license_level.py
+kensu_datagalaxy_client/models/license_list.py
+kensu_datagalaxy_client/models/license_report.py
+kensu_datagalaxy_client/models/linked_entities.py
+kensu_datagalaxy_client/models/linked_entity.py
+kensu_datagalaxy_client/models/links.py
+kensu_datagalaxy_client/models/links_bulktree_payload.py
+kensu_datagalaxy_client/models/links_creation_request.py
+kensu_datagalaxy_client/models/local_synonym.py
+kensu_datagalaxy_client/models/local_synonym_creation_body.py
+kensu_datagalaxy_client/models/local_synonym_update_body.py
+kensu_datagalaxy_client/models/lower_case_all_types.py
+kensu_datagalaxy_client/models/mapping_path.py
+kensu_datagalaxy_client/models/max_depth.py
+kensu_datagalaxy_client/models/module.py
+kensu_datagalaxy_client/models/module_authorizations.py
+kensu_datagalaxy_client/models/module_authorizations_update.py
+kensu_datagalaxy_client/models/module_names.py
+kensu_datagalaxy_client/models/module_role.py
+kensu_datagalaxy_client/models/object_history_entry.py
+kensu_datagalaxy_client/models/object_location.py
+kensu_datagalaxy_client/models/objects_history_result.py
+kensu_datagalaxy_client/models/omit_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
+kensu_datagalaxy_client/models/omit_search_body_included_attributes_or_include_access_data_.py
+kensu_datagalaxy_client/models/omit_team_id_or_icon_hash_or_members_count_.py
+kensu_datagalaxy_client/models/paginated_response_attributes_response_body_.py
+kensu_datagalaxy_client/models/paginated_response_dpi_data_.py
+kensu_datagalaxy_client/models/paginated_response_entity_summary_.py
+kensu_datagalaxy_client/models/paginated_response_tags_response_body_.py
+kensu_datagalaxy_client/models/paginated_response_user_.py
+kensu_datagalaxy_client/models/paginated_response_user_authorizations_.py
+kensu_datagalaxy_client/models/paginated_response_version_.py
+kensu_datagalaxy_client/models/partial_team_creation_payload_.py
+kensu_datagalaxy_client/models/pick_entity_summary_exclude_keyof_entity_summary_access_data_or_attributes_or_links_or_children_count_.py
+kensu_datagalaxy_client/models/pick_entity_summary_exclude_keyof_entity_summary_links_.py
+kensu_datagalaxy_client/models/pick_search_body_exclude_keyof_search_body_included_attributes_or_include_access_data_.py
+kensu_datagalaxy_client/models/pick_team_exclude_keyof_team_id_or_icon_hash_or_members_count_.py
+kensu_datagalaxy_client/models/pk_column.py
+kensu_datagalaxy_client/models/primary_key.py
+kensu_datagalaxy_client/models/primary_key_payload.py
+kensu_datagalaxy_client/models/properties_bulk_tree_creation_request.py
+kensu_datagalaxy_client/models/property_creation_request.py
+kensu_datagalaxy_client/models/property_type.py
+kensu_datagalaxy_client/models/queries_history_result.py
+kensu_datagalaxy_client/models/quick_filter.py
+kensu_datagalaxy_client/models/reference_object.py
+kensu_datagalaxy_client/models/reference_parents.py
+kensu_datagalaxy_client/models/rich_text.py
+kensu_datagalaxy_client/models/roles.py
+kensu_datagalaxy_client/models/saved_query.py
+kensu_datagalaxy_client/models/scim_error.py
+kensu_datagalaxy_client/models/scim_list_response_user_.py
+kensu_datagalaxy_client/models/scim_patch_operation_payload.py
+kensu_datagalaxy_client/models/scim_patch_operation_payload_operations.py
+kensu_datagalaxy_client/models/scim_user.py
+kensu_datagalaxy_client/models/scim_user_emails.py
+kensu_datagalaxy_client/models/scim_user_meta.py
+kensu_datagalaxy_client/models/scim_user_name.py
+kensu_datagalaxy_client/models/scim_user_photos.py
+kensu_datagalaxy_client/models/screen_data_types.py
+kensu_datagalaxy_client/models/search_body.py
+kensu_datagalaxy_client/models/search_filter.py
+kensu_datagalaxy_client/models/search_filter_operator.py
+kensu_datagalaxy_client/models/search_query.py
+kensu_datagalaxy_client/models/search_response.py
+kensu_datagalaxy_client/models/search_response_result.py
+kensu_datagalaxy_client/models/social_comment.py
+kensu_datagalaxy_client/models/source_bulk_creation.py
+kensu_datagalaxy_client/models/source_bulk_update.py
+kensu_datagalaxy_client/models/source_creation_request.py
+kensu_datagalaxy_client/models/source_type.py
+kensu_datagalaxy_client/models/source_update_request.py
+kensu_datagalaxy_client/models/structure_bulk_creation.py
+kensu_datagalaxy_client/models/structure_bulk_update.py
+kensu_datagalaxy_client/models/structure_creation_request.py
+kensu_datagalaxy_client/models/structure_type.py
+kensu_datagalaxy_client/models/structure_update_request.py
+kensu_datagalaxy_client/models/system_attribute.py
+kensu_datagalaxy_client/models/tags_body.py
+kensu_datagalaxy_client/models/tags_response_body.py
+kensu_datagalaxy_client/models/task.py
+kensu_datagalaxy_client/models/task_creation_payload.py
+kensu_datagalaxy_client/models/task_status.py
+kensu_datagalaxy_client/models/task_type.py
+kensu_datagalaxy_client/models/task_update_payload.py
+kensu_datagalaxy_client/models/team.py
+kensu_datagalaxy_client/models/team_creation_payload.py
+kensu_datagalaxy_client/models/team_id.py
+kensu_datagalaxy_client/models/team_member.py
+kensu_datagalaxy_client/models/team_role.py
+kensu_datagalaxy_client/models/team_update_payload.py
+kensu_datagalaxy_client/models/teams_result.py
+kensu_datagalaxy_client/models/technology.py
+kensu_datagalaxy_client/models/technology_module.py
+kensu_datagalaxy_client/models/time_series_color_rule.py
+kensu_datagalaxy_client/models/time_series_entry.py
+kensu_datagalaxy_client/models/time_series_frequency.py
+kensu_datagalaxy_client/models/time_series_value.py
+kensu_datagalaxy_client/models/update_request.py
+kensu_datagalaxy_client/models/update_technology_body.py
+kensu_datagalaxy_client/models/url.py
+kensu_datagalaxy_client/models/usage_bulktree_creation.py
+kensu_datagalaxy_client/models/usage_creation_request.py
+kensu_datagalaxy_client/models/usage_type.py
+kensu_datagalaxy_client/models/usage_update_request.py
+kensu_datagalaxy_client/models/user.py
+kensu_datagalaxy_client/models/user_authorizations.py
+kensu_datagalaxy_client/models/user_creation_body.py
+kensu_datagalaxy_client/models/user_update_authorizations.py
+kensu_datagalaxy_client/models/user_update_authorizations_definition.py
+kensu_datagalaxy_client/models/user_update_body.py
+kensu_datagalaxy_client/models/users_update_authorizations_body.py
+kensu_datagalaxy_client/models/uuid.py
+kensu_datagalaxy_client/models/version.py
+kensu_datagalaxy_client/models/version_id.py
+kensu_datagalaxy_client/models/workspace.py
+kensu_datagalaxy_client/models/workspace_authorization.py
+kensu_datagalaxy_client/models/workspaces.py
```

### Comparing `kensu-datagalaxy-client-1.0.0/setup.py` & `kensu-datagalaxy-client-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kensu-datagalaxy-client"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

#### html2text {}

```diff
@@ -49,15 +49,15 @@
 This layout displays informations in a modern way and contains more
 informations about requests parameters - [Swagger layout](/v2/documentation/
 old)
 This is our legacy layout. It's main perk is the \"Try it\" feature which let's
 you send requests directly from the documentation. # noqa: E501 OpenAPI spec
 version: 2.12.0 Generated by: https://github.com/swagger-api/swagger-
 codegen.git """ from setuptools import setup, find_packages # noqa: H301 NAME =
-"kensu-datagalaxy-client" VERSION = "1.0.0" # To install the library, run the
+"kensu-datagalaxy-client" VERSION = "1.0.1" # To install the library, run the
 following # # python setup.py install # # prerequisite: setuptools # http://
 pypi.python.org/pypi/setuptools REQUIRES = ["urllib3 >= 1.15", "six >= 1.10",
 "certifi", "python-dateutil"] setup( name=NAME, version=VERSION,
 description="Developer API - DataGalaxy", author_email="", url="", keywords=
 ["Swagger", "Kensu", "Developer API - DataGalaxy"], install_requires=REQUIRES,
 packages=find_packages(), include_package_data=True, long_description="""\ The
 DataGalaxy API for Kensu Connector# noqa: E501 """ )
```

