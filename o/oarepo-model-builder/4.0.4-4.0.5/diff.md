# Comparing `tmp/oarepo-model-builder-4.0.4.tar.gz` & `tmp/oarepo-model-builder-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-4.0.4.tar", last modified: Wed May 24 15:47:16 2023, max compression
+gzip compressed data, was "oarepo-model-builder-4.0.5.tar", last modified: Thu May 25 11:32:02 2023, max compression
```

## Comparing `oarepo-model-builder-4.0.4.tar` & `oarepo-model-builder-4.0.5.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.094508 oarepo-model-builder-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-24 15:47:16.098508 oarepo-model-builder-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.054507 oarepo-model-builder-4.0.4/oarepo_model_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.058507 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/json_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/python_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/setup_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.058507 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/templates/setup.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builders/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.058507 oarepo-model-builder-4.0.4/oarepo_model_builder/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/builtin_models/invenio.json
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.058507 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.062507 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.062507 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.062507 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.066507 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.070507 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/array.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/primitive_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/generate_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.074507 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_api_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_app_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_resource_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_script_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.078507 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/api_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/app_views.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/ext.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/imports.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/proxies.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/version.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.078507 oarepo-model-builder-4.0.4/oarepo_model_builder/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.082507 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/json_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/python.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.082507 oarepo-model-builder-4.0.4/oarepo_model_builder/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/profiles/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/profiles/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.082507 oarepo-model-builder-4.0.4/oarepo_model_builder/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/settings/opensearch.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/settings/python.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.082507 oarepo-model-builder-4.0.4/oarepo_model_builder/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.086507 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/absolute_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/camelcase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.086507 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/indented_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/simple_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/facet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/python_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/utils/verbose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.086507 oarepo-model-builder-4.0.4/oarepo_model_builder/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/validation/extensibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/validation/model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/oarepo_model_builder/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.054507 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-24 15:47:15.000000 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-24 15:47:16.000000 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:47:15.000000 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-24 15:47:15.000000 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-24 15:47:15.000000 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 15:47:15.000000 oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-24 15:47:16.098508 oarepo-model-builder-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:47:16.094508 oarepo-model-builder-4.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/faker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/multilang.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_builder_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_cfg_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_datatype_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_datatype_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_empty_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (123)    28951 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_fulltext_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_jsonchema_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_mapping_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_marshmallow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_marshmallow_ui_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_model_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_overwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_pid_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_plugin_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_python_mergers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_sample_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_schema_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_search_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_simple_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_template_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_type_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 15:46:07.000000 oarepo-model-builder-4.0.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.452272 oarepo-model-builder-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 11:32:02.452272 oarepo-model-builder-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.420271 oarepo-model-builder-4.0.5/oarepo_model_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.424271 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/json_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/python_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/setup_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.424271 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/templates/setup.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builders/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.424271 oarepo-model-builder-4.0.5/oarepo_model_builder/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/builtin_models/invenio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.428271 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.428271 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.428271 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.428271 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.432271 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.432271 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/primitive_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/generate_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.436271 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_api_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_app_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_resource_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_ui_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_ui_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_script_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.440271 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/api_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/app_views.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/ext.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/imports.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/invenio_record_facets.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/pid_provider.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/proxies.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/record_dumper.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/resource_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/ui_serializer.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/version.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.440271 oarepo-model-builder-4.0.5/oarepo_model_builder/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.440271 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/json_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.440271 oarepo-model-builder-4.0.5/oarepo_model_builder/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/profiles/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/profiles/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.440271 oarepo-model-builder-4.0.5/oarepo_model_builder/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/settings/opensearch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/settings/python.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.440271 oarepo-model-builder-4.0.5/oarepo_model_builder/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.444271 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/absolute_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/camelcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.444271 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/indented_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/simple_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/facet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/python_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/utils/verbose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.444271 oarepo-model-builder-4.0.5/oarepo_model_builder/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/validation/extensibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/validation/model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.424271 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 11:32:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-25 11:32:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:32:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-25 11:32:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 11:32:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 11:32:02.000000 oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-25 11:32:02.452272 oarepo-model-builder-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:32:02.452272 oarepo-model-builder-4.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/faker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/multilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_builder_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_cfg_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12992 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_datatype_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_datatype_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_empty_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   396304 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28951 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_fulltext_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_jsonchema_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_marshmallow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_marshmallow_ui_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23543 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_model_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_overwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_pid_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_plugin_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_python_mergers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_sample_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_schema_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_simple_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_template_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_type_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 11:31:02.000000 oarepo-model-builder-4.0.5/tests/utils.py
```

### Comparing `oarepo-model-builder-4.0.4/LICENSE` & `oarepo-model-builder-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/PKG-INFO` & `oarepo-model-builder-4.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 4.0.4
+Version: 4.0.5
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builder.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/extend.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/extend.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/json_base.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/json_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/jsonschema.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/mapping.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/model_saver.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/python.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/python.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/python_structure.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/python_structure.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builders/utils.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builders/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/builtin_models/invenio.json` & `oarepo-model-builder-4.0.5/oarepo_model_builder/builtin_models/invenio.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/cli.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/enum.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/enum.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/array.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/array.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/field.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/nested.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/nested.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/facets/object.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/facets/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/array.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/array.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/field.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/graph.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/graph.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/object.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/ui_array.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/ui_field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/marshmallow/ui_object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/app.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/app.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/blueprints.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/blueprints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/defaults.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/facets.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/facets.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             datatype,
             "build_facets",
             facets=facets,
             facet_definition=None,
             searchable=searchable,
         )
         section.config["facets"] = facets
-        datatype.definition["config"]["facets"] = facets
         return section
 
     def build_facets(self, datatype, facets, facet_definition=None, searchable=True):
         for c in datatype.children.values():
             if c.model_type == "array":
                 children = c.item.children
             else:
```

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/jsonschema.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/mapping.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/marshmallow.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/model_saver.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/permissions.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/pid.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/plugins.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/plugins.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/proxy.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/proxy.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/record.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/record_dumper.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/record_dumper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/record_metadata.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/record_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/resource.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/sample.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/search_options.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/search_options.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/service.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/ui.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/ui_marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/model/utils.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/model/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/sample.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/sample.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/components/ui.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/components/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/array.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/array.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/containers/object.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/containers/object.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/datatypes.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/datatypes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/dates.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/dates.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/model.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/model.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/primitive_types.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/primitive_types.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/datatypes/strings.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/datatypes/strings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/entrypoints.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/entrypoints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/fs.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/fs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/generate_doc.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/generate_doc.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_base.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_ext_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_jsonschemas_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_marshmallow.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_metadata_alembic_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_metadata_models_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_resource_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_search.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-
 from oarepo_model_builder.datatypes import DataType
 
 from .invenio_base import InvenioBaseClassPythonBuilder
 
 
 class InvenioRecordSearchFacetsBuilder(InvenioBaseClassPythonBuilder):
-    # TYPE = "invenio_record_search"
+    TYPE = "invenio_record_search"
     # class_config = "record-search-options-class"
     template = "record-search-options"
 
     def build_node(self, node: DataType):
         # everything is done in finish
         pass
 
     def finish(self, **extra_kwargs):
         self._generate_facets(self.current_model, **extra_kwargs)
 
     def _generate_facets(self, node: DataType, **extra_kwargs):
-        facets = node.definition["config"]["facets"]
+        facets = self.current_model.section_facets.config["facets"]
 
         package = node.definition["facets"]["module"]
         search_options_data = []
         python_path = self.class_to_path(f"{package}.facets")
         imports = []
         for f in facets:
             search_options_data.append({f["path"]: f["class"]})
```

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_search_options.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_search_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 
 class InvenioRecordSearchOptionsBuilder(InvenioBaseClassPythonBuilder):
     TYPE = "invenio_record_search_options"
     section = "search-options"
     template = "record-search-options"
 
     def finish(self, **extra_kwargs):
-        facets = self.current_model.definition["config"]["facets"]
+        facets = self.current_model.section_facets.config["facets"]
         search_data = []
         for f in facets:
             search_data.append({f["path"]: "facets." + f["path"]})
         extra_kwargs["search_data"] = search_data
         super().finish(**extra_kwargs)
```

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_search_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_record_service_config.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_record_service_config.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/invenio_script_sample_data.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/invenio_script_sample_data.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/api_views.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/api_views.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/app_views.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/app_views.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/config.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/ext.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/ext.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/invenio_record_search_options.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/marshmallow.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/permissions.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/record.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/resource_config.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/resource_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/invenio/templates/service_config.py.jinja2` & `oarepo-model-builder-4.0.5/oarepo_model_builder/invenio/templates/service_config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/loaders/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/merger.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/merger.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/cfg.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/diff.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/diff.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/json.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/json.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/json_stack.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/json_stack.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/python.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/python.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/text.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/text.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/toml.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/toml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/outputs/yaml.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/profiles/record.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/profiles/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/schema.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/templates/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/call.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/call.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/collections.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/collections.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/common.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/common.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/indented_nodes.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/indented_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/mergers.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/cst/simple_nodes.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/cst/simple_nodes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/deepmerge.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/deepmerge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/facet_helpers.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/facet_helpers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/jinja.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/properties.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/properties.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/python_name.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/python_name.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/utils/verbose.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/utils/verbose.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/validation/__init__.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/validation/extensibility.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/validation/extensibility.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/validation/model_validation.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/validation/model_validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder/validation/utils.py` & `oarepo-model-builder-4.0.5/oarepo_model_builder/validation/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/PKG-INFO` & `oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder
-Version: 4.0.4
+Version: 4.0.5
 Summary: A utility library that generates OARepo required data model files from a JSON specification file
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo model builder
```

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/SOURCES.txt` & `oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/oarepo_model_builder.egg-info/entry_points.txt` & `oarepo-model-builder-4.0.5/oarepo_model_builder.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/setup.cfg` & `oarepo-model-builder-4.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder
-version = 4.0.4
+version = 4.0.5
 description = A utility library that generates OARepo required data model files from a JSON specification file
 authors = Miroslav Bauer <bauer@cesnet.cz>, Miroslav Simek <simeki@vscht.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-4.0.4/tests/multilang.py` & `oarepo-model-builder-4.0.5/tests/multilang.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_builder_from_entrypoints.py` & `oarepo-model-builder-4.0.5/tests/test_builder_from_entrypoints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_cfg_builders.py` & `oarepo-model-builder-4.0.5/tests/test_cfg_builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_datatype_prepare.py` & `oarepo-model-builder-4.0.5/tests/test_datatype_prepare.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_datatype_validator.py` & `oarepo-model-builder-4.0.5/tests/test_datatype_validator.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_dependencies.py` & `oarepo-model-builder-4.0.5/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_empty_metadata.py` & `oarepo-model-builder-4.0.5/tests/test_empty_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_extend.py` & `oarepo-model-builder-4.0.5/tests/test_extend.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_facets.py` & `oarepo-model-builder-4.0.5/tests/test_facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_fulltext_keyword.py` & `oarepo-model-builder-4.0.5/tests/test_fulltext_keyword.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_jsonchema_builder.py` & `oarepo-model-builder-4.0.5/tests/test_jsonchema_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_loading.py` & `oarepo-model-builder-4.0.5/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_mapping_builder.py` & `oarepo-model-builder-4.0.5/tests/test_mapping_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_marshmallow_builder.py` & `oarepo-model-builder-4.0.5/tests/test_marshmallow_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_marshmallow_ui_builder.py` & `oarepo-model-builder-4.0.5/tests/test_marshmallow_ui_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_merge.py` & `oarepo-model-builder-4.0.5/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_model_saver.py` & `oarepo-model-builder-4.0.5/tests/test_model_saver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_overwrite.py` & `oarepo-model-builder-4.0.5/tests/test_overwrite.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_pid_provider.py` & `oarepo-model-builder-4.0.5/tests/test_pid_provider.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_plugin_configuration.py` & `oarepo-model-builder-4.0.5/tests/test_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_python_mergers.py` & `oarepo-model-builder-4.0.5/tests/test_python_mergers.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_raw.py` & `oarepo-model-builder-4.0.5/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_sample_builder.py` & `oarepo-model-builder-4.0.5/tests/test_sample_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_schema_props.py` & `oarepo-model-builder-4.0.5/tests/test_schema_props.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_search_options.py` & `oarepo-model-builder-4.0.5/tests/test_search_options.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_shortcuts.py` & `oarepo-model-builder-4.0.5/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_simple_builders.py` & `oarepo-model-builder-4.0.5/tests/test_simple_builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_type_shortcuts.py` & `oarepo-model-builder-4.0.5/tests/test_type_shortcuts.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/test_validation.py` & `oarepo-model-builder-4.0.5/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-4.0.4/tests/utils.py` & `oarepo-model-builder-4.0.5/tests/utils.py`

 * *Files identical despite different names*

