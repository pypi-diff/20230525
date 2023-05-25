# Comparing `tmp/iparapheur-provisioning-1.6.1.tar.gz` & `tmp/iparapheur-provisioning-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.6.1.tar", last modified: Fri May 19 18:25:52 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.6.2.tar", last modified: Thu May 25 14:10:15 2023, max compression
```

## Comparing `iparapheur-provisioning-1.6.1.tar` & `iparapheur-provisioning-1.6.2.tar`

### file list

```diff
@@ -1,290 +1,243 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18951 2023-05-19 18:23:31.000000 iparapheur-provisioning-1.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.645561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.649561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7708 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.649561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-19 18:23:23.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-19 18:23:23.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.653561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1012 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     2894 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-05-19 18:22:59.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/composite_id.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-05-19 18:23:00.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    30318 2023-05-19 18:23:01.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3807 2023-05-19 18:23:02.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-05-19 18:23:02.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3282 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9051 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_layer.py
--rw-r--r--   0 root         (0) root         (0)     9078 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_metadata.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9141 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    25904 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     3320 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_metadata.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9363 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-05-19 18:23:13.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     4236 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     2639 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-05-19 18:23:20.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-05-19 18:23:20.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-05-19 18:23:20.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-05-19 18:23:17.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-05-19 18:23:17.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-05-19 18:23:18.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.661561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17482 2023-05-19 18:23:26.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-05-19 18:23:25.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-05-19 18:23:26.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-05-19 18:23:28.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-05-19 18:23:25.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-05-19 18:23:25.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-05-19 18:23:29.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/
--rw-r--r--   0 root         (0) root         (0)      521 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15568 2023-05-19 18:23:26.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15504 2023-05-19 18:23:27.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/
--rw-r--r--   0 root         (0) root         (0)      483 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15478 2023-05-19 18:23:27.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-19 18:23:28.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-05-19 18:23:22.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.665561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.669561 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-05-19 18:23:15.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-05-19 18:23:15.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.645561 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17214 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-19 18:25:52.000000 iparapheur-provisioning-1.6.1/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.645561 iparapheur-provisioning-1.6.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.673561 iparapheur-provisioning-1.6.1/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:32.000000 iparapheur-provisioning-1.6.1/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-19 18:22:59.000000 iparapheur-provisioning-1.6.1/test/test_models/test_composite_id.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-19 18:23:00.000000 iparapheur-provisioning-1.6.1/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-19 18:23:01.000000 iparapheur-provisioning-1.6.1/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-19 18:23:02.000000 iparapheur-provisioning-1.6.1/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-05-19 18:23:03.000000 iparapheur-provisioning-1.6.1/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-19 18:23:04.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-19 18:23:05.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_layer.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_metadata.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-19 18:23:06.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-05-19 18:23:07.000000 iparapheur-provisioning-1.6.1/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-19 18:23:08.000000 iparapheur-provisioning-1.6.1/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-19 18:23:09.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_metadata.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-19 18:23:10.000000 iparapheur-provisioning-1.6.1/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-19 18:23:11.000000 iparapheur-provisioning-1.6.1/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/test/test_models/test_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-19 18:23:12.000000 iparapheur-provisioning-1.6.1/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-19 18:23:13.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-19 18:23:14.000000 iparapheur-provisioning-1.6.1/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.673561 iparapheur-provisioning-1.6.1/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.673561 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-19 18:23:21.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-19 18:23:19.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/__init__.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1121 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.677562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-19 18:23:30.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-19 18:23:24.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 18:25:52.681562 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-19 18:23:16.000000 iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.981750 iparapheur-provisioning-1.6.2/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-25 14:10:15.981750 iparapheur-provisioning-1.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17390 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.945749 iparapheur-provisioning-1.6.2/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.949750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.949750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.949750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-05-25 14:06:11.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    30320 2023-05-25 14:06:12.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-05-25 14:06:13.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-05-25 14:06:13.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2023-05-25 14:06:13.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    28616 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-25 14:06:19.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-05-25 14:06:19.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-05-25 14:06:19.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-05-25 14:06:20.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     3734 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-05-25 14:06:27.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-05-25 14:06:27.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-05-25 14:06:25.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-05-25 14:06:25.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.957750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-05-25 14:06:36.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-05-25 14:06:33.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-05-25 14:06:34.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-05-25 14:06:35.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-05-25 14:06:35.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-05-25 14:06:33.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-05-25 14:06:34.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-05-25 14:06:35.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-05-25 14:06:30.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-05-25 14:06:29.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-25 14:06:30.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-05-25 14:06:29.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-05-25 14:06:23.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.961750 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-05-25 14:06:22.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-05-25 14:06:22.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-05-25 14:06:23.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-05-25 14:06:39.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.949750 iparapheur-provisioning-1.6.2/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-25 14:10:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13603 2023-05-25 14:10:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 14:10:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-25 14:10:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 14:10:15.000000 iparapheur-provisioning-1.6.2/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-25 14:10:15.981750 iparapheur-provisioning-1.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.945749 iparapheur-provisioning-1.6.2/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-25 14:06:11.000000 iparapheur-provisioning-1.6.2/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-25 14:06:13.000000 iparapheur-provisioning-1.6.2/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-25 14:06:13.000000 iparapheur-provisioning-1.6.2/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-25 14:06:13.000000 iparapheur-provisioning-1.6.2/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-25 14:06:14.000000 iparapheur-provisioning-1.6.2/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-25 14:06:15.000000 iparapheur-provisioning-1.6.2/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-25 14:06:16.000000 iparapheur-provisioning-1.6.2/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-25 14:06:17.000000 iparapheur-provisioning-1.6.2/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-25 14:06:18.000000 iparapheur-provisioning-1.6.2/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-25 14:06:19.000000 iparapheur-provisioning-1.6.2/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-25 14:06:19.000000 iparapheur-provisioning-1.6.2/test/test_models/test_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-25 14:06:19.000000 iparapheur-provisioning-1.6.2/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-05-25 14:06:20.000000 iparapheur-provisioning-1.6.2/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-25 14:06:21.000000 iparapheur-provisioning-1.6.2/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-05-25 14:06:28.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-25 14:06:26.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.973750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.977750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.977750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-25 14:06:37.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.977750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-25 14:06:38.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.977750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.977750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-05-25 14:06:31.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.977750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:10:15.981750 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-05-25 14:06:24.000000 iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.6.1/LICENSE.md` & `iparapheur-provisioning-1.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/README.md` & `iparapheur-provisioning-1.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.6.1
+- Package version: 1.6.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
@@ -188,14 +188,15 @@
 *AdminAllUsersApi* | [**get_user_as_super_admin**](docs/apis/tags/AdminAllUsersApi.md#get_user_as_super_admin) | **get** /api/provisioning/v1/admin/user/{userId} | Get a full user representation
 *AdminAllUsersApi* | [**list_users_as_super_admin**](docs/apis/tags/AdminAllUsersApi.md#list_users_as_super_admin) | **get** /api/provisioning/v1/admin/user | List all users on the instance
 *AdminAllUsersApi* | [**update_user_as_super_admin**](docs/apis/tags/AdminAllUsersApi.md#update_user_as_super_admin) | **put** /api/provisioning/v1/admin/user/{userId} | Edit a user
 *AdminDeskApi* | [**create_desk**](docs/apis/tags/AdminDeskApi.md#create_desk) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/desk | Create a desk
 *AdminDeskApi* | [**delete_desk**](docs/apis/tags/AdminDeskApi.md#delete_desk) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Delete a desk
 *AdminDeskApi* | [**edit_desk**](docs/apis/tags/AdminDeskApi.md#edit_desk) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Edit a desk
 *AdminDeskApi* | [**get_desk_as_admin**](docs/apis/tags/AdminDeskApi.md#get_desk_as_admin) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId} | Get a full desk description
+*AdminDeskApi* | [**list_desks**](docs/apis/tags/AdminDeskApi.md#list_desks) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/desk | List desks
 *AdminTenantApi* | [**create_tenant**](docs/apis/tags/AdminTenantApi.md#create_tenant) | **post** /api/provisioning/v1/admin/tenant | Create a new tenant
 *AdminTenantApi* | [**delete_tenant**](docs/apis/tags/AdminTenantApi.md#delete_tenant) | **delete** /api/provisioning/v1/admin/tenant/{tenantId} | Delete a tenant
 *AdminTenantApi* | [**get_tenant**](docs/apis/tags/AdminTenantApi.md#get_tenant) | **get** /api/provisioning/v1/admin/tenant/{tenantId} | Get a full tenant description
 *AdminTenantApi* | [**update_tenant**](docs/apis/tags/AdminTenantApi.md#update_tenant) | **put** /api/provisioning/v1/admin/tenant/{tenantId} | Edit a tenant
 *AdminTenantUserApi* | [**create_user**](docs/apis/tags/AdminTenantUserApi.md#create_user) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/user | Create a new user
 *AdminTenantUserApi* | [**get_user**](docs/apis/tags/AdminTenantUserApi.md#get_user) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/user/{userId} | Get a full user description
 *AdminTenantUserApi* | [**list_tenant_users**](docs/apis/tags/AdminTenantUserApi.md#list_tenant_users) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/user | List all users associated with the tenant
@@ -203,61 +204,49 @@
 *AdminTenantUserApi* | [**update_user**](docs/apis/tags/AdminTenantUserApi.md#update_user) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/user/{userId} | Edit a user
 *AdminTypologyApi* | [**create_subtype**](docs/apis/tags/AdminTypologyApi.md#create_subtype) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype | Create a subtype
 *AdminTypologyApi* | [**create_type**](docs/apis/tags/AdminTypologyApi.md#create_type) | **post** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type | Create a type
 *AdminTypologyApi* | [**delete_subtype**](docs/apis/tags/AdminTypologyApi.md#delete_subtype) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Delete a subtype
 *AdminTypologyApi* | [**delete_type**](docs/apis/tags/AdminTypologyApi.md#delete_type) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Delete a type
 *AdminTypologyApi* | [**get_subtype**](docs/apis/tags/AdminTypologyApi.md#get_subtype) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Get a subtype with every information set
 *AdminTypologyApi* | [**get_type**](docs/apis/tags/AdminTypologyApi.md#get_type) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Get a type with every information set
-*AdminTypologyApi* | [**get_typology_hierarchy**](docs/apis/tags/AdminTypologyApi.md#get_typology_hierarchy) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology | Get typology list, sorted by hierarchy.
-*AdminTypologyApi* | [**list_creation_permitted_desks**](docs/apis/tags/AdminTypologyApi.md#list_creation_permitted_desks) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/creationPermittedDesks | List the desks permitted to use this subtype in a folder creation.
-*AdminTypologyApi* | [**list_filterable_by_desks**](docs/apis/tags/AdminTypologyApi.md#list_filterable_by_desks) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/filterableByDesks | List the desks permitted to use this subtype in a filter.
-*AdminTypologyApi* | [**list_layers_from_subtype**](docs/apis/tags/AdminTypologyApi.md#list_layers_from_subtype) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/layer | List the layers associated with the given subtype
-*AdminTypologyApi* | [**list_metadata_from_subtype**](docs/apis/tags/AdminTypologyApi.md#list_metadata_from_subtype) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/metadata | List the metadata associated with the given subtype
 *AdminTypologyApi* | [**list_subtypes**](docs/apis/tags/AdminTypologyApi.md#list_subtypes) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype | Get subtypes
 *AdminTypologyApi* | [**list_types**](docs/apis/tags/AdminTypologyApi.md#list_types) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type | List types
 *AdminTypologyApi* | [**update_subtype**](docs/apis/tags/AdminTypologyApi.md#update_subtype) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Edit a subtype
 *AdminTypologyApi* | [**update_type**](docs/apis/tags/AdminTypologyApi.md#update_type) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Edit a type
 
 ## Documentation For Models
 
- - [CompositeId](docs/models/CompositeId.md)
  - [DelegationSortBy](docs/models/DelegationSortBy.md)
  - [DeskDto](docs/models/DeskDto.md)
  - [DeskRepresentation](docs/models/DeskRepresentation.md)
  - [ErrorResponse](docs/models/ErrorResponse.md)
- - [ExternalSignatureConfig](docs/models/ExternalSignatureConfig.md)
+ - [ExternalSignatureConfigRepresentation](docs/models/ExternalSignatureConfigRepresentation.md)
  - [ExternalSignatureConfigSortBy](docs/models/ExternalSignatureConfigSortBy.md)
  - [ExternalSignatureProvider](docs/models/ExternalSignatureProvider.md)
  - [FolderSortBy](docs/models/FolderSortBy.md)
  - [InternalMetadata](docs/models/InternalMetadata.md)
  - [LayerRepresentation](docs/models/LayerRepresentation.md)
  - [LayerSortBy](docs/models/LayerSortBy.md)
- - [Metadata](docs/models/Metadata.md)
  - [MetadataDto](docs/models/MetadataDto.md)
  - [MetadataRepresentation](docs/models/MetadataRepresentation.md)
  - [MetadataSortBy](docs/models/MetadataSortBy.md)
  - [MetadataType](docs/models/MetadataType.md)
  - [PageDeskRepresentation](docs/models/PageDeskRepresentation.md)
- - [PageSubtypeLayer](docs/models/PageSubtypeLayer.md)
- - [PageSubtypeMetadata](docs/models/PageSubtypeMetadata.md)
  - [PageSubtypeRepresentation](docs/models/PageSubtypeRepresentation.md)
  - [PageTypeRepresentation](docs/models/PageTypeRepresentation.md)
- - [PageTypologyRepresentation](docs/models/PageTypologyRepresentation.md)
  - [PageUserRepresentation](docs/models/PageUserRepresentation.md)
  - [PageableObject](docs/models/PageableObject.md)
  - [PdfSignaturePosition](docs/models/PdfSignaturePosition.md)
  - [SealCertificateSortBy](docs/models/SealCertificateSortBy.md)
  - [SignatureFormat](docs/models/SignatureFormat.md)
  - [SignatureProtocol](docs/models/SignatureProtocol.md)
  - [SortObject](docs/models/SortObject.md)
  - [SubtypeDto](docs/models/SubtypeDto.md)
- - [SubtypeLayer](docs/models/SubtypeLayer.md)
  - [SubtypeLayerAssociation](docs/models/SubtypeLayerAssociation.md)
  - [SubtypeLayerDto](docs/models/SubtypeLayerDto.md)
- - [SubtypeMetadata](docs/models/SubtypeMetadata.md)
  - [SubtypeMetadataDto](docs/models/SubtypeMetadataDto.md)
  - [SubtypeRepresentation](docs/models/SubtypeRepresentation.md)
  - [TenantDto](docs/models/TenantDto.md)
  - [TenantRepresentation](docs/models/TenantRepresentation.md)
  - [TenantSortBy](docs/models/TenantSortBy.md)
  - [TypeDto](docs/models/TypeDto.md)
  - [TypeRepresentation](docs/models/TypeRepresentation.md)
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.1/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.2/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/path_to_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import ApiProvisioningV1AdminTenantTenantIdDeskDeskId
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant import ApiProvisioningV1AdminTenant
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_user import ApiProvisioningV1AdminTenantTenantIdUser
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import ApiProvisioningV1AdminTenantTenantIdTypologyType
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import ApiProvisioningV1AdminTenantTenantIdDesk
 from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_user import ApiProvisioningV1AdminUser
-from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology import ApiProvisioningV1AdminTenantTenantIdTypology
-from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdMetadata
-from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdLayer
-from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdFilterableByDesks
-from iparapheur_provisioning.apis.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks import ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdCreationPermittedDesks
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.API_PROVISIONING_V1_ADMIN_USER_USER_ID: ApiProvisioningV1AdminUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID: ApiProvisioningV1AdminTenantTenantId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER_USER_ID: ApiProvisioningV1AdminTenantTenantIdUserUserId,
@@ -30,19 +25,14 @@
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID: ApiProvisioningV1AdminTenantTenantIdDeskDeskId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT: ApiProvisioningV1AdminTenant,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER: ApiProvisioningV1AdminTenantTenantIdUser,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE: ApiProvisioningV1AdminTenantTenantIdTypologyType,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK: ApiProvisioningV1AdminTenantTenantIdDesk,
         PathValues.API_PROVISIONING_V1_ADMIN_USER: ApiProvisioningV1AdminUser,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY: ApiProvisioningV1AdminTenantTenantIdTypology,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_METADATA: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdMetadata,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_LAYER: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdLayer,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_FILTERABLE_BY_DESKS: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdFilterableByDesks,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_CREATION_PERMITTED_DESKS: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdCreationPermittedDesks,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.API_PROVISIONING_V1_ADMIN_USER_USER_ID: ApiProvisioningV1AdminUserUserId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID: ApiProvisioningV1AdminTenantTenantId,
@@ -52,14 +42,9 @@
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID: ApiProvisioningV1AdminTenantTenantIdDeskDeskId,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT: ApiProvisioningV1AdminTenant,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER: ApiProvisioningV1AdminTenantTenantIdUser,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE: ApiProvisioningV1AdminTenantTenantIdTypologyType,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype,
         PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK: ApiProvisioningV1AdminTenantTenantIdDesk,
         PathValues.API_PROVISIONING_V1_ADMIN_USER: ApiProvisioningV1AdminUser,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY: ApiProvisioningV1AdminTenantTenantIdTypology,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_METADATA: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdMetadata,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_LAYER: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdLayer,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_FILTERABLE_BY_DESKS: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdFilterableByDesks,
-        PathValues.API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_CREATION_PERMITTED_DESKS: ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdCreationPermittedDesks,
     }
 )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     Generated by: https://openapi-generator.tech
 """
 
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk.post import CreateDesk
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.delete import DeleteDesk
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.put import EditDesk
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.get import GetDeskAsAdmin
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk.get import ListDesks
 
 
 class AdminDeskApi(
     CreateDesk,
     DeleteDesk,
     EditDesk,
     GetDeskAsAdmin,
+    ListDesks,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     pass
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,37 +12,27 @@
 
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.post import CreateSubtype
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type.post import CreateType
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.delete import DeleteSubtype
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.delete import DeleteType
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.get import GetSubtype
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.get import GetType
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology.get import GetTypologyHierarchy
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks.get import ListCreationPermittedDesks
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks.get import ListFilterableByDesks
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer.get import ListLayersFromSubtype
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata.get import ListMetadataFromSubtype
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.get import ListSubtypes
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type.get import ListTypes
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.put import UpdateSubtype
 from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.put import UpdateType
 
 
 class AdminTypologyApi(
     CreateSubtype,
     CreateType,
     DeleteSubtype,
     DeleteType,
     GetSubtype,
     GetType,
-    GetTypologyHierarchy,
-    ListCreationPermittedDesks,
-    ListFilterableByDesks,
-    ListLayersFromSubtype,
-    ListMetadataFromSubtype,
     ListSubtypes,
     ListTypes,
     UpdateSubtype,
     UpdateType,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.6.1".\
+               "SDK Package Version: 1.6.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/composite_id.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/sort_object.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,60 +20,80 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class CompositeId(
+class SortObject(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         
         class properties:
-            metadataId = schemas.StrSchema
+            empty = schemas.BoolSchema
+            unsorted = schemas.BoolSchema
+            sorted = schemas.BoolSchema
             __annotations__ = {
-                "metadataId": metadataId,
+                "empty": empty,
+                "unsorted": unsorted,
+                "sorted": sorted,
             }
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["metadataId"]) -> MetaOapg.properties.metadataId: ...
+    def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["unsorted"]) -> MetaOapg.properties.unsorted: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["sorted"]) -> MetaOapg.properties.sorted: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["metadataId", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["metadataId"]) -> typing.Union[MetaOapg.properties.metadataId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["unsorted"]) -> typing.Union[MetaOapg.properties.unsorted, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["sorted"]) -> typing.Union[MetaOapg.properties.sorted, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["metadataId", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        metadataId: typing.Union[MetaOapg.properties.metadataId, str, schemas.Unset] = schemas.unset,
+        empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
+        unsorted: typing.Union[MetaOapg.properties.unsorted, bool, schemas.Unset] = schemas.unset,
+        sorted: typing.Union[MetaOapg.properties.sorted, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'CompositeId':
+    ) -> 'SortObject':
         return super().__new__(
             cls,
             *_args,
-            metadataId=metadataId,
+            empty=empty,
+            unsorted=unsorted,
+            sorted=sorted,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/desk_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
             
             
             class shortName(
                 schemas.StrSchema
             ):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/desk_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             tenantId = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
                 "tenantId": tenantId,
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,158 +20,189 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class ExternalSignatureConfig(
+class MetadataDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+            "key",
+        }
         
         class properties:
+            
+            
+            class name(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
+            
+            
+            class key(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 128
+                    min_length = 1
             id = schemas.StrSchema
-            name = schemas.StrSchema
+            
+            
+            class index(
+                schemas.Int32Base,
+                schemas.IntBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneDecimalMixin
+            ):
+            
+            
+                class MetaOapg:
+                    format = 'int32'
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[None, decimal.Decimal, int, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'index':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
         
             @staticmethod
-            def serviceName() -> typing.Type['ExternalSignatureProvider']:
-                return ExternalSignatureProvider
-            url = schemas.StrSchema
-            token = schemas.StrSchema
-            password = schemas.StrSchema
-            login = schemas.StrSchema
+            def type() -> typing.Type['MetadataType']:
+                return MetadataType
             
             
-            class transactionIds(
+            class restrictedValues(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    unique_items = True
                     items = schemas.StrSchema
             
                 def __new__(
                     cls,
                     _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'transactionIds':
+                ) -> 'restrictedValues':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
             __annotations__ = {
-                "id": id,
                 "name": name,
-                "serviceName": serviceName,
-                "url": url,
-                "token": token,
-                "password": password,
-                "login": login,
-                "transactionIds": transactionIds,
+                "key": key,
+                "id": id,
+                "index": index,
+                "type": type,
+                "restrictedValues": restrictedValues,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    name: MetaOapg.properties.name
+    key: MetaOapg.properties.key
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["serviceName"]) -> 'ExternalSignatureProvider': ...
+    def __getitem__(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["token"]) -> MetaOapg.properties.token: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["password"]) -> MetaOapg.properties.password: ...
+    def __getitem__(self, name: typing_extensions.Literal["index"]) -> MetaOapg.properties.index: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["login"]) -> MetaOapg.properties.login: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> 'MetadataType': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["transactionIds"]) -> MetaOapg.properties.transactionIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["restrictedValues"]) -> MetaOapg.properties.restrictedValues: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "serviceName", "url", "token", "password", "login", "transactionIds", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "key", "id", "index", "type", "restrictedValues", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["serviceName"]) -> typing.Union['ExternalSignatureProvider', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["url"]) -> typing.Union[MetaOapg.properties.url, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["token"]) -> typing.Union[MetaOapg.properties.token, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["password"]) -> typing.Union[MetaOapg.properties.password, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["index"]) -> typing.Union[MetaOapg.properties.index, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["login"]) -> typing.Union[MetaOapg.properties.login, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> typing.Union['MetadataType', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["transactionIds"]) -> typing.Union[MetaOapg.properties.transactionIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["restrictedValues"]) -> typing.Union[MetaOapg.properties.restrictedValues, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "serviceName", "url", "token", "password", "login", "transactionIds", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "key", "id", "index", "type", "restrictedValues", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        key: typing.Union[MetaOapg.properties.key, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        serviceName: typing.Union['ExternalSignatureProvider', schemas.Unset] = schemas.unset,
-        url: typing.Union[MetaOapg.properties.url, str, schemas.Unset] = schemas.unset,
-        token: typing.Union[MetaOapg.properties.token, str, schemas.Unset] = schemas.unset,
-        password: typing.Union[MetaOapg.properties.password, str, schemas.Unset] = schemas.unset,
-        login: typing.Union[MetaOapg.properties.login, str, schemas.Unset] = schemas.unset,
-        transactionIds: typing.Union[MetaOapg.properties.transactionIds, list, tuple, schemas.Unset] = schemas.unset,
+        index: typing.Union[MetaOapg.properties.index, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        type: typing.Union['MetadataType', schemas.Unset] = schemas.unset,
+        restrictedValues: typing.Union[MetaOapg.properties.restrictedValues, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ExternalSignatureConfig':
+    ) -> 'MetadataDto':
         return super().__new__(
             cls,
             *_args,
-            id=id,
             name=name,
-            serviceName=serviceName,
-            url=url,
-            token=token,
-            password=password,
-            login=login,
-            transactionIds=transactionIds,
+            key=key,
+            id=id,
+            index=index,
+            type=type,
+            restrictedValues=restrictedValues,
             _configuration=_configuration,
             **kwargs,
         )
 
-from iparapheur_provisioning.model.external_signature_provider import ExternalSignatureProvider
+from iparapheur_provisioning.model.metadata_type import MetadataType
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/layer_representation.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_representation.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,137 +20,157 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class Metadata(
+class MetadataRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+            "key",
+        }
         
         class properties:
+            
+            
+            class name(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
+            
+            
+            class key(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 128
+                    min_length = 1
             id = schemas.StrSchema
-            key = schemas.StrSchema
-            name = schemas.StrSchema
-            index = schemas.Int32Schema
-        
-            @staticmethod
-            def type() -> typing.Type['MetadataType']:
-                return MetadataType
             
             
-            class restrictedValues(
-                schemas.ListSchema
+            class index(
+                schemas.Int32Base,
+                schemas.IntBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneDecimalMixin
             ):
             
             
                 class MetaOapg:
-                    items = schemas.StrSchema
+                    format = 'int32'
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'restrictedValues':
+                ) -> 'index':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
+        
+            @staticmethod
+            def type() -> typing.Type['MetadataType']:
+                return MetadataType
             __annotations__ = {
-                "id": id,
-                "key": key,
                 "name": name,
+                "key": key,
+                "id": id,
                 "index": index,
                 "type": type,
-                "restrictedValues": restrictedValues,
             }
     
+    name: MetaOapg.properties.name
+    key: MetaOapg.properties.key
+    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["index"]) -> MetaOapg.properties.index: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> 'MetadataType': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["restrictedValues"]) -> MetaOapg.properties.restrictedValues: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "key", "name", "index", "type", "restrictedValues", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "key", "id", "index", "type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["key"]) -> typing.Union[MetaOapg.properties.key, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["index"]) -> typing.Union[MetaOapg.properties.index, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> typing.Union['MetadataType', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["restrictedValues"]) -> typing.Union[MetaOapg.properties.restrictedValues, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "key", "name", "index", "type", "restrictedValues", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "key", "id", "index", "type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        key: typing.Union[MetaOapg.properties.key, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        key: typing.Union[MetaOapg.properties.key, str, schemas.Unset] = schemas.unset,
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        index: typing.Union[MetaOapg.properties.index, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        index: typing.Union[MetaOapg.properties.index, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         type: typing.Union['MetadataType', schemas.Unset] = schemas.unset,
-        restrictedValues: typing.Union[MetaOapg.properties.restrictedValues, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'Metadata':
+    ) -> 'MetadataRepresentation':
         return super().__new__(
             cls,
             *_args,
-            id=id,
-            key=key,
             name=name,
+            key=key,
+            id=id,
             index=index,
             type=type,
-            restrictedValues=restrictedValues,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.metadata_type import MetadataType
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/typology_representation.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,158 +20,107 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class MetadataRepresentation(
+class TypologyRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
             "name",
-            "key",
         }
         
         class properties:
             
             
             class name(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
-            
-            
-            class key(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 128
-                    min_length = 1
             id = schemas.StrSchema
-            
-            
-            class index(
-                schemas.Int32Base,
-                schemas.IntBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneDecimalMixin
-            ):
-            
-            
-                class MetaOapg:
-                    format = 'int32'
-            
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[None, decimal.Decimal, int, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'index':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                    )
-        
-            @staticmethod
-            def type() -> typing.Type['MetadataType']:
-                return MetadataType
+            parentId = schemas.StrSchema
+            childrenCount = schemas.Int32Schema
             __annotations__ = {
                 "name": name,
-                "key": key,
                 "id": id,
-                "index": index,
-                "type": type,
+                "parentId": parentId,
+                "childrenCount": childrenCount,
             }
     
     name: MetaOapg.properties.name
-    key: MetaOapg.properties.key
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["index"]) -> MetaOapg.properties.index: ...
+    def __getitem__(self, name: typing_extensions.Literal["parentId"]) -> MetaOapg.properties.parentId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["type"]) -> 'MetadataType': ...
+    def __getitem__(self, name: typing_extensions.Literal["childrenCount"]) -> MetaOapg.properties.childrenCount: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "key", "id", "index", "type", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "parentId", "childrenCount", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["key"]) -> MetaOapg.properties.key: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["index"]) -> typing.Union[MetaOapg.properties.index, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["parentId"]) -> typing.Union[MetaOapg.properties.parentId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> typing.Union['MetadataType', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["childrenCount"]) -> typing.Union[MetaOapg.properties.childrenCount, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "key", "id", "index", "type", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "parentId", "childrenCount", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
-        key: typing.Union[MetaOapg.properties.key, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        index: typing.Union[MetaOapg.properties.index, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        type: typing.Union['MetadataType', schemas.Unset] = schemas.unset,
+        parentId: typing.Union[MetaOapg.properties.parentId, str, schemas.Unset] = schemas.unset,
+        childrenCount: typing.Union[MetaOapg.properties.childrenCount, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MetadataRepresentation':
+    ) -> 'TypologyRepresentation':
         return super().__new__(
             cls,
             *_args,
             name=name,
-            key=key,
             id=id,
-            index=index,
-            type=type,
+            parentId=parentId,
+            childrenCount=childrenCount,
             _configuration=_configuration,
             **kwargs,
         )
-
-from iparapheur_provisioning.model.metadata_type import MetadataType
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_layer.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class PageSubtypeLayer(
+class PageSubtypeRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -46,29 +46,29 @@
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SubtypeLayer']:
-                        return SubtypeLayer
+                    def items() -> typing.Type['SubtypeRepresentation']:
+                        return SubtypeRepresentation
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['SubtypeLayer'], typing.List['SubtypeLayer']],
+                    _arg: typing.Union[typing.Tuple['SubtypeRepresentation'], typing.List['SubtypeRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'content':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SubtypeLayer':
+                def __getitem__(self, i: int) -> 'SubtypeRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
             first = schemas.BoolSchema
@@ -186,15 +186,15 @@
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PageSubtypeLayer':
+    ) -> 'PageSubtypeRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
@@ -207,8 +207,8 @@
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
-from iparapheur_provisioning.model.subtype_layer import SubtypeLayer
+from iparapheur_provisioning.model.subtype_representation import SubtypeRepresentation
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_metadata.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_type_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class PageSubtypeMetadata(
+class PageTypeRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -46,29 +46,29 @@
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SubtypeMetadata']:
-                        return SubtypeMetadata
+                    def items() -> typing.Type['TypeRepresentation']:
+                        return TypeRepresentation
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['SubtypeMetadata'], typing.List['SubtypeMetadata']],
+                    _arg: typing.Union[typing.Tuple['TypeRepresentation'], typing.List['TypeRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'content':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SubtypeMetadata':
+                def __getitem__(self, i: int) -> 'TypeRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
             first = schemas.BoolSchema
@@ -186,15 +186,15 @@
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PageSubtypeMetadata':
+    ) -> 'PageTypeRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
@@ -207,8 +207,8 @@
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
-from iparapheur_provisioning.model.subtype_metadata import SubtypeMetadata
+from iparapheur_provisioning.model.type_representation import TypeRepresentation
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/page_user_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class PageSubtypeRepresentation(
+class PageUserRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
@@ -46,29 +46,29 @@
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SubtypeRepresentation']:
-                        return SubtypeRepresentation
+                    def items() -> typing.Type['UserRepresentation']:
+                        return UserRepresentation
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['SubtypeRepresentation'], typing.List['SubtypeRepresentation']],
+                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'content':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SubtypeRepresentation':
+                def __getitem__(self, i: int) -> 'UserRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
             first = schemas.BoolSchema
@@ -186,15 +186,15 @@
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
         numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PageSubtypeRepresentation':
+    ) -> 'PageUserRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
@@ -207,8 +207,8 @@
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
-from iparapheur_provisioning.model.subtype_representation import SubtypeRepresentation
+from iparapheur_provisioning.model.user_representation import UserRepresentation
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/type_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,195 +20,217 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class PageTypeRepresentation(
+class TypeDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+        }
         
         class properties:
-            totalElements = schemas.Int64Schema
-            totalPages = schemas.Int32Schema
-            size = schemas.Int32Schema
             
             
-            class content(
-                schemas.ListSchema
+            class name(
+                schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['TypeRepresentation']:
-                        return TypeRepresentation
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
+            id = schemas.StrSchema
+            
+            
+            class description(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 3
+        
+            @staticmethod
+            def signatureFormat() -> typing.Type['SignatureFormat']:
+                return SignatureFormat
+        
+            @staticmethod
+            def protocol() -> typing.Type['SignatureProtocol']:
+                return SignatureProtocol
+            signatureVisible = schemas.BoolSchema
+        
+            @staticmethod
+            def signaturePosition() -> typing.Type['PdfSignaturePosition']:
+                return PdfSignaturePosition
+            
+            
+            class signatureLocation(
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
+            ):
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['TypeRepresentation'], typing.List['TypeRepresentation']],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'content':
+                ) -> 'signatureLocation':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'TypeRepresentation':
-                    return super().__getitem__(i)
-            number = schemas.Int32Schema
-        
-            @staticmethod
-            def sort() -> typing.Type['SortObject']:
-                return SortObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
-            numberOfElements = schemas.Int32Schema
-        
-            @staticmethod
-            def pageable() -> typing.Type['PageableObject']:
-                return PageableObject
-            empty = schemas.BoolSchema
+            
+            class signatureZipCode(
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
+            ):
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[None, str, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'signatureZipCode':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
             __annotations__ = {
-                "totalElements": totalElements,
-                "totalPages": totalPages,
-                "size": size,
-                "content": content,
-                "number": number,
-                "sort": sort,
-                "first": first,
-                "last": last,
-                "numberOfElements": numberOfElements,
-                "pageable": pageable,
-                "empty": empty,
+                "name": name,
+                "id": id,
+                "description": description,
+                "signatureFormat": signatureFormat,
+                "protocol": protocol,
+                "signatureVisible": signatureVisible,
+                "signaturePosition": signaturePosition,
+                "signatureLocation": signatureLocation,
+                "signatureZipCode": signatureZipCode,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["totalPages"]) -> MetaOapg.properties.totalPages: ...
+    name: MetaOapg.properties.name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["content"]) -> MetaOapg.properties.content: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["signatureFormat"]) -> 'SignatureFormat': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["protocol"]) -> 'SignatureProtocol': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["signatureVisible"]) -> MetaOapg.properties.signatureVisible: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["signaturePosition"]) -> 'PdfSignaturePosition': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["signatureLocation"]) -> MetaOapg.properties.signatureLocation: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
+    def __getitem__(self, name: typing_extensions.Literal["signatureZipCode"]) -> MetaOapg.properties.signatureZipCode: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "signatureFormat", "protocol", "signatureVisible", "signaturePosition", "signatureLocation", "signatureZipCode", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["totalPages"]) -> typing.Union[MetaOapg.properties.totalPages, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["size"]) -> typing.Union[MetaOapg.properties.size, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["content"]) -> typing.Union[MetaOapg.properties.content, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["signatureFormat"]) -> typing.Union['SignatureFormat', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["protocol"]) -> typing.Union['SignatureProtocol', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["signatureVisible"]) -> typing.Union[MetaOapg.properties.signatureVisible, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["signaturePosition"]) -> typing.Union['PdfSignaturePosition', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["signatureLocation"]) -> typing.Union[MetaOapg.properties.signatureLocation, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["signatureZipCode"]) -> typing.Union[MetaOapg.properties.signatureZipCode, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "signatureFormat", "protocol", "signatureVisible", "signaturePosition", "signatureLocation", "signatureZipCode", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
-        number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
-        last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
-        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
-        empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        signatureFormat: typing.Union['SignatureFormat', schemas.Unset] = schemas.unset,
+        protocol: typing.Union['SignatureProtocol', schemas.Unset] = schemas.unset,
+        signatureVisible: typing.Union[MetaOapg.properties.signatureVisible, bool, schemas.Unset] = schemas.unset,
+        signaturePosition: typing.Union['PdfSignaturePosition', schemas.Unset] = schemas.unset,
+        signatureLocation: typing.Union[MetaOapg.properties.signatureLocation, None, str, schemas.Unset] = schemas.unset,
+        signatureZipCode: typing.Union[MetaOapg.properties.signatureZipCode, None, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PageTypeRepresentation':
+    ) -> 'TypeDto':
         return super().__new__(
             cls,
             *_args,
-            totalElements=totalElements,
-            totalPages=totalPages,
-            size=size,
-            content=content,
-            number=number,
-            sort=sort,
-            first=first,
-            last=last,
-            numberOfElements=numberOfElements,
-            pageable=pageable,
-            empty=empty,
+            name=name,
+            id=id,
+            description=description,
+            signatureFormat=signatureFormat,
+            protocol=protocol,
+            signatureVisible=signatureVisible,
+            signaturePosition=signaturePosition,
+            signatureLocation=signatureLocation,
+            signatureZipCode=signatureZipCode,
             _configuration=_configuration,
             **kwargs,
         )
 
-from iparapheur_provisioning.model.pageable_object import PageableObject
-from iparapheur_provisioning.model.sort_object import SortObject
-from iparapheur_provisioning.model.type_representation import TypeRepresentation
+from iparapheur_provisioning.model.pdf_signature_position import PdfSignaturePosition
+from iparapheur_provisioning.model.signature_format import SignatureFormat
+from iparapheur_provisioning.model.signature_protocol import SignatureProtocol
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/type_representation.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,80 +20,106 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class SortObject(
+class TypeRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+        }
         
         class properties:
-            empty = schemas.BoolSchema
-            unsorted = schemas.BoolSchema
-            sorted = schemas.BoolSchema
+            
+            
+            class name(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
+            id = schemas.StrSchema
+            
+            
+            class description(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 3
             __annotations__ = {
-                "empty": empty,
-                "unsorted": unsorted,
-                "sorted": sorted,
+                "name": name,
+                "id": id,
+                "description": description,
             }
     
+    name: MetaOapg.properties.name
+    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["unsorted"]) -> MetaOapg.properties.unsorted: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sorted"]) -> MetaOapg.properties.sorted: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["unsorted"]) -> typing.Union[MetaOapg.properties.unsorted, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sorted"]) -> typing.Union[MetaOapg.properties.sorted, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
-        unsorted: typing.Union[MetaOapg.properties.unsorted, bool, schemas.Unset] = schemas.unset,
-        sorted: typing.Union[MetaOapg.properties.sorted, bool, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SortObject':
+    ) -> 'TypeRepresentation':
         return super().__new__(
             cls,
             *_args,
-            empty=empty,
-            unsorted=unsorted,
-            sorted=sorted,
+            name=name,
+            id=id,
+            description=description,
             _configuration=_configuration,
             **kwargs,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             
             
             class description(
                 schemas.StrSchema
             ):
@@ -228,89 +227,159 @@
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
         
             @staticmethod
-            def externalSignatureConfig() -> typing.Type['ExternalSignatureConfig']:
-                return ExternalSignatureConfig
+            def externalSignatureConfig() -> typing.Type['ExternalSignatureConfigRepresentation']:
+                return ExternalSignatureConfigRepresentation
             
             
-            class parentTypeId(
-                schemas.StrBase,
+            class creationPermittedDeskIds(
+                schemas.ListBase,
                 schemas.NoneBase,
                 schemas.Schema,
-                schemas.NoneStrMixin
+                schemas.NoneTupleMixin
             ):
             
             
+                class MetaOapg:
+                    
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
+            
+            
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, str, ],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'parentTypeId':
+                ) -> 'creationPermittedDeskIds':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
-        
-            @staticmethod
-            def parentType() -> typing.Type['TypeRepresentation']:
-                return TypeRepresentation
             
             
-            class creationPermittedDeskIds(
-                schemas.ListSchema
+            class creationPermittedDesks(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
-                    items = schemas.StrSchema
+                    
+                    @staticmethod
+                    def items() -> typing.Type['DeskRepresentation']:
+                        return DeskRepresentation
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'creationPermittedDeskIds':
+                ) -> 'creationPermittedDesks':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            
             
             class filterableByDeskIds(
-                schemas.ListSchema
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
-                    items = schemas.StrSchema
+                    
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'filterableByDeskIds':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
+            
+            class filterableByDesks(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['DeskRepresentation']:
+                        return DeskRepresentation
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[list, tuple, None, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'filterableByDesks':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
             maxMainDocuments = schemas.Int32Schema
-            annexeIncluded = schemas.BoolSchema
             multiDocuments = schemas.BoolSchema
+            annexeIncluded = schemas.BoolSchema
             digitalSignatureMandatory = schemas.BoolSchema
             readingMandatory = schemas.BoolSchema
             sealAutomatic = schemas.BoolSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
                 "description": description,
@@ -321,21 +390,21 @@
                 "externalSignatureAutomatic": externalSignatureAutomatic,
                 "secureMailServerId": secureMailServerId,
                 "sealCertificateId": sealCertificateId,
                 "subtypeMetadataList": subtypeMetadataList,
                 "subtypeLayers": subtypeLayers,
                 "externalSignatureConfigId": externalSignatureConfigId,
                 "externalSignatureConfig": externalSignatureConfig,
-                "parentTypeId": parentTypeId,
-                "parentType": parentType,
                 "creationPermittedDeskIds": creationPermittedDeskIds,
+                "creationPermittedDesks": creationPermittedDesks,
                 "filterableByDeskIds": filterableByDeskIds,
+                "filterableByDesks": filterableByDesks,
                 "maxMainDocuments": maxMainDocuments,
-                "annexeIncluded": annexeIncluded,
                 "multiDocuments": multiDocuments,
+                "annexeIncluded": annexeIncluded,
                 "digitalSignatureMandatory": digitalSignatureMandatory,
                 "readingMandatory": readingMandatory,
                 "sealAutomatic": sealAutomatic,
             }
     
     name: MetaOapg.properties.name
     
@@ -375,50 +444,50 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["subtypeLayers"]) -> MetaOapg.properties.subtypeLayers: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> MetaOapg.properties.externalSignatureConfigId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> 'ExternalSignatureConfig': ...
+    def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> 'ExternalSignatureConfigRepresentation': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["parentTypeId"]) -> MetaOapg.properties.parentTypeId: ...
+    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> MetaOapg.properties.creationPermittedDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["parentType"]) -> 'TypeRepresentation': ...
+    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDesks"]) -> MetaOapg.properties.creationPermittedDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> MetaOapg.properties.creationPermittedDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> MetaOapg.properties.filterableByDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> MetaOapg.properties.filterableByDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["filterableByDesks"]) -> MetaOapg.properties.filterableByDesks: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["maxMainDocuments"]) -> MetaOapg.properties.maxMainDocuments: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["annexeIncluded"]) -> MetaOapg.properties.annexeIncluded: ...
+    def __getitem__(self, name: typing_extensions.Literal["multiDocuments"]) -> MetaOapg.properties.multiDocuments: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["multiDocuments"]) -> MetaOapg.properties.multiDocuments: ...
+    def __getitem__(self, name: typing_extensions.Literal["annexeIncluded"]) -> MetaOapg.properties.annexeIncluded: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> MetaOapg.properties.digitalSignatureMandatory: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["readingMandatory"]) -> MetaOapg.properties.readingMandatory: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sealAutomatic"]) -> MetaOapg.properties.sealAutomatic: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "parentTypeId", "parentType", "creationPermittedDeskIds", "filterableByDeskIds", "maxMainDocuments", "annexeIncluded", "multiDocuments", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
@@ -455,50 +524,50 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["subtypeLayers"]) -> typing.Union[MetaOapg.properties.subtypeLayers, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> typing.Union[MetaOapg.properties.externalSignatureConfigId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> typing.Union['ExternalSignatureConfig', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["parentTypeId"]) -> typing.Union[MetaOapg.properties.parentTypeId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> typing.Union[MetaOapg.properties.creationPermittedDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["parentType"]) -> typing.Union['TypeRepresentation', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDesks"]) -> typing.Union[MetaOapg.properties.creationPermittedDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> typing.Union[MetaOapg.properties.creationPermittedDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> typing.Union[MetaOapg.properties.filterableByDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> typing.Union[MetaOapg.properties.filterableByDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDesks"]) -> typing.Union[MetaOapg.properties.filterableByDesks, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["maxMainDocuments"]) -> typing.Union[MetaOapg.properties.maxMainDocuments, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["annexeIncluded"]) -> typing.Union[MetaOapg.properties.annexeIncluded, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["multiDocuments"]) -> typing.Union[MetaOapg.properties.multiDocuments, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["multiDocuments"]) -> typing.Union[MetaOapg.properties.multiDocuments, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["annexeIncluded"]) -> typing.Union[MetaOapg.properties.annexeIncluded, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> typing.Union[MetaOapg.properties.digitalSignatureMandatory, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["readingMandatory"]) -> typing.Union[MetaOapg.properties.readingMandatory, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sealAutomatic"]) -> typing.Union[MetaOapg.properties.sealAutomatic, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "parentTypeId", "parentType", "creationPermittedDeskIds", "filterableByDeskIds", "maxMainDocuments", "annexeIncluded", "multiDocuments", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
@@ -510,22 +579,22 @@
         annotationsAllowed: typing.Union[MetaOapg.properties.annotationsAllowed, bool, schemas.Unset] = schemas.unset,
         externalSignatureAutomatic: typing.Union[MetaOapg.properties.externalSignatureAutomatic, bool, schemas.Unset] = schemas.unset,
         secureMailServerId: typing.Union[MetaOapg.properties.secureMailServerId, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sealCertificateId: typing.Union[MetaOapg.properties.sealCertificateId, None, str, schemas.Unset] = schemas.unset,
         subtypeMetadataList: typing.Union[MetaOapg.properties.subtypeMetadataList, list, tuple, schemas.Unset] = schemas.unset,
         subtypeLayers: typing.Union[MetaOapg.properties.subtypeLayers, list, tuple, schemas.Unset] = schemas.unset,
         externalSignatureConfigId: typing.Union[MetaOapg.properties.externalSignatureConfigId, None, str, schemas.Unset] = schemas.unset,
-        externalSignatureConfig: typing.Union['ExternalSignatureConfig', schemas.Unset] = schemas.unset,
-        parentTypeId: typing.Union[MetaOapg.properties.parentTypeId, None, str, schemas.Unset] = schemas.unset,
-        parentType: typing.Union['TypeRepresentation', schemas.Unset] = schemas.unset,
-        creationPermittedDeskIds: typing.Union[MetaOapg.properties.creationPermittedDeskIds, list, tuple, schemas.Unset] = schemas.unset,
-        filterableByDeskIds: typing.Union[MetaOapg.properties.filterableByDeskIds, list, tuple, schemas.Unset] = schemas.unset,
+        externalSignatureConfig: typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset] = schemas.unset,
+        creationPermittedDeskIds: typing.Union[MetaOapg.properties.creationPermittedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        creationPermittedDesks: typing.Union[MetaOapg.properties.creationPermittedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        filterableByDeskIds: typing.Union[MetaOapg.properties.filterableByDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        filterableByDesks: typing.Union[MetaOapg.properties.filterableByDesks, list, tuple, None, schemas.Unset] = schemas.unset,
         maxMainDocuments: typing.Union[MetaOapg.properties.maxMainDocuments, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        annexeIncluded: typing.Union[MetaOapg.properties.annexeIncluded, bool, schemas.Unset] = schemas.unset,
         multiDocuments: typing.Union[MetaOapg.properties.multiDocuments, bool, schemas.Unset] = schemas.unset,
+        annexeIncluded: typing.Union[MetaOapg.properties.annexeIncluded, bool, schemas.Unset] = schemas.unset,
         digitalSignatureMandatory: typing.Union[MetaOapg.properties.digitalSignatureMandatory, bool, schemas.Unset] = schemas.unset,
         readingMandatory: typing.Union[MetaOapg.properties.readingMandatory, bool, schemas.Unset] = schemas.unset,
         sealAutomatic: typing.Union[MetaOapg.properties.sealAutomatic, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SubtypeDto':
         return super().__new__(
@@ -541,25 +610,25 @@
             externalSignatureAutomatic=externalSignatureAutomatic,
             secureMailServerId=secureMailServerId,
             sealCertificateId=sealCertificateId,
             subtypeMetadataList=subtypeMetadataList,
             subtypeLayers=subtypeLayers,
             externalSignatureConfigId=externalSignatureConfigId,
             externalSignatureConfig=externalSignatureConfig,
-            parentTypeId=parentTypeId,
-            parentType=parentType,
             creationPermittedDeskIds=creationPermittedDeskIds,
+            creationPermittedDesks=creationPermittedDesks,
             filterableByDeskIds=filterableByDeskIds,
+            filterableByDesks=filterableByDesks,
             maxMainDocuments=maxMainDocuments,
-            annexeIncluded=annexeIncluded,
             multiDocuments=multiDocuments,
+            annexeIncluded=annexeIncluded,
             digitalSignatureMandatory=digitalSignatureMandatory,
             readingMandatory=readingMandatory,
             sealAutomatic=sealAutomatic,
             _configuration=_configuration,
             **kwargs,
         )
 
-from iparapheur_provisioning.model.external_signature_config import ExternalSignatureConfig
+from iparapheur_provisioning.model.desk_representation import DeskRepresentation
+from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
 from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
-from iparapheur_provisioning.model.type_representation import TypeRepresentation
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/tenant_representation.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,79 +20,87 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class SubtypeLayer(
+class TenantRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+        }
         
         class properties:
-        
-            @staticmethod
-            def id() -> typing.Type['CompositeId']:
-                return CompositeId
-        
-            @staticmethod
-            def association() -> typing.Type['SubtypeLayerAssociation']:
-                return SubtypeLayerAssociation
+            
+            
+            class name(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
+            id = schemas.StrSchema
             __annotations__ = {
+                "name": name,
                 "id": id,
-                "association": association,
             }
     
+    name: MetaOapg.properties.name
+    
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> 'CompositeId': ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["association"]) -> 'SubtypeLayerAssociation': ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "association", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union['CompositeId', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["association"]) -> typing.Union['SubtypeLayerAssociation', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "association", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        id: typing.Union['CompositeId', schemas.Unset] = schemas.unset,
-        association: typing.Union['SubtypeLayerAssociation', schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SubtypeLayer':
+    ) -> 'TenantRepresentation':
         return super().__new__(
             cls,
             *_args,
+            name=name,
             id=id,
-            association=association,
             _configuration=_configuration,
             **kwargs,
         )
-
-from iparapheur_provisioning.model.composite_id import CompositeId
-from iparapheur_provisioning.model.subtype_layer_association import SubtypeLayerAssociation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_metadata.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_representation.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,109 +20,87 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class SubtypeMetadata(
+class SubtypeRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
+        required = {
+            "name",
+        }
         
         class properties:
-        
-            @staticmethod
-            def id() -> typing.Type['CompositeId']:
-                return CompositeId
-        
-            @staticmethod
-            def metadata() -> typing.Type['Metadata']:
-                return Metadata
-            defaultValue = schemas.StrSchema
-            mandatory = schemas.BoolSchema
-            editable = schemas.BoolSchema
+            
+            
+            class name(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
+            id = schemas.StrSchema
             __annotations__ = {
+                "name": name,
                 "id": id,
-                "metadata": metadata,
-                "defaultValue": defaultValue,
-                "mandatory": mandatory,
-                "editable": editable,
             }
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> 'CompositeId': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> 'Metadata': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["defaultValue"]) -> MetaOapg.properties.defaultValue: ...
+    name: MetaOapg.properties.name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["mandatory"]) -> MetaOapg.properties.mandatory: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["editable"]) -> MetaOapg.properties.editable: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "metadata", "defaultValue", "mandatory", "editable", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union['CompositeId', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union['Metadata', schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["defaultValue"]) -> typing.Union[MetaOapg.properties.defaultValue, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["mandatory"]) -> typing.Union[MetaOapg.properties.mandatory, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["editable"]) -> typing.Union[MetaOapg.properties.editable, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "metadata", "defaultValue", "mandatory", "editable", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        id: typing.Union['CompositeId', schemas.Unset] = schemas.unset,
-        metadata: typing.Union['Metadata', schemas.Unset] = schemas.unset,
-        defaultValue: typing.Union[MetaOapg.properties.defaultValue, str, schemas.Unset] = schemas.unset,
-        mandatory: typing.Union[MetaOapg.properties.mandatory, bool, schemas.Unset] = schemas.unset,
-        editable: typing.Union[MetaOapg.properties.editable, bool, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SubtypeMetadata':
+    ) -> 'SubtypeRepresentation':
         return super().__new__(
             cls,
             *_args,
+            name=name,
             id=id,
-            metadata=metadata,
-            defaultValue=defaultValue,
-            mandatory=mandatory,
-            editable=editable,
             _configuration=_configuration,
             **kwargs,
         )
-
-from iparapheur_provisioning.model.composite_id import CompositeId
-from iparapheur_provisioning.model.metadata import Metadata
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/tenant_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class SubtypeRepresentation(
+class TenantDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    body
     """
 
 
     class MetaOapg:
         required = {
             "name",
         }
@@ -47,16 +49,15 @@
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
             id = schemas.StrSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
             }
     
@@ -92,15 +93,15 @@
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SubtypeRepresentation':
+    ) -> 'TenantDto':
         return super().__new__(
             cls,
             *_args,
             name=name,
             id=id,
             _configuration=_configuration,
             **kwargs,
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,107 +20,114 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class TypeRepresentation(
+class ExternalSignatureConfigRepresentation(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
-        required = {
-            "name",
-        }
         
         class properties:
+            id = schemas.StrSchema
             
             
             class name(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
-                    regex=[{
-                        'pattern': r'^[^
- ]+$',  # noqa: E501
-                    }]
-            id = schemas.StrSchema
-            
-            
-            class description(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 255
-                    min_length = 3
+        
+            @staticmethod
+            def serviceName() -> typing.Type['ExternalSignatureProvider']:
+                return ExternalSignatureProvider
+            url = schemas.StrSchema
+            login = schemas.StrSchema
             __annotations__ = {
-                "name": name,
                 "id": id,
-                "description": description,
+                "name": name,
+                "serviceName": serviceName,
+                "url": url,
+                "login": login,
             }
     
-    name: MetaOapg.properties.name
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["serviceName"]) -> 'ExternalSignatureProvider': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["login"]) -> MetaOapg.properties.login: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "serviceName", "url", "login", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["serviceName"]) -> typing.Union['ExternalSignatureProvider', schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["url"]) -> typing.Union[MetaOapg.properties.url, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["login"]) -> typing.Union[MetaOapg.properties.login, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "serviceName", "url", "login", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
+        serviceName: typing.Union['ExternalSignatureProvider', schemas.Unset] = schemas.unset,
+        url: typing.Union[MetaOapg.properties.url, str, schemas.Unset] = schemas.unset,
+        login: typing.Union[MetaOapg.properties.login, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TypeRepresentation':
+    ) -> 'ExternalSignatureConfigRepresentation':
         return super().__new__(
             cls,
             *_args,
-            name=name,
             id=id,
-            description=description,
+            name=name,
+            serviceName=serviceName,
+            url=url,
+            login=login,
             _configuration=_configuration,
             **kwargs,
         )
+
+from iparapheur_provisioning.model.external_signature_provider import ExternalSignatureProvider
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,49 +7,42 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from iparapheur_provisioning.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from iparapheur_provisioning.model.composite_id import CompositeId
 from iparapheur_provisioning.model.delegation_sort_by import DelegationSortBy
 from iparapheur_provisioning.model.desk_dto import DeskDto
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.external_signature_config import ExternalSignatureConfig
+from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_provisioning.model.external_signature_config_sort_by import ExternalSignatureConfigSortBy
 from iparapheur_provisioning.model.external_signature_provider import ExternalSignatureProvider
 from iparapheur_provisioning.model.folder_sort_by import FolderSortBy
 from iparapheur_provisioning.model.internal_metadata import InternalMetadata
 from iparapheur_provisioning.model.layer_representation import LayerRepresentation
 from iparapheur_provisioning.model.layer_sort_by import LayerSortBy
-from iparapheur_provisioning.model.metadata import Metadata
 from iparapheur_provisioning.model.metadata_dto import MetadataDto
 from iparapheur_provisioning.model.metadata_representation import MetadataRepresentation
 from iparapheur_provisioning.model.metadata_sort_by import MetadataSortBy
 from iparapheur_provisioning.model.metadata_type import MetadataType
 from iparapheur_provisioning.model.page_desk_representation import PageDeskRepresentation
-from iparapheur_provisioning.model.page_subtype_layer import PageSubtypeLayer
-from iparapheur_provisioning.model.page_subtype_metadata import PageSubtypeMetadata
 from iparapheur_provisioning.model.page_subtype_representation import PageSubtypeRepresentation
 from iparapheur_provisioning.model.page_type_representation import PageTypeRepresentation
-from iparapheur_provisioning.model.page_typology_representation import PageTypologyRepresentation
 from iparapheur_provisioning.model.page_user_representation import PageUserRepresentation
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.pdf_signature_position import PdfSignaturePosition
 from iparapheur_provisioning.model.seal_certificate_sort_by import SealCertificateSortBy
 from iparapheur_provisioning.model.signature_format import SignatureFormat
 from iparapheur_provisioning.model.signature_protocol import SignatureProtocol
 from iparapheur_provisioning.model.sort_object import SortObject
 from iparapheur_provisioning.model.subtype_dto import SubtypeDto
-from iparapheur_provisioning.model.subtype_layer import SubtypeLayer
 from iparapheur_provisioning.model.subtype_layer_association import SubtypeLayerAssociation
 from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
-from iparapheur_provisioning.model.subtype_metadata import SubtypeMetadata
 from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
 from iparapheur_provisioning.model.subtype_representation import SubtypeRepresentation
 from iparapheur_provisioning.model.tenant_dto import TenantDto
 from iparapheur_provisioning.model.tenant_representation import TenantRepresentation
 from iparapheur_provisioning.model.tenant_sort_by import TenantSortBy
 from iparapheur_provisioning.model.type_dto import TypeDto
 from iparapheur_provisioning.model.type_representation import TypeRepresentation
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,12 +14,7 @@
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK_DESK_ID = "/api/provisioning/v1/admin/tenant/{tenantId}/desk/{deskId}"
     API_PROVISIONING_V1_ADMIN_TENANT = "/api/provisioning/v1/admin/tenant"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_USER = "/api/provisioning/v1/admin/tenant/{tenantId}/user"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype"
     API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_DESK = "/api/provisioning/v1/admin/tenant/{tenantId}/desk"
     API_PROVISIONING_V1_ADMIN_USER = "/api/provisioning/v1/admin/user"
-    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY = "/api/provisioning/v1/admin/tenant/{tenantId}/typology"
-    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_METADATA = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/metadata"
-    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_LAYER = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/layer"
-    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_FILTERABLE_BY_DESKS = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/filterableByDesks"
-    API_PROVISIONING_V1_ADMIN_TENANT_TENANT_ID_TYPOLOGY_TYPE_TYPE_ID_SUBTYPE_SUBTYPE_ID_CREATION_PERMITTED_DESKS = "/api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId}/creationPermittedDesks"
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,69 +40,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -136,17 +136,17 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '403': _response_for_403,
     '400': _response_for_400,
+    '401': _response_for_401,
     '201': _response_for_201,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -54,31 +54,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -104,38 +104,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
-    '403': _response_for_403,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,31 +55,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -93,57 +93,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '400': _response_for_400,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -104,31 +104,31 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -142,59 +142,59 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
+    '404': _response_for_404,
     '201': _response_for_201,
-    '409': _response_for_409,
     '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,31 +62,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -112,38 +112,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
-    '403': _response_for_403,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,31 +63,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -101,57 +101,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -112,97 +112,97 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
-    '409': _response_for_409,
+    '404': _response_for_404,
     '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,44 +22,19 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.page_typology_representation import PageTypologyRepresentation
+from iparapheur_provisioning.model.page_user_representation import PageUserRepresentation
 
 from . import path
 
 # Query params
-CollapseAllSchema = schemas.BoolSchema
-
-
-class ReverseIdListSchema(
-    schemas.ListSchema
-):
-
-
-    class MetaOapg:
-        unique_items = True
-        items = schemas.StrSchema
-
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ReverseIdListSchema':
-        return super().__new__(
-            cls,
-            _arg,
-            _configuration=_configuration,
-        )
-
-    def __getitem__(self, i: int) -> MetaOapg.items:
-        return super().__getitem__(i)
 
 
 class PageSchema(
     schemas.IntSchema
 ):
 
 
@@ -102,41 +77,27 @@
     'RequestRequiredQueryParams',
     {
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
-        'collapseAll': typing.Union[CollapseAllSchema, bool, ],
-        'reverseIdList': typing.Union[ReverseIdListSchema, list, tuple, ],
         'page': typing.Union[PageSchema, decimal.Decimal, int, ],
         'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
         'sort': typing.Union[SortSchema, list, tuple, ],
         'searchTerm': typing.Union[SearchTermSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_collapse_all = api_client.QueryParameter(
-    name="collapseAll",
-    style=api_client.ParameterStyle.FORM,
-    schema=CollapseAllSchema,
-    explode=True,
-)
-request_query_reverse_id_list = api_client.QueryParameter(
-    name="reverseIdList",
-    style=api_client.ParameterStyle.FORM,
-    schema=ReverseIdListSchema,
-    explode=True,
-)
 request_query_page = api_client.QueryParameter(
     name="page",
     style=api_client.ParameterStyle.FORM,
     schema=PageSchema,
     explode=True,
 )
 request_query_size = api_client.QueryParameter(
@@ -153,139 +114,75 @@
 )
 request_query_search_term = api_client.QueryParameter(
     name="searchTerm",
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
-# Path params
-TenantIdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'tenantId': typing.Union[TenantIdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
-
-
-request_path_tenant_id = api_client.PathParameter(
-    name="tenantId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=TenantIdSchema,
-    required=True,
-)
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor404(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
-    },
-)
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor401(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
-)
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageTypologyRepresentation
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -297,101 +194,79 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
-    '406': _response_for_406,
     '403': _response_for_403,
     '400': _response_for_400,
+    '401': _response_for_401,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_typology_hierarchy_oapg(
+    def _list_users_as_super_admin_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _get_typology_hierarchy_oapg(
+    def _list_users_as_super_admin_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_typology_hierarchy_oapg(
+    def _list_users_as_super_admin_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_typology_hierarchy_oapg(
+    def _list_users_as_super_admin_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get typology list, sorted by hierarchy.
+        List all users on the instance
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
-        _path_params = {}
-        for parameter in (
-            request_path_tenant_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-
         prefix_separator_iterator = None
         for parameter in (
-            request_query_collapse_all,
-            request_query_reverse_id_list,
             request_query_page,
             request_query_size,
             request_query_sort,
             request_query_search_term,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
@@ -432,127 +307,117 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetTypologyHierarchy(BaseApi):
+class ListUsersAsSuperAdmin(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_typology_hierarchy(
+    def list_users_as_super_admin(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def get_typology_hierarchy(
+    def list_users_as_super_admin(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_typology_hierarchy(
+    def list_users_as_super_admin(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_typology_hierarchy(
+    def list_users_as_super_admin(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_typology_hierarchy_oapg(
+        return self._list_users_as_super_admin_oapg(
             query_params=query_params,
-            path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_typology_hierarchy_oapg(
+        return self._list_users_as_super_admin_oapg(
             query_params=query_params,
-            path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,31 +135,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -173,57 +173,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,58 +123,58 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '201': _response_for_201,
-    '409': _response_for_409,
     '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,31 +62,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -112,38 +112,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
-    '403': _response_for_403,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,31 +63,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -101,57 +101,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -112,57 +112,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,31 +143,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -181,57 +181,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -112,31 +112,31 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -150,59 +150,59 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
+    '404': _response_for_404,
     '201': _response_for_201,
-    '409': _response_for_409,
     '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,31 +70,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -120,38 +120,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
-    '403': _response_for_403,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,31 +71,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -109,57 +109,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,31 +82,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor204ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
@@ -139,31 +139,31 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -178,18 +178,18 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
-    '403': _response_for_403,
+    '404': _response_for_404,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.page_desk_representation import PageDeskRepresentation
+from iparapheur_provisioning.model.page_user_representation import PageUserRepresentation
 
 from . import path
 
 # Query params
 
 
 class PageSchema(
@@ -68,25 +68,29 @@
             cls,
             _arg,
             _configuration=_configuration,
         )
 
     def __getitem__(self, i: int) -> MetaOapg.items:
         return super().__getitem__(i)
+SearchTermSchema = schemas.StrSchema
+DeskIdSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
         'page': typing.Union[PageSchema, decimal.Decimal, int, ],
         'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
         'sort': typing.Union[SortSchema, list, tuple, ],
+        'searchTerm': typing.Union[SearchTermSchema, str, ],
+        'deskId': typing.Union[DeskIdSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -106,24 +110,32 @@
 )
 request_query_sort = api_client.QueryParameter(
     name="sort",
     style=api_client.ParameterStyle.FORM,
     schema=SortSchema,
     explode=True,
 )
+request_query_search_term = api_client.QueryParameter(
+    name="searchTerm",
+    style=api_client.ParameterStyle.FORM,
+    schema=SearchTermSchema,
+    explode=True,
+)
+request_query_desk_id = api_client.QueryParameter(
+    name="deskId",
+    style=api_client.ParameterStyle.FORM,
+    schema=DeskIdSchema,
+    explode=True,
+)
 # Path params
 TenantIdSchema = schemas.StrSchema
-TypeIdSchema = schemas.StrSchema
-SubtypeIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'tenantId': typing.Union[TenantIdSchema, str, ],
-        'typeId': typing.Union[TypeIdSchema, str, ],
-        'subtypeId': typing.Union[SubtypeIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -136,46 +148,53 @@
 
 request_path_tenant_id = api_client.PathParameter(
     name="tenantId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
-request_path_type_id = api_client.PathParameter(
-    name="typeId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=TypeIdSchema,
-    required=True,
-)
-request_path_subtype_id = api_client.PathParameter(
-    name="subtypeId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=SubtypeIdSchema,
-    required=True,
-)
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor400(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor400ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -189,126 +208,125 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _list_creation_permitted_desks_oapg(
+    def _list_tenant_users_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _list_creation_permitted_desks_oapg(
+    def _list_tenant_users_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_creation_permitted_desks_oapg(
+    def _list_tenant_users_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _list_creation_permitted_desks_oapg(
+    def _list_tenant_users_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List the desks permitted to use this subtype in a folder creation.
+        List all users associated with the tenant
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_tenant_id,
-            request_path_type_id,
-            request_path_subtype_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
@@ -316,14 +334,16 @@
             used_path = used_path.replace('{%s}' % k, v)
 
         prefix_separator_iterator = None
         for parameter in (
             request_query_page,
             request_query_size,
             request_query_sort,
+            request_query_search_term,
+            request_query_desk_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -360,65 +380,65 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class ListCreationPermittedDesks(BaseApi):
+class ListTenantUsers(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_creation_permitted_desks(
+    def list_tenant_users(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def list_creation_permitted_desks(
+    def list_tenant_users(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_creation_permitted_desks(
+    def list_tenant_users(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def list_creation_permitted_desks(
+    def list_tenant_users(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_creation_permitted_desks_oapg(
+        return self._list_tenant_users_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
@@ -470,15 +490,15 @@
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_creation_permitted_desks_oapg(
+        return self._list_tenant_users_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,25 +68,27 @@
             cls,
             _arg,
             _configuration=_configuration,
         )
 
     def __getitem__(self, i: int) -> MetaOapg.items:
         return super().__getitem__(i)
+SearchTermSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
         'page': typing.Union[PageSchema, decimal.Decimal, int, ],
         'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
         'sort': typing.Union[SortSchema, list, tuple, ],
+        'searchTerm': typing.Union[SearchTermSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -106,24 +108,26 @@
 )
 request_query_sort = api_client.QueryParameter(
     name="sort",
     style=api_client.ParameterStyle.FORM,
     schema=SortSchema,
     explode=True,
 )
+request_query_search_term = api_client.QueryParameter(
+    name="searchTerm",
+    style=api_client.ParameterStyle.FORM,
+    schema=SearchTermSchema,
+    explode=True,
+)
 # Path params
 TenantIdSchema = schemas.StrSchema
-TypeIdSchema = schemas.StrSchema
-SubtypeIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'tenantId': typing.Union[TenantIdSchema, str, ],
-        'typeId': typing.Union[TypeIdSchema, str, ],
-        'subtypeId': typing.Union[SubtypeIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -136,84 +140,72 @@
 
 request_path_tenant_id = api_client.PathParameter(
     name="tenantId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
-request_path_type_id = api_client.PathParameter(
-    name="typeId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=TypeIdSchema,
-    required=True,
-)
-request_path_subtype_id = api_client.PathParameter(
-    name="subtypeId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=SubtypeIdSchema,
-    required=True,
-)
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -228,87 +220,85 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _list_filterable_by_desks_oapg(
+    def _list_desks_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _list_filterable_by_desks_oapg(
+    def _list_desks_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_filterable_by_desks_oapg(
+    def _list_desks_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _list_filterable_by_desks_oapg(
+    def _list_desks_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List the desks permitted to use this subtype in a filter.
+        List desks
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_tenant_id,
-            request_path_type_id,
-            request_path_subtype_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
@@ -316,14 +306,15 @@
             used_path = used_path.replace('{%s}' % k, v)
 
         prefix_separator_iterator = None
         for parameter in (
             request_query_page,
             request_query_size,
             request_query_sort,
+            request_query_search_term,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -360,65 +351,65 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class ListFilterableByDesks(BaseApi):
+class ListDesks(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_filterable_by_desks(
+    def list_desks(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def list_filterable_by_desks(
+    def list_desks(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_filterable_by_desks(
+    def list_desks(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def list_filterable_by_desks(
+    def list_desks(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_filterable_by_desks_oapg(
+        return self._list_desks_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
@@ -470,15 +461,15 @@
         query_params: RequestQueryParams = frozendict.frozendict(),
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_filterable_by_desks_oapg(
+        return self._list_desks_oapg(
             query_params=query_params,
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,161 +21,95 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
+from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.page_subtype_layer import PageSubtypeLayer
 
 from . import path
 
-# Query params
-
-
-class PageSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 0
-
-
-class SizeSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 1
-
-
-class SortSchema(
-    schemas.ListSchema
-):
-
-
-    class MetaOapg:
-        items = schemas.StrSchema
-
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'SortSchema':
-        return super().__new__(
-            cls,
-            _arg,
-            _configuration=_configuration,
-        )
-
-    def __getitem__(self, i: int) -> MetaOapg.items:
-        return super().__getitem__(i)
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
-        'sort': typing.Union[SortSchema, list, tuple, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_page = api_client.QueryParameter(
-    name="page",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
-    explode=True,
-)
-request_query_size = api_client.QueryParameter(
-    name="size",
-    style=api_client.ParameterStyle.FORM,
-    schema=SizeSchema,
-    explode=True,
-)
-request_query_sort = api_client.QueryParameter(
-    name="sort",
-    style=api_client.ParameterStyle.FORM,
-    schema=SortSchema,
-    explode=True,
-)
 # Path params
-TenantIdSchema = schemas.StrSchema
-TypeIdSchema = schemas.StrSchema
-SubtypeIdSchema = schemas.StrSchema
+UserIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'tenantId': typing.Union[TenantIdSchema, str, ],
-        'typeId': typing.Union[TypeIdSchema, str, ],
-        'subtypeId': typing.Union[SubtypeIdSchema, str, ],
+        'userId': typing.Union[UserIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
 )
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_path_tenant_id = api_client.PathParameter(
-    name="tenantId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=TenantIdSchema,
-    required=True,
-)
-request_path_type_id = api_client.PathParameter(
-    name="typeId",
+request_path_user_id = api_client.PathParameter(
+    name="userId",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=TypeIdSchema,
+    schema=UserIdSchema,
     required=True,
 )
-request_path_subtype_id = api_client.PathParameter(
-    name="subtypeId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=SubtypeIdSchema,
+# body param
+SchemaForRequestBodyApplicationJson = UserDto
+
+
+request_body_user_dto = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor400(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor400ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -189,161 +123,176 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeLayer
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '400': _response_for_400,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _list_layers_from_subtype_oapg(
+    def _update_user_as_super_admin_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _list_layers_from_subtype_oapg(
+    def _update_user_as_super_admin_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def _update_user_as_super_admin_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_layers_from_subtype_oapg(
+    def _update_user_as_super_admin_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _list_layers_from_subtype_oapg(
+    def _update_user_as_super_admin_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List the layers associated with the given subtype
+        Edit a user
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
-            request_path_tenant_id,
-            request_path_type_id,
-            request_path_subtype_id,
+            request_path_user_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_page,
-            request_query_size,
-            request_query_sort,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_user_dto.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='put'.upper(),
             headers=_headers,
+            fields=_fields,
+            body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -360,127 +309,167 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class ListLayersFromSubtype(BaseApi):
+class UpdateUserAsSuperAdmin(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_layers_from_subtype(
+    def update_user_as_super_admin(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def update_user_as_super_admin(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
-    def list_layers_from_subtype(
+    def update_user_as_super_admin(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_layers_from_subtype(
+    def update_user_as_super_admin(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def list_layers_from_subtype(
+    def update_user_as_super_admin(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_layers_from_subtype_oapg(
-            query_params=query_params,
+        return self._update_user_as_super_admin_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiForput(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def put(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def put(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
-    def get(
+    def put(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def put(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def put(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_layers_from_subtype_oapg(
-            query_params=query_params,
+        return self._update_user_as_super_admin_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,109 +21,27 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
+from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.page_subtype_metadata import PageSubtypeMetadata
 
 from . import path
 
-# Query params
-
-
-class PageSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 0
-
-
-class SizeSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 1
-
-
-class SortSchema(
-    schemas.ListSchema
-):
-
-
-    class MetaOapg:
-        items = schemas.StrSchema
-
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'SortSchema':
-        return super().__new__(
-            cls,
-            _arg,
-            _configuration=_configuration,
-        )
-
-    def __getitem__(self, i: int) -> MetaOapg.items:
-        return super().__getitem__(i)
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
-        'sort': typing.Union[SortSchema, list, tuple, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_page = api_client.QueryParameter(
-    name="page",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
-    explode=True,
-)
-request_query_size = api_client.QueryParameter(
-    name="size",
-    style=api_client.ParameterStyle.FORM,
-    schema=SizeSchema,
-    explode=True,
-)
-request_query_sort = api_client.QueryParameter(
-    name="sort",
-    style=api_client.ParameterStyle.FORM,
-    schema=SortSchema,
-    explode=True,
-)
 # Path params
 TenantIdSchema = schemas.StrSchema
-TypeIdSchema = schemas.StrSchema
-SubtypeIdSchema = schemas.StrSchema
+UserIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'tenantId': typing.Union[TenantIdSchema, str, ],
-        'typeId': typing.Union[TypeIdSchema, str, ],
-        'subtypeId': typing.Union[SubtypeIdSchema, str, ],
+        'userId': typing.Union[UserIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -136,46 +54,51 @@
 
 request_path_tenant_id = api_client.PathParameter(
     name="tenantId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
-request_path_type_id = api_client.PathParameter(
-    name="typeId",
+request_path_user_id = api_client.PathParameter(
+    name="userId",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=TypeIdSchema,
+    schema=UserIdSchema,
     required=True,
 )
-request_path_subtype_id = api_client.PathParameter(
-    name="subtypeId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=SubtypeIdSchema,
+# body param
+SchemaForRequestBodyApplicationJson = UserDto
+
+
+request_body_user_dto = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -189,34 +112,34 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeMetadata
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -227,123 +150,158 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor404(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor404ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
+    '401': _response_for_401,
+    '406': _response_for_406,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _list_metadata_from_subtype_oapg(
+    def _update_user_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def _update_user_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
-    def _list_metadata_from_subtype_oapg(
+    def _update_user_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_metadata_from_subtype_oapg(
+    def _update_user_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _list_metadata_from_subtype_oapg(
+    def _update_user_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List the metadata associated with the given subtype
+        Edit a user
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_tenant_id,
-            request_path_type_id,
-            request_path_subtype_id,
+            request_path_user_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_page,
-            request_query_size,
-            request_query_sort,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_user_dto.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='put'.upper(),
             headers=_headers,
+            fields=_fields,
+            body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -360,127 +318,167 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class ListMetadataFromSubtype(BaseApi):
+class UpdateUser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_metadata_from_subtype(
+    def update_user(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def list_metadata_from_subtype(
+    def update_user(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def update_user(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_metadata_from_subtype(
+    def update_user(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def list_metadata_from_subtype(
+    def update_user(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_metadata_from_subtype_oapg(
-            query_params=query_params,
+        return self._update_user_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiForput(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def put(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def put(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
+
     @typing.overload
-    def get(
+    def put(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def put(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def put(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_metadata_from_subtype_oapg(
-            query_params=query_params,
+        return self._update_user_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,115 +21,19 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
+from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.page_user_representation import PageUserRepresentation
 
 from . import path
 
-# Query params
-
-
-class PageSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 0
-
-
-class SizeSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 1
-
-
-class SortSchema(
-    schemas.ListSchema
-):
-
-
-    class MetaOapg:
-        items = schemas.StrSchema
-
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'SortSchema':
-        return super().__new__(
-            cls,
-            _arg,
-            _configuration=_configuration,
-        )
-
-    def __getitem__(self, i: int) -> MetaOapg.items:
-        return super().__getitem__(i)
-SearchTermSchema = schemas.StrSchema
-DeskIdSchema = schemas.StrSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
-        'sort': typing.Union[SortSchema, list, tuple, ],
-        'searchTerm': typing.Union[SearchTermSchema, str, ],
-        'deskId': typing.Union[DeskIdSchema, str, ],
-    },
-    total=False
-)
-
-
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_page = api_client.QueryParameter(
-    name="page",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
-    explode=True,
-)
-request_query_size = api_client.QueryParameter(
-    name="size",
-    style=api_client.ParameterStyle.FORM,
-    schema=SizeSchema,
-    explode=True,
-)
-request_query_sort = api_client.QueryParameter(
-    name="sort",
-    style=api_client.ParameterStyle.FORM,
-    schema=SortSchema,
-    explode=True,
-)
-request_query_search_term = api_client.QueryParameter(
-    name="searchTerm",
-    style=api_client.ParameterStyle.FORM,
-    schema=SearchTermSchema,
-    explode=True,
-)
-request_query_desk_id = api_client.QueryParameter(
-    name="deskId",
-    style=api_client.ParameterStyle.FORM,
-    schema=DeskIdSchema,
-    explode=True,
-)
 # Path params
 TenantIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'tenantId': typing.Union[TenantIdSchema, str, ],
     }
@@ -148,34 +52,45 @@
 
 request_path_tenant_id = api_client.PathParameter(
     name="tenantId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
+# body param
+SchemaForRequestBodyApplicationJson = UserDto
+
+
+request_body_user_dto = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
+    required=True,
+)
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -189,138 +104,156 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
-    '400': _response_for_400,
-    '200': _response_for_200,
+    '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _list_tenant_users_oapg(
+    def _create_user_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
     ]: ...
 
     @typing.overload
-    def _list_tenant_users_oapg(
+    def _create_user_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor201,
+    ]: ...
+
+
+    @typing.overload
+    def _create_user_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_tenant_users_oapg(
+    def _create_user_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _list_tenant_users_oapg(
+    def _create_user_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List all users associated with the tenant
+        Create a new user
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_tenant_id,
         ):
@@ -329,41 +262,37 @@
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
 
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_page,
-            request_query_size,
-            request_query_sort,
-            request_query_search_term,
-            request_query_desk_id,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_user_dto.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
+            fields=_fields,
+            body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -380,127 +309,167 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class ListTenantUsers(BaseApi):
+class CreateUser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_tenant_users(
+    def create_user(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
     ]: ...
 
     @typing.overload
-    def list_tenant_users(
+    def create_user(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor201,
+    ]: ...
+
+
+    @typing.overload
+    def create_user(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_tenant_users(
+    def create_user(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def list_tenant_users(
+    def create_user(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_tenant_users_oapg(
-            query_params=query_params,
+        return self._create_user_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
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
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
     ]: ...
 
     @typing.overload
-    def get(
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor201,
+    ]: ...
+
+
+    @typing.overload
+    def post(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def post(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def post(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        body: typing.Union[SchemaForRequestBodyApplicationJson,],
+        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_tenant_users_oapg(
-            query_params=query_params,
+        return self._create_user_oapg(
+            body=body,
             path_params=path_params,
+            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,25 +21,26 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
-from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
 
 from . import path
 
 # Path params
 TenantIdSchema = schemas.StrSchema
+UserIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'tenantId': typing.Union[TenantIdSchema, str, ],
+        'userId': typing.Union[UserIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
@@ -52,47 +53,23 @@
 
 request_path_tenant_id = api_client.PathParameter(
     name="tenantId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
-# body param
-SchemaForRequestBodyApplicationJson = UserDto
-
-
-request_body_user_dto = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
+request_path_user_id = api_client.PathParameter(
+    name="userId",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor401(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -104,162 +81,132 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '403': _response_for_403,
-    '201': _response_for_201,
-    '409': _response_for_409,
-    '507': _response_for_507,
+    '204': _response_for_204,
+    '401': _response_for_401,
+    '406': _response_for_406,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _create_user_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"] = ...,
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor201,
-    ]: ...
-
-    @typing.overload
-    def _create_user_oapg(
+    def _remove_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor204,
     ]: ...
 
-
     @typing.overload
-    def _create_user_oapg(
+    def _remove_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _create_user_oapg(
+    def _remove_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor204,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _create_user_oapg(
+    def _remove_user_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Create a new user
+        Remove the given user from the tenant, deleting it if it was the last tenant linked
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
             request_path_tenant_id,
+            request_path_user_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
@@ -268,31 +215,18 @@
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
-        serialized_data = request_body_user_dto.serialize(body, content_type)
-        _headers.add('Content-Type', content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='delete'.upper(),
             headers=_headers,
-            fields=_fields,
-            body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
             api_response = api_client.ApiResponseWithoutDeserialization(response=response)
@@ -309,167 +243,117 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class CreateUser(BaseApi):
+class RemoveUser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def create_user(
+    def remove_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor204,
     ]: ...
 
     @typing.overload
-    def create_user(
+    def remove_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor201,
-    ]: ...
-
-
-    @typing.overload
-    def create_user(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def create_user(
+    def remove_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor204,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def create_user(
+    def remove_user(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_user_oapg(
-            body=body,
+        return self._remove_user_oapg(
             path_params=path_params,
-            content_type=content_type,
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
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor204,
     ]: ...
 
     @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        path_params: RequestPathParams = frozendict.frozendict(),
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor201,
-    ]: ...
-
-
-    @typing.overload
-    def post(
+    def delete(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def post(
+    def delete(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor204,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def post(
+    def delete(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._create_user_oapg(
-            body=body,
+        return self._remove_user_oapg(
             path_params=path_params,
-            content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
+from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
 
 from . import path
 
 # Path params
 TenantIdSchema = schemas.StrSchema
 UserIdSchema = schemas.StrSchema
@@ -62,25 +63,32 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor204(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -93,109 +101,109 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '204': _response_for_204,
-    '401': _response_for_401,
-    '406': _response_for_406,
     '403': _response_for_403,
+    '401': _response_for_401,
+    '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _remove_user_oapg(
+    def _get_user_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor204,
+        ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _remove_user_oapg(
+    def _get_user_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _remove_user_oapg(
+    def _get_user_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor204,
+        ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _remove_user_oapg(
+    def _get_user_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Remove the given user from the tenant, deleting it if it was the last tenant linked
+        Get a full user description
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
@@ -217,15 +225,15 @@
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
@@ -243,116 +251,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class RemoveUser(BaseApi):
+class GetUser(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def remove_user(
+    def get_user(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor204,
+        ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def remove_user(
+    def get_user(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def remove_user(
+    def get_user(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor204,
+        ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def remove_user(
+    def get_user(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._remove_user_oapg(
+        return self._get_user_oapg(
             path_params=path_params,
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
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor204,
+        ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor204,
+        ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def delete(
+    def get(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._remove_user_oapg(
+        return self._get_user_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,23 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
-from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
 
 from . import path
 
 # Path params
-TenantIdSchema = schemas.StrSchema
 UserIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'tenantId': typing.Union[TenantIdSchema, str, ],
         'userId': typing.Union[UserIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
@@ -48,172 +45,158 @@
 )
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_path_tenant_id = api_client.PathParameter(
-    name="tenantId",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=TenantIdSchema,
-    required=True,
-)
 request_path_user_id = api_client.PathParameter(
     name="userId",
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
-    '200': _response_for_200,
+    '204': _response_for_204,
+    '400': _response_for_400,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _get_user_oapg(
+    def _delete_user_as_super_admin_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor204,
     ]: ...
 
     @typing.overload
-    def _get_user_oapg(
+    def _delete_user_as_super_admin_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _get_user_oapg(
+    def _delete_user_as_super_admin_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor204,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _get_user_oapg(
+    def _delete_user_as_super_admin_oapg(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Get a full user description
+        Delete a user
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
         for parameter in (
-            request_path_tenant_id,
             request_path_user_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
@@ -225,15 +208,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='delete'.upper(),
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
@@ -251,116 +234,116 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class GetUser(BaseApi):
+class DeleteUserAsSuperAdmin(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def get_user(
+    def delete_user_as_super_admin(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor204,
     ]: ...
 
     @typing.overload
-    def get_user(
+    def delete_user_as_super_admin(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get_user(
+    def delete_user_as_super_admin(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor204,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get_user(
+    def delete_user_as_super_admin(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_user_oapg(
+        return self._delete_user_as_super_admin_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
-class ApiForget(BaseApi):
+class ApiFordelete(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def get(
+    def delete(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor204,
     ]: ...
 
     @typing.overload
-    def get(
+    def delete(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def get(
+    def delete(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor204,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def get(
+    def delete(
         self,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._get_user_oapg(
+        return self._delete_user_as_super_admin_oapg(
             path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,168 +21,106 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
+from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.error_response import ErrorResponse
-from iparapheur_provisioning.model.page_user_representation import PageUserRepresentation
 
 from . import path
 
-# Query params
-
-
-class PageSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 0
-
-
-class SizeSchema(
-    schemas.IntSchema
-):
-
-
-    class MetaOapg:
-        inclusive_minimum = 1
-
-
-class SortSchema(
-    schemas.ListSchema
-):
-
-
-    class MetaOapg:
-        items = schemas.StrSchema
-
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'SortSchema':
-        return super().__new__(
-            cls,
-            _arg,
-            _configuration=_configuration,
-        )
-
-    def __getitem__(self, i: int) -> MetaOapg.items:
-        return super().__getitem__(i)
-SearchTermSchema = schemas.StrSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
+# Path params
+UserIdSchema = schemas.StrSchema
+RequestRequiredPathParams = typing_extensions.TypedDict(
+    'RequestRequiredPathParams',
     {
+        'userId': typing.Union[UserIdSchema, str, ],
     }
 )
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
+RequestOptionalPathParams = typing_extensions.TypedDict(
+    'RequestOptionalPathParams',
     {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
-        'sort': typing.Union[SortSchema, list, tuple, ],
-        'searchTerm': typing.Union[SearchTermSchema, str, ],
     },
     total=False
 )
 
 
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_query_page = api_client.QueryParameter(
-    name="page",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
-    explode=True,
-)
-request_query_size = api_client.QueryParameter(
-    name="size",
-    style=api_client.ParameterStyle.FORM,
-    schema=SizeSchema,
-    explode=True,
-)
-request_query_sort = api_client.QueryParameter(
-    name="sort",
-    style=api_client.ParameterStyle.FORM,
-    schema=SortSchema,
-    explode=True,
-)
-request_query_search_term = api_client.QueryParameter(
-    name="searchTerm",
-    style=api_client.ParameterStyle.FORM,
-    schema=SearchTermSchema,
-    explode=True,
+request_path_user_id = api_client.PathParameter(
+    name="userId",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=UserIdSchema,
+    required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
@@ -193,93 +131,110 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor404(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor404ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '401': _response_for_401,
     '403': _response_for_403,
     '400': _response_for_400,
+    '401': _response_for_401,
     '200': _response_for_200,
+    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
-    def _list_users_as_super_admin_oapg(
+    def _get_user_as_super_admin_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def _list_users_as_super_admin_oapg(
+    def _get_user_as_super_admin_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_users_as_super_admin_oapg(
+    def _get_user_as_super_admin_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def _list_users_as_super_admin_oapg(
+    def _get_user_as_super_admin_oapg(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List all users on the instance
+        Get a full user representation
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
-        prefix_separator_iterator = None
+        _path_params = {}
         for parameter in (
-            request_query_page,
-            request_query_size,
-            request_query_sort,
-            request_query_search_term,
+            request_path_user_id,
         ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
+            parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
@@ -307,117 +262,117 @@
                 reason=response.reason,
                 api_response=api_response
             )
 
         return api_response
 
 
-class ListUsersAsSuperAdmin(BaseApi):
+class GetUserAsSuperAdmin(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_users_as_super_admin(
+    def get_user_as_super_admin(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
-    def list_users_as_super_admin(
+    def get_user_as_super_admin(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_users_as_super_admin(
+    def get_user_as_super_admin(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
-    def list_users_as_super_admin(
+    def get_user_as_super_admin(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_users_as_super_admin_oapg(
-            query_params=query_params,
+        return self._get_user_as_super_admin_oapg(
+            path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
         ApiResponseFor200,
     ]: ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
 
     def get(
         self,
-        query_params: RequestQueryParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_users_as_super_admin_oapg(
-            query_params=query_params,
+        return self._get_user_as_super_admin_oapg(
+            path_params=path_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
             skip_deserialization=skip_deserialization
         )
```

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.6.2/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/setup.py` & `iparapheur-provisioning-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.6.1"
+VERSION = "1.6.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_composite_id.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_sort_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.composite_id import CompositeId
+from iparapheur_provisioning.model.sort_object import SortObject
 from iparapheur_provisioning import configuration
 
 
-class TestCompositeId(unittest.TestCase):
-    """CompositeId unit test stubs"""
+class TestSortObject(unittest.TestCase):
+    """SortObject unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_external_signature_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.external_signature_config import ExternalSignatureConfig
+from iparapheur_provisioning.model.external_signature_provider import ExternalSignatureProvider
 from iparapheur_provisioning import configuration
 
 
-class TestExternalSignatureConfig(unittest.TestCase):
-    """ExternalSignatureConfig unit test stubs"""
+class TestExternalSignatureProvider(unittest.TestCase):
+    """ExternalSignatureProvider unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_subtype_layer_dto.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.external_signature_provider import ExternalSignatureProvider
+from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
 from iparapheur_provisioning import configuration
 
 
-class TestExternalSignatureProvider(unittest.TestCase):
-    """ExternalSignatureProvider unit test stubs"""
+class TestSubtypeLayerDto(unittest.TestCase):
+    """SubtypeLayerDto unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_metadata.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_type_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.metadata import Metadata
+from iparapheur_provisioning.model.type_dto import TypeDto
 from iparapheur_provisioning import configuration
 
 
-class TestMetadata(unittest.TestCase):
-    """Metadata unit test stubs"""
+class TestTypeDto(unittest.TestCase):
+    """TypeDto unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_layer.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_pageable_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.page_subtype_layer import PageSubtypeLayer
+from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning import configuration
 
 
-class TestPageSubtypeLayer(unittest.TestCase):
-    """PageSubtypeLayer unit test stubs"""
+class TestPageableObject(unittest.TestCase):
+    """PageableObject unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_metadata.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_pdf_signature_position.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.page_subtype_metadata import PageSubtypeMetadata
+from iparapheur_provisioning.model.pdf_signature_position import PdfSignaturePosition
 from iparapheur_provisioning import configuration
 
 
-class TestPageSubtypeMetadata(unittest.TestCase):
-    """PageSubtypeMetadata unit test stubs"""
+class TestPdfSignaturePosition(unittest.TestCase):
+    """PdfSignaturePosition unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_typology_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_typology_representation.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.page_typology_representation import PageTypologyRepresentation
+from iparapheur_provisioning.model.typology_representation import TypologyRepresentation
 from iparapheur_provisioning import configuration
 
 
-class TestPageTypologyRepresentation(unittest.TestCase):
-    """PageTypologyRepresentation unit test stubs"""
+class TestTypologyRepresentation(unittest.TestCase):
+    """TypologyRepresentation unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_user_dto.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.pageable_object import PageableObject
+from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning import configuration
 
 
-class TestPageableObject(unittest.TestCase):
-    """PageableObject unit test stubs"""
+class TestUserDto(unittest.TestCase):
+    """UserDto unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_subtype_layer_association.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.pdf_signature_position import PdfSignaturePosition
+from iparapheur_provisioning.model.subtype_layer_association import SubtypeLayerAssociation
 from iparapheur_provisioning import configuration
 
 
-class TestPdfSignaturePosition(unittest.TestCase):
-    """PdfSignaturePosition unit test stubs"""
+class TestSubtypeLayerAssociation(unittest.TestCase):
+    """SubtypeLayerAssociation unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_tenant_dto.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.sort_object import SortObject
+from iparapheur_provisioning.model.tenant_dto import TenantDto
 from iparapheur_provisioning import configuration
 
 
-class TestSortObject(unittest.TestCase):
-    """SortObject unit test stubs"""
+class TestTenantDto(unittest.TestCase):
+    """TenantDto unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_user_privilege.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.subtype_layer import SubtypeLayer
+from iparapheur_provisioning.model.user_privilege import UserPrivilege
 from iparapheur_provisioning import configuration
 
 
-class TestSubtypeLayer(unittest.TestCase):
-    """SubtypeLayer unit test stubs"""
+class TestUserPrivilege(unittest.TestCase):
+    """UserPrivilege unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_user_representation.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.subtype_layer_association import SubtypeLayerAssociation
+from iparapheur_provisioning.model.user_representation import UserRepresentation
 from iparapheur_provisioning import configuration
 
 
-class TestSubtypeLayerAssociation(unittest.TestCase):
-    """SubtypeLayerAssociation unit test stubs"""
+class TestUserRepresentation(unittest.TestCase):
+    """UserRepresentation unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_subtype_metadata_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
+from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
 from iparapheur_provisioning import configuration
 
 
-class TestSubtypeLayerDto(unittest.TestCase):
-    """SubtypeLayerDto unit test stubs"""
+class TestSubtypeMetadataDto(unittest.TestCase):
+    """SubtypeMetadataDto unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_metadata.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_type_representation.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.subtype_metadata import SubtypeMetadata
+from iparapheur_provisioning.model.type_representation import TypeRepresentation
 from iparapheur_provisioning import configuration
 
 
-class TestSubtypeMetadata(unittest.TestCase):
-    """SubtypeMetadata unit test stubs"""
+class TestTypeRepresentation(unittest.TestCase):
+    """TypeRepresentation unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_typology_sort_by.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
+from iparapheur_provisioning.model.typology_sort_by import TypologySortBy
 from iparapheur_provisioning import configuration
 
 
-class TestSubtypeMetadataDto(unittest.TestCase):
-    """SubtypeMetadataDto unit test stubs"""
+class TestTypologySortBy(unittest.TestCase):
+    """TypologySortBy unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_tenant_sort_by.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.tenant_dto import TenantDto
+from iparapheur_provisioning.model.tenant_sort_by import TenantSortBy
 from iparapheur_provisioning import configuration
 
 
-class TestTenantDto(unittest.TestCase):
-    """TenantDto unit test stubs"""
+class TestTenantSortBy(unittest.TestCase):
+    """TenantSortBy unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_user_sort_by.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.tenant_sort_by import TenantSortBy
+from iparapheur_provisioning.model.user_sort_by import UserSortBy
 from iparapheur_provisioning import configuration
 
 
-class TestTenantSortBy(unittest.TestCase):
-    """TenantSortBy unit test stubs"""
+class TestUserSortBy(unittest.TestCase):
+    """UserSortBy unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_external_signature_config_representation.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.type_dto import TypeDto
+from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_provisioning import configuration
 
 
-class TestTypeDto(unittest.TestCase):
-    """TypeDto unit test stubs"""
+class TestExternalSignatureConfigRepresentation(unittest.TestCase):
+    """ExternalSignatureConfigRepresentation unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.6.2/test/test_models/test_workflow_definition_sort_by.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.type_representation import TypeRepresentation
+from iparapheur_provisioning.model.workflow_definition_sort_by import WorkflowDefinitionSortBy
 from iparapheur_provisioning import configuration
 
 
-class TestTypeRepresentation(unittest.TestCase):
-    """TypeRepresentation unit test stubs"""
+class TestWorkflowDefinitionSortBy(unittest.TestCase):
+    """WorkflowDefinitionSortBy unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_typology_representation.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 # coding: utf-8
 
 """
-    iparapheur
 
-    iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
-    The version of the OpenAPI document: DEVELOP
-    Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.typology_representation import TypologyRepresentation
-from iparapheur_provisioning import configuration
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestTypologyRepresentation(unittest.TestCase):
-    """TypologyRepresentation unit test stubs"""
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+    """
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
+    """
     _configuration = configuration.Configuration()
 
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    response_status = 403
+
+
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 # coding: utf-8
 
 """
-    iparapheur
 
-    iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
-    The version of the OpenAPI document: DEVELOP
-    Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
+from unittest.mock import patch
+
+import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.user_dto import UserDto
-from iparapheur_provisioning import configuration
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
+from iparapheur_provisioning import configuration, schemas, api_client
+
+from .. import ApiTestMixin
 
 
-class TestUserDto(unittest.TestCase):
-    """UserDto unit test stubs"""
+class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
+    """
+    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
+        List desks  # noqa: E501
+    """
     _configuration = configuration.Configuration()
 
+    def setUp(self):
+        used_api_client = api_client.ApiClient(configuration=self._configuration)
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    response_status = 403
+
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/__init__.py` & `iparapheur-provisioning-1.6.2/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenant unit test stubs
-        Create a new tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Edit a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Delete a tenant  # noqa: E501
+        Get a full tenant description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Get a full tenant description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Edit a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Delete a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Delete a desk  # noqa: E501
+        Get a full desk description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Get a full desk description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypology(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypology unit test stubs
-        Get typology list, sorted by hierarchy.  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        List types  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        List types  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
+        Get a type with every information set  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
-        Get a type with every information set  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
+        Edit a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Create a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        List all users associated with the tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Edit a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
+        Create a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_creation_permitted_desks import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdCreationPermittedDesks(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdCreationPermittedDesks unit test stubs
-        List the desks permitted to use this subtype in a folder creation.  # noqa: E501
+    ApiProvisioningV1AdminUser unit test stubs
+        List all users on the instance  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_filterable_by_desks import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdFilterableByDesks(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdFilterableByDesks unit test stubs
-        List the desks permitted to use this subtype in a filter.  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_layer import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdLayer(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdLayer unit test stubs
-        List the layers associated with the given subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id_metadata import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdMetadata(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeIdMetadata unit test stubs
-        List the metadata associated with the given subtype  # noqa: E501
+    ApiProvisioningV1AdminTenant unit test stubs
+        Create a new tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        List all users associated with the tenant  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Delete a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Delete a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

