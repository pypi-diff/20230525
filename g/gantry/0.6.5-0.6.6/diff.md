# Comparing `tmp/gantry-0.6.5.tar.gz` & `tmp/gantry-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.5.tar", last modified: Wed May 24 20:58:09 2023, max compression
+gzip compressed data, was "gantry-0.6.6.tar", last modified: Thu May 25 20:47:42 2023, max compression
```

## Comparing `gantry-0.6.5.tar` & `gantry-0.6.6.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.618367 gantry-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-24 20:57:58.000000 gantry-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 20:57:58.000000 gantry-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-24 20:58:09.618367 gantry-0.6.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.582364 gantry-0.6.5/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.582364 gantry-0.6.5/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.586365 gantry-0.6.5/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28655 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/applications/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/applications/llm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.586365 gantry-0.6.5/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.586365 gantry-0.6.5/gantry/automations/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.590365 gantry-0.6.5/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.590365 gantry-0.6.5/gantry/automations/triggers/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/automations/triggers/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.590365 gantry-0.6.5/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.594365 gantry-0.6.5/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.594365 gantry-0.6.5/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.594365 gantry-0.6.5/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.598365 gantry-0.6.5/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93878 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.598365 gantry-0.6.5/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.602366 gantry-0.6.5/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.602366 gantry-0.6.5/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.602366 gantry-0.6.5/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 20:57:58.000000 gantry-0.6.5/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.582364 gantry-0.6.5/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-24 20:58:09.000000 gantry-0.6.5/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-24 20:58:09.000000 gantry-0.6.5/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:58:09.000000 gantry-0.6.5/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 20:58:09.000000 gantry-0.6.5/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 20:58:09.000000 gantry-0.6.5/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 20:58:09.000000 gantry-0.6.5/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:58:09.618367 gantry-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-24 20:57:58.000000 gantry-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.602366 gantry-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.606366 gantry-0.6.5/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.606366 gantry-0.6.5/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/applications/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/applications/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/applications/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/applications/test_llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/applications/test_llm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.610366 gantry-0.6.5/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.610366 gantry-0.6.5/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.610366 gantry-0.6.5/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.610366 gantry-0.6.5/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.614367 gantry-0.6.5/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   110078 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.614367 gantry-0.6.5/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.618367 gantry-0.6.5/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.618367 gantry-0.6.5/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:09.618367 gantry-0.6.5/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-24 20:57:58.000000 gantry-0.6.5/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-25 20:47:31.000000 gantry-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 20:47:31.000000 gantry-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 20:47:42.634967 gantry-0.6.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.614966 gantry-0.6.6/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28655 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/automations/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/automations/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/automations/triggers/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93878 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.622967 gantry-0.6.6/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38303 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 20:47:31.000000 gantry-0.6.6/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.618966 gantry-0.6.6/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 20:47:42.000000 gantry-0.6.6/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:47:42.634967 gantry-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-25 20:47:31.000000 gantry-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.626967 gantry-0.6.6/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/applications/test_llm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.630967 gantry-0.6.6/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110078 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38963 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:42.634967 gantry-0.6.6/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 20:47:31.000000 gantry-0.6.6/tests/test_validator.py
```

### Comparing `gantry-0.6.5/LICENSE` & `gantry-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/PKG-INFO` & `gantry-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.5
+Version: 0.6.6
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.5/gantry/__init__.py` & `gantry-0.6.6/gantry/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/alerts/client.py` & `gantry-0.6.6/gantry/alerts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         MEAN
         STD
         PDF
         QUANTILES
         PERCENT_NULL
         PERCENT_TRUE
         PERCENT_FALSE
+        PERCENT_TRUE_NOT_NULL
+        PERCENT_FALSE_NOT_NULL
         CATEGORY_PERCENTS
         ACCURACY
         MAE
         MSE
         MAPE
         MAX_ERROR
         CONFUSION_MATRIX
@@ -71,14 +73,16 @@
     MEAN = "mean"
     STD = "stddev"
     PDF = "pdf"
     QUANTILES = "quantiles"
     PERCENT_NULL = "percent_null"
     PERCENT_TRUE = "percent_true"
     PERCENT_FALSE = "percent_false"
+    PERCENT_TRUE_NOT_NULL = "percent_true_not_null"
+    PERCENT_FALSE_NOT_NULL = "percent_false_not_null"
     CATEGORY_PERCENTS = "category_percents"
     # Metric Aggregations
     ACCURACY = "accuracy_score"
     MAE = "mean_absolute_error"
     MSE = "mean_squared_error"
     MAPE = "mean_absolute_percentage_error"
     MAX_ERROR = "maximum_error"
@@ -117,15 +121,14 @@
     column_names: List[str]
     lower_bound: float
     upper_bound: float
     check_type: str = "range_check"
 
 
 class GantryAlerts:
-
     ALERT_TYPE = "RangeAlert"  # only one supported
     CHANNEL_TYPE = "SLACK_WEBHOOK"  # only one supported
 
     def __init__(self, api_client: APIClient):
         self._api_client = api_client
 
     @classmethod
```

### Comparing `gantry-0.6.5/gantry/alerts/globals.py` & `gantry-0.6.6/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/alerts/main.py` & `gantry-0.6.6/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/api_client.py` & `gantry-0.6.6/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/applications/client.py` & `gantry-0.6.6/gantry/applications/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/applications/core.py` & `gantry-0.6.6/gantry/applications/core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/applications/llm.py` & `gantry-0.6.6/gantry/applications/llm.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/applications/llm_utils.py` & `gantry-0.6.6/gantry/applications/llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/applications/main.py` & `gantry-0.6.6/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/actions/actions.py` & `gantry-0.6.6/gantry/automations/actions/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/automations.py` & `gantry-0.6.6/gantry/automations/automations.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/curators/__init__.py` & `gantry-0.6.6/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/curators/curators.py` & `gantry-0.6.6/gantry/automations/curators/curators.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,19 +167,19 @@
     A class representing a user defined curator, where the user provides the
     selection criteria using a list of selectors, as well as other metadata
     needed to create and manage the creation jobs.
     """
 
     def __init__(
         self,
+        name: str,
+        application_name: str,
         api_client: Optional[APIClient] = None,
         id: Optional[uuid.UUID] = None,
-        name: Optional[str] = None,
         curated_dataset_name: Optional[str] = None,
-        application_name: Optional[str] = None,
         start_on: Optional[datetime.datetime] = None,
         curation_interval: datetime.timedelta = datetime.timedelta(days=1),
         curation_delay: datetime.timedelta = datetime.timedelta(days=0),
         curate_past_intervals: bool = True,
         created_at: Optional[datetime.datetime] = None,
         selectors: Optional[List[Selector]] = None,
     ):
@@ -204,15 +204,15 @@
         Args:
             api_client (Optional[APIClient], optional): APIClient to use. Defaults to None,
                 in which case the Curator will use the global APIClient.
             id (Optional[uuid.UUID], optional): The id of the curator. Defaults to None. The
                 id only exists in Gantry for curators that have been created. Typically, you
                 will not need to set this. But some methods, such as
                 `Curator.from_curator_info`, will set this for you.
-            name (Optional[str], optional): The name of the curator. Defaults to None.
+            name str: The name of the curator.
             curated_dataset_name (Optional[str], optional): The name of the curated dataset.
                 Defaults to None. If None, the curated dataset name will be the same as the
                 curator name.
             application_name (str): The name of the application that the curator is running in.
             start_on (Optional[datetime.datetime], optional): The time at which the curator
                 should start curating. Defaults to None. If None, the curator will start
                 curating immediately, looking back one curation_interval.
@@ -450,30 +450,30 @@
         Args:
             api_client (APIClient): _description_
             curator_info (CuratorInfo): _description_
 
         Returns:
             Curator: _description_
         """
-        return cls(api_client, **curator_info.dict())
+        return cls(api_client=api_client, **curator_info.dict())
 
     def _form_create_curator_request(self) -> CreateCuratorRequest:
         """
         Forms a create curator request model.
 
         Returns:
             CreateCuratorRequest: Create request model.
         """
         return CreateCuratorRequest(
             name=self._name,
             curated_dataset_name=self._curated_dataset_name,
             application_name=self._application_name,
             start_on=self._start_on,
             curation_interval=self._curation_interval,
-            offset=self._curation_delay,
+            curation_delay=self._curation_delay,
             curate_past_intervals=self._curate_past_intervals,
             selectors=self._selectors,
         )
 
     def _create_curator(
         self,
         create_curator_request: CreateCuratorRequest,
```

### Comparing `gantry-0.6.5/gantry/automations/curators/main.py` & `gantry-0.6.6/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/curators/models.py` & `gantry-0.6.6/gantry/automations/curators/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from gantry.automations.curators.selectors import Selector
 
 
 class CreateCuratorRequest(BaseModel):
     application_name: str
     name: str
-    curated_dataset_name: str
     start_on: datetime.datetime
     curation_interval: datetime.timedelta
+    curated_dataset_name: Optional[str]
     curation_delay: datetime.timedelta = datetime.timedelta(days=0)
     curate_past_intervals: bool = False
     selectors: List[Selector]
 
 
 class UpdateCuratorRequest(BaseModel):
     name: str
```

### Comparing `gantry-0.6.5/gantry/automations/curators/selectors.py` & `gantry-0.6.6/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/curators/stock_curators.py` & `gantry-0.6.6/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/main.py` & `gantry-0.6.6/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/automations/triggers/triggers.py` & `gantry-0.6.6/gantry/automations/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/application.py` & `gantry-0.6.6/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/bucket.py` & `gantry-0.6.6/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/data_connector.py` & `gantry-0.6.6/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/labeling.py` & `gantry-0.6.6/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/main.py` & `gantry-0.6.6/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/projection.py` & `gantry-0.6.6/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/cli/secret.py` & `gantry-0.6.6/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/data_generator/data_generator.py` & `gantry-0.6.6/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/dataset/client.py` & `gantry-0.6.6/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/dataset/constants.py` & `gantry-0.6.6/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/dataset/gantry_dataset.py` & `gantry-0.6.6/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/dataset/main.py` & `gantry-0.6.6/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.6/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/exceptions.py` & `gantry-0.6.6/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/client.py` & `gantry-0.6.6/gantry/logger/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/constants.py` & `gantry-0.6.6/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/consumer.py` & `gantry-0.6.6/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/event_builder.py` & `gantry-0.6.6/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/main.py` & `gantry-0.6.6/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/stores.py` & `gantry-0.6.6/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/types.py` & `gantry-0.6.6/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/logger/utils.py` & `gantry-0.6.6/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/__init__.py` & `gantry-0.6.6/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/client.py` & `gantry-0.6.6/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/core/dataframe.py` & `gantry-0.6.6/gantry/query/core/dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -967,7 +967,69 @@
             Float with null percentage if num_points=1 and group_by=None (by default),
                 else pd.DataFrame.
         """
         try:
             return self._aggregate_query("percent_null", num_points=num_points, group_by=group_by)
         except (AttributeError, ValueError, KeyError):
             raise QueryError("Invalid query. GantrySeries cannot determine percent_null.")
+
+    @runs_on("bool")
+    def percent_true_not_null(
+        self, dropna: bool = False, num_points: int = 1, group_by: Optional[str] = None
+    ):
+        """
+        Runs on boolean series only.
+        Percent true of not null values, optionally drop null values before calculating result.
+
+        Args:
+            data_node (GantrySeries): GantrySeries which will be calculated
+            dropna (bool, defaults to False): if True, first drops NaN values
+                before calculating result.
+            num_points (int, defaults to 1): number of points to divide the
+                time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
+
+        Returns:
+            Float with true percentage if num_points=1 and group_by=None (by default),
+                else pd.DataFrame.
+        """
+        _temp = self
+        if dropna:
+            _temp = _temp[_temp.notna()]  # type: ignore
+        try:
+            return _temp._aggregate_query(
+                "percent_true_not_null", num_points=num_points, group_by=group_by
+            )
+        except (AttributeError, ValueError, KeyError):
+            raise QueryError("Invalid query. GantrySeries cannot determine percent_true_not_null")
+
+    @runs_on("bool")
+    def percent_false_not_null(
+        self, dropna: bool = False, num_points: int = 1, group_by: Optional[str] = None
+    ):
+        """
+        Runs on boolean series only.
+        Percent false of not null values, optionally drop null values before calculating result.
+
+        Args:
+            data_node (GantrySeries): GantrySeries which will be calculated
+            dropna (bool, defaults to False): if True, first drops NaN values
+                before calculating result.
+            num_points (int, defaults to 1): number of points to divide the
+                time window of the GantrySeries into
+            group_by (str, defaults to None): column to use as group_by. If None
+                then no group_by operation is performed and a single result is returned.
+
+        Returns:
+            Float with false percentage if num_points=1 and group_by=None (by default),
+                else pd.DataFrame.
+        """
+        _temp = self
+        if dropna:
+            _temp = _temp[_temp.notna()]  # type: ignore
+        try:
+            return _temp._aggregate_query(
+                "percent_false_not_null", num_points=num_points, group_by=group_by
+            )
+        except (AttributeError, ValueError, KeyError):
+            raise QueryError("Invalid query. GantrySeries cannot determine percent_false_not_null")
```

### Comparing `gantry-0.6.5/gantry/query/core/distance.py` & `gantry-0.6.6/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/core/metric.py` & `gantry-0.6.6/gantry/query/core/metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -530,7 +530,53 @@
                 time window of the GantrySeries into
 
         Returns:
             (pd.DataFrame) pd.DataFrame of shape (num_points, 1) percent_false
         """
         stat = "percent_false"
         return self._percent_query(stat, data_node, dropna, num_points)
+
+    @bool_type_check
+    def percent_true_not_null(
+        self,
+        data_node: GantrySeries,
+        dropna: bool = False,
+        num_points: int = 1,
+    ) -> pd.DataFrame:
+        """
+        Percent true after excluding null values
+
+        Args:
+            data_node (GantrySeries): GantrySeries which will be calculated
+            dropna (bool, defaults to False): if True, first drops NaN values
+                before calculating result.
+            num_points (int, defaults to 1): number of points to divide the
+                time window of the GantrySeries into
+
+        Returns:
+            (pd.DataFrame) pd.DataFrame of shape (num_points, 1) percent_true_not_null
+        """
+        stat = "percent_true_not_null"
+        return self._percent_query(stat, data_node, dropna, num_points)
+
+    @bool_type_check
+    def percent_false_not_null(
+        self,
+        data_node: GantrySeries,
+        dropna: bool = False,
+        num_points: int = 1,
+    ) -> pd.DataFrame:
+        """
+        Percent false after excluding null values
+
+        Args:
+            data_node (GantrySeries): GantrySeries which will be calculated
+            dropna (bool, defaults to False): if True, first drops NaN values
+                before calculating result.
+            num_points (int, defaults to 1): number of points to divide the
+                time window of the GantrySeries into
+
+        Returns:
+            (pd.DataFrame) pd.DataFrame of shape (num_points, 1) percent_false_not_null
+        """
+        stat = "percent_false_not_null"
+        return self._percent_query(stat, data_node, dropna, num_points)
```

### Comparing `gantry-0.6.5/gantry/query/core/queryframe.py` & `gantry-0.6.6/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/core/utils.py` & `gantry-0.6.6/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/distance/main.py` & `gantry-0.6.6/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/globals.py` & `gantry-0.6.6/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/main.py` & `gantry-0.6.6/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/query/metric/main.py` & `gantry-0.6.6/gantry/query/metric/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,7 +74,21 @@
 
 
 @_query_alias
 def percent_false(*args, **kwargs):
     validate_init()
     assert isinstance(globals._Query, GantryQuery)  # mypy bug- mypy/issues/4805
     return globals._Query.metric.percent_false(*args, **kwargs)
+
+
+@_query_alias
+def percent_true_not_null(*args, **kwargs):
+    validate_init()
+    assert isinstance(globals._Query, GantryQuery)  # mypy bug- mypy/issues/4805
+    return globals._Query.metric.percent_true_not_null(*args, **kwargs)
+
+
+@_query_alias
+def percent_false_not_null(*args, **kwargs):
+    validate_init()
+    assert isinstance(globals._Query, GantryQuery)  # mypy bug- mypy/issues/4805
+    return globals._Query.metric.percent_false_not_null(*args, **kwargs)
```

### Comparing `gantry-0.6.5/gantry/query/time_window.py` & `gantry-0.6.6/gantry/query/time_window.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/serializers.py` & `gantry-0.6.6/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/utils.py` & `gantry-0.6.6/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry/validators.py` & `gantry-0.6.6/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/gantry.egg-info/PKG-INFO` & `gantry-0.6.6/gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.5
+Version: 0.6.6
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.5/gantry.egg-info/SOURCES.txt` & `gantry-0.6.6/gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/setup.py` & `gantry-0.6.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     "pyyaml>=5.3.1",
     "colorama>=0.4.0",
     "label-studio-sdk>=0.0.19,<0.0.22",
     "marshmallow>=3.11.1",
     "marshmallow-oneofschema>=3.0.1",
     "monotonic>=1.4",
     "tabulate~=0.8",
-    "typing-extensions>=4.0,<4.6",
+    "typing-extensions>=4.6",
     "tqdm~=4.64",
     "halo~=0.0.31",
     "isodate~=0.6",
-    "pydantic==1.9.0",
+    "pydantic>=1.10.8",
     "python-dateutil>=2.8.1",
     "pandas",
     "numpy",
 ]
 
 
 # https://packaging.python.org/tutorials/packaging-projects/
```

### Comparing `gantry-0.6.5/tests/alerts/test_client.py` & `gantry-0.6.6/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/alerts/test_main.py` & `gantry-0.6.6/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/applications/test_client.py` & `gantry-0.6.6/tests/applications/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/applications/test_core.py` & `gantry-0.6.6/tests/applications/test_core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/applications/test_llm.py` & `gantry-0.6.6/tests/applications/test_llm.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/applications/test_llm_utils.py` & `gantry-0.6.6/tests/applications/test_llm_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/cli/test_bucket.py` & `gantry-0.6.6/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/cli/test_data_connector.py` & `gantry-0.6.6/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/cli/test_labeling.py` & `gantry-0.6.6/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/cli/test_projection.py` & `gantry-0.6.6/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/cli/test_secrets.py` & `gantry-0.6.6/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/conftest.py` & `gantry-0.6.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/curator/conftest.py` & `gantry-0.6.6/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/curator/test_curator.py` & `gantry-0.6.6/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/curator/test_main.py` & `gantry-0.6.6/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/curator/test_selectors.py` & `gantry-0.6.6/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/data_generator/test_data_generator.py` & `gantry-0.6.6/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/dataset/conftest.py` & `gantry-0.6.6/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/dataset/test_client.py` & `gantry-0.6.6/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.6/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/dataset/test_main.py` & `gantry-0.6.6/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/logger/test_client.py` & `gantry-0.6.6/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/logger/test_consumer.py` & `gantry-0.6.6/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/logger/test_event_builder.py` & `gantry-0.6.6/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/logger/test_main.py` & `gantry-0.6.6/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/logger/test_stores.py` & `gantry-0.6.6/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/logger/test_utils.py` & `gantry-0.6.6/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/conftest.py` & `gantry-0.6.6/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/core/test_dataframe.py` & `gantry-0.6.6/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/core/test_distance.py` & `gantry-0.6.6/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/core/test_filters.py` & `gantry-0.6.6/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/core/test_metric.py` & `gantry-0.6.6/tests/query/core/test_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,14 @@
 @pytest.mark.parametrize("num_points", [1, 2, 10])
 @pytest.mark.parametrize("multioutput", ["uniform_average", "raw_values", None])
 @pytest.mark.parametrize("squared", [False, True])
 @mock.patch("gantry.query.core.metric.GantryMetric._metric_query")
 def test_mean_squared_error(
     mock_query, squared, multioutput, num_points, dropna, gantry_metric_obj, series_obj_factory
 ):
-
     stat = "mean_squared_error"
     series_obj_1 = series_obj_factory("float")
     series_obj_2 = series_obj_factory("float")
     timestamp = "2022-03-20T00:00:00"
     mock_query.return_value = [{"time_stamp": timestamp, "value": 0.99}]
     result = gantry_metric_obj.mean_squared_error(
         series_obj_1,
@@ -213,15 +212,14 @@
 @pytest.mark.parametrize("dropna", [False, True])
 @pytest.mark.parametrize("num_points", [1, 2, 10])
 @pytest.mark.parametrize("multioutput", ["uniform_average", "raw_values", None])
 @mock.patch("gantry.query.core.metric.GantryMetric._metric_query")
 def test_r2_score(
     mock_query, multioutput, num_points, dropna, gantry_metric_obj, series_obj_factory
 ):
-
     stat = "r2_score"
     series_obj_1 = series_obj_factory("float")
     series_obj_2 = series_obj_factory("float")
     timestamp = "2022-03-20T00:00:00"
     mock_query.return_value = [{"time_stamp": timestamp, "value": 0.99}]
     result = gantry_metric_obj.r2_score(
         series_obj_1,
@@ -269,14 +267,16 @@
 @pytest.mark.parametrize("num_points", [1, 2, 10])
 @pytest.mark.parametrize(
     "func_name, stat",
     [
         ["percent_null", "percent_null"],
         ["percent_true", "percent_true"],
         ["percent_false", "percent_false"],
+        ["percent_true_not_null", "percent_true_not_null"],
+        ["percent_false_not_null", "percent_false_not_null"],
     ],
 )
 @mock.patch("gantry.query.core.metric.GantryMetric._metric_query")
 @mock.patch("gantry.query.core.metric._prepare_pandas_dataframe")
 @mock.patch("gantry.query.core.dataframe.GantrySeries.__getitem__")
 def test_percent_metric(
     mock_getitem,
@@ -324,15 +324,18 @@
             [series_obj_1],
             stat,
             num_points=num_points,
         )
         series_obj_1.notna.assert_not_called()
 
 
-@pytest.mark.parametrize("func_name", ["percent_true", "percent_false"])
+@pytest.mark.parametrize(
+    "func_name",
+    ["percent_true", "percent_false", "percent_true_not_null", "percent_false_not_null"],
+)
 def test_percent_bool_invalid_data_type(func_name, gantry_metric_obj, series_obj_factory):
     test_data_node = series_obj_factory("str")
     with pytest.raises(NotImplementedError):
         getattr(gantry_metric_obj, func_name)(
             data_node=test_data_node,
             stat="this-is-not-used",
             num_points=1,
```

### Comparing `gantry-0.6.5/tests/query/core/test_queryframe.py` & `gantry-0.6.6/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/core/test_series.py` & `gantry-0.6.6/tests/query/core/test_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -939,7 +939,107 @@
 @pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
 @mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
 def test_percent_false_error(mock_query, error, series_obj_bool):
     mock_query.side_effect = error
     with pytest.raises(QueryError):
         series_obj_bool.percent_false()
     mock_query.assert_called_once_with("percent_false", num_points=1, group_by=None)
+
+
+@mock.patch("gantry.query.core.dataframe.GantrySeries._filter_builder")
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+@mock.patch("gantry.query.core.dataframe.get_application_node_id")
+@mock.patch(
+    "gantry.query.core.queryframe.GantryQueryFrame.metadata",
+    return_value=MULTIPLE_FEATURES_INT_DATA,
+    new_callable=mock.PropertyMock,
+)
+@pytest.mark.parametrize("dropna", [True, False])
+def test_percent_true_not_null(
+    metadata,
+    get_application_node_id_mock,
+    mock_query,
+    mock_na,
+    series_obj_bool,
+    dropna,
+    api_client_obj,
+):
+    get_application_node_id_mock.return_value = "12345"
+    df = dataframe.GantryDataFrame(
+        api_client=api_client_obj,
+        application="foobar",
+        version="1.2.3",
+        env="dev",
+        start_time=START_TIME,
+        end_time=END_TIME,
+        filters=[],
+        tags={"foo": "bar"},
+    )
+
+    series_obj_bool.parent_dataframe = df
+
+    filters = dataframe.Filters._from_single_filter({"foo": "bar"}, series_obj_bool)
+    mock_query.return_value = 50.0
+    mock_na.return_value = filters
+    assert series_obj_bool.percent_true_not_null(dropna=dropna) == 50.0
+    mock_query.assert_called_once_with("percent_true_not_null", num_points=1, group_by=None)
+    if dropna:
+        mock_na.assert_called_once_with("null_value", False)
+
+
+@pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_percent_true_not_null_error(mock_query, error, series_obj_bool):
+    mock_query.side_effect = error
+    with pytest.raises(QueryError):
+        series_obj_bool.percent_true_not_null()
+    mock_query.assert_called_once_with("percent_true_not_null", num_points=1, group_by=None)
+
+
+@mock.patch("gantry.query.core.dataframe.GantrySeries._filter_builder")
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+@mock.patch("gantry.query.core.dataframe.get_application_node_id")
+@mock.patch(
+    "gantry.query.core.queryframe.GantryQueryFrame.metadata",
+    return_value=MULTIPLE_FEATURES_INT_DATA,
+    new_callable=mock.PropertyMock,
+)
+@pytest.mark.parametrize("dropna", [True, False])
+def test_percent_false_not_null(
+    metadata,
+    get_application_node_id_mock,
+    mock_query,
+    mock_na,
+    series_obj_bool,
+    dropna,
+    api_client_obj,
+):
+    get_application_node_id_mock.return_value = "12345"
+    df = dataframe.GantryDataFrame(
+        api_client=api_client_obj,
+        application="foobar",
+        version="1.2.3",
+        env="dev",
+        start_time=START_TIME,
+        end_time=END_TIME,
+        filters=[],
+        tags={"foo": "bar"},
+    )
+
+    series_obj_bool.parent_dataframe = df
+
+    filters = dataframe.Filters._from_single_filter({"foo": "bar"}, series_obj_bool)
+    mock_query.return_value = 50.0
+    mock_na.return_value = filters
+    assert series_obj_bool.percent_false_not_null(dropna=dropna) == 50.0
+    mock_query.assert_called_once_with("percent_false_not_null", num_points=1, group_by=None)
+    if dropna:
+        mock_na.assert_called_once_with("null_value", False)
+
+
+@pytest.mark.parametrize("error", [AttributeError, ValueError, KeyError])
+@mock.patch("gantry.query.core.dataframe.GantrySeries._aggregate_query")
+def test_percent_false_not_null_error(mock_query, error, series_obj_bool):
+    mock_query.side_effect = error
+    with pytest.raises(QueryError):
+        series_obj_bool.percent_false_not_null()
+    mock_query.assert_called_once_with("percent_false_not_null", num_points=1, group_by=None)
```

### Comparing `gantry-0.6.5/tests/query/core/test_utils.py` & `gantry-0.6.6/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/distance/test_main.py` & `gantry-0.6.6/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/metric/test_main.py` & `gantry-0.6.6/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/test_client.py` & `gantry-0.6.6/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/query/test_main.py` & `gantry-0.6.6/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/test_api_client.py` & `gantry-0.6.6/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/test_init.py` & `gantry-0.6.6/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/test_utils.py` & `gantry-0.6.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.5/tests/test_validator.py` & `gantry-0.6.6/tests/test_validator.py`

 * *Files identical despite different names*

