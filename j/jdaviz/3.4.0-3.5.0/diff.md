# Comparing `tmp/jdaviz-3.4.0.tar.gz` & `tmp/jdaviz-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdaviz-3.4.0.tar", last modified: Wed Mar 22 17:26:13 2023, max compression
+gzip compressed data, was "jdaviz-3.5.0.tar", last modified: Thu May 25 17:33:01 2023, max compression
```

## Comparing `jdaviz-3.4.0.tar` & `jdaviz-3.5.0.tar`

### file list

```diff
@@ -1,469 +1,483 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.641273 jdaviz-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.597273 jdaviz-3.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.597273 jdaviz-3.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.597273 jdaviz-3.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/changelog_check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/predeps_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-22 17:25:52.000000 jdaviz-3.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    40287 2023-03-22 17:25:52.000000 jdaviz-3.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-03-22 17:25:52.000000 jdaviz-3.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-22 17:25:52.000000 jdaviz-3.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-22 17:25:52.000000 jdaviz-3.4.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-22 17:25:52.000000 jdaviz-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-03-22 17:26:13.641273 jdaviz-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-03-22 17:25:52.000000 jdaviz-3.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-22 17:25:52.000000 jdaviz-3.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.601273 jdaviz-3.4.0/jdaviz/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79822 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/app.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.601273 jdaviz-3.4.0/jdaviz/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/docs_link.vue
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/external_link.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/glue_state_sync_wrapper.vue
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/layer_viewer_icon.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/number_uncertainty.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/play_pause_widget.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_add_results.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_auto_label.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_dataset_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_layer_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_popout.vue
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_section_header.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_subset_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_table.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/plugin_viewer_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/toolbar_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/toolbar_nested.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/tooltip.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/tray_plugin.vue
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/viewer_data_select.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/components/viewer_data_select_item.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.601273 jdaviz-3.4.0/jdaviz/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.601273 jdaviz-3.4.0/jdaviz/configs/cubeviz/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/cubeviz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/default/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/collapse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/collapse.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.605273 jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/export_plot/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/export_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/export_plot/export_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/markers.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38609 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.609273 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/default/plugins/viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/default/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/imviz/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/imviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28668 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/compass.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/compass.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.613273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/tests/test_compass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/coords_info/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/line_profile_xy/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/links_control/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/links_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/links_control/links_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue
--rw-r--r--   0 runner    (1001) docker     (123)    11608 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/imviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/imviz/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_linking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_links_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/imviz/wcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.617273 jdaviz-3.4.0/jdaviz/configs/mosviz/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41106 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/mosviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39033 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/row_lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/mosviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_data_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27491 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
--rw-r--r--   0 runner    (1001) docker     (123)    21086 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/plugins/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/specviz.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.621273 jdaviz-3.4.0/jdaviz/configs/specviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz/tests/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.625273 jdaviz-3.4.0/jdaviz/configs/specviz2d/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.625273 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.625273 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42877 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.625273 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/specviz2d.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.625273 jdaviz-3.4.0/jdaviz/configs/specviz2d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/configs/specviz2d/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/container.vue
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.625273 jdaviz-3.4.0/jdaviz/core/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/astrowidgets_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/data_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/freezable_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    35069 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/linelists.py
--rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/marks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/region_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/registries.py
--rw-r--r--   0 runner    (1001) docker     (123)    96899 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/template_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.629273 jdaviz-3.4.0/jdaviz/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/test_custom_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/test_data_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/test_region_translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/test_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/core/validunits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/jdaviz/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.629273 jdaviz-3.4.0/jdaviz/data/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/blink.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/checktoradial.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/compass.svg
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/contrast.svg
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/line_select.svg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/line_select_disabled.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/pan.svg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/pan2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/pan_x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/pan_y.svg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/panzoom_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/pixelspectra.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/radialtocheck.svg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_ellipse.svg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_lasso.svg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_single_pixel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_x.svg
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_xy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/select_y.svg
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/slice.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/spectral_range.svg
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/tune.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/zoom_back.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/zoom_box.svg
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/zoom_box_match.svg
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/zoom_xrange.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/icons/zoom_yrange.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.633273 jdaviz-3.4.0/jdaviz/data/linelists/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Atomic-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Atomic-Ionic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/CO-band-heads.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/CO.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Common_nebular.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/Common_stellar.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/DEV_NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/H-He.csv
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/H2-ISO.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/H2-alt.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/H2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/HeI-HeII.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/JWST_line_list_original.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/PAH.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/SDSS-IV.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/SDSS.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/data/linelists/linelist_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/jdaviz_cli.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.633273 jdaviz-3.4.0/jdaviz/models/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/models/physical_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.633273 jdaviz-3.4.0/jdaviz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/test_data_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/test_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/tests/test_viewer_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-03-22 17:25:52.000000 jdaviz-3.4.0/jdaviz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.601273 jdaviz-3.4.0/jdaviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 17:26:13.000000 jdaviz-3.4.0/jdaviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.637273 jdaviz-3.4.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-22 17:25:52.000000 jdaviz-3.4.0/licenses/GINGA_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-22 17:25:52.000000 jdaviz-3.4.0/licenses/IMEXAM_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-22 17:25:52.000000 jdaviz-3.4.0/licenses/IPYFILECHOOSER_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-22 17:25:52.000000 jdaviz-3.4.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-22 17:25:52.000000 jdaviz-3.4.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.637273 jdaviz-3.4.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/CubevizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/ImvizDitheredExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/ImvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/MosvizExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/MosvizNIRISSExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/Specviz2dExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/SpecvizExample.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.641273 jdaviz-3.4.0/notebooks/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_data_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_color_display.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_compass_mpl.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_custom_colormap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_line_profiles.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_load_3d_slices.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/mosviz_concept.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/mosviz_generate_photometry.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/mosviz_niriss_parser.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/mosviz_overplot_slit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/pypi_metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/specviz_from_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    82825 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/specviz_from_splot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/specviz_line_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/specviz_minimal.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/specviz_spectrum_list.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-22 17:25:52.000000 jdaviz-3.4.0/notebooks/concepts/specviz_unit_conversion.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-22 17:25:52.000000 jdaviz-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-22 17:26:13.641273 jdaviz-3.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-03-22 17:25:52.000000 jdaviz-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/share/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.641273 jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-03-22 17:25:52.000000 jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-03-22 17:25:52.000000 jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 17:25:52.000000 jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     3265 2023-03-22 17:25:52.000000 jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
--rwxr-xr-x   0 runner    (1001) docker     (123)     5993 2023-03-22 17:25:52.000000 jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.593273 jdaviz-3.4.0/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:26:13.641273 jdaviz-3.4.0/share/jupyter/voila/templates/jdaviz-default/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-22 17:25:52.000000 jdaviz-3.4.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-22 17:25:52.000000 jdaviz-3.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.bandit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/changelog_check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-25 17:32:41.000000 jdaviz-3.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    43042 2023-05-25 17:32:41.000000 jdaviz-3.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-25 17:32:41.000000 jdaviz-3.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-25 17:32:41.000000 jdaviz-3.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-25 17:32:41.000000 jdaviz-3.5.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 17:32:41.000000 jdaviz-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-25 17:33:01.116366 jdaviz-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-25 17:32:41.000000 jdaviz-3.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-25 17:32:41.000000 jdaviz-3.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.064365 jdaviz-3.5.0/jdaviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91295 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/app.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/docs_link.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/external_link.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/glue_state_sync_wrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/layer_viewer_icon.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/number_uncertainty.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/play_pause_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_add_results.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_auto_label.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_dataset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_layer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_popout.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_section_header.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_subset_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_table.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/plugin_viewer_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/toolbar_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/toolbar_nested.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/tooltip.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/tray_plugin.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/viewer_data_select.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/components/viewer_data_select_item.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz/configs/cubeviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/cubeviz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_cubeviz_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.072365 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/export_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/markers.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.076365 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40907 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/plot_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/plot_options.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/default/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/imviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.080366 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/tests/test_compass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.084365 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14173 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/imviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)    41043 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_linking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_links_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25880 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser_roman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_subset_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/imviz/wcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43652 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/mosviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40162 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.088365 jdaviz-3.5.0/jdaviz/configs/specviz/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27550 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/plugins/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/specviz.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz/tests/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42877 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/specviz2d.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.092365 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/container.vue
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.100365 jdaviz-3.5.0/jdaviz/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/astrowidgets_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/freezable_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/linelists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21700 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99210 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/template_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.100365 jdaviz-3.5.0/jdaviz/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_custom_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_data_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_region_translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/core/validunits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/jdaviz/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.104365 jdaviz-3.5.0/jdaviz/data/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/blink.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/checktoradial.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/compass.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/contrast.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/left-east.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/line_select.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/line_select_disabled.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan_x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pan_y.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/panzoom_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/pixelspectra.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/radialtocheck.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/right-east.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_ellipse.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_lasso.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_single_pixel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_x.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_xy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/select_y.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/slice.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/spectral_range.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/tune.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_box_match.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_xrange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/icons/zoom_yrange.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/jdaviz/data/linelists/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Atomic-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/CO-band-heads.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/CO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_nebular.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/Common_stellar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/DEV_NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H-He.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H-Paschen-Brackett.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20639 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H2-ISO.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H2-alt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/H2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/HeI-HeII.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/JWST_line_list_original.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/PAH.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/SDSS-IV.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/SDSS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/UV_linelist_vacuum.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/data/linelists/linelist_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/jdaviz_cli.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/jdaviz/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/models/physical_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/jdaviz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_data_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/tests/test_viewer_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-25 17:32:41.000000 jdaviz-3.5.0/jdaviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.068365 jdaviz-3.5.0/jdaviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-05-25 17:33:01.000000 jdaviz-3.5.0/jdaviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 17:33:00.000000 jdaviz-3.5.0/jdaviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.108365 jdaviz-3.5.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/GINGA_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/IMEXAM_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/IPYFILECHOOSER_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-25 17:32:41.000000 jdaviz-3.5.0/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.112365 jdaviz-3.5.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/CubevizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/ImvizDitheredExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/ImvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/MosvizExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/MosvizNIRISSExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/Specviz2dExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/SpecvizExample.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/notebooks/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_contour_overlay.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_data_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_color_display.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15370 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_compass_mpl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_custom_colormap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_dithered_gwcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_line_profiles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_load_3d_slices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_load_fits_hdu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_roman_asdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/imviz_simple_aper_phot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_concept.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_generate_photometry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_niriss_parser.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/mosviz_overplot_slit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/pypi_metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_from_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    82825 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_from_splot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_line_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_minimal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_spectrum_list.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-25 17:32:41.000000 jdaviz-3.5.0/notebooks/concepts/specviz_unit_conversion.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-25 17:32:41.000000 jdaviz-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:33:01.116366 jdaviz-3.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-05-25 17:32:41.000000 jdaviz-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3265 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5993 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.060365 jdaviz-3.5.0/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:33:01.116366 jdaviz-3.5.0/share/jupyter/voila/templates/jdaviz-default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-25 17:32:41.000000 jdaviz-3.5.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-25 17:32:41.000000 jdaviz-3.5.0/tox.ini
```

### Comparing `jdaviz-3.4.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `jdaviz-3.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `jdaviz-3.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/.github/PULL_REQUEST_TEMPLATE.md` & `jdaviz-3.5.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/.github/workflows/ci_workflows.yml` & `jdaviz-3.5.0/.github/workflows/ci_workflows.yml`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,18 @@
 
           - name: OS X - Python 3.9
             os: macos-latest
             python: 3.9
             toxenv: py39-test
             allow_failure: false
 
-          - name: Windows - Python 3.8
+          - name: Windows - Python 3.9
             os: windows-latest
-            python: 3.8
-            toxenv: py38-test
+            python: 3.9
+            toxenv: py39-test
             allow_failure: false
 
           # This also runs on cron but we want to make sure new changes
           # won't break this job at the PR stage.
           - name: Python 3.11 with latest dev versions of key dependencies, and remote data
             os: ubuntu-latest
             python: '3.11'
```

### Comparing `jdaviz-3.4.0/.github/workflows/codeql-analysis.yml` & `jdaviz-3.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/.github/workflows/predeps_workflows.yml` & `jdaviz-3.5.0/.github/workflows/predeps_workflows.yml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/.github/workflows/publish.yml` & `jdaviz-3.5.0/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
 
     - name: Install python-build and twine
       run: python -m pip install build "twine>=3.3"
 
     - name: Build package
       run: python -m build --sdist --wheel .
```

### Comparing `jdaviz-3.4.0/.gitignore` & `jdaviz-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/.readthedocs.yaml` & `jdaviz-3.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/CHANGES.rst` & `jdaviz-3.5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,101 @@
+3.5 (2023-05-25)
+================
+
+New Features
+------------
+
+- Model fitting results are logged in a table within the plugin. [#2093]
+
+- Auto-identify a configuration/helper for a given data file. [#2124]
+
+- Exact-text filtering for metadata plugin. [#2147]
+
+- Update Subset Plugin to utilize ``get_subsets()``. [#2157]
+
+- Histogram showing image values in stretch limits section of plot options plugin. [#2153]
+
+- Vertical (y-range) zoom tool for all spectrum and spectrum-2d viewers.  This also modifies
+  the icon of the horizontal (x-range) tool to be more consistent with the horizontal subset
+  selection tool. [#2206, #2212]
+
+- Allow Subset Plugin to edit composite subsets. [#2182]
+
+- Support for Scatter plots/markers in plot options. [#2193]
+
+Cubeviz
+^^^^^^^
+
+- ``get_data`` now supports ``function=True`` to adopt the collapse-function from the spectrum viewer.
+  [#2117]
+
+- ``get_data`` now supports applying a spectral mask to a collapse spatial subset. [#2199, #2214]
+
+Imviz
+^^^^^
+
+- Table exposing past results in the aperture photometry plugin. [#1985, #2015]
+
+- New canvas rotation plugin to rotate displayed image without affecting actual data. [#1983]
+
+- Preliminary support for Roman ASDF data products. This requires
+  ``roman-datamodels`` to be installed separately by the user. [#1822]
+
+- Canvas Rotation plugin is now disabled for non-Chromium based browsers [#2192]
+
+Mosviz
+^^^^^^
+
+- NIRSpec automatic loader now can take a single image as input, instead of requiring
+  the number of cutouts to be the same as the number of 1D spectra. [#2146]
+
+API Changes
+-----------
+
+- Add ``get_subsets()`` method to app level to centralize subset information
+  retrieval. [#2087, #2116, #2138]
+
+Imviz
+^^^^^
+
+- Saving a plot to a PNG (via the astrowidgets API or export plot plugin API) with a provided
+  filename will no longer show the file dialog.  If the given file exists, it is silently
+  overwritten. [#929]
+
+Bug Fixes
+---------
+
+- Fixed a bug where Import Data button crashes under certain condition. [#2110]
+
+Cubeviz
+^^^^^^^
+
+- Fixed get_model_parameters error when retrieving parameters for a cube fit. This
+  also removed the "_3d" previously appended to model labels in the returned dict. [#2171]
+
+Imviz
+^^^^^
+
+- Do not hide previous results in aperture photometry when there is a failure, but rather show
+  the failure message within the plugin UI to indicate the shown results are "out of date". [#2112]
+
+- More efficient parser for Roman data products in Imviz [#2176]
+
+Mosviz
+^^^^^^
+
+- Fixed several data loader bugs for uncommon use cases. [#2146]
+
+Other Changes and Additions
+---------------------------
+
+- move build configuration to ``pyproject.toml`` as defined in PEP621 [#1661]
+
+- drop support for Python 3.8 [#2152]
+
 3.4 (2023-03-22)
 ================
 
 New Features
 ------------
 
 - CLI launchers no longer require data to be specified. [#1890]
@@ -54,14 +148,15 @@
 - Removed deprecated ``MosViz``; use ``Mosviz``. [#2092]
 
 Specviz
 ^^^^^^^
 
 - Removed deprecated ``SpecViz``; use ``Specviz``. [#2092]
 
+
 Bug Fixes
 ---------
 
 Cubeviz
 ^^^^^^^
 
 - Fixed a bug where sky coordinates reported to coordinates info panel
```

### Comparing `jdaviz-3.4.0/CITATION.cff` & `jdaviz-3.5.0/CITATION.cff`

 * *Files 5% similar despite different names*

```diff
@@ -56,19 +56,22 @@
   orcid: "https://orcid.org/0000-0002-4679-5692"
 - family-names: "Pacifici"
   given-names: "Camilla"
   orcid: "https://orcid.org/0000-0003-4196-0617"
 - family-names: "Robitaille"
   given-names: "Thomas"
   orcid: "https://orcid.org/0000-0002-8642-1329"
+- family-names: "Shanahan"
+  given-names: "Clare"
+  orcid: "https://orcid.org/0009-0008-4112-7418"
 - family-names: "Tollerud"
   given-names: "Erik"
   orcid: "https://orcid.org/0000-0002-9599-310X"
 - family-names: "Volfman"
   given-names: "Sabrina"
 title: "Jdaviz"
-version: 3.4.0
+version: 3.5.0
 doi: https://doi.org/10.5281/zenodo.5513927
-date-released: 2023-03-22
+date-released: 2023-05-25
 url: "https://github.com/spacetelescope/jdaviz"
 
 # see a full list of contributors here: https://github.com/spacetelescope/jdaviz/graphs/contributors
```

### Comparing `jdaviz-3.4.0/CODE_OF_CONDUCT.md` & `jdaviz-3.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/LICENSE.rst` & `jdaviz-3.5.0/LICENSE.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020-2022 JDADF Developers
+Copyright 2020-2023 JDADF Developers
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jdaviz-3.4.0/PKG-INFO` & `jdaviz-3.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.4.0
+Version: 3.5.0
 Summary: Astronomical data analysis development leveraging the Jupyter platform
-Home-page: https://jdaviz.readthedocs.io/en/latest/
-Author: JDADF Developers
-Author-email: rosteen@stsci.edu
-License: BSD 3-Clause
+Author-email: JDADF Developers <rosteen@stsci.edu>
+Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: roman
 License-File: LICENSE.rst
 
 .. image:: docs/logos/jdaviz.svg
     :width: 400
     :alt: Jdaviz logo
     :align: center
 
@@ -106,18 +105,22 @@
 The power of ``jdaviz`` is that it can integrated into your Jupyter notebook workflow:
 
 .. code-block:: python
 
     from jdaviz import Specviz
 
     specviz = Specviz()
-    specviz.app
+    specviz.show()
 
 To learn more about the various ``jdaviz`` application configurations and loading data, see the
-`specviz <https://jdaviz.readthedocs.io/en/latest/specviz/import_data.html>`_, `cubeviz <https://jdaviz.readthedocs.io/en/latest/cubeviz/import_data.html>`_, `mosviz <https://jdaviz.readthedocs.io/en/latest/mosviz/import_data.html>`_, or `imviz <https://jdaviz.readthedocs.io/en/latest/imviz/import_data.html>`_ tools.
+`Specviz <https://jdaviz.readthedocs.io/en/latest/specviz/import_data.html>`_,
+`Cubeviz <https://jdaviz.readthedocs.io/en/latest/cubeviz/import_data.html>`_,
+`Mosviz <https://jdaviz.readthedocs.io/en/latest/mosviz/import_data.html>`_,
+`Imviz <https://jdaviz.readthedocs.io/en/latest/imviz/import_data.html>`_,
+or `Specviz2D <https://jdaviz.readthedocs.io/en/latest/specviz2d/import_data.html>`_ tools.
 
 ``jdaviz`` also provides a directory of `sample notebooks <https://jdaviz.readthedocs.io/en/latest/sample_notebooks.html>`_ to test the application, located in the ``notebooks`` sub-directory
 of the git repository.  ``CubevizExample.ipynb`` is provided as an example that loads a JWST data cube with the
 ``Cubeviz`` configuration.  To run the provided example, start the Jupyter kernel with the notebook path:
 
 .. code-block:: bash
 
@@ -127,14 +130,19 @@
 ----
 
 If you uncover any issues or bugs, you can
 `open a GitHub issue <https://github.com/spacetelescope/jdaviz/issues/new/choose>`_
 if they are not already reported. For faster responses, however, we encourage you to
 submit a `JWST Help Desk Ticket <https://jwsthelp.stsci.edu>`_.
 
+Recordings and instructional notebooks from live Jdaviz tutorials (as part of the JWebbinars series)
+can be found at `the JWebbinar website <https://www.stsci.edu/jwst/science-execution/jwebbinars>`_
+under the "Materials and Videos" expandable section. Scroll down to the bottom of that section to
+find materials from the most recent session (JWebbinar 24, March 2023).
+
 License & Attribution
 ---------------------
 
 This project is Copyright (c) JDADF Developers and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
 the `Astropy package template <https://github.com/astropy/package-template>`_
 which is licensed under the BSD 3-clause licence. See the
@@ -142,15 +150,15 @@
 folder for more information.
 
 Cite ``jdaviz`` via our Zenodo record: https://doi.org/10.5281/zenodo.5513927.
 
 Contributing
 ------------
 
-We love contributions! jdaviz is open source,
+We love contributions! ``jdaviz`` is open source,
 built on open source, and we'd love to have you hang out in our community.
 
 **Imposter syndrome disclaimer**: We want your help. No, really.
 
 There may be a little voice inside your head that is telling you that you're not
 ready to be an open source contributor; that your skills aren't nearly good
 enough to contribute. What could you possibly offer a project like this one?
```

### Comparing `jdaviz-3.4.0/README.rst` & `jdaviz-3.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -92,18 +92,22 @@
 The power of ``jdaviz`` is that it can integrated into your Jupyter notebook workflow:
 
 .. code-block:: python
 
     from jdaviz import Specviz
 
     specviz = Specviz()
-    specviz.app
+    specviz.show()
 
 To learn more about the various ``jdaviz`` application configurations and loading data, see the
-`specviz <https://jdaviz.readthedocs.io/en/latest/specviz/import_data.html>`_, `cubeviz <https://jdaviz.readthedocs.io/en/latest/cubeviz/import_data.html>`_, `mosviz <https://jdaviz.readthedocs.io/en/latest/mosviz/import_data.html>`_, or `imviz <https://jdaviz.readthedocs.io/en/latest/imviz/import_data.html>`_ tools.
+`Specviz <https://jdaviz.readthedocs.io/en/latest/specviz/import_data.html>`_,
+`Cubeviz <https://jdaviz.readthedocs.io/en/latest/cubeviz/import_data.html>`_,
+`Mosviz <https://jdaviz.readthedocs.io/en/latest/mosviz/import_data.html>`_,
+`Imviz <https://jdaviz.readthedocs.io/en/latest/imviz/import_data.html>`_,
+or `Specviz2D <https://jdaviz.readthedocs.io/en/latest/specviz2d/import_data.html>`_ tools.
 
 ``jdaviz`` also provides a directory of `sample notebooks <https://jdaviz.readthedocs.io/en/latest/sample_notebooks.html>`_ to test the application, located in the ``notebooks`` sub-directory
 of the git repository.  ``CubevizExample.ipynb`` is provided as an example that loads a JWST data cube with the
 ``Cubeviz`` configuration.  To run the provided example, start the Jupyter kernel with the notebook path:
 
 .. code-block:: bash
 
@@ -113,14 +117,19 @@
 ----
 
 If you uncover any issues or bugs, you can
 `open a GitHub issue <https://github.com/spacetelescope/jdaviz/issues/new/choose>`_
 if they are not already reported. For faster responses, however, we encourage you to
 submit a `JWST Help Desk Ticket <https://jwsthelp.stsci.edu>`_.
 
+Recordings and instructional notebooks from live Jdaviz tutorials (as part of the JWebbinars series)
+can be found at `the JWebbinar website <https://www.stsci.edu/jwst/science-execution/jwebbinars>`_
+under the "Materials and Videos" expandable section. Scroll down to the bottom of that section to
+find materials from the most recent session (JWebbinar 24, March 2023).
+
 License & Attribution
 ---------------------
 
 This project is Copyright (c) JDADF Developers and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
 the `Astropy package template <https://github.com/astropy/package-template>`_
 which is licensed under the BSD 3-clause licence. See the
@@ -128,15 +137,15 @@
 folder for more information.
 
 Cite ``jdaviz`` via our Zenodo record: https://doi.org/10.5281/zenodo.5513927.
 
 Contributing
 ------------
 
-We love contributions! jdaviz is open source,
+We love contributions! ``jdaviz`` is open source,
 built on open source, and we'd love to have you hang out in our community.
 
 **Imposter syndrome disclaimer**: We want your help. No, really.
 
 There may be a little voice inside your head that is telling you that you're not
 ready to be an open source contributor; that your skills aren't nearly good
 enough to contribute. What could you possibly offer a project like this one?
```

### Comparing `jdaviz-3.4.0/conftest.py` & `jdaviz-3.5.0/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,10 @@
     PYTEST_HEADER_MODULES['ipysplitpanes'] = 'ipysplitpanes'
     PYTEST_HEADER_MODULES['ipygoldenlayout'] = 'ipygoldenlayout'
     PYTEST_HEADER_MODULES['voila'] = 'voila'
     PYTEST_HEADER_MODULES['vispy'] = 'vispy'
     PYTEST_HEADER_MODULES['gwcs'] = 'gwcs'
     PYTEST_HEADER_MODULES['asdf'] = 'asdf'
     PYTEST_HEADER_MODULES['stdatamodels'] = 'stdatamodels'
+    PYTEST_HEADER_MODULES['roman_datamodels'] = 'roman_datamodels'
 
     TESTED_VERSIONS['jdaviz'] = __version__
```

### Comparing `jdaviz-3.4.0/jdaviz/__init__.py` & `jdaviz-3.5.0/jdaviz/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/app.py` & `jdaviz-3.5.0/jdaviz/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import os
 import pathlib
 import re
 import uuid
 import warnings
 from inspect import isclass
+import operator
 
 from ipywidgets import widget_serialization
 import ipyvue
 
 from astropy.nddata import CCDData, NDData
 from astropy.io import fits
+from astropy import units as u
+from astropy.coordinates import Angle
+from astropy.time import Time
+from regions import PixCoord, CirclePixelRegion, RectanglePixelRegion, EllipsePixelRegion
 
 from echo import CallbackProperty, DictCallbackProperty, ListCallbackProperty
 from ipygoldenlayout import GoldenLayout
 from ipysplitpanes import SplitPanes
 from traitlets import Dict, Bool, Unicode, Any
 from specutils import Spectrum1D, SpectralRegion
 import matplotlib.cm as cm
@@ -27,28 +32,31 @@
 from glue.plugins.wcs_autolinking.wcs_autolinking import WCSLink, IncompatibleWCS
 from glue.core.message import (DataCollectionAddMessage,
                                DataCollectionDeleteMessage,
                                SubsetCreateMessage,
                                SubsetUpdateMessage,
                                SubsetDeleteMessage)
 from glue.core.state_objects import State
-from glue.core.subset import Subset, RangeSubsetState, RoiSubsetState
+from glue.core.subset import (Subset, RangeSubsetState, RoiSubsetState,
+                              CompositeSubsetState, InvertState)
+from glue.core.roi import CircularROI, EllipticalROI, RectangularROI
 from glue_astronomy.spectral_coordinates import SpectralCoordinates
 from glue_jupyter.app import JupyterApplication
 from glue_jupyter.common.toolbar_vuetify import read_icon
 from glue_jupyter.state_traitlets_helpers import GlueState
 from glue_jupyter.bqplot.profile import BqplotProfileView
 from ipyvuetify import VuetifyTemplate
 
 from jdaviz import __version__
 from jdaviz.core.config import read_configuration, get_configuration
 from jdaviz.core.events import (LoadDataMessage, NewViewerMessage, AddDataMessage,
                                 SnackbarMessage, RemoveDataMessage,
                                 AddDataToViewerMessage, RemoveDataFromViewerMessage,
                                 ViewerAddedMessage, ViewerRemovedMessage)
+from jdaviz.core.style_widget import StyleWidget
 from jdaviz.core.registries import (tool_registry, tray_registry, viewer_registry,
                                     data_parser_registry)
 from jdaviz.core.tools import ICON_DIR
 from jdaviz.utils import SnackbarQueue, alpha_index
 from ipypopout import PopoutButton
 
 __all__ = ['Application']
@@ -169,14 +177,18 @@
     tray_items_filter = CallbackProperty(
         '', docstring='User-filter on tray items')
 
     stack_items = ListCallbackProperty(
         docstring="Nested collection of viewers constructed to support the "
                   "Golden Layout viewer area.")
 
+    style_widget = CallbackProperty(
+        '', docstring="Jupyter widget that won't be displayed but can apply css to the app"
+    )
+
 
 class Application(VuetifyTemplate, HubListener):
     """
     The main application object containing implementing the ipyvue/vuetify
     template instructions for composing the interface.
     """
     _metadata = Dict({"mount_id": "content"}).tag(sync=True)
@@ -340,14 +352,28 @@
 
     @history_verbosity.setter
     def history_verbosity(self, val):
         if val not in _verbosity_levels:
             raise ValueError(f'Invalid verbosity: {val}')
         self._history_verbosity = val
 
+    def set_style_template_file(self, path):
+        """
+        Sets the path to a vue file containing a <style> tag that will be applied on top of the
+        style defined in ``app.vue``.  This is useful for config-specific or downstream styling
+        at the app-level.
+
+        Parameters
+        ----------
+        path : str or tuple
+            Path to a ``.vue`` file containing style rules to inject into the app.
+        """
+        style_widget = StyleWidget(path)
+        self.state.style_widget = "IPY_MODEL_" + style_widget.model_id
+
     def _on_snackbar_message(self, msg):
         """
         Displays a toast message with an editable message that be dismissed
         manually or will dismiss automatically after a timeout.
 
         Whether the message shows as a snackbar popup is controlled by ``self.verbosity``,
         whether the message is added to the history log is controlled by ``self.history_verbosity``.
@@ -561,33 +587,32 @@
         This is *not* an ``IPyWidget``. This is stored here because
         the state of the viewer and data methods that allow add/removing data
         to the viewer exist in a wrapper around the core ``IPyWidget``, which
         is needed to interact with the data rendered within a viewer.
 
         Notes
         -----
-            This is only used in cases where the viewers have been pre-defined
-            in the configuration file. Otherwise, viewers are not stored via
-            reference.
+        If viewer does not have a reference, it is going to try to look
+        up the viewer using the given reference as ID.
 
         Parameters
         ----------
         viewer_reference : str
             The reference to the viewer defined with the ``reference`` key
-            in the yaml configuration file.
+            in the YAML configuration file.
 
         Returns
         -------
-        `~glue_jupyter.bqplot.common.BqplotBaseView`
+        viewer : `~glue_jupyter.bqplot.common.BqplotBaseView`
             The viewer class instance.
         """
-        return self._viewer_by_reference(viewer_reference)
+        return self._viewer_by_reference(viewer_reference, fallback_to_id=True)
 
     def get_viewer_by_id(self, vid):
-        """Like :meth:`get_viewer` but use ID instead of reference name.
+        """Like :meth:`get_viewer` but use ID directly instead of reference name.
         This is useful when reference name is `None`.
         """
         return self._viewer_store.get(vid)
 
     def get_data_from_viewer(self, viewer_reference, data_label=None,
                              cls='default', include_subsets=True):
         """
@@ -676,16 +701,21 @@
                 elif isinstance(layer_state.layer, Subset):
                     if include_subsets:
                         layer_data = layer_state.layer
 
                         if cls is not None:
                             handler, _ = data_translator.get_handler_for(cls)
                             try:
-                                layer_data = handler.to_object(layer_data,
-                                                               statistic=statistic)
+                                if cls == Spectrum1D:
+                                    # if this is a spectrum, apply the `statistic`:
+                                    layer_data = handler.to_object(layer_data,
+                                                                   statistic=statistic)
+                                else:
+                                    # otherwise simply translate to an object:
+                                    layer_data = handler.to_object(layer_data)
                             except IncompatibleAttribute:
                                 continue
 
                         data[label] = layer_data
 
         # If a data label was provided, return only the corresponding data, otherwise return all:
         return data.get(data_label, data)
@@ -725,62 +755,14 @@
         """
         viewer = self.get_viewer(viewer_reference)
         data = self.get_data_from_viewer(viewer_reference,
                                          data_label,
                                          cls=None)
         regions = {}
 
-        def _get_all_subregions(mask, spec_axis_data):
-            """
-            Return all subregions within a subset.
-
-            Parameters
-            ----------
-            mask : list
-                List of indices in spec_axis_data that are part of the subset.
-            spec_axis_data : list
-                List of spectral axis values.
-            Returns
-            -------
-            combined_spec_region : `~specutils.SpectralRegion`
-                SpectralRegion object containing all subregions of the subset.
-            """
-            if len(mask) == 0:
-                # Mask should only be 0 if ApplyROI is used to incorrectly
-                # create subsets via the API
-                raise ValueError("Mask has length 0, ApplyROI may have been used incorrectly")
-
-            current_edge = 0
-            combined_spec_region = None
-            for index in range(1, len(mask)):
-                # Find spot where mask == True is for a different region of the subset
-                # i.e. mask = [0, 1, 4, 5]
-                # mask[2] != mask[1] + 1
-                if mask[index] != mask[index - 1] + 1:
-                    subset_region = spec_axis_data[mask[current_edge]: mask[index - 1] + 1]
-                    if not combined_spec_region:
-                        combined_spec_region = SpectralRegion(min(subset_region),
-                                                              max(subset_region))
-                    else:
-                        combined_spec_region += SpectralRegion(min(subset_region),
-                                                               max(subset_region))
-                    current_edge = index
-
-            # Get last region within the subset
-            if current_edge != index:
-                subset_region = spec_axis_data[mask[current_edge]: mask[index] + 1]
-                # No if check here because len(mask) must be greater than 1
-                # so combined_spec_region will have been instantiated in the for loop
-                if combined_spec_region is None:
-                    combined_spec_region = SpectralRegion(min(subset_region), max(subset_region))
-                else:
-                    combined_spec_region += SpectralRegion(min(subset_region), max(subset_region))
-
-            return combined_spec_region
-
         if data_label is not None:
             data = {data_label: data}
 
         for key, value in data.items():
             if isinstance(value, Subset):
                 # Get the component type in a compound subset
                 if hasattr(value.subset_state, "state1"):
@@ -807,38 +789,20 @@
                     continue
 
                 # There is a special case for 1d data (which is also not
                 #  supported currently). We now eschew the use of the
                 #  translation machinery entirely and construct the astropy
                 #  region ourselves.
                 elif value.data.ndim == 1:
-                    # Grab the data units from the glue-astronomy spectral axis
-                    # TODO: this needs to be much simpler; i.e. data units in
-                    #  the glue component objects
-                    # Cases where there is a single subset
-                    if '_orig_spec' in value.data.meta:  # Hack for Cubeviz WCS propagation
-                        data_wcs = value.data.meta['_orig_spec']
-                    else:
-                        data_wcs = value.data.coords
-
-                    subregions_in_subset = _get_all_subregions(
-                            np.where(value.to_mask() == True)[0], # noqa
-                            data_wcs.spectral_axis)
-
-                    regions[key] = subregions_in_subset
+                    regions[key] = self.get_subsets(key)
                     continue
 
                 temp_data = self.get_data_from_viewer(viewer_reference, value.label)
                 if isinstance(temp_data, Spectrum1D):
-                    # Note that we look for mask == False here, rather than True above,
-                    # because specutils masks are the reverse of Glue (of course)
-                    subregions_in_subset = _get_all_subregions(
-                             np.where(~temp_data.mask)[0], # noqa
-                             temp_data.spectral_axis)
-                    regions[key] = subregions_in_subset
+                    regions[key] = self.get_subsets(key)
                     continue
 
                 # Get the pixel coordinate [z] of the 3D data, repeating the
                 #  wavelength axis. This doesn't seem strictly necessary as it
                 #  returns the same data if the pixel axis is [y] or [x]
                 xid = value.data.pixel_component_ids[0]
 
@@ -883,14 +847,290 @@
                 #  useful, only the x values are.
                 region = subset_group.subsets[0].data.get_selection_definition(
                     format='astropy-regions')
                 regions[key] = region
 
         return regions
 
+    def get_subsets(self, subset_name=None, spectral_only=False,
+                    spatial_only=False, object_only=False, simplify_spectral=True):
+        """
+        Returns all branches of glue subset tree in the form that subset plugin can recognize.
+
+        Parameters
+        ----------
+        subset_name : str
+            The subset name.
+        spectral_only : bool
+            Return only spectral subsets.
+        spatial_only : bool
+            Return only spatial subsets, except masked subsets (uncommon).
+        object_only : bool
+            Return only object relevant information and
+            leave out the region class name and glue_state.
+        simplify_spectral : bool
+            Return a composite spectral subset collapsed to a simplified SpectralRegion.
+
+        Returns
+        -------
+        data : dict
+            A dict with keys representing the subset name and values as astropy regions
+            objects.
+        """
+
+        dc = self.data_collection
+        subsets = dc.subset_groups
+
+        all_subsets = {}
+
+        for subset in subsets:
+            label = subset.label
+            if isinstance(subset.subset_state, CompositeSubsetState):
+                # Region composed of multiple ROI or Range subset
+                # objects that must be traversed
+                subset_region = self.get_sub_regions(subset.subset_state, simplify_spectral)
+            elif isinstance(subset.subset_state, RoiSubsetState):
+                # 3D regions represented as a dict including an
+                # AstropyRegion object if possible
+                subset_region = self._get_roi_subset_definition(subset.subset_state)
+            elif isinstance(subset.subset_state, RangeSubsetState):
+                # 2D regions represented as SpectralRegion objects
+                subset_region = self._get_range_subset_bounds(subset.subset_state,
+                                                              simplify_spectral)
+            else:
+                # subset.subset_state can be an instance of MaskSubsetState
+                # or something else we do not know how to handle
+                all_subsets[label] = None
+                continue
+
+            # Is the subset spectral, spatial, temporal?
+            is_spectral = self._is_subset_spectral(subset_region)
+            is_temporal = self._is_subset_temporal(subset_region)
+
+            # Remove duplicate spectral regions
+            if is_spectral and isinstance(subset_region, SpectralRegion):
+                subset_region = self._remove_duplicate_bounds(subset_region)
+
+            if spectral_only and is_spectral:
+                if object_only and not simplify_spectral:
+                    all_subsets[label] = [reg['region'] for reg in subset_region]
+                else:
+                    all_subsets[label] = subset_region
+            elif spatial_only and not is_spectral:
+                if object_only:
+                    all_subsets[label] = [reg['region'] for reg in subset_region]
+                else:
+                    all_subsets[label] = subset_region
+            elif not spectral_only and not spatial_only:
+                if object_only and not isinstance(subset_region, SpectralRegion):
+                    all_subsets[label] = [reg['region'] for reg in subset_region]
+                else:
+                    all_subsets[label] = subset_region
+
+            if not (spectral_only or spatial_only) and is_temporal:
+                if object_only:
+                    all_subsets[label] = [reg['region'] for reg in subset_region]
+                else:
+                    all_subsets[label] = subset_region
+
+        all_subset_names = [subset.label for subset in dc.subset_groups]
+        if subset_name and subset_name in all_subset_names:
+            return all_subsets[subset_name]
+        elif subset_name:
+            raise ValueError(f"{subset_name} not in {all_subset_names}")
+        else:
+            return all_subsets
+
+    def _is_subset_spectral(self, subset_region):
+        if isinstance(subset_region, SpectralRegion):
+            return True
+        elif isinstance(subset_region, list) and len(subset_region) > 0:
+            if isinstance(subset_region[0]['region'], SpectralRegion):
+                return True
+        return False
+
+    def _is_subset_temporal(self, subset_region):
+        if isinstance(subset_region, Time):
+            return True
+        elif isinstance(subset_region, list) and len(subset_region) > 0:
+            if isinstance(subset_region[0]['region'], Time):
+                return True
+        return False
+
+    def _remove_duplicate_bounds(self, spec_regions):
+        regions_no_dups = None
+
+        for region in spec_regions:
+            if not regions_no_dups:
+                regions_no_dups = region
+            elif region.bounds not in regions_no_dups.subregions:
+                regions_no_dups += region
+        return regions_no_dups
+
+    def _get_range_subset_bounds(self, subset_state, simplify_spectral=True):
+        # TODO: Use global display units
+        # units = dc[0].data.coords.spectral_axis.unit
+        viewer = self.get_viewer(self._jdaviz_helper. _default_spectrum_viewer_reference_name)
+        data = viewer.data()
+        if viewer:
+            units = u.Unit(viewer.state.x_display_unit)
+        elif data and len(data) > 0 and isinstance(data[0], Spectrum1D):
+            units = data[0].spectral_axis.unit
+        else:
+            raise ValueError("Unable to find spectral axis units")
+
+        spec_region = SpectralRegion(subset_state.lo * units, subset_state.hi * units)
+        if not simplify_spectral:
+            return [{"name": subset_state.__class__.__name__,
+                     "glue_state": subset_state.__class__.__name__,
+                     "region": spec_region,
+                     "subset_state": subset_state}]
+        return spec_region
+
+    def _get_roi_subset_definition(self, subset_state):
+        _around_decimals = 6
+        roi = subset_state.roi
+        roi_as_region = None
+        if isinstance(roi, CircularROI):
+            x, y = roi.get_center()
+            r = roi.radius
+            roi_as_region = CirclePixelRegion(PixCoord(x, y), r)
+
+        elif isinstance(roi, RectangularROI):
+            theta = np.around(np.degrees(roi.theta), decimals=_around_decimals)
+            roi_as_region = RectanglePixelRegion(PixCoord(roi.center()[0], roi.center()[1]),
+                                                 roi.width(), roi.height(), Angle(theta, "deg"))
+
+        elif isinstance(roi, EllipticalROI):
+            xc = roi.xc
+            yc = roi.yc
+            rx = roi.radius_x
+            ry = roi.radius_y
+            theta = np.around(np.degrees(roi.theta), decimals=_around_decimals)
+            roi_as_region = EllipsePixelRegion(PixCoord(xc, yc), rx, ry, Angle(theta, "deg"))
+
+        return [{"name": subset_state.roi.__class__.__name__,
+                 "glue_state": subset_state.__class__.__name__,
+                 "region": roi_as_region,
+                 "subset_state": subset_state}]
+
+    def get_sub_regions(self, subset_state, simplify_spectral=True):
+
+        if isinstance(subset_state, CompositeSubsetState):
+            if subset_state and hasattr(subset_state, "state2") and subset_state.state2:
+                one = self.get_sub_regions(subset_state.state1, simplify_spectral)
+                two = self.get_sub_regions(subset_state.state2, simplify_spectral)
+
+                if isinstance(one, list) and "glue_state" in one[0]:
+                    one[0]["glue_state"] = subset_state.__class__.__name__
+
+                if isinstance(subset_state.state2, InvertState):
+                    # This covers the REMOVE subset mode
+
+                    # As an example for how this works:
+                    # a = SpectralRegion(4 * u.um, 7 * u.um) + SpectralRegion(9 * u.um, 11 * u.um)
+                    # b = SpectralRegion(5 * u.um, 6 * u.um)
+                    # After running the following code with a as one and b as two:
+                    # Spectral Region, 3 sub-regions:
+                    #   (4.0 um, 5.0 um)    (6.0 um, 7.0 um)    (9.0 um, 11.0 um)
+                    if isinstance(two, SpectralRegion):
+                        new_spec = None
+                        for sub in one:
+                            if not new_spec:
+                                new_spec = two.invert(sub.lower, sub.upper)
+                            else:
+                                new_spec += two.invert(sub.lower, sub.upper)
+                        return new_spec
+                    else:
+                        if isinstance(two, list):
+                            two[0]['glue_state'] = "AndNotState"
+                        # Return two first so that we preserve the chronology of how
+                        # subset regions are applied.
+                        return one + two
+                elif subset_state.op is operator.and_:
+                    # This covers the AND subset mode
+
+                    # Example of how this works with "one" being the AND region
+                    # and "two" being two Range subsets connected by an OR state:
+                    # one = SpectralRegion(4.5 * u.um, 7.5 * u.um)
+                    # two = SpectralRegion(4 * u.um, 5 * u.um) + SpectralRegion(7 * u.um, 8 * u.um)
+                    #
+                    # oppo = two.invert(one.lower, one.upper)
+                    # Spectral Region, 1 sub-regions:
+                    #   (5.0 um, 7.0 um)
+                    #
+                    # oppo.invert(one.lower, one.upper)
+                    # Spectral Region, 2 sub-regions:
+                    #   (4.5 um, 5.0 um)   (7.0 um, 7.5 um)
+                    if isinstance(two, SpectralRegion):
+                        # Taking an AND state of an empty region is allowed
+                        # but there is no way for SpectralRegion to display that information.
+                        # Instead, we raise a ValueError
+                        if one.upper.value < two.lower.value or one.lower.value > two.upper.value:
+                            raise ValueError("AND mode should overlap with existing subset")
+                        oppo = two.invert(one.lower, one.upper)
+
+                        return oppo.invert(one.lower, one.upper)
+                    else:
+                        return two + one
+                elif subset_state.op is operator.or_:
+                    # This covers the ADD subset mode
+                    # one + two works for both Range and ROI subsets
+                    if one and two:
+                        return two + one
+                    elif one:
+                        return one
+                    elif two:
+                        return two
+                elif subset_state.op is operator.xor:
+                    # This covers the ADD subset mode
+
+                    # Example of how this works, with "one" acting
+                    # as the XOR region and "two" as two ranges joined
+                    # by an OR:
+                    # a = SpectralRegion(4 * u.um, 5 * u.um)
+                    # b = SpectralRegion(6 * u.um, 9 * u.um)
+                    #
+                    # one = SpectralRegion(4.5 * u.um, 12 * u.um)
+                    # two = a + b
+
+                    # two.invert(one.lower, one.upper)
+                    # Spectral Region, 2 sub-regions:
+                    #   (5.0 um, 6.0 um)    (9.0 um, 12.0 um)
+
+                    # one.invert(two.lower, two.upper)
+                    # Spectral Region, 1 sub-regions:
+                    #   (4.0 um, 4.5 um)
+
+                    # two.invert(one.lower, one.upper) + one.invert(two.lower, two.upper)
+                    # Spectral Region, 3 sub-regions:
+                    #   (4.0 um, 4.5 um)    (5.0 um, 6.0 um)    (9.0 um, 12.0 um)
+
+                    if isinstance(two, SpectralRegion):
+                        if one.lower > two.lower:
+                            # If one.lower is less than two.lower, it will be included
+                            # in the two.invert() call. Otherwise, we can add it like this.
+                            return (two.invert(one.lower, one.upper) +
+                                    one.invert(two.lower, two.upper))
+                        return two.invert(one.lower, one.upper)
+                    else:
+                        return two + one
+            else:
+                # This gets triggered in the InvertState case where state1
+                # is an object and state2 is None
+                return self.get_sub_regions(subset_state.state1, simplify_spectral)
+        elif subset_state is not None:
+            # This is the leaf node of the glue subset state tree where
+            # a subset_state is either ROI or Range.
+            if isinstance(subset_state, RoiSubsetState):
+                return self._get_roi_subset_definition(subset_state)
+
+            elif isinstance(subset_state, RangeSubsetState):
+                return self._get_range_subset_bounds(subset_state, simplify_spectral)
+
     def add_data(self, data, data_label=None, notify_done=True):
         """
         Add data to the Glue ``DataCollection``.
 
         Parameters
         ----------
         data : any
@@ -1255,30 +1495,33 @@
                     if result is not None:
                         return result
 
         viewer_item = find_viewer_item(self.state.stack_items)
 
         return viewer_item
 
-    def _viewer_by_reference(self, reference):
+    def _viewer_by_reference(self, reference, fallback_to_id=False):
         """
         Viewer instance by reference defined in the yaml configuration file.
 
         Parameters
         ----------
         reference : str
             Reference for viewer defined in the yaml configuration file.
 
         Returns
         -------
-        `~glue_jupyter.bqplot.common.BqplotBaseView`
+        viewer : `~glue_jupyter.bqplot.common.BqplotBaseView`
             The viewer class instance.
         """
         viewer_item = self._viewer_item_by_reference(reference)
 
+        if viewer_item is None and fallback_to_id:
+            return self._viewer_by_id(reference)
+
         return self._viewer_store[viewer_item['id']]
 
     def _viewer_item_by_reference(self, reference):
         """
         Retrieve a viewer item dictionary by reference.
 
         Parameters
@@ -1641,14 +1884,16 @@
             'name': name or vid,
             'widget': "IPY_MODEL_" + viewer.figure_widget.model_id,
             'toolbar': "IPY_MODEL_" + viewer.toolbar.model_id if viewer.toolbar else '',  # noqa
             'layer_options': "IPY_MODEL_" + viewer.layer_options.model_id,
             'viewer_options': "IPY_MODEL_" + viewer.viewer_options.model_id,
             'selected_data_items': {},  # noqa data_id: visibility state (visible, hidden, mixed), READ-ONLY
             'visible_layers': {},  # label: {color, label_suffix}, READ-ONLY
+            'canvas_angle': 0,  # canvas rotation clockwise rotation angle in deg
+            'canvas_flip_horizontal': False,  # canvas rotation horizontal flip
             'config': self.config,  # give viewer access to app config/layout
             'data_open': False,
             'collapse': True,
             'reference': reference}
 
     def _on_new_viewer(self, msg, vid=None, name=None):
         """
@@ -1674,24 +1919,25 @@
         viewer : `~glue_jupyter.bqplot.common.BqplotBaseView`
             The new viewer instance.
         """
         viewer = self._application_handler.new_data_viewer(
             msg.cls, data=msg.data, show=False)
         viewer.figure_widget.layout.height = '100%'
 
-        links_control_plugin = self._jdaviz_helper.plugins.get('Links Control', None)
-        if links_control_plugin is not None:
-            viewer.state.linked_by_wcs = links_control_plugin.link_type.selected == 'WCS'
-        elif len(self._viewer_store):
-            # The plugin would only not exist for instances of Imviz where the user has
-            # intentionally removed the Links Control plugin, but in that case we will
-            # adopt "linked_by_wcs" from the first (assuming all are the same)
-            # NOTE: deleting the default viewer is forbidden both by API and UI, but if
-            # for some reason that was the case here, linked_by_wcs will default to False
-            viewer.state.linked_by_wcs = list(self._viewer_store.values())[0].state.linked_by_wcs
+        if hasattr(viewer.state, 'linked_by_wcs'):
+            links_control_plugin = self._jdaviz_helper.plugins.get('Links Control', None)
+            if links_control_plugin is not None:
+                viewer.state.linked_by_wcs = links_control_plugin.link_type.selected == 'WCS'
+            elif len(self._viewer_store):
+                # The plugin would only not exist for instances of Imviz where the user has
+                # intentionally removed the Links Control plugin, but in that case we will
+                # adopt "linked_by_wcs" from the first (assuming all are the same)
+                # NOTE: deleting the default viewer is forbidden both by API and UI, but if
+                # for some reason that was the case here, linked_by_wcs will default to False
+                viewer.state.linked_by_wcs = list(self._viewer_store.values())[0].state.linked_by_wcs  # noqa
 
         if msg.x_attr is not None:
             x = msg.data.id[msg.x_attr]
             viewer.state.x_att = x
 
         # Create the viewer item dictionary
         if name is None:
```

### Comparing `jdaviz-3.4.0/jdaviz/app.vue` & `jdaviz-3.5.0/jdaviz/app.vue`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 <template>
   <v-app id="web-app" :class="'jdaviz ' + config" ref="mainapp">
+    <jupyter-widget
+      v-if="state.style_widget"
+      :widget="state.style_widget"
+      style="display: none"
+    ></jupyter-widget>
     <v-overlay v-if="state.logger_overlay"
       absolute
       opacity="0.7">
       <div :style="!state.settings.dense_toolbar ? 'position: absolute; top: 14px; right: 55px' : 'position: absolute; top: 6px; right: 55px'">
         <j-tooltip tipid="app-snackbar-history">
           <v-btn icon @click="state.logger_overlay = !state.logger_overlay" :class="{active : state.logger_overlay}">
             <v-icon medium style="padding-top: 2px">mdi-message-reply</v-icon>
```

### Comparing `jdaviz-3.4.0/jdaviz/cli.py` & `jdaviz-3.5.0/jdaviz/cli.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/docs_link.vue` & `jdaviz-3.5.0/jdaviz/components/docs_link.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/glue_state_sync_wrapper.vue` & `jdaviz-3.5.0/jdaviz/components/glue_state_sync_wrapper.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/layer_viewer_icon.vue` & `jdaviz-3.5.0/jdaviz/components/layer_viewer_icon.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/number_uncertainty.vue` & `jdaviz-3.5.0/jdaviz/components/number_uncertainty.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/play_pause_widget.vue` & `jdaviz-3.5.0/jdaviz/components/play_pause_widget.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_add_results.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_add_results.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_auto_label.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_auto_label.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_dataset_select.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_dataset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_layer_select.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_layer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_section_header.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_section_header.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_subset_select.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_subset_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_table.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_table.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/plugin_viewer_select.vue` & `jdaviz-3.5.0/jdaviz/components/plugin_viewer_select.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/toolbar_nested.py` & `jdaviz-3.5.0/jdaviz/components/toolbar_nested.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/toolbar_nested.vue` & `jdaviz-3.5.0/jdaviz/components/toolbar_nested.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/tooltip.vue` & `jdaviz-3.5.0/jdaviz/components/tooltip.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/components/tray_plugin.vue` & `jdaviz-3.5.0/jdaviz/components/tray_plugin.vue`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <template>
   <v-container class="tray-plugin" style="padding-left: 24px; padding-right: 24px; padding-top: 12px">
+    <v-row>
+      <div style="width: calc(100% - 32px)">
+        <j-docs-link :link="link">{{ description }}</j-docs-link>
+      </div>
+      <div style="width: 32px">
+        <j-plugin-popout :popout_button="popout_button"></j-plugin-popout>
+      </div>
+    </v-row>
+    
     <v-row v-if="isDisabled()">
       <span> {{ getDisabledMsg() }}</span>
     </v-row>
     <div v-else>
-      <v-row>
-        <div style="width: calc(100% - 32px)">
-          <j-docs-link :link="link">{{ description }}</j-docs-link>
-        </div>
-        <div style="width: 32px">
-          <j-plugin-popout :popout_button="popout_button"></j-plugin-popout>
-        </div>
-      </v-row>
       <slot></slot>
     </div>
   </v-container>
 </template>
 
 <script>
 module.exports = {
```

### Comparing `jdaviz-3.4.0/jdaviz/components/viewer_data_select.vue` & `jdaviz-3.5.0/jdaviz/components/viewer_data_select.vue`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,17 @@
       // toggle the visibility of the extra items in the menu
       this.showExtraItems = !this.showExtraItems
     },
   },
   computed: {
     viewerTitleCase() {
       var title = this.$props.viewer.reference || this.$props.viewer.id
-      return title.toLowerCase().replaceAll('-', ' ').split(' ').map((word) => {return (word.charAt(0).toUpperCase() + word.slice(1))}).join(' ');
+      // this translates from kebab-case to human readable (individual words, in title case)
+      // each word that should NOT be capitalized needs to explicitly be set here
+      return title.toLowerCase().replaceAll('-', ' ').split(' ').map((word) => {if (['vs'].indexOf(word) !== -1) {return word} else {return word.charAt(0).toUpperCase() + word.slice(1)}}).join(' ');
     },
     showModeToggle() {
       if (this.$props.viewer.config === 'cubeviz') {
         if (this.$props.viewer.reference !== 'spectrum-viewer') {
           return true
         }
       }
```

### Comparing `jdaviz-3.4.0/jdaviz/components/viewer_data_select_item.vue` & `jdaviz-3.5.0/jdaviz/components/viewer_data_select_item.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/cubeviz.yaml` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/cubeviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/helper.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -116,39 +116,57 @@
         A Specviz helper (:class:`~jdaviz.configs.specviz.helper.Specviz`) for the Jdaviz
         application that is wrapped by Cubeviz.
         """
         if not hasattr(self, '_specviz'):
             self._specviz = Specviz(app=self.app)
         return self._specviz
 
-    def get_data(self, data_label=None, cls=None, subset_to_apply=None, function=None):
+    def get_data(self, data_label=None, spatial_subset=None, spectral_subset=None, function=None,
+                 cls=None):
         """
         Returns data with name equal to data_label of type cls with subsets applied from
         subset_to_apply.
 
         Parameters
         ----------
         data_label : str, optional
             Provide a label to retrieve a specific data set from data_collection.
+        spatial_subset : str, optional
+            Spatial subset applied to data.
+        spectral_subset : str, optional
+            Spectral subset applied to data.
+        function : {True, False, 'minimum', 'maximum', 'mean', 'median', 'sum'}, optional
+            Ignored if ``data_label`` does not point to cube-like data.
+            If True, will collapse according to the current collapse function defined in the
+            spectrum viewer.  If provided as a string, the cube will be collapsed with the provided
+            function.  If False, None, or not passed, the entire cube will be returned (unless there
+            are values for ``spatial_subset`` and ``spectral_subset``).
         cls : `~specutils.Spectrum1D`, `~astropy.nddata.CCDData`, optional
             The type that data will be returned as.
-        subset_to_apply : str, optional
-            Subset that is to be applied to data before it is returned.
-        function : {'minimum', 'maximum', 'mean', 'median', 'sum'}, optional
-            If provided and not ``None`` and ``data_label`` points to cube-like data, the cube will
-            be collapsed with the provided function.  Otherwise the entire cube will be returned.
 
         Returns
         -------
         data : cls
             Data is returned as type cls with subsets applied.
 
         """
-        return self._get_data(data_label=data_label, cls=cls, subset_to_apply=subset_to_apply,
-                              function=function)
+        # If function is a value ('sum' or 'minimum') or True and spatial and spectral
+        # are set, then we collapse the cube along the spatial subset using the function, then
+        # we apply the mask from the spectral subset.
+        # If function is any value other than False, we use specviz
+        if (function is not False and spectral_subset and spatial_subset) or function:
+            return self.specviz.get_data(data_label=data_label, spectral_subset=spectral_subset,
+                                         cls=cls, spatial_subset=spatial_subset, function=function)
+        elif function is False and spectral_subset:
+            raise ValueError("function cannot be False if spectral_subset"
+                             " is set")
+        elif function is False:
+            function = None
+        return self._get_data(data_label=data_label, spatial_subset=spatial_subset,
+                              spectral_subset=spectral_subset, function=function, cls=cls)
 
 
 def layer_is_cube_image_data(layer):
     return isinstance(layer, BaseData) and layer.ndim in (2, 3)
 
 
 # TODO: We can remove this when specutils supports it, i.e.,
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/moment_maps.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/moment_maps/tests/test_moment_maps.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/parsers.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/slice.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/slice.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/slice/tests/test_slice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import pytest
 import numpy as np
 
 from jdaviz.configs.cubeviz.plugins.slice.slice import Slice
 
 
 def test_slice(cubeviz_helper, spectrum1d_cube):
@@ -52,15 +54,16 @@
 
     assert len(sl._watched_viewers) == 2  # flux-viewer, uncert-viewer
     assert len(sl._indicator_viewers) == 1  # spectrum-viewer
 
     # test setting a static 2d image to the "watched" flux viewer to make sure it disconnects
     mm = app.get_tray_item_from_name('cubeviz-moment-maps')
     mm.add_to_viewer_selected = 'flux-viewer'
-    with pytest.warns(UserWarning, match='No observer defined on WCS'):
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', message=r'.*No observer defined on WCS.*')
         mm.vue_calculate_moment()
 
     assert len(sl._watched_viewers) == 2
     assert len(sl._indicator_viewers) == 1
 
     # test in conjunction with as_steps
     sv = app.get_viewer('spectrum-viewer')
@@ -110,7 +113,24 @@
     assert indicator.label.visible is True
 
     sl.show_indicator = False
     assert indicator._show_if_inactive is False
 
     sl.show_wavelength = False
     assert indicator.label.visible is False
+
+
+@pytest.mark.filterwarnings('ignore:No observer defined on WCS')
+def test_init_slice(cubeviz_helper, spectrum1d_cube):
+    cubeviz_helper.load_data(spectrum1d_cube, data_label='test')
+
+    fv = cubeviz_helper.app.get_viewer('flux-viewer')
+    sl = cubeviz_helper.plugins['Slice']
+    assert sl.slice == 1
+    assert fv.state.slices == (0, 0, 1)
+
+    # make sure adding new data doesn't revert slice to 0
+    mm = cubeviz_helper.plugins['Moment Maps']
+    mm.calculate_moment(add_data=True)
+
+    assert sl.slice == 1
+    assert fv.state.slices == (0, 0, 1)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_data_selection.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
     cubeviz_helper.app.add_data_to_viewer('spectrum-viewer', 'test')
     cubeviz_helper.app.get_viewer('spectrum-viewer').apply_roi(XRangeROI(6600, 7400))
 
     subsets = cubeviz_helper.app.get_subsets_from_viewer("spectrum-viewer")
     reg = subsets.get('Subset 1')
 
     assert len(subsets) == 1
-    assert_allclose(reg.lower.value, 6666.666666666667)
-    assert_allclose(reg.upper.value, 7333.333333333334)
+    assert_allclose(reg.lower.value, 6600.)
+    assert_allclose(reg.upper.value, 7400.)
     assert reg.lower.unit == 'Angstrom'
     assert reg.upper.unit == 'Angstrom'
 
 
 @pytest.mark.filterwarnings('ignore')
 def test_fits_image_hdu_parse_from_file(tmpdir, image_cube_hdu_obj, cubeviz_helper):
     f = tmpdir.join("test_fits_image.fits")
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/tools.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/cubeviz/plugins/viewers.py` & `jdaviz-3.5.0/jdaviz/configs/cubeviz/plugins/viewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 
 @viewer_registry("cubeviz-profile-viewer", label="Profile 1D (Cubeviz)")
 class CubevizProfileView(SpecvizProfileView):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
-                    ['jdaviz:boxzoom', 'jdaviz:xrangezoom'],
+                    ['jdaviz:boxzoom', 'jdaviz:xrangezoom', 'jdaviz:yrangezoom'],
                     ['jdaviz:panzoom', 'jdaviz:panzoom_x', 'jdaviz:panzoom_y'],
                     ['bqplot:xrange'],
                     ['jdaviz:selectslice', 'jdaviz:selectline'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     def __init__(self, *args, **kwargs):
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/__init__.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/collapse.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/collapse.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/collapse.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/collapse/tests/test_collapse.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/data_tools.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from jdaviz.core.template_mixin import TemplateMixin
-from traitlets import Unicode, Bool
 import os
+
+from traitlets import Unicode, Bool
+
 from jdaviz.configs.default.plugins.data_tools.file_chooser import FileChooser
 from jdaviz.core.registries import tool_registry
+from jdaviz.core.template_mixin import TemplateMixin
 
 __all__ = ['DataTools']
 
 
 @tool_registry('g-data-tools')
 class DataTools(TemplateMixin):
     template_file = __file__, "data_tools.vue"
@@ -22,17 +24,18 @@
         self._file_upload = FileChooser(start_path)
 
         self.components = {'g-file-import': self._file_upload}
 
         self._file_upload.observe(self._on_file_path_changed, names='file_path')
 
     def _on_file_path_changed(self, event):
-        if (self._file_upload.file_path is not None
-                and not os.path.exists(self._file_upload.file_path)
-                or not os.path.isfile(self._file_upload.file_path)):
+        if self._file_upload.file_path is None:
+            self.valid_path = False
+        elif (not os.path.exists(self._file_upload.file_path)
+              or not os.path.isfile(self._file_upload.file_path)):
             self.valid_path = False
         else:
             self.valid_path = True
 
     def vue_load_data(self, *args, **kwargs):
         if self._file_upload.file_path is None:
             self.error_message = "No file selected"
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/data_tools.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/data_tools/file_chooser.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,17 +320,15 @@
     def _selected_filename(self):
         if self._dircontent.value is None:
             return None
         else:
             return self._map_disp_to_name[self._dircontent.value]
 
     def _update_file_path(self):
-        if self._selected_filename is None or self._selected_path is None:
-            self.file_path = None
-        else:
+        if self._selected_filename is not None and self._selected_path is not None:
             self.file_path = os.path.join(self._selected_path,
                                           self._selected_filename)
 
     def refresh(self):
         """Re-render the form."""
         self._set_form_values(
             self._selected_path,
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/export_plot/export_plot.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/export_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, ViewerSelectMixin
 from jdaviz.core.user_api import PluginUserApi
 
 __all__ = ['ExportViewer']
 
 
@@ -28,14 +30,17 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def save_figure(self, filename=None, filetype=None):
         """
         Save the figure to an image with a provided filename or through an interactive save dialog.
 
+        If ``filetype`` is 'png' (or defaults to 'png' based on ``filename``), the interactive save
+        dialog will be bypassed (this is not supported for 'svg').
+
         Parameters
         ----------
         filename : str or `None`
             Filename to autopopulate the save dialog.
         filetype : {'png', 'svg', `None`}
             Filetype (PNG or SVG).  If `None`, will default based on filename or to PNG.
 
@@ -45,15 +50,23 @@
                 filetype = filename.split('.')[-1]
             else:
                 # default to png
                 filetype = 'png'
 
         viewer = self.viewer.selected_obj
         if filetype == "png":
-            viewer.figure.save_png(filename)
+            if filename is None:
+                viewer.figure.save_png()
+            else:
+                # support writing without save dialog
+                # https://github.com/bqplot/bqplot/pull/1397
+                def on_img_received(data):
+                    with open(os.path.expanduser(filename), 'bw') as f:
+                        f.write(data)
+                viewer.figure.get_png_data(on_img_received)
         elif filetype == "svg":
             viewer.figure.save_svg(filename)
         else:
             raise NotImplementedError(f"filetype={filetype} not supported")
 
     def vue_save_figure(self, filetype):
         """
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/export_plot/export_plot.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/gaussian_smooth.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/gaussian_smooth/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_list_mixin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/line_lists.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/line_lists.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/line_lists/tests/test_line_lists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/markers.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/markers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,14 @@
 from jdaviz.core.marks import MarkersMark
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, ViewerSelectMixin, TableMixin
 from jdaviz.core.user_api import PluginUserApi
 
 __all__ = ['Markers']
 
-_default_table_values = {'spectral_axis': np.nan,
-                         'spectral_axis:unit': '',
-                         'slice': np.nan,
-                         'pixel': (np.nan, np.nan),
-                         'pixel:unreliable': None,
-                         'world': (np.nan, np.nan),
-                         'world:unreliable': None,
-                         'value': np.nan,
-                         'value:unit': '',
-                         'value:unreliable': None,
-                         'index': np.nan}
-
 
 @tray_registry('g-markers', label="Markers")
 class Markers(PluginTemplateMixin, ViewerSelectMixin, TableMixin):
     """
     See the :ref:`Markers Plugin Documentation <markers-plugin>` for more details.
 
     Only the following attributes and methods are available through the
@@ -33,14 +21,26 @@
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.open_in_tray`
     * :meth:`clear_table`
     * :meth:`~jdaviz.core.template_mixin.TableMixin.export_table`
     """
     template_file = __file__, "markers.vue"
 
+    _default_table_values = {'spectral_axis': np.nan,
+                             'spectral_axis:unit': '',
+                             'slice': np.nan,
+                             'pixel': (np.nan, np.nan),
+                             'pixel:unreliable': None,
+                             'world': (np.nan, np.nan),
+                             'world:unreliable': None,
+                             'value': np.nan,
+                             'value:unit': '',
+                             'value:unreliable': None,
+                             'index': np.nan}
+
     @property
     def user_api(self):
         return PluginUserApi(self, expose=('clear_table', 'export_table',))
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.config == 'cubeviz':
@@ -62,20 +62,22 @@
             headers = ['spectral_axis', 'spectral_axis:unit',
                        'pixel', 'value', 'value:unit', 'viewer']
         elif self.config == 'mosviz':
             headers = ['spectral_axis', 'spectral_axis:unit',
                        'pixel', 'world', 'index', 'value', 'value:unit',
                        'viewer']
         else:
-            headers = []
+            # allow downstream configs to override headers
+            headers = kwargs.get('headers', [])
 
         headers += ['data_label']
 
         self.table.headers_avail = headers
         self.table.headers_visible = headers
+        self.table._default_values_by_colname = self._default_table_values
 
         # subscribe to mouse events on any new viewers
         self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewer_added)
 
     def _create_viewer_callbacks(self, viewer):
         if not self.plugin_opened:
             return
@@ -96,14 +98,18 @@
 
     @property
     def marks(self):
         return {viewer_id: self._get_mark(viewer)
                 for viewer_id, viewer in self.app._viewer_store.items()
                 if hasattr(viewer, 'figure')}
 
+    @property
+    def coords_info(self):
+        return self.app.session.application._tools['g-coords-info']
+
     @observe('plugin_opened')
     def _on_plugin_opened_changed(self, *args):
         if self.disabled_msg:
             return
 
         # toggle visibility of markers
         for mark in self.marks.values():
@@ -119,21 +125,21 @@
             if self.plugin_opened:
                 viewer.add_event_callback(callback, events=['keydown'])
             else:
                 viewer.remove_event_callback(callback)
 
     def _on_viewer_key_event(self, viewer, data):
         if data['event'] == 'keydown' and data['key'] == 'm':
-            row_info = self.app.session.application._tools['g-coords-info'].as_dict()
+            row_info = self.coords_info.as_dict()
 
             if 'viewer' in self.table.headers_avail:
                 row_info['viewer'] = viewer.reference if viewer.reference is not None else viewer.reference_id  # noqa
 
             for k in self.table.headers_avail:
-                row_info.setdefault(k, _default_table_values.get(k, ''))
+                row_info.setdefault(k, self._default_table_values.get(k, ''))
 
             try:
                 self.table.add_item({k: v for k, v in row_info.items()
                                      if k in self.table.headers_avail})
             except ValueError as err:
                 raise ValueError(f'failed to add {row_info} to table: {repr(err)}')
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/markers/tests/test_markers_plugin.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from traitlets import Bool, List, observe
+from traitlets import Any, Bool, List, observe
 
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, DatasetSelectMixin
 from jdaviz.core.user_api import PluginUserApi
 from jdaviz.utils import PRIHDR_KEY, COMMENTCARD_KEY
 
 __all__ = ['MetadataViewer']
@@ -30,14 +30,15 @@
     """
     template_file = __file__, "metadata_viewer.vue"
     has_metadata = Bool(False).tag(sync=True)
     has_primary = Bool(False).tag(sync=True)
     show_primary = Bool(False).tag(sync=True)
     has_comments = Bool(False).tag(sync=True)
     metadata = List([]).tag(sync=True)
+    metadata_filter = Any().tag(sync=True)  # string or None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # override the default filters on dataset entries to require metadata in entries
         self.dataset.add_filter('not_from_plugin')
 
     @property
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/metadata_viewer.vue`

 * *Files 20% similar despite different names*

```diff
@@ -21,21 +21,31 @@
         v-model="show_primary"
         persistent-hint>
       </v-switch>
     </v-row>
 
     <j-plugin-section-header>Metadata</j-plugin-section-header>
     <div v-if="has_metadata">
+      <v-row>
+        <v-text-field
+          v-model='metadata_filter'
+          append-icon='mdi-magnify'
+          style="padding: 0px 8px"
+          clearable
+          hide-details
+        ></v-text-field>
+      </v-row>
+  
       <v-row no-gutters>
         <v-col cols=6><U><B>Key</B></U></v-col>
         <v-col cols=6><U>Value</U></v-col>
         <v-col v-if="has_comments" cols=6 class="text--secondary"><U>Comment</U></v-col>
       </v-row>
       <v-row
-        v-for="item in metadata"
+        v-for="item in metadata.filter((item) => {return metadata_filter === null || item.join().toLowerCase().indexOf(metadata_filter.toLowerCase()) !== -1})"
         :key="item[0]"
         no-gutters>
         <v-col cols=6><B>{{ item[0] }}</B></v-col>
         <v-col cols=6>{{ item[1] }}</v-col>
         <v-col v-if="has_comments" cols=6 class="text--secondary">{{ item[2] }}</v-col>
       </v-row>
     </div>
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/metadata_viewer/tests/test_metadata_viewer.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/fitting_backend.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/initializers.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/initializers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from jdaviz.core.template_mixin import (PluginTemplateMixin,
                                         SelectPluginComponent,
                                         SpectralSubsetSelectMixin,
                                         SubsetSelect,
                                         DatasetSelectMixin,
                                         DatasetSpectralSubsetValidMixin,
                                         AutoTextField,
-                                        AddResultsMixin)
+                                        AddResultsMixin,
+                                        TableMixin)
 from jdaviz.core.custom_traitlets import IntHandleEmpty
 from jdaviz.core.user_api import PluginUserApi
 from jdaviz.configs.default.plugins.model_fitting.fitting_backend import fit_model_to_spectrum
 from jdaviz.configs.default.plugins.model_fitting.initializers import (MODELS,
                                                                        initialize,
                                                                        get_model_parameters)
 
@@ -35,15 +36,15 @@
         self.quantity = u.Quantity(self.value,
                                    self.unit if self.unit is not None else u.dimensionless_unscaled)
 
 
 @tray_registry('g-model-fitting', label="Model Fitting", viewer_requirements='spectrum')
 class ModelFitting(PluginTemplateMixin, DatasetSelectMixin,
                    SpectralSubsetSelectMixin, DatasetSpectralSubsetValidMixin,
-                   AddResultsMixin):
+                   AddResultsMixin, TableMixin):
     """
     See the :ref:`Model Fitting Plugin Documentation <specviz-model-fitting>` for more details.
 
     Only the following attributes and methods are available through the
     :ref:`public plugin API <plugin-apis>`:
 
     * :meth:`~jdaviz.core.template_mixin.PluginTemplateMixin.show`
@@ -59,14 +60,15 @@
     * :meth:`create_model_component`
     * :meth:`remove_model_component`
     * :meth:`model_components`
     * :meth:`get_model_component`
     * :meth:`set_model_component`
     * :meth:`reestimate_model_parameters`
     * ``equation`` (:class:`~jdaviz.core.template_mixin.AutoTextField`)
+    * :meth:`equation_components`
     * ``cube_fit``
       Only exposed for Cubeviz.  Whether to fit the model to the cube instead of to the
       collapsed spectrum.
     * ``add_results`` (:class:`~jdaviz.core.template_mixin.AddResults`)
     * ``residuals_calculate`` (bool)
       Whether to calculate and expose the residuals (model minus data).
     * ``residuals`` (:class:`~jdaviz.core.template_mixin.AutoTextField`)
@@ -150,29 +152,40 @@
 
         self.equation = AutoTextField(self, 'model_equation', 'model_equation_default',
                                       'model_equation_auto', 'model_equation_invalid_msg')
 
         self.residuals = AutoTextField(self, 'residuals_label', 'residuals_label_default',
                                        'residuals_label_auto', 'residuals_label_invalid_msg')
 
+        headers = ['model', 'data_label', 'spectral_subset', 'equation']
+        if self.config == 'cubeviz':
+            headers += ['spatial_subset', 'cube_fit']
+
+        self.table.headers_avail = headers
+        self.table.headers_visible = headers
+        # when model parameters are added as columns, only show the value columns by default
+        # (other columns can be show in the dropdown by the user)
+        self.table._new_col_visible = lambda colname: colname.split(':')[-1] not in ('unit', 'fixed', 'uncert', 'std')  # noqa
+
         # set the filter on the viewer options
         self._update_viewer_filters()
 
     @property
     def user_api(self):
         expose = ['dataset']
         if self.config == "cubeviz":
             expose += ['spatial_subset']
         expose += ['spectral_subset', 'model_component', 'poly_order', 'model_component_label',
                    'model_components', 'create_model_component', 'remove_model_component',
                    'get_model_component', 'set_model_component', 'reestimate_model_parameters',
-                   'equation', 'add_results', 'residuals_calculate', 'residuals']
+                   'equation', 'equation_components',
+                   'add_results', 'residuals_calculate', 'residuals']
         if self.config == "cubeviz":
             expose += ['cube_fit']
-        expose += ['calculate_fit']
+        expose += ['calculate_fit', 'clear_table', 'export_table']
         return PluginUserApi(self, expose=expose)
 
     def _param_units(self, param, model_type=None):
         """Helper function to handle units that depend on x and y"""
         y_params = ["amplitude", "amplitude_L", "intercept", "scale"]
 
         if param == "slope":
@@ -527,14 +540,15 @@
                                if x["id"] == model_component_label][0]
         except IndexError:
             raise ValueError(f"'{model_component_label}' is not a label of an existing model component")  # noqa
 
         comp = {"model_type": model_component['model_type'],
                 "parameters": {p['name']: {'value': p['value'],
                                            'unit': p['unit'],
+                                           'std': p.get('std', np.nan),
                                            'fixed': p['fixed']} for p in model_component['parameters']}}  # noqa
 
         if parameter is not None:
             return comp['parameters'].get(parameter)
         return comp
 
     def set_model_component(self, model_component_label, parameter, value=None, fixed=None):
@@ -626,14 +640,21 @@
     @property
     def model_components(self):
         """
         List of the labels of existing model components
         """
         return [x["id"] for x in self.component_models]
 
+    @property
+    def equation_components(self):
+        """
+        List of the labels of model components in the current equation
+        """
+        return re.split('[+*/-]', self.equation.value)
+
     def vue_add_model(self, event):
         self.create_model_component()
 
     def vue_remove_model(self, event):
         self.remove_model_component(event)
 
     @observe('model_equation')
@@ -684,17 +705,47 @@
         residuals (if ``residuals_calculate`` is set to ``True``)
         """
         if not self.spectral_subset_valid:
             valid, spec_range, subset_range = self._check_dataset_spectral_subset_valid(return_ranges=True)  # noqa
             raise ValueError(f"spectral subset '{self.spectral_subset.selected}' {subset_range} is outside data range of '{self.dataset.selected}' {spec_range}")  # noqa
 
         if self.cube_fit:
-            return self._fit_model_to_cube(add_data=add_data)
+            ret = self._fit_model_to_cube(add_data=add_data)
         else:
-            return self._fit_model_to_spectrum(add_data=add_data)
+            ret = self._fit_model_to_spectrum(add_data=add_data)
+
+        if ret is None:  # pragma: no cover
+            # something went wrong in the fitting call and (hopefully) already raised a warning,
+            # but we don't have anything to add to the table
+            return ret
+
+        if self.cube_fit:
+            # cube fits are currently unsupported in tables
+            return ret
+
+        row = {'model': self.results_label if add_data else '',
+               'data_label': self.dataset_selected,
+               'spectral_subset': self.spectral_subset_selected,
+               'equation': self.equation.value}
+        if self.app.config == 'cubeviz':
+            row['spatial_subset'] = self.spatial_subset_selected
+            row['cube_fit'] = self.cube_fit
+
+        equation_components = self.equation_components
+        for comp_ind, comp in enumerate(equation_components):
+            for param_name, param_dict in self.get_model_component(comp).get('parameters', {}).items():  # noqa
+                colprefix = f"{comp}:{param_name}_{comp_ind}"
+                row[colprefix] = param_dict.get('value')
+                row[f"{colprefix}:unit"] = param_dict.get('unit')
+                row[f"{colprefix}:fixed"] = param_dict.get('fixed')
+                row[f"{colprefix}:std"] = param_dict.get('std')
+
+        self.table.add_item(row)
+
+        return ret
 
     def vue_apply(self, event):
         self.calculate_fit()
 
     def _fit_model_to_spectrum(self, add_data):
         """
         Run fitting on the initialized models, fixing any parameters marked
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/model_fitting.vue`

 * *Files 6% similar despite different names*

```diff
@@ -215,14 +215,20 @@
           v-model="cube_fit"
           label="Cube Fit"
           hint="Whether to fit to the collapsed spectrum or entire cube"
           persistent-hint
         ></v-switch>
       </v-row>
 
+      <v-row v-if="cube_fit">
+        <span class="v-messages v-messages__message text--secondary">
+            Note: cube fit results are not logged to table.
+        </span>
+      </v-row>
+
       <plugin-add-results
         :label.sync="results_label"
         :label_default="results_label_default"
         :label_auto.sync="results_label_auto"
         :label_invalid_msg="results_label_invalid_msg"
         :label_overwrite="results_label_overwrite"
         label_hint="Label for the model"
@@ -263,14 +269,17 @@
       </plugin-add-results>
 
       <v-row>
         <span class="v-messages v-messages__message text--secondary">
             If fit is not sufficiently converged, click Fit Model again to run additional iterations.
         </span>
       </v-row>
+
+      <j-plugin-section-header>Results History</j-plugin-section-header>
+      <jupyter-widget :widget="table_widget"></jupyter-widget> 
     </div>
   </j-tray-plugin>
 </template>
 
 <script>
   module.exports = {
     created() {
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_fitting.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.io import fits
 from astropy.io.registry.base import IORegistryError
 from astropy.modeling import models, parameters as params
 from astropy.nddata import StdDevUncertainty
+from astropy.tests.helper import assert_quantity_allclose
 from astropy.wcs import WCS
 from numpy.testing import assert_allclose, assert_array_equal
 from specutils.spectra import Spectrum1D
 
 from jdaviz.configs.default.plugins.model_fitting import fitting_backend as fb
 from jdaviz.configs.default.plugins.model_fitting import initializers
 from jdaviz.configs.default.plugins.model_fitting.model_fitting import ModelFitting
@@ -73,14 +74,38 @@
     with pytest.raises(
             ValueError,
             match="invalid model component label 'invalid-string'"):
         plugin.comp_label = 'invalid-string'
         plugin.vue_add_model({})
 
 
+@pytest.mark.filterwarnings(r"ignore:Model is linear in parameters.*")
+def test_parameter_retrieval(cubeviz_helper, spectral_cube_wcs):
+    flux = np.ones((3, 4, 5))
+    flux[2, 2, :] = [1, 2, 3, 4, 5]
+    cubeviz_helper.load_data(Spectrum1D(flux=flux * u.nJy, wcs=spectral_cube_wcs),
+                             data_label='test')
+    plugin = cubeviz_helper.plugins["Model Fitting"]
+    plugin.create_model_component("Linear1D", "L")
+    plugin.cube_fit = True
+    plugin.calculate_fit()
+
+    params = cubeviz_helper.get_model_parameters()
+    slope_res = np.zeros((4, 3))
+    slope_res[2, 2] = 1.0
+    slope_res = slope_res * u.nJy / u.Hz
+    intercept_res = np.ones((4, 3))
+    intercept_res[2, 2] = 0
+    intercept_res = intercept_res * u.nJy
+    assert_quantity_allclose(params['cube-fit model']['slope'], slope_res,
+                             atol=1e-10 * u.nJy / u.Hz)
+    assert_quantity_allclose(params['cube-fit model']['intercept'], intercept_res,
+                             atol=1e-10 * u.nJy)
+
+
 @pytest.mark.parametrize('unc', ('zeros', None))
 def test_fitting_backend(unc):
     np.random.seed(42)
 
     x, y = build_spectrum()
 
     # The uncertainty array of all zero should be ignored when fitting
@@ -259,7 +284,46 @@
     coo = data_sci.coords.pixel_to_world(1, 0, 2)
     assert_allclose(coo[0].value, coo_expected[0].value)  # SpectralCoord
     assert_allclose([coo[1].ra.deg, coo[1].dec.deg],
                     [coo_expected[1].ra.deg, coo_expected[1].dec.deg])
     data_mask = cubeviz_helper.app.data_collection["fitted_cube.fits[MASK]"]
     flux_mask = data_mask.get_component("flux")
     assert_array_equal(flux_mask.data, mask)
+
+
+@pytest.mark.filterwarnings(r"ignore:Model is linear in parameters.*")
+@pytest.mark.filterwarnings(r"ignore:The fit may be unsuccessful.*")
+def test_results_table(specviz_helper, spectrum1d):
+    data_label = 'test'
+    specviz_helper.load_data(spectrum1d, data_label=data_label)
+
+    mf = specviz_helper.plugins['Model Fitting']
+    mf.create_model_component('Linear1D')
+
+    mf.add_results.label = 'linear model'
+    mf.calculate_fit(add_data=True)
+    mf_table = mf.export_table()
+    assert len(mf_table) == 1
+    assert mf_table['equation'][-1] == 'L'
+    assert mf_table.colnames == ['model', 'data_label', 'spectral_subset', 'equation',
+                                 'L:slope_0', 'L:slope_0:unit',
+                                 'L:slope_0:fixed', 'L:slope_0:std',
+                                 'L:intercept_0', 'L:intercept_0:unit',
+                                 'L:intercept_0:fixed', 'L:intercept_0:std']
+
+    mf.create_model_component('Gaussian1D')
+    mf.add_results.label = 'composite model'
+    mf.calculate_fit(add_data=True)
+    mf_table = mf.export_table()
+    assert len(mf_table) == 2
+    assert mf_table['equation'][-1] == 'L+G'
+    assert mf_table.colnames == ['model', 'data_label', 'spectral_subset', 'equation',
+                                 'L:slope_0', 'L:slope_0:unit',
+                                 'L:slope_0:fixed', 'L:slope_0:std',
+                                 'L:intercept_0', 'L:intercept_0:unit',
+                                 'L:intercept_0:fixed', 'L:intercept_0:std',
+                                 'G:amplitude_1', 'G:amplitude_1:unit',
+                                 'G:amplitude_1:fixed', 'G:amplitude_1:std',
+                                 'G:mean_1', 'G:mean_1:unit',
+                                 'G:mean_1:fixed', 'G:mean_1:std',
+                                 'G:stddev_1', 'G:stddev_1:unit',
+                                 'G:stddev_1:fixed', 'G:stddev_1:std']
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/model_fitting/tests/test_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,12 +346,12 @@
     assert plugin.dataset == 'right_spectrum'
     assert plugin.spectral_subset == 'Entire Spectrum'
     assert plugin._obj.spectral_subset_valid
 
     plugin.spectral_subset = 'Subset 1'
     assert not plugin._obj.spectral_subset_valid
 
-    with pytest.raises(ValueError, match=r"spectral subset 'Subset 1' \(5000.0, 5888.888888888889\) is outside data range of 'right_spectrum' \(6000.0, 8000.0\)"):  # noqa
+    with pytest.raises(ValueError, match=r"spectral subset 'Subset 1' \(5000.0, 6000.0\) is outside data range of 'right_spectrum' \(6000.0, 8000.0\)"):  # noqa
         plugin.calculate_fit()
 
     plugin.dataset = 'left_spectrum'
     assert plugin._obj.spectral_subset_valid
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/plot_options/tests/test_plot_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import pytest
+from numpy import allclose
+from numpy.testing import assert_allclose
 
 
 @pytest.mark.filterwarnings('ignore')
 def test_multiselect(cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube)
     po = cubeviz_helper.app.get_tray_item_from_name('g-plot-options')
 
@@ -54,14 +56,42 @@
 
     po.viewer.selected = 'spectrum-viewer'
     assert po.axes_visible.sync['in_subscribed_states'] is False
     assert len(po.axes_visible.linked_states) == 0
 
 
 @pytest.mark.filterwarnings('ignore')
+def test_stretch_histogram(cubeviz_helper, spectrum1d_cube_with_uncerts):
+    cubeviz_helper.load_data(spectrum1d_cube_with_uncerts)
+    po = cubeviz_helper.app.get_tray_item_from_name('g-plot-options')
+    po.open_in_tray()  # forces histogram to draw
+
+    assert po.stretch_histogram is not None
+
+    flux_cube_sample = po.stretch_histogram.marks[0].sample
+
+    # changing viewer should change results
+    po.viewer.selected = 'uncert-viewer'
+    assert not allclose(po.stretch_histogram.marks[0].sample, flux_cube_sample)
+
+    po.viewer.selected = 'flux-viewer'
+    assert_allclose(po.stretch_histogram.marks[0].sample, flux_cube_sample)
+
+    # change viewer limits
+    fv = cubeviz_helper.app.get_viewer('flux-viewer')
+    fv.state.x_max = 0.5 * fv.state.x_max
+    # viewer limits should not be affected by default
+    assert_allclose(po.stretch_histogram.marks[0].sample, flux_cube_sample)
+
+    # set to listen to viewer limits, the length of the samples will change
+    po.stretch_hist_zoom_limits = True
+    assert len(po.stretch_histogram.marks[0].sample) != len(flux_cube_sample)
+
+
+@pytest.mark.filterwarnings('ignore')
 def test_user_api(cubeviz_helper, spectrum1d_cube):
     cubeviz_helper.load_data(spectrum1d_cube)
     po = cubeviz_helper.plugins['Plot Options']
 
     assert po.multiselect is False
     assert "multiselect" in po.viewer.__repr__()
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,36 +11,39 @@
 from jdaviz.core.registries import tray_registry
 from jdaviz.core.template_mixin import PluginTemplateMixin, DatasetSelectMixin, SubsetSelect
 
 __all__ = ['SubsetPlugin']
 
 SUBSET_MODES = {
     'replace': ReplaceMode,
-    'add': OrMode,
-    'and': AndMode,
-    'xor': XorMode,
-    'remove': AndNotMode
+    'OrState': OrMode,
+    'AndState': AndMode,
+    'XorState': XorMode,
+    'AndNotState': AndNotMode,
+    'RangeSubsetState': RangeSubsetState,
+    'RoiSubsetState': RoiSubsetState
 }
 
 
 @tray_registry('g-subset-plugin', label="Subset Tools")
 class SubsetPlugin(PluginTemplateMixin, DatasetSelectMixin):
     template_file = __file__, "subset_plugin.vue"
     select = List([]).tag(sync=True)
     subset_items = List([]).tag(sync=True)
     subset_selected = Unicode("Create New").tag(sync=True)
     mode_selected = Unicode('add').tag(sync=True)
     show_region_info = Bool(True).tag(sync=True)
     subset_types = List([]).tag(sync=True)
     subset_definitions = List([]).tag(sync=True)
+    glue_state_types = List([]).tag(sync=True)
     has_subset_details = Bool(False).tag(sync=True)
 
     subplugins_opened = Any().tag(sync=True)
 
-    is_editable = Bool(False).tag(sync=True)
+    is_centerable = Bool(False).tag(sync=True)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.components = {
             'g-subset-mode': SelectionModeMenu(session=self.session)
         }
@@ -50,14 +53,15 @@
         self.session.hub.subscribe(self, SubsetUpdateMessage,
                                    handler=self._on_subset_update)
 
         self.subset_select = SubsetSelect(self,
                                           'subset_items',
                                           'subset_selected',
                                           default_text="Create New")
+        self.subset_states = []
 
     def _sync_selected_from_state(self, *args):
         if not hasattr(self, 'subset_select'):
             # during initial init, this can trigger before the component is initialized
             return
         if self.session.edit_subset_mode.edit_subset == []:
             if self.subset_selected != self.subset_select.default_text:
@@ -87,15 +91,16 @@
                              self.subset_select._subset_to_dict(subset) for subset in
                              self.data_collection.subset_groups]
 
     @observe('subset_selected')
     def _sync_selected_from_ui(self, change):
         self.subset_definitions = []
         self.subset_types = []
-        self.is_editable = False
+        self.glue_state_types = []
+        self.is_centerable = False
 
         if not hasattr(self, 'subset_select'):
             # during initial init, this can trigger before the component is initialized
             return
 
         if change['new'] != self.subset_select.default_text:
             self._get_subset_definition(change['new'])
@@ -109,134 +114,165 @@
     # g-subset-mode component
     @observe("mode_selected")
     def _mode_selected_changed(self, event={}):
         if self.session.edit_subset_mode != self.mode_selected:
             self.session.edit_subset_mode = self.mode_selected
     '''
 
-    def _unpack_nested_subset(self, subset_state):
-        '''
-        Navigate through the tree of subset states for composite
-        subsets made up of multiple regions.
-        '''
-        if isinstance(subset_state, CompositeSubsetState):
-            self._unpack_nested_subset(subset_state.state1)
-            self._unpack_nested_subset(subset_state.state2)
-            self.is_editable = False
-        else:
-            if subset_state is not None:
-                self._get_subset_subregion_definition(subset_state)
-
-    def _get_subset_subregion_definition(self, subset_state):
+    def _unpack_get_subsets_for_ui(self):
         """
-        Get the type and parameters for a single region in the subset. Note that
-        the string type and operation (if in a composite subset) need to be stored
-        separately from the float parameters for display reasons.
+        Convert what app.get_subsets returns into something the UI of this plugin
+        can display.
+
+        Returns
+        -------
+
         """
-        subset_type = ''
-        subset_definition = []
-        self.is_editable = False
+        subset_information = self.app.get_subsets(self.subset_selected, simplify_spectral=False)
         _around_decimals = 6  # Avoid 30 degrees from coming back as 29.999999999999996
+        if not subset_information:
+            return
+        if len(subset_information) == 1:
+            self.is_centerable = True
+        else:
+            self.is_centerable = False
 
-        if isinstance(subset_state, RoiSubsetState):
-            if isinstance(subset_state.roi, CircularROI):
-                x, y = subset_state.roi.get_center()
-                r = subset_state.roi.radius
-                subset_definition = [{"name": "X Center", "att": "xc", "value": x, "orig": x},
-                                     {"name": "Y Center", "att": "yc", "value": y, "orig": y},
-                                     {"name": "Radius", "att": "radius", "value": r, "orig": r}]
-                self.is_editable = True
-
-            elif isinstance(subset_state.roi, RectangularROI):
-                for att in ("Xmin", "Xmax", "Ymin", "Ymax"):
-                    real_att = att.lower()
-                    val = getattr(subset_state.roi, real_att)
+        for spec in subset_information:
+            subset_definition = []
+            subset_type = ''
+            subset_state = spec["subset_state"]
+            glue_state = spec["glue_state"]
+            if isinstance(subset_state, RoiSubsetState):
+                if isinstance(subset_state.roi, CircularROI):
+                    x, y = subset_state.roi.get_center()
+                    r = subset_state.roi.radius
+                    subset_definition = [{"name": "X Center", "att": "xc", "value": x, "orig": x},
+                                         {"name": "Y Center", "att": "yc", "value": y, "orig": y},
+                                         {"name": "Radius", "att": "radius", "value": r, "orig": r}]
+
+                elif isinstance(subset_state.roi, RectangularROI):
+                    for att in ("Xmin", "Xmax", "Ymin", "Ymax"):
+                        real_att = att.lower()
+                        val = getattr(subset_state.roi, real_att)
+                        subset_definition.append(
+                            {"name": att, "att": real_att, "value": val, "orig": val})
+                    theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
                     subset_definition.append(
-                        {"name": att, "att": real_att, "value": val, "orig": val})
-                theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
-                subset_definition.append(
-                    {"name": "Angle", "att": "theta", "value": theta, "orig": theta})
-                self.is_editable = True
-
-            elif isinstance(subset_state.roi, EllipticalROI):
-                xc = subset_state.roi.xc
-                yc = subset_state.roi.yc
-                rx = subset_state.roi.radius_x
-                ry = subset_state.roi.radius_y
-                theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
-                subset_definition = [
-                    {"name": "X Center", "att": "xc", "value": xc, "orig": xc},
-                    {"name": "Y Center", "att": "yc", "value": yc, "orig": yc},
-                    {"name": "X Radius", "att": "radius_x", "value": rx, "orig": rx},
-                    {"name": "Y Radius", "att": "radius_y", "value": ry, "orig": ry},
-                    {"name": "Angle", "att": "theta", "value": theta, "orig": theta}]
-                self.is_editable = True
+                        {"name": "Angle", "att": "theta", "value": theta, "orig": theta})
 
-            subset_type = subset_state.roi.__class__.__name__
-
-        elif isinstance(subset_state, RangeSubsetState):
-            lo = subset_state.lo
-            hi = subset_state.hi
-            subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo, "orig": lo},
-                                 {"name": "Upper bound", "att": "hi", "value": hi, "orig": hi}]
-            self.is_editable = True
-            subset_type = "Range"
-
-        if len(subset_definition) > 0 and subset_definition not in self.subset_definitions:
-            # Note: .append() does not work for List traitlet.
-            self.subset_definitions = self.subset_definitions + [subset_definition]
-            self.subset_types = self.subset_types + [subset_type]
+                elif isinstance(subset_state.roi, EllipticalROI):
+                    xc = subset_state.roi.xc
+                    yc = subset_state.roi.yc
+                    rx = subset_state.roi.radius_x
+                    ry = subset_state.roi.radius_y
+                    theta = np.around(np.degrees(subset_state.roi.theta), decimals=_around_decimals)
+                    subset_definition = [
+                        {"name": "X Center", "att": "xc", "value": xc, "orig": xc},
+                        {"name": "Y Center", "att": "yc", "value": yc, "orig": yc},
+                        {"name": "X Radius", "att": "radius_x", "value": rx, "orig": rx},
+                        {"name": "Y Radius", "att": "radius_y", "value": ry, "orig": ry},
+                        {"name": "Angle", "att": "theta", "value": theta, "orig": theta}]
+
+                subset_type = subset_state.roi.__class__.__name__
+
+            elif isinstance(subset_state, RangeSubsetState):
+                lo = subset_state.lo
+                hi = subset_state.hi
+                subset_definition = [{"name": "Lower bound", "att": "lo", "value": lo, "orig": lo},
+                                     {"name": "Upper bound", "att": "hi", "value": hi, "orig": hi}]
+                subset_type = "Range"
+            if len(subset_definition) > 0:
+                # Note: .append() does not work for List traitlet.
+                self.subset_definitions = self.subset_definitions + [subset_definition]
+                self.subset_types = self.subset_types + [subset_type]
+                self.glue_state_types = self.glue_state_types + [glue_state]
+                self.subset_states = self.subset_states + [subset_state]
 
     def _get_subset_definition(self, *args):
         """
         Retrieve the parameters defining the selected subset, for example the
         upper and lower bounds for a simple spectral subset.
         """
         self.subset_definitions = []
         self.subset_types = []
+        self.glue_state_types = []
+        self.subset_states = []
 
-        self._unpack_nested_subset(self.subset_select.selected_subset_state)
+        self._unpack_get_subsets_for_ui()
 
     def vue_update_subset(self, *args):
-        if not self.is_editable:  # no-op
+        status, reason = self._check_input()
+        if not status:
+            self.hub.broadcast(SnackbarMessage(reason, color='error', sender=self))
             return
 
-        subset_state = self.subset_select.selected_subset_state
-
-        # Composite region cannot be edited, so just grab first element.
-        subset_type = self.subset_types[0]
-        subset_definition = self.subset_definitions[0]
-
-        try:
-            if subset_type == "Range":
-                sbst_obj = subset_state
-            else:
-                sbst_obj = subset_state.roi
-
-            for d_att in subset_definition:
+        for index, sub in enumerate(self.subset_definitions):
+            if len(self.subset_states) <= index:
+                return
+            sub_states = self.subset_states[index]
+            for d_att in sub:
                 if d_att["att"] == 'theta':  # Humans use degrees but glue uses radians
                     d_val = np.radians(d_att["value"])
                 else:
-                    d_val = d_att["value"]
+                    d_val = float(d_att["value"])
 
-                setattr(sbst_obj, d_att["att"], d_val)
-
-            # Force glue to update the Subset. This is the same call used in
-            # glue.core.edit_subset_mode.EditSubsetMode.update() but we do not
-            # want to deal with all the contract stuff tied to the update() method.
-            self.session.edit_subset_mode._combine_data(subset_state, override_mode=ReplaceMode)
+                if float(d_att["orig"]) != d_val:
+                    if self.subset_types[index] == "Range":
+                        setattr(sub_states, d_att["att"], d_val)
+                    else:
+                        setattr(sub_states.roi, d_att["att"], d_val)
+        try:
+            dc = self.data_collection
+            subsets = dc.subset_groups
+            self.session.edit_subset_mode._combine_data(
+                subsets[[x.label for x in subsets].index(self.subset_selected)].subset_state,
+                override_mode=ReplaceMode)
         except Exception as err:  # pragma: no cover
             self.hub.broadcast(SnackbarMessage(
                 f"Failed to update Subset: {repr(err)}", color='error', sender=self))
 
+    def _check_input(self):
+        status = True
+        reason = ""
+        for index, sub in enumerate(self.subset_definitions):
+            lo = hi = xmin = xmax = ymin = ymax = None
+            for d_att in sub:
+                if d_att["att"] == "lo":
+                    lo = d_att["value"]
+                elif d_att["att"] == "hi":
+                    hi = d_att["value"]
+                elif d_att["att"] == "radius" and d_att["value"] <= 0:
+                    status = False
+                    reason = "Failed to update Subset: radius must be a positive scalar"
+                    break
+                elif d_att["att"] == "xmin":
+                    xmin = d_att["value"]
+                elif d_att["att"] == "xmax":
+                    xmax = d_att["value"]
+                elif d_att["att"] == "ymin":
+                    ymin = d_att["value"]
+                elif d_att["att"] == "ymax":
+                    ymax = d_att["value"]
+
+                if lo and hi and hi <= lo:
+                    status = False
+                    reason = "Failed to update Subset: lower bound must be less than upper bound"
+                    break
+                elif xmin and xmax and ymin and ymax and (xmax - xmin <= 0 or ymax - ymin <= 0):
+                    status = False
+                    reason = "Failed to update Subset: width and length must be positive scalars"
+                    break
+
+        return status, reason
+
     def vue_recenter_subset(self, *args):
-        # Composite region cannot be edited. This only works for Imviz.
-        if not self.is_editable or self.config != 'imviz':  # no-op
+        # Composite region cannot be centered. This only works for Imviz.
+        if not self.is_centerable or self.config != 'imviz':  # no-op
             raise NotImplementedError(
-                f'Cannot recenter: is_editable={self.is_editable}, config={self.config}')
+                f'Cannot recenter: is_centerable={self.is_centerable}, config={self.config}')
 
         from photutils.aperture import ApertureStats
         from jdaviz.core.region_translators import regions2aperture, _get_region_from_spatial_subset
 
         try:
             reg = _get_region_from_spatial_subset(self, self.subset_selected)
             aperture = regions2aperture(reg)
@@ -265,24 +301,24 @@
         This may or may not be the centroid obtain from data.
 
         Returns
         -------
         cen : number, tuple of numbers, or `None`
             The center of the Subset in ``x`` or ``(x, y)``,
             depending on the Subset type, if applicable.
-            If Subset is not editable, this returns `None`.
+            If Subset is not centerable, this returns `None`.
 
         Raises
         ------
         NotImplementedError
             Subset type is not supported.
 
         """
-        # Composite region cannot be edited.
-        if not self.is_editable:  # no-op
+        # Composite region cannot be centered.
+        if not self.is_centerable:  # no-op
             return
 
         subset_state = self.subset_select.selected_subset_state
 
         if isinstance(subset_state, RoiSubsetState):
             sbst_obj = subset_state.roi
             if isinstance(sbst_obj, (CircularROI, EllipticalROI)):
@@ -292,23 +328,26 @@
             else:  # pragma: no cover
                 raise NotImplementedError(
                     f'Getting center of {sbst_obj.__class__} is not supported')
 
         elif isinstance(subset_state, RangeSubsetState):
             cen = (subset_state.hi - subset_state.lo) * 0.5 + subset_state.lo
 
+        elif isinstance(subset_state, CompositeSubsetState):
+            cen = None
+
         else:  # pragma: no cover
             raise NotImplementedError(
                 f'Getting center of {subset_state.__class__} is not supported')
 
         return cen
 
     def set_center(self, new_cen, update=False):
         """Set the desired center for the selected Subset, if applicable.
-        If Subset is not editable, nothing is done.
+        If Subset is not centerable, nothing is done.
 
         Parameters
         ----------
         new_cen : number or tuple of numbers
             The new center defined either as ``x`` or ``(x, y)``,
             depending on the Subset type.
 
@@ -319,16 +358,16 @@
 
         Raises
         ------
         NotImplementedError
             Subset type is not supported.
 
         """
-        # Composite region cannot be edited, so just grab first element.
-        if not self.is_editable:  # no-op
+        # Composite region cannot be centered, so just grab first element.
+        if not self.is_centerable:  # no-op
             return
 
         subset_state = self.subset_select.selected_subset_state
 
         if isinstance(subset_state, RoiSubsetState):
             x, y = new_cen
             sbst_obj = subset_state.roi
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/subset_plugin.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,84 @@
 <template>
-  <j-tray-plugin
-    description='Tools for selecting and interacting with subsets.'
-    :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#subset-tools'"
+  <j-tray-plugin  
+    description="Rotate viewer canvas to any orientation (note: this does not affect the underlying data)."
+    :link="'https://jdaviz.readthedocs.io/en/'+vdocs+'/'+config+'/plugins.html#canvas-rotation'"
+    :disabled_msg="isChromium() ? '' : 'Image rotation is not supported by your browser. Please see our docs for more information.'"
     :popout_button="popout_button">
-
-    <v-row align=center>
-      <v-col cols=10 justify="left">
-        <plugin-subset-select 
-          :items="subset_items"
-          :selected.sync="subset_selected"
-          :show_if_single_entry="true"
-          label="Subset"
-          hint="Select subset to edit."
-        />
-      </v-col>
-
-      <v-col justify="center" cols=2>
-        <j-tooltip tipid='g-subset-mode'>
-          <g-subset-mode></g-subset-mode>
-        </j-tooltip>
-      </v-col>
+    <plugin-viewer-select
+      :items="viewer_items"
+      :selected.sync="viewer_selected"
+      label="Viewer"
+      hint="Select viewer."
+    />
+
+    <v-row>
+      <span style="line-height: 36px">Presets:</span>
+      <j-tooltip tooltipcontent="reset rotation and flip">
+        <v-btn icon @click="reset">
+          <v-icon>mdi-restore</v-icon>
+        </v-btn>
+      </j-tooltip>
+      <j-tooltip v-if="has_wcs" tooltipcontent="north up, east right">
+        <v-btn icon @click="set_north_up_east_right">
+          <img :src="icon_nuer" width="24" class="invert-if-dark" style="opacity: 0.65"/>
+        </v-btn>
+      </j-tooltip>
+      <j-tooltip v-if="has_wcs" tooltipcontent="north up, east left">
+        <v-btn icon @click="set_north_up_east_left">
+          <img :src="icon_nuel" width="24" class="invert-if-dark" style="opacity: 0.65"/>
+        </v-btn>
+      </j-tooltip>
     </v-row>
-
-    <!-- Sub-plugin for recentering of spatial subset (Imviz only) -->
-    <v-row v-if="config=='imviz' && is_editable">
-      <v-expansion-panels accordion v-model="subplugins_opened">
-        <v-expansion-panel>
-          <v-expansion-panel-header >
-            <span style="padding: 6px">Recenter</span>
-          </v-expansion-panel-header>
-          <v-expansion-panel-content>
-            <plugin-dataset-select
-             :items="dataset_items"
-             :selected.sync="dataset_selected"
-             :show_if_single_entry="true"
-             label="Data"
-             hint="Select the data for centroiding."
-            />
-            <v-row justify="end" no-gutters>
-              <v-btn color="primary" text @click="recenter_subset">Recenter</v-btn>
-            </v-row>
-          </v-expansion-panel-content>
-        </v-expansion-panel>
-      </v-expansion-panels>
+    
+    <v-row>
+      <v-slider
+        v-model="angle"
+        class="align-center"
+        max="180"
+        min="-180"
+        step="1"
+        color="#00617E"
+        track-color="#00617E"
+        thumb-color="#153A4B"
+        hide-details
+      >
+      </v-slider>
     </v-row>
 
-    <!-- Composite region cannot be edited, so just grab first element. -->
-    <div v-if="is_editable">
-      <v-row v-for="(item, index2) in subset_definitions[0]"
-       class="pt-0 pb-0 mt-0 mb-0">
+    <v-row>
+      <v-col>
         <v-text-field
-          :label="item.name"
-          v-model.number="item.value"
+          v-model.number="angle"
           type="number"
+          label="Angle"
+          hint="Rotation angle in degrees clockwise"
         ></v-text-field>
-      </v-row>
+      </v-col>
+    </v-row>
 
-      <v-row justify="end" no-gutters>
-        <v-btn color="primary" text @click="update_subset">Update</v-btn>
-      </v-row>
-    </div>
+    <v-row>
+      <v-switch v-model="flip_horizontal" label="Flip horizontally after rotation"></v-switch>
+    </v-row>
 
-    <div v-if="show_region_info">
-      <j-plugin-section-header>Subset Region Definition</j-plugin-section-header>
-      <div v-if="subset_definitions.length">
-        <v-row v-for="(subset_definition, index) in subset_definitions" no-gutters>
-          <v-col>
-            <v-row class="pt-0 pb-0 mt-0 mb-0">
-              <v-col>Subset type:</v-col>
-              <v-col>{{ subset_types[index] }}</v-col>
-            </v-row>
-            <v-row v-for="(item, index2) in subset_definition"
-             class="pt-0 pb-0 mt-0 mb-0" no-gutters>
-              <v-col>{{ item.name }}:</v-col>
-              <v-col>
-                <j-number-uncertainty
-                  :value="item.orig"
-                  :defaultDigs="6"
-                ></j-number-uncertainty>
-              </v-col>
-            </v-row>
-          </v-col>
-        </v-row>
-      </div>
-    </div>
   </j-tray-plugin>
 </template>
+
+<script>
+module.exports = {
+  methods: {
+    isChromium() {
+      try {
+        for (brand_version_pair of navigator.userAgentData.brands) {
+            if (brand_version_pair.brand == "Chromium"){
+                return true;
+            }
+        }
+        return false;
+      }
+      catch {
+        return false
+      }
+    }
+  }
+}
+</script>
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_plugin/tests/test_subset_plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import warnings
 import pytest
+
 from glue.core.roi import XRangeROI
 
 
 @pytest.mark.filterwarnings('ignore')
 def test_plugin(specviz_helper, spectrum1d):
     specviz_helper.load_spectrum(spectrum1d)
     p = specviz_helper.plugins['Subset Tools']
@@ -12,7 +14,14 @@
     sv.apply_roi(XRangeROI(6500, 7400))
 
     p._obj.subset_select.selected = 'Create New'
 
     po = specviz_helper.plugins['Plot Options']
     po.layer = 'Subset 1'
     po.line_color = 'green'
+
+
+def test_subset_definition_with_composite_subset(cubeviz_helper, spectrum1d_cube):
+    with warnings.catch_warnings():
+        warnings.simplefilter('ignore')
+        cubeviz_helper.load_data(spectrum1d_cube)
+    cubeviz_helper.app.get_tray_item_from_name('g-subset-plugin')
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/subset_tools/subset_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/viewer_creator/viewer_creator.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/default/plugins/viewers.py` & `jdaviz-3.5.0/jdaviz/configs/default/plugins/viewers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/helper.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,16 @@
               keyword is also given)
             * ``'filename.fits[SCI]'`` (loads only first SCI extension)
             * ``'filename.fits[SCI,2]'`` (loads the second SCI extension)
             * ``'filename.jpg'`` (requires ``scikit-image``; grayscale only)
             * ``'filename.png'`` (requires ``scikit-image``; grayscale only)
             * JWST ASDF-in-FITS file (requires ``stdatamodels`` and ``gwcs``; ``data`` or given
               ``ext`` + GWCS)
+            * Roman ASDF file or `roman_datamodels.datamodels.ImageModel`
+              (requires ``roman-datamodels``)
             * `~astropy.io.fits.HDUList` object (first image extension found
               is loaded unless ``ext`` keyword is also given)
             * `~astropy.io.fits.ImageHDU` object
             * `~astropy.nddata.NDData` object (2D only but may have unit,
               mask, or uncertainty attached)
             * Numpy array (2D or 3D); if 3D, it will treat each slice at
               ``axis=0`` as a separate image (limit is 16 slices), however
@@ -233,14 +235,36 @@
         -------
         results : `~astropy.table.QTable` or `None`
             Table of sources if available or `None` otherwise.
 
         """
         return getattr(self.app, '_catalog_source_table', None)
 
+    def get_data(self, data_label=None, spatial_subset=None, cls=None):
+        """
+        Returns data with name equal to data_label of type cls with subsets applied from
+        spatial_subset.
+
+        Parameters
+        ----------
+        data_label : str, optional
+            Provide a label to retrieve a specific data set from data_collection.
+        spatial_subset : str, optional
+            Spatial subset applied to data.
+        cls : `~specutils.Spectrum1D`, `~astropy.nddata.CCDData`, optional
+            The type that data will be returned as.
+
+        Returns
+        -------
+        data : cls
+            Data is returned as type cls with subsets applied.
+
+        """
+        return self._get_data(data_label=data_label, spatial_subset=spatial_subset, cls=cls)
+
 
 def split_filename_with_fits_ext(filename):
     """Split a ``filename[ext]`` input into filename and FITS extension.
 
     Parameters
     ----------
     filename : str
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/imviz.yaml` & `jdaviz-3.5.0/jdaviz/configs/imviz/imviz.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - g-subset-plugin
   - g-markers
   - imviz-links-control
   - imviz-compass
   - imviz-line-profile-xy
   - imviz-aper-phot-simple
   - imviz-catalogs
+  - imviz-rotate-canvas
   - g-export-plot
 viewer_area:
   - container: col
     children:
       - container: row
         viewers:
           - name: imviz-0
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     background_value = Any(0).tag(sync=True)
     bg_annulus_inner_r = FloatHandleEmpty(0).tag(sync=True)
     bg_annulus_width = FloatHandleEmpty(10).tag(sync=True)
     pixel_area = Any(0).tag(sync=True)
     counts_factor = Any(0).tag(sync=True)
     flux_scaling = Any(0).tag(sync=True)
     result_available = Bool(False).tag(sync=True)
+    result_failed_msg = Unicode("").tag(sync=True)
     results = List().tag(sync=True)
     plot_types = List([]).tag(sync=True)
     current_plot_type = Unicode().tag(sync=True)
     plot_available = Bool(False).tag(sync=True)
     radial_plot = Any('').tag(sync=True, **widget_serialization)
     fit_radial_profile = Bool(False).tag(sync=True)
     fit_results = List().tag(sync=True)
@@ -86,27 +87,19 @@
         self.plot_types = ["Curve of Growth", "Radial Profile", "Radial Profile (Raw)"]
         self.current_plot_type = self.plot_types[0]
         self._fitted_model_name = 'phot_radial_profile'
 
         self.session.hub.subscribe(self, SubsetUpdateMessage, handler=self._on_subset_update)
         self.session.hub.subscribe(self, LinkUpdatedMessage, handler=self._on_link_update)
 
-    def reset_results(self):
-        self.result_available = False
-        self.results = []
-        self.plot_available = False
-        self.radial_plot = ''
-        bqplot_clear_figure(self._fig)
-
     @observe('dataset_selected')
     def _dataset_selected_changed(self, event={}):
         try:
             self._selected_data = self.dataset.selected_dc_item
             if self._selected_data is None:
-                self.reset_results()
                 return
             self.counts_factor = 0
             self.pixel_area = 0
             self.flux_scaling = 0
 
             # Extract telescope specific unit conversion factors, if applicable.
             meta = self._selected_data.meta.copy()
@@ -139,15 +132,14 @@
                         self.pixel_area = 0.028 * 0.025
                     elif detector == 'sbc':  # pragma: no cover
                         self.pixel_area = 0.034 * 0.03
                 elif instrument == 'wfc3' and detector == 'uvis':  # pragma: no cover
                     self.pixel_area = 0.04 * 0.04
 
         except Exception as e:
-            self.reset_results()
             self._selected_data = None
             self.hub.broadcast(SnackbarMessage(
                 f"Failed to extract {self.dataset_selected}: {repr(e)}",
                 color='error', sender=self))
 
         # Update self._selected_subset with the new self._selected_data
         # and auto-populate background, if applicable.
@@ -170,15 +162,14 @@
         # Force background auto-calculation (including annulus) to update when linking has changed.
         self._subset_selected_changed()
 
     @observe('subset_selected')
     def _subset_selected_changed(self, event={}):
         subset_selected = event.get('new', self.subset_selected)
         if self._selected_data is None or subset_selected == '':
-            self.reset_results()
             return
 
         try:
             self._selected_subset = _get_region_from_spatial_subset(self, subset_selected)
             self._selected_subset.meta['label'] = subset_selected
 
             if isinstance(self._selected_subset, CirclePixelRegion):
@@ -192,15 +183,14 @@
             else:  # pragma: no cover
                 raise TypeError(f'Unsupported region shape: {self._selected_subset.__class__}')
 
             self.subset_area = int(np.ceil(self._selected_subset.area))
 
         except Exception as e:
             self._selected_subset = None
-            self.reset_results()
             self.hub.broadcast(SnackbarMessage(
                 f"Failed to extract {subset_selected}: {repr(e)}", color='error', sender=self))
 
         else:
             self._bg_subset_selected_changed()
 
     def _calc_bg_subset_median(self, reg):
@@ -245,15 +235,14 @@
         except Exception as e:
             self.background_value = 0
             self.hub.broadcast(SnackbarMessage(
                 f"Failed to extract {bg_subset_selected}: {repr(e)}", color='error', sender=self))
 
     def vue_do_aper_phot(self, *args, **kwargs):
         if self._selected_data is None or self._selected_subset is None:
-            self.reset_results()
             self.hub.broadcast(SnackbarMessage(
                 "No data for aperture photometry", color='error', sender=self))
             return
 
         data = self._selected_data
         reg = self._selected_subset
         xcenter = reg.center.x
@@ -426,22 +415,23 @@
                     bqplot_fit = bqplot.Lines(x=x_data, y=y_fit, marker=None,
                                               scales={'x': line_x_sc, 'y': line_y_sc},
                                               colors='magenta', line_style='dashed')
                     bqplot_marks = [bqplot_line, bqplot_fit]
                 else:
                     bqplot_marks = [bqplot_line]
 
-            self._fig.marks = bqplot_marks
-
         except Exception as e:  # pragma: no cover
-            self.reset_results()
-            self.hub.broadcast(SnackbarMessage(
-                f"Aperture photometry failed: {repr(e)}", color='error', sender=self))
-
+            bqplot_clear_figure(self._fig)
+            msg = f"Aperture photometry failed: {repr(e)}"
+            self.hub.broadcast(SnackbarMessage(msg, color='error', sender=self))
+            self.result_failed_msg = msg
         else:
+            self.result_failed_msg = ''
+            self._fig.marks = bqplot_marks
+
             # Parse results for GUI.
             tmp = []
             for key in phot_table.colnames:
                 if key in ('id', 'data_label', 'subset_label', 'background', 'pixarea_tot',
                            'counts_fac', 'aperture_sum_counts_err', 'flux_scaling', 'timestamp'):
                     continue
                 x = phot_table[key][0]
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/aper_phot_simple/aper_phot_simple.vue`

 * *Files 8% similar despite different names*

```diff
@@ -135,14 +135,20 @@
 
         <v-row justify="end">
           <v-btn color="primary" text @click="do_aper_phot" :disabled="subset_selected === bg_subset_selected">Calculate</v-btn>
         </v-row>
       </div>
     </div>
 
+    <v-row v-if="result_failed_msg.length > 0">
+      <span class="v-messages v-messages__message text--secondary" style="color: red !important">
+          <b>WARNING</b>: {{result_failed_msg}}
+      </span>
+    </v-row>
+
     <v-row v-if="plot_available">
       <!-- NOTE: the internal bqplot widget defaults to 480 pixels, so if choosing something else,
            we will likely need to override that with custom CSS rules in order to avoid the initial
            rendering of the plot from overlapping with content below -->
       <jupyter-widget :widget="radial_plot" style="width: 100%; height: 480px" />
     </v-row>
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/catalogs/catalogs.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/compass/compass.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/compass/compass.vue`

 * *Files 24% similar despite different names*

```diff
@@ -38,19 +38,40 @@
 00000250: 2020 2020 3c2f 762d 6368 6970 3e0d 0a20      </v-chip>.. 
 00000260: 2020 203c 2f76 2d72 6f77 3e0d 0a0d 0a20     </v-row>.... 
 00000270: 2020 203c 696d 6720 636c 6173 733d 2769     <img class='i
 00000280: 6e76 6572 742d 696e 2d64 6172 6b27 2076  nvert-in-dark' v
 00000290: 2d69 663d 2269 6d67 5f64 6174 6122 203a  -if="img_data" :
 000002a0: 7372 633d 2260 6461 7461 3a69 6d61 6765  src="`data:image
 000002b0: 2f70 6e67 3b62 6173 6536 342c 247b 696d  /png;base64,${im
-000002c0: 675f 6461 7461 7d60 2220 7374 796c 653d  g_data}`" style=
-000002d0: 2277 6964 7468 3a20 3130 3025 3b20 6d61  "width: 100%; ma
-000002e0: 782d 7769 6474 683a 2034 3030 7078 2220  x-width: 400px" 
-000002f0: 2f3e 0d0a 0d0a 2020 3c2f 6a2d 7472 6179  />....  </j-tray
-00000300: 2d70 6c75 6769 6e3e 0d0a 3c2f 7465 6d70  -plugin>..</temp
-00000310: 6c61 7465 3e0d 0a0d 0a3c 7374 796c 653e  late>....<style>
-00000320: 0d0a 2e74 6865 6d65 2d2d 6461 726b 202e  ...theme--dark .
-00000330: 696e 7665 7274 2d69 6e2d 6461 726b 207b  invert-in-dark {
-00000340: 0d0a 2020 6669 6c74 6572 3a20 6272 6967  ..  filter: brig
-00000350: 6874 6e65 7373 2830 2e38 3829 2069 6e76  htness(0.88) inv
-00000360: 6572 7428 3129 3b0d 0a7d 0d0a 3c2f 7374  ert(1);..}..</st
-00000370: 796c 653e 0d0a                           yle>..
+000002c0: 675f 6461 7461 7d60 2220 3a73 7479 6c65  g_data}`" :style
+000002d0: 3d22 2777 6964 7468 3a20 3130 3025 3b20  ="'width: 100%; 
+000002e0: 6d61 782d 7769 6474 683a 2034 3030 7078  max-width: 400px
+000002f0: 3b20 6d61 7267 696e 2d74 6f70 3a20 3530  ; margin-top: 50
+00000300: 7078 3b20 7472 616e 7366 6f72 6d3a 2072  px; transform: r
+00000310: 6f74 6174 6559 2827 2b76 6965 7765 725f  otateY('+viewer_
+00000320: 726f 7461 7465 5928 6361 6e76 6173 5f66  rotateY(canvas_f
+00000330: 6c69 705f 686f 7269 7a6f 6e74 616c 292b  lip_horizontal)+
+00000340: 2729 2072 6f74 6174 6528 272b 6361 6e76  ') rotate('+canv
+00000350: 6173 5f61 6e67 6c65 2b27 6465 6729 2722  as_angle+'deg)'"
+00000360: 202f 3e0d 0a0d 0a20 203c 2f6a 2d74 7261   />....  </j-tra
+00000370: 792d 706c 7567 696e 3e0d 0a3c 2f74 656d  y-plugin>..</tem
+00000380: 706c 6174 653e 0d0a 0d0a 3c73 6372 6970  plate>....<scrip
+00000390: 743e 0d0a 6d6f 6475 6c65 2e65 7870 6f72  t>..module.expor
+000003a0: 7473 203d 207b 0d0a 2020 6d65 7468 6f64  ts = {..  method
+000003b0: 733a 207b 0d0a 2020 2020 7669 6577 6572  s: {..    viewer
+000003c0: 5f72 6f74 6174 6559 2863 616e 7661 735f  _rotateY(canvas_
+000003d0: 666c 6970 5f68 6f72 697a 6f6e 7461 6c29  flip_horizontal)
+000003e0: 207b 0d0a 2020 2020 2020 6966 2028 6361   {..      if (ca
+000003f0: 6e76 6173 5f66 6c69 705f 686f 7269 7a6f  nvas_flip_horizo
+00000400: 6e74 616c 2920 7b0d 0a20 2020 2020 2020  ntal) {..       
+00000410: 2072 6574 7572 6e20 2731 3830 6465 6727   return '180deg'
+00000420: 0d0a 2020 2020 2020 7d20 656c 7365 207b  ..      } else {
+00000430: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000440: 2027 3064 6567 270d 0a20 2020 2020 207d   '0deg'..      }
+00000450: 0d0a 2020 2020 7d0d 0a20 207d 0d0a 7d3b  ..    }..  }..};
+00000460: 0d0a 3c2f 7363 7269 7074 3e0d 0a0d 0a0d  ..</script>.....
+00000470: 0a3c 7374 796c 653e 0d0a 2e74 6865 6d65  .<style>...theme
+00000480: 2d2d 6461 726b 202e 696e 7665 7274 2d69  --dark .invert-i
+00000490: 6e2d 6461 726b 207b 0d0a 2020 6669 6c74  n-dark {..  filt
+000004a0: 6572 3a20 6272 6967 6874 6e65 7373 2830  er: brightness(0
+000004b0: 2e38 3829 2069 6e76 6572 7428 3129 3b0d  .88) invert(1);.
+000004c0: 0a7d 0d0a 3c2f 7374 796c 653e 0d0a       .}..</style>..
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,27 @@
 from jdaviz.core.helpers import data_has_valid_wcs
 from jdaviz.core.marks import PluginScatter
 from jdaviz.core.registries import tool_registry
 from jdaviz.core.template_mixin import TemplateMixin, DatasetSelectMixin
 
 __all__ = ['CoordsInfo']
 
-_supported_viewer_classes = (SpecvizProfileView,
-                             ImvizImageView,
-                             CubevizImageView,
-                             MosvizImageView,
-                             MosvizProfile2DView)
-
 
 @tool_registry('g-coords-info')
 class CoordsInfo(TemplateMixin, DatasetSelectMixin):
     template_file = __file__, "coords_info.vue"
 
+    _supported_viewer_classes = (SpecvizProfileView,
+                                 ImvizImageView,
+                                 CubevizImageView,
+                                 MosvizImageView,
+                                 MosvizProfile2DView)
+
+    _viewer_classes_with_marker = (SpecvizProfileView,)
+
     dataset_icon = Unicode("").tag(sync=True)  # option for layer (auto, none, or specific layer)
     icon = Unicode("").tag(sync=True)  # currently exposed layer
 
     row1a_title = Unicode("").tag(sync=True)
     row1a_text = Unicode("").tag(sync=True)
     row1b_title = Unicode("").tag(sync=True)
     row1b_text = Unicode("").tag(sync=True)
@@ -53,31 +55,43 @@
         self._marks = {}
         self._dict = {}  # dictionary representation of current mouseover info
         self._x, self._y = None, None  # latest known cursor positions
 
         # subscribe/unsubscribe to mouse events across all existing viewers
         viewer_refs = []
         for viewer in self.app._viewer_store.values():
-            if isinstance(viewer, _supported_viewer_classes):
+            if isinstance(viewer, self._supported_viewer_classes):
                 self._create_viewer_callbacks(viewer)
                 viewer_refs.append(viewer.reference_id)
 
         self.dataset._manual_options = ['auto', 'none']
         self.dataset.filters = ['layer_in_viewers']
         if self.app.config == 'imviz':
             # filter out scatter-plot entries (from add_markers API, for example)
             self.dataset.add_filter('is_image')
         # we also want to include auto-collapsed spectra (spatial subsets)
         self.dataset._cubeviz_include_spatial_subsets()
 
         # subscribe to mouse events on any new viewers
         self.hub.subscribe(self, ViewerAddedMessage, handler=self._on_viewer_added)
 
+    def _create_marks_for_viewer(self, viewer, id=None):
+        if id is None:
+            id = viewer.reference_id
+        if id in self._marks:
+            return
+        self._marks[id] = PluginScatter(viewer,
+                                        marker='rectangle', stroke_width=1,
+                                        visible=False)
+        viewer.figure.marks = viewer.figure.marks + [self._marks[id]]
+
     def _create_viewer_callbacks(self, viewer):
-        if isinstance(viewer, _supported_viewer_classes):
+        if isinstance(viewer, self._supported_viewer_classes):
+            if isinstance(viewer, self._viewer_classes_with_marker):
+                self._create_marks_for_viewer(viewer)
             callback = self._viewer_callback(viewer, self._viewer_mouse_event)
             viewer.add_event_callback(callback, events=['mousemove', 'mouseleave', 'mouseenter'])
 
             viewer.state.add_callback('layers', lambda msg: self._layers_changed(viewer))
 
     def _on_viewer_added(self, msg):
         self._create_viewer_callbacks(self.app.get_viewer_by_id(msg.viewer_id))
@@ -90,19 +104,16 @@
         if self._marks:
             # TODO: replace with cache property?
             return self._marks
 
         # create marks for each of the spectral viewers (will need a listener event to create marks
         # for new viewers if dynamic creation of spectral viewers is ever supported)
         for id, viewer in self.app._viewer_store.items():
-            if isinstance(viewer, SpecvizProfileView):
-                self._marks[id] = PluginScatter(viewer,
-                                                marker='rectangle', stroke_width=1,
-                                                visible=False)
-                viewer.figure.marks = viewer.figure.marks + [self._marks[id]]
+            if isinstance(viewer, self._viewer_classes_with_marker):
+                self._create_marks_for_viewer(viewer, id)
         return self._marks
 
     def as_text(self):
         return (f"{self.row1a_title} {self.row1a_text} {self.row1b_title} {self.row1b_text}".strip(),  # noqa
                 f"{self.row2_title} {self.row2_text}".strip(),
                 f"{self.row3_title} {self.row3_text}".strip())
 
@@ -238,15 +249,14 @@
         elif isinstance(viewer, ImvizImageView):
             x, y, coords_status, (unreliable_world, unreliable_pixel) = viewer._get_real_xy(image, x, y)  # noqa
             if coords_status:
                 try:
                     sky = image.coords.pixel_to_world(x, y).icrs
                 except Exception:  # WCS might not be celestial
                     coords_status = False
-                    self.reset_coords_display()
 
         elif isinstance(viewer, CubevizImageView):
             # TODO: This assumes data_collection[0] is the main reference
             #  data for this application. This section will need to be updated
             #  when that is no longer true.
             # Hack to insert WCS for generated 2D and 3D images using FLUX cube WCS.
             if 'Plugin' in getattr(image, 'meta', {}) and not image.coords:
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/coords_info/coords_info.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/links_control/links_control.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/links_control/links_control.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/parsers.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import os
 
 import numpy as np
 from astropy import units as u
 from astropy.io import fits
 from astropy.nddata import NDData
 from astropy.wcs import WCS
+from astropy.utils.data import cache_contents
+
 from glue.core.data import Component, Data
 from gwcs.wcs import WCS as GWCS
 from stdatamodels import asdf_in_fits
 
 from jdaviz.core.registries import data_parser_registry
 from jdaviz.core.events import SnackbarMessage
 from jdaviz.utils import standardize_metadata, PRIHDR_KEY
 
+try:
+    from roman_datamodels import datamodels as rdd
+except ImportError:
+    HAS_ROMAN_DATAMODELS = False
+else:
+    HAS_ROMAN_DATAMODELS = True
+
 __all__ = ['parse_data']
 
 INFO_MSG = ("The file contains more viewable extensions. Add the '[*]' suffix"
             " to the file name to load all of them.")
 
 
 @data_parser_registry("imviz-data-parser")
@@ -37,35 +46,58 @@
     data_label : str, optional
         The label to be applied to the Glue data component.
 
     """
     if isinstance(file_obj, str):
         if data_label is None:
             data_label = os.path.splitext(os.path.basename(file_obj))[0]
-        if file_obj.lower().endswith(('.jpg', '.jpeg', '.png')):
+
+        # If file_obj is a path to a cached file from
+        # astropy.utils.data.download_file, the path has no file extension.
+        # Here we check if the file is in the download cache, and if it is,
+        # we look up the file extension from the source URL:
+        if file_obj.endswith('contents'):
+            path_to_url_mapping = {v: k for k, v in cache_contents().items() if file_obj}
+            source_url = path_to_url_mapping[file_obj]
+            # file_obj_lower is only used for checking extensions,
+            # file_obj is passed for parsing and is not modified here:
+            file_obj_lower = source_url.split('/')[-1].lower()
+        else:
+            file_obj_lower = file_obj.lower()
+
+        if file_obj_lower.endswith(('.jpg', '.jpeg', '.png')):
             from skimage.io import imread
             from skimage.color import rgb2gray, rgba2rgb
             im = imread(file_obj)
             if im.shape[2] == 4:
                 pf = rgb2gray(rgba2rgb(im))
             else:  # Assume RGB
                 pf = rgb2gray(im)
             pf = pf[::-1, :]  # Flip it
             _parse_image(app, pf, data_label, ext=ext)
+
+        elif file_obj_lower.endswith('.asdf'):
+            if not HAS_ROMAN_DATAMODELS:
+                raise ImportError(
+                    "ASDF detected but roman-datamodels is not installed."
+                )
+            with rdd.open(file_obj) as pf:
+                _parse_image(app, pf, data_label, ext=ext)
         else:  # Assume FITS
             with fits.open(file_obj) as pf:
                 _parse_image(app, pf, data_label, ext=ext)
     else:
         _parse_image(app, file_obj, data_label, ext=ext)
 
 
 def get_image_data_iterator(app, file_obj, data_label, ext=None):
     """This function is for internal use, so other viz can also extract image data
     like Imviz does.
     """
+
     if isinstance(file_obj, fits.HDUList):
         if 'ASDF' in file_obj:  # JWST ASDF-in-FITS
             # Load all extensions
             if ext == '*':
                 data_iter = _jwst_all_to_glue_data(file_obj, data_label)
 
             # Load only specified extension
@@ -107,14 +139,18 @@
 
     elif isinstance(file_obj, NDData):
         data_iter = _nddata_to_glue_data(file_obj, data_label)
 
     elif isinstance(file_obj, np.ndarray):
         data_iter = _ndarray_to_glue_data(file_obj, data_label)
 
+    # Roman 2D datamodels
+    elif HAS_ROMAN_DATAMODELS and isinstance(file_obj, rdd.DataModel):
+        data_iter = _roman_2d_to_glue_data(file_obj, data_label, ext=ext)
+
     else:
         raise NotImplementedError(f'Imviz does not support {file_obj}')
 
     return data_iter
 
 
 def _parse_image(app, file_obj, data_label, ext=None):
@@ -260,15 +296,45 @@
             ext = 'sci'
         hdu = file_obj[ext]
         return _hdu2data(hdu, data_label, file_obj, include_wcs=False)
 
     return data, new_data_label
 
 
-# ---- Functions that handle input from non-JWST FITS files -----
+# ---- Functions that handle input from Roman ASDF files -----
+
+def _roman_2d_to_glue_data(file_obj, data_label, ext=None):
+
+    if ext == '*' or ext is None:
+        # NOTE: Update as needed. Should cover all the image extensions available.
+        ext_list = ('data', 'dq', 'err', 'var_poisson', 'var_rnoise')
+    elif isinstance(ext, (list, tuple)):
+        ext_list = ext
+    else:
+        ext_list = (ext, )
+
+    meta = getattr(file_obj, 'meta', {})
+    coords = getattr(meta, 'wcs', None)
+
+    for cur_ext in ext_list:
+        comp_label = cur_ext.upper()
+        new_data_label = f'{data_label}[{comp_label}]'
+        data = Data(coords=coords, label=new_data_label)
+
+        # This could be a quantity or a ndarray:
+        ext_values = getattr(file_obj, cur_ext)
+        bunit = getattr(ext_values, 'unit', '')
+        component = Component.autotyped(np.array(ext_values), units=bunit)
+        data.add_component(component=component, label=comp_label)
+        data.meta.update(standardize_metadata(dict(meta)))
+
+        yield data, new_data_label
+
+
+# ---- Functions that handle input from non-JWST, non-Roman FITS files -----
 
 def _hdu_to_glue_data(hdu, data_label, hdulist=None):
     data, data_label = _hdu2data(hdu, data_label, hdulist)
     yield data, data_label
 
 
 def _hdus_to_glue_data(file_obj, data_label):
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/tools.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/plugins/viewers.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/plugins/viewers.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,15 @@
                 (self.state.y_min, self.state.y_max, self.state.y_max, self.state.y_min)))
             zoom_limits = np.array(list(zip(x[0], x[1])))
         else:
             zoom_limits = np.array(((self.state.x_min, self.state.y_min),
                                     (self.state.x_min, self.state.y_max),
                                     (self.state.x_max, self.state.y_max),
                                     (self.state.x_max, self.state.y_min)))
+
         return zoom_limits
 
     def set_compass(self, image):
         """Update the Compass plugin with info from the given image Data object."""
         if self.compass is None:  # Maybe another viewer has it
             return
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_astrowidgets_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from astropy.utils.data import get_pkg_data_filename
 from astropy.visualization import AsinhStretch, LinearStretch, LogStretch, SqrtStretch
 from numpy.testing import assert_allclose
 
 from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_NoWCS, BaseImviz_WCS_WCS
 
 
-# TODO: Remove skip when https://github.com/bqplot/bqplot/issues/1393 is resolved.
-@pytest.mark.skip(reason="Cannot test due to file dialog popup")
+# TODO: Remove skip when https://github.com/bqplot/bqplot/pull/1397/files#r726500097 is resolved.
+@pytest.mark.skip(reason="Cannot test due to async JS callback")
 class TestSave(BaseImviz_WCS_NoWCS):
 
     def test_save(self, tmpdir):
         filename = os.path.join(tmpdir.strpath, 'myimage')
         self.viewer.save(filename)
 
         # This only tests that something saved, not the content.
-        assert os.path.isfile(os.path.join(tmpdir.strpath, 'myimage.png'))
+        assert os.path.isfile(f'{filename}.png')
 
 
 class TestCenterOffset(BaseImviz_WCS_NoWCS):
 
     def test_center_offset_pixel(self):
         self.viewer.center_on((0, 1))
         assert_allclose((self.viewer.state.x_min, self.viewer.state.x_max,
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_catalogs.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_helper.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_line_profile_xy.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_linking.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_links_control.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_links_control.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_parser.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.io import fits
 from astropy.nddata import NDData, StdDevUncertainty
 from astropy.tests.helper import assert_quantity_allclose
-from astropy.utils.data import download_file
+from astropy.utils.data import download_file, get_pkg_data_filename
 from astropy.wcs import WCS
 from gwcs import WCS as GWCS
 from numpy.testing import assert_allclose, assert_array_equal
 from regions import CirclePixelRegion, RectanglePixelRegion
 from skimage.io import imsave
 from stdatamodels import asdf_in_fits
 
 from jdaviz.configs.imviz.helper import split_filename_with_fits_ext
 from jdaviz.configs.imviz.plugins.parsers import (
-    parse_data, _validate_fits_image2d, _validate_bunit, _parse_image)
+    parse_data, _validate_fits_image2d, _validate_bunit, _parse_image, HAS_ROMAN_DATAMODELS)
 
 
 @pytest.mark.parametrize(
     ('filename', 'ans'),
     [('/path/to/cache/contents', ['/path/to/cache/contents', None, 'contents']),
      ('file://path/image.fits[SCI]', ['file://path/image.fits', 'SCI', 'image']),
      ('image.fits[dq,2]', ['image.fits', ('dq', 2), 'image']),
@@ -499,7 +499,14 @@
     with pytest.raises(ValueError, match='Imviz cannot load this array with ndim=1'):
         imviz_helper.load_data(np.zeros(2), show_in_viewer=False)
 
     # Make sure valid data is still there.
     assert (len(imviz_helper.app.data_collection) == 1
             and imviz_helper.app.data_collection.labels == ['valid'])
     assert_allclose(imviz_helper.app.data_collection[0].get_component('DATA').data, 1)
+
+
+@pytest.mark.skipif(not HAS_ROMAN_DATAMODELS, reason="roman_datamodels is not installed")
+def test_roman_parser(imviz_helper):
+    filename = get_pkg_data_filename('data/roman_wfi_image_model.asdf')
+    imviz_helper.load_data(filename)
+    assert len(imviz_helper.app.data_collection) == 1
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_regions.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import glue_astronomy
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import SkyCoord, Angle
 from astropy.utils.data import get_pkg_data_filename
+from packaging.version import Version
 from photutils.aperture import CircularAperture, SkyCircularAperture
 from regions import (PixCoord, CircleSkyRegion, RectanglePixelRegion, CirclePixelRegion,
                      EllipsePixelRegion, PointSkyRegion, PolygonPixelRegion,
-                     CircleAnnulusSkyRegion, Regions)
+                     CircleAnnulusPixelRegion, CircleAnnulusSkyRegion, Regions)
 
 from jdaviz.configs.imviz.tests.utils import BaseImviz_WCS_NoWCS
 
+GLUE_ASTRONOMY_LT_0_7_1 = not (Version(glue_astronomy.__version__) >= Version("0.7.1.dev"))
+
 
 class BaseRegionHandler:
     """Test to see if region is loaded.
     Does not check if region is actually at the correct place in display.
     """
     def verify_region_loaded(self, region_label, count=2):
         n = 0
@@ -226,17 +230,23 @@
         assert isinstance(subsets['Subset 2'], CirclePixelRegion)
 
         # Create a third subset that is an annulus.
         subset_groups = self.imviz.app.data_collection.subset_groups
         new_subset = subset_groups[0].subset_state & ~subset_groups[1].subset_state
         self.viewer.apply_subset_state(new_subset)
 
-        # Annulus is no longer accessible by API but also should not crash Imviz.
+        # In older glue-astronomy, annulus is no longer accessible by API
+        # but also should not crash Imviz.
         subsets = self.imviz.get_interactive_regions()
         assert len(self.imviz.app.data_collection.subset_groups) == 3
-        assert list(subsets.keys()) == ['Subset 1', 'Subset 2'], subsets
+        if GLUE_ASTRONOMY_LT_0_7_1:
+            expected_subset_keys = ['Subset 1', 'Subset 2']
+        else:
+            expected_subset_keys = ['Subset 1', 'Subset 2', 'Subset 3']
+            assert isinstance(subsets['Subset 3'], CircleAnnulusPixelRegion)
+        assert list(subsets.keys()) == expected_subset_keys, subsets
         assert isinstance(subsets['Subset 1'], CirclePixelRegion)
         assert isinstance(subsets['Subset 2'], CirclePixelRegion)
 
         # Clear the regions for next test.
         self.imviz._delete_all_regions()
         assert len(self.imviz.app.data_collection.subset_groups) == 0
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_simple_aper_phot.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_subset_centroid.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_subset_centroid.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_tools.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_viewer_tools.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewer_tools.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_viewers.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_viewers.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,21 @@
     assert imviz_helper.plugins['Imviz Line Profiles (XY)']._obj.viewer_items == viewer_names
     assert sorted(imviz_helper.plugins['Compass'].viewer.labels) == viewer_names
 
     imviz_helper.destroy_viewer(actual_name)
     assert imviz_helper.app.get_viewer_ids() == ['imviz-0']
 
 
+def test_get_viewer_created(imviz_helper):
+    # This viewer has no reference but has ID.
+    viewer1 = imviz_helper.create_image_viewer()
+    viewer2 = imviz_helper.app.get_viewer('imviz-1')
+    assert viewer1 is viewer2
+
+
 def test_destroy_viewer_invalid(imviz_helper):
     assert imviz_helper.app.get_viewer_ids() == ['imviz-0']
 
     imviz_helper.destroy_viewer('foo')
     assert imviz_helper.app.get_viewer_ids() == ['imviz-0']
 
     with pytest.raises(ValueError, match='cannot be destroyed'):
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/test_wcs_utils.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/tests/utils.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 from astropy import units as u
 from astropy.coordinates import ICRS
 from astropy.io import fits
 from astropy.modeling import models
 from astropy.nddata import NDData
 from astropy.wcs import WCS
-from gwcs import coordinate_frames as cf
+from gwcs import coordinate_frames as cf, wcs as gwcs_wcs
 
 __all__ = ['BaseImviz_WCS_NoWCS', 'BaseImviz_WCS_WCS', 'BaseImviz_WCS_GWCS', 'BaseImviz_GWCS_GWCS']
 
 
 class BaseImviz_WCS_NoWCS:
     @pytest.fixture(autouse=True)
     def setup_class(self, imviz_helper):
@@ -197,7 +197,73 @@
         self.wcs_2 = w_gwcs_2
         self.imviz = imviz_helper
         self.viewer = imviz_helper.default_viewer
 
         # Since we are not really displaying, need this to test zoom.
         self.viewer.shape = (100, 100)
         self.viewer.state._set_axes_aspect_ratio(1)
+
+
+# --- This was used to generate data/roman_wfi_image_model.asdf ---
+
+def create_example_gwcs(shape):
+    # Example adapted from photutils:
+    #   https://github.com/astropy/photutils/blob/
+    #   2825356f1d876cacefb3a03d104a4c563065375f/photutils/datasets/make.py#L821
+    rho = np.pi / 3.0
+    # Roman plate scale:
+    scale = (0.11 * (u.arcsec / u.pixel)).to_value(u.deg / u.pixel)
+
+    shift_by_crpix = (models.Shift((-shape[1] / 2) + 1)
+                      & models.Shift((-shape[0] / 2) + 1))
+
+    cd_matrix = np.array([[-scale * np.cos(rho), scale * np.sin(rho)],
+                          [scale * np.sin(rho), scale * np.cos(rho)]])
+
+    rotation = models.AffineTransformation2D(cd_matrix, translation=[0, 0])
+    rotation.inverse = models.AffineTransformation2D(
+        np.linalg.inv(cd_matrix), translation=[0, 0])
+
+    tan = models.Pix2Sky_TAN()
+    celestial_rotation = models.RotateNative2Celestial(197.8925, -1.36555556, 180.0)
+
+    det2sky = shift_by_crpix | rotation | tan | celestial_rotation
+    det2sky.name = 'linear_transform'
+
+    detector_frame = cf.Frame2D(name='detector', axes_names=('x', 'y'), unit=(u.pix, u.pix))
+
+    sky_frame = cf.CelestialFrame(reference_frame=ICRS(), name='icrs', unit=(u.deg, u.deg))
+
+    pipeline = [(detector_frame, det2sky), (sky_frame, None)]
+
+    return gwcs_wcs.WCS(pipeline)
+
+
+def create_wfi_image_model(image_shape, **kwargs):
+    """
+    Create a dummy Roman WFI ImageModel instance with valid values
+    for attributes required by the schema.
+
+    Requires roman_datamodels >= 0.14.2
+
+    Parameters
+    ----------
+    image_shape : tuple
+        Shape of the synthetic image to produce.
+
+    **kwargs
+        Additional or overridden attributes.
+
+    Returns
+    -------
+    data_model : `roman_datamodels.datamodel.ImageModel`
+
+    """  # noqa: E501
+    from roman_datamodels import datamodels as rdd
+    from roman_datamodels.maker_utils import mk_level2_image
+
+    wfi_image = mk_level2_image(shape=image_shape, **kwargs)
+
+    # introduce synthetic gwcs:
+    wfi_image["meta"]["wcs"] = create_example_gwcs(image_shape)
+
+    return rdd.ImageModel(wfi_image)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/imviz/wcs_utils.py` & `jdaviz-3.5.0/jdaviz/configs/imviz/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/helper.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from time import time
 from zipfile import is_zipfile
 
 import numpy as np
@@ -14,15 +15,16 @@
 
 from jdaviz.core.helpers import ConfigHelper
 from jdaviz.core.events import SnackbarMessage, TableClickMessage, RedshiftMessage, RowLockMessage
 from jdaviz.configs.specviz import Specviz
 from jdaviz.configs.specviz.helper import _apply_redshift_to_spectra
 from jdaviz.configs.specviz2d import Specviz2d
 from jdaviz.configs.mosviz.plugins import jwst_header_to_skyregion
-from jdaviz.configs.mosviz.plugins.parsers import FALLBACK_NAME
+from jdaviz.configs.mosviz.plugins.parsers import (
+    FALLBACK_NAME, mos_spec1d_parser, mos_spec2d_parser)
 from jdaviz.configs.default.plugins.line_lists.line_list_mixin import LineListMixin
 
 __all__ = ['Mosviz']
 
 
 class Mosviz(ConfigHelper, LineListMixin):
     """Mosviz Helper class"""
@@ -284,91 +286,90 @@
         self._handle_flipped_data()
         # expose the row to vue for each of the viewers
         self.app.state.settings = {**self.app.state.settings, 'mosviz_row': msg.selected_index}
 
     def _handle_image_zoom(self, msg):
         mos_data = self.app.data_collection['MOS Table']
 
-        # trigger zooming the image, if there is an image
-        if mos_data.find_component_id("Images") is not None:
-            if msg.shared_image:
-                center, height = self._zoom_to_object_params(msg)
-            else:
-                try:
-                    center, height = self._zoom_to_slit_params(msg)
-                except IndexError:
-                    # If there's nothing in the spectrum2d viewer, we can't get slit info
-                    return
+        if mos_data.find_component_id("Images") is None:
+            return
 
-            if center is None or height is None:
-                # Can't zoom if we couldn't figure out where to zoom (e.g. if RA/Dec not in table)
-                return
+        imview = self.app.get_viewer(self._default_image_viewer_reference_name)
 
-            imview = self.app.get_viewer(self._default_image_viewer_reference_name)
+        # trigger zooming the image, if there is an image
+        if msg.shared_image:
+            center, height = self._zoom_to_object_params(msg)
+        else:
+            center, height = self._zoom_to_slit_params(msg)
 
-            image_axis_ratio = ((imview.axis_x.scale.max - imview.axis_x.scale.min) /
-                                (imview.axis_y.scale.max - imview.axis_y.scale.min))
+        if height is not None:
+            image_axis_ratio = (abs(imview.state.x_max - imview.state.x_min) /
+                                abs(imview.state.y_max - imview.state.y_min))
+            x_height = image_axis_ratio * height
+            cur_xcen = (imview.state.x_min + imview.state.x_max) * 0.5
+            cur_ycen = (imview.state.y_min + imview.state.y_max) * 0.5
 
             with delay_callback(imview.state, 'x_min', 'x_max', 'y_min', 'y_max'):
-                imview.state.x_min = center[0] - image_axis_ratio*height
-                imview.state.y_min = center[1] - height
-                imview.state.x_max = center[0] + image_axis_ratio*height
-                imview.state.y_max = center[1] + height
+                imview.state.x_min = cur_xcen - x_height
+                imview.state.y_min = cur_ycen - height
+                imview.state.x_max = cur_xcen + x_height
+                imview.state.y_max = cur_ycen + height
+
+        if center is not None:
+            imview.center_on(center)
 
     def _handle_flipped_data(self):
         # Workaround for flipped data
         if self._is_world_flipped():
             min, max = self._scales2d.max, self._scales2d.min
             with self._scales2d.hold_sync():
                 self._scales2d.min = min
                 self._scales2d.max = max
 
     def _zoom_to_object_params(self, msg):
 
         table_data = self.app.data_collection['MOS Table']
-        imview = self.app.get_viewer(self._default_image_viewer_reference_name)
         specview = self.app.get_viewer(self._default_spectrum_2d_viewer_reference_name)
 
         if ("R.A." not in table_data.component_ids() or
                 "Dec." not in table_data.component_ids()):
             return None, None
 
         ra = table_data["R.A."][msg.selected_index]
         dec = table_data["Dec."][msg.selected_index]
 
         if (ra == FALLBACK_NAME) or (dec == FALLBACK_NAME):
             return None, None
 
-        pixel_height = 0.5*(specview.axis_y.scale.max - specview.axis_y.scale.min)
-        point = SkyCoord(ra*u.deg, dec*u.deg)
-
-        pix = imview.layers[0].layer.coords.world_to_pixel(point)
+        try:
+            pixel_height = abs(specview.axis_y.scale.max - specview.axis_y.scale.min) * 0.5
+        except Exception:
+            pixel_height = None
+        else:
+            if pixel_height < 1:
+                pixel_height = None
+        sky = SkyCoord(ra, dec, unit='deg')
 
-        return pix, pixel_height
+        return sky, pixel_height
 
     def _zoom_to_slit_params(self, msg):
         imview = self.app.get_viewer(self._default_image_viewer_reference_name)
         specview = self.app.get_viewer(self._default_spectrum_2d_viewer_reference_name)
 
         try:
             sky_region = jwst_header_to_skyregion(specview.layers[0].layer.meta)
-        except KeyError:
+        except Exception:
             # If the header didn't have slit params, can't zoom to it.
             return None, None
-        ra = sky_region.center.ra.deg
-        dec = sky_region.center.dec.deg
-
-        pix = imview.layers[0].layer.coords.world_to_pixel(sky_region.center)
 
-        # Height of slit in decimal degrees
-        height = sky_region.height.deg
-
-        upper = imview.layers[0].layer.coords.world_to_pixel(SkyCoord(ra*u.deg,
-                                                             (dec + height)*u.deg))
-        pixel_height = upper[1] - pix[1]
+        sky = sky_region.center
+        w = imview.layers[0].layer.coords
+        pix = w.world_to_pixel(sky)
+        upper = w.world_to_pixel(SkyCoord(sky.ra, sky.dec + sky_region.height))
+        pixel_height = abs(upper[1] - pix[1])  # y
 
         return pix, pixel_height
 
     def _add_redshift_column(self):
         # Parse any information from the files into columns in the table
         def _get_sp_attribute(table_data, row, attr, fill=None):
             try:
@@ -402,15 +403,15 @@
         redshifts = np.asarray([_get_sp_attribute(table_data, row, 'redshift', 0)
                                 for row in range(int(table_data.size))])
         self._add_or_update_column(column_name='Redshift', data=redshifts,
                                    show=np.any(redshifts != 0))
 
     def load_data(self, spectra_1d=None, spectra_2d=None, images=None,
                   spectra_1d_label=None, spectra_2d_label=None,
-                  images_label=None, *args, **kwargs):
+                  images_label=None, directory=None, instrument=None):
         """
         Load and parse a set of MOS spectra and images.
 
         Parameters
         ----------
         spectra_1d : list or str
             A list of spectra as translatable container objects (e.g.
@@ -441,81 +442,113 @@
             String representing the label for the data item loaded via
             ``images``. Can be a list of strings representing data labels
             for each item in ``images`` if  ``images`` is a list.
 
         directory : str, optional
             Instead of loading lists of spectra and images, the path to a directory
             containing all files for a single JWST observation may be given.
+            If this is provided, all the above inputs are ignored.
 
         instrument : {'niriss', 'nircam', 'nirspec'}, optional
-            Required if ``directory`` is specified. Value is not case sensitive.
+            Required and only used if ``directory`` is specified. Value is not case sensitive.
         """
         # Link data after everything is loaded
         self.app.auto_link = False
         allow_link_table = True
 
-        directory = kwargs.pop('directory', None)
-        instrument = kwargs.pop('instrument', None)
-        if instrument is not None:
+        if isinstance(instrument, str):
             instrument = instrument.lower()
 
-        if directory is not None and Path(directory).is_dir():
-            if instrument not in ('nirspec', 'niriss', 'nircam'):
-                raise ValueError(
-                    "Ambiguous MOS Instrument: Only JWST NIRSpec, NIRCam, and "
-                    f"NIRISS folder parsing are currently supported but got '{instrument}'")
-            if instrument == "nirspec":
-                super().load_data(directory, parser_reference="mosviz-nirspec-directory-parser")
-            else:  # niriss or nircam
-                self.load_jwst_directory(directory, instrument=instrument)
-        elif directory is not None and is_zipfile(str(directory)):
-            raise TypeError("Please extract your data first and provide the directory")
+        if images is not None and not isinstance(images, (list, tuple)):
+            single_image = True
+        else:
+            single_image = False
+
+        if directory is not None:
+            if is_zipfile(str(directory)):
+                raise TypeError("Please extract your data first and provide the directory")
+            elif os.path.isdir(directory):
+                if instrument not in ('nirspec', 'niriss', 'nircam'):
+                    raise ValueError(
+                        "Ambiguous MOS Instrument: Only JWST NIRSpec, NIRCam, and "
+                        f"NIRISS folder parsing are currently supported but got '{instrument}'")
+                if instrument == "nirspec":
+                    super().load_data(directory, parser_reference="mosviz-nirspec-directory-parser")
+                else:  # niriss or nircam
+                    self.load_jwst_directory(directory, instrument=instrument)
+            else:
+                raise NotImplementedError(f"{directory} is not a directory")
+
+        # For the following, always load in this order: 1d, 2d, images, metadata
 
         elif (spectra_1d is not None and spectra_2d is not None
                 and images is not None):
-            # If we have a single image for multiple spectra, tell the table viewer
-            if not isinstance(images, (list, tuple)) and isinstance(spectra_1d, (list, tuple)):
+            n_specs = self.load_1d_spectra(spectra_1d, spectra_1d_label)
+            self.load_2d_spectra(spectra_2d, spectra_2d_label)
+
+            # If we have a single image for multiple spectra, tell the table viewer.
+            if single_image:
                 self._shared_image = True
                 self.app.get_viewer(self._default_table_viewer_reference_name)._shared_image = True
-                self.load_images(images, images_label, share_image=len(spectra_1d))
+                if n_specs > 1:
+                    self.load_images(images, images_label, share_image=n_specs)
+                else:
+                    self.load_images(images, images_label)
             else:
                 self.load_images(images, images_label)
 
-            self.load_2d_spectra(spectra_2d, spectra_2d_label)
-            self.load_1d_spectra(spectra_1d, spectra_1d_label)
             self.load_metadata()
 
         elif spectra_1d is not None and spectra_2d is not None:
             self.load_1d_spectra(spectra_1d, spectra_1d_label)
             self.load_2d_spectra(spectra_2d, spectra_2d_label)
             self.load_metadata()
 
         elif spectra_1d and images:
-            self.load_1d_spectra(spectra_1d, spectra_1d_label)
-            self.load_images(images, images_label)
+            n_specs = self.load_1d_spectra(spectra_1d, spectra_1d_label)
+
+            # If we have a single image for multiple spectra, tell the table viewer.
+            if single_image:
+                self._shared_image = True
+                self.app.get_viewer(self._default_table_viewer_reference_name)._shared_image = True
+                if n_specs > 1:
+                    self.load_images(images, images_label, share_image=n_specs)
+                else:
+                    self.load_images(images, images_label)
+            else:
+                self.load_images(images, images_label)
+
             allow_link_table = False
 
         elif spectra_2d and images:
-            self.load_2d_spectra(spectra_2d, spectra_2d_label)
-            self.load_images(images, images_label)
+            n_specs = self.load_2d_spectra(spectra_2d, spectra_2d_label)
+
+            # If we have a single image for multiple spectra, tell the table viewer.
+            if single_image:
+                self._shared_image = True
+                self.app.get_viewer(self._default_table_viewer_reference_name)._shared_image = True
+                if n_specs > 1:
+                    self.load_images(images, images_label, share_image=n_specs)
+                else:
+                    self.load_images(images, images_label)
+            else:
+                self.load_images(images, images_label)
+
             allow_link_table = False
 
         elif spectra_1d:
             self.load_1d_spectra(spectra_1d, spectra_1d_label)
             allow_link_table = False
 
         elif spectra_2d:
             self.load_2d_spectra(spectra_2d, spectra_2d_label)
             allow_link_table = False
 
         else:
-            self.app.hub.broadcast(SnackbarMessage(
-                "Warning: Please set valid values for the load_data() method",
-                color='warning', sender=self))
-            return
+            raise NotImplementedError("Please set valid values for the Mosviz.load_data() method")
 
         if allow_link_table:
             self.link_table_data(None)
 
         self._add_redshift_column()
 
         # Any subsequently added data will automatically be linked
@@ -530,16 +563,16 @@
             self._default_image_viewer_reference_name
         ).figure.axes[1].label_offset = "-50"
 
         # Load the first object into the viewers automatically
         self.app.get_viewer(self._default_table_viewer_reference_name).figure_widget.highlighted = 0
 
         # Notify the user that this all loaded successfully
-        loaded_msg = SnackbarMessage("MOS data loaded successfully", color="success", sender=self)
-        self.app.hub.broadcast(loaded_msg)
+        self.app.hub.broadcast(SnackbarMessage(
+            "MOS data loaded successfully", color="success", sender=self))
 
         self._default_visible_columns = self.get_column_names(True)
 
     def link_table_data(self, data_obj):
         """
         Batch link data in the Mosviz table rather than doing it on
         data load.
@@ -586,63 +619,84 @@
 
     def load_metadata(self):
         """
         Parse the internal meta for our expected information
         """
         self.app.load_data(file_obj=None, parser_reference="mosviz-metadata-parser")
 
-    def load_1d_spectra(self, data_obj, data_labels=None):
+    def load_1d_spectra(self, data_obj, data_labels=None, add_redshift_column=False):
         """
         Load and parse a set of 1D spectra objects.
 
         Parameters
         ----------
         data_obj : list or str
             A list of spectra as translatable container objects (e.g.
             ``Spectrum1D``) that can be read by glue-jupyter. Alternatively,
             can be a string file path.
         data_labels : str or list
             String representing the label for the data item loaded via
             ``data_obj``. Can be a list of strings representing data labels
             for each item in ``data_obj`` if  ``data_obj`` is a list.
+        add_redshift_column : bool
+            Add redshift column to Mosviz table.
+
+        Returns
+        -------
+        n_specs : int
+            Number of data objects loaded.
+
         """
-        super().load_data(data_obj, parser_reference="mosviz-spec1d-parser",
-                          data_labels=data_labels)
-        self._add_redshift_column()
+        n_specs = mos_spec1d_parser(self.app, data_obj, data_labels=data_labels)
+        if add_redshift_column:
+            self._add_redshift_column()
+        return n_specs
 
-    def load_2d_spectra(self, data_obj, data_labels=None):
+    def load_2d_spectra(self, data_obj, data_labels=None, add_redshift_column=False):
         """
         Load and parse a set of 2D spectra objects.
 
         Parameters
         ----------
         data_obj : list or str
             A list of 2D spectra as translatable container objects (e.g.
             ``Spectrum1D``) that can be read by glue-jupyter. Alternatively,
             can be a string file path.
         data_labels : str or list
             String representing the label for the data item loaded via
             ``data_obj``. Can be a list of strings representing data labels
             for each item in ``data_obj`` if  ``data_obj`` is a list.
-        """
-        super().load_data(data_obj, parser_reference="mosviz-spec2d-parser",
-                          data_labels=data_labels)
-        self._add_redshift_column()
+        add_redshift_column : bool
+            Add redshift column to Mosviz table.
 
-    def load_jwst_directory(self, data_obj, data_labels=None, instrument=None):
+        Returns
+        -------
+        n_specs : int
+            Number of data objects loaded.
+
+        """
+        n_specs = mos_spec2d_parser(self.app, data_obj, data_labels=data_labels)
+        if add_redshift_column:
+            self._add_redshift_column()
+        return n_specs
+
+    def load_jwst_directory(self, data_obj, data_labels=None, instrument=None,
+                            add_redshift_column=False):
+        """Load NIRISS or NIRCam data from a directory."""
         self.app.auto_link = False
         super().load_data(data_obj, parser_reference="mosviz-niriss-parser",
                           instrument=instrument)
 
         self.link_table_data(data_obj)
-        self._add_redshift_column()
+        if add_redshift_column:
+            self._add_redshift_column()
 
         self.app.auto_link = True
 
-    def load_images(self, data_obj, data_labels=None, share_image=0):
+    def load_images(self, data_obj, data_labels=None, share_image=0, add_redshift_column=False):
         """
         Load and parse a set of image objects. If providing a file path, it
         must be readable by ``astropy.io.fits``.
 
         Parameters
         ----------
         data_obj : list of obj, str, or `None`
@@ -655,18 +709,21 @@
             for each item in ``data_obj`` if  ``data_obj`` is a list.
         share_image : int, optional
             If 0, images are treated as applying to individual spectra. If non-zero,
             a single image will be shared by multiple spectra so that clicking a
             different row in the table does not reload the displayed image.
             Currently, if non-zero, the provided number must match the number of
             spectra.
+        add_redshift_column : bool
+            Add redshift column to Mosviz table.
         """
         super().load_data(data_obj, parser_reference="mosviz-image-parser",
                           data_labels=data_labels, share_image=share_image)
-        self._add_redshift_column()
+        if add_redshift_column:
+            self._add_redshift_column()
 
     def get_column_names(self, visible=None):
         """
         List the names of the columns in the table.
 
         Parameters
         ----------
@@ -1015,7 +1072,29 @@
             but raise a warning.
 
         Returns
         -------
         `~specutils.Spectrum1D`
         """
         return self._get_spectrum('2D Spectra', row, apply_slider_redshift)
+
+    def get_data(self, data_label=None, spectral_subset=None, cls=None):
+        """
+        Returns data with name equal to data_label of type cls with subsets applied from
+        spectral_subset.
+
+        Parameters
+        ----------
+        data_label : str, optional
+            Provide a label to retrieve a specific data set from data_collection.
+        spectral_subset : str, optional
+            Spectral subset applied to data.
+        cls : `~specutils.Spectrum1D`, `~astropy.nddata.CCDData`, optional
+            The type that data will be returned as.
+
+        Returns
+        -------
+        data : cls
+            Data is returned as type cls with subsets applied.
+
+        """
+        return self._get_data(data_label=data_label, spectral_subset=spectral_subset, cls=cls)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/mosviz.yaml` & `jdaviz-3.5.0/jdaviz/configs/mosviz/mosviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/parsers.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections.abc import Iterable
 import csv
-import glob
 import os
 from pathlib import Path
 import warnings
 
 from astropy import units as u
 from astropy.io import fits
 from astropy.io.registry import IORegistryError
@@ -150,46 +149,54 @@
 def mos_nirspec_directory_parser(app, data_obj, data_labels=None):
 
     spectra_1d = []
     spectra_2d = []
 
     # Load spectra
     level3_path = Path(data_obj)
-    for file_path in glob.iglob(str(level3_path / '*')):
+    for p in sorted(level3_path.glob('*.fits*')):
+        file_path = str(p)
         if 'x1d' in file_path or 'c1d' in file_path:
             spectra_1d.append(file_path)
         elif 's2d' in file_path:
             spectra_2d.append(file_path)
 
-    spectra_1d.sort()
-    spectra_2d.sort()
-    mos_spec1d_parser(app, spectra_1d)
+    n_specs = mos_spec1d_parser(app, spectra_1d)
     mos_spec2d_parser(app, spectra_2d)
 
     # Load images, if present
     image_path = None
 
     # Potential names of subdirectories where images are stored
-    for image_dir_name in ["cutouts", "mosviz_cutouts", "images"]:
-        if os.path.isdir(Path(str(level3_path / image_dir_name))):
-            image_path = Path(str(level3_path / image_dir_name))
+    for image_dir_name in ("cutouts", "mosviz_cutouts", "images"):
+        cur_path = level3_path / image_dir_name
+        if cur_path.is_dir():
+            image_path = cur_path
             break
     if image_path is not None:
-        images = sorted([file_path for file_path in glob.iglob(str(image_path / '*'))])
+        images = sorted(image_path.glob('*.fits*'))
+        n_images = len(images)
 
         # The amount of images needs to be equal to the amount of rows
         # of the other columns in the table
-        if len(images) == len(spectra_1d):
-            mos_image_parser(app, images)
+        if n_images == 1:
+            app._jdaviz_helper._shared_image = True
+            app.get_viewer(app._jdaviz_helper._default_table_viewer_reference_name)._shared_image = True  # noqa: E501
+            if n_specs > 1:
+                kwargs = {'share_image': n_specs}
+            else:
+                kwargs = {}
+            mos_image_parser(app, str(images[0]), **kwargs)
+        elif n_images == n_specs:
+            mos_image_parser(app, list(map(str, images)))
         else:
-            msg = ("The number of images in this directory does not match the"
-                   " number of spectra 1d and 2d files, please make the "
-                   "amounts equal or load images separately.")
-            msg = SnackbarMessage(msg, color='warning', sender=app)
-            app.hub.broadcast(msg)
+            app.hub.broadcast(SnackbarMessage(
+                "The number of images in this directory does not match the "
+                "number of spectra 1d and 2d files, please make the "
+                "amounts equal or load images separately.", color='warning', sender=app))
 
     mos_meta_parser(app)
 
 
 @data_parser_registry("mosviz-spec1d-parser")
 def mos_spec1d_parser(app, data_obj, data_labels=None,
                       table_viewer_reference_name='table-viewer'):
@@ -201,16 +208,21 @@
     app : `~jdaviz.app.Application`
         The application-level object used to reference the viewers.
     data_obj : str or list or spectrum-like
         File path, list, or spectrum-like object to be read as a new row in
         the mosviz table.
     data_labels : str, optional
         The label applied to the glue data component.
-    """
 
+    Returns
+    -------
+    n_specs : int
+        Number of data objects loaded.
+
+    """
     if isinstance(data_labels, str):
         data_labels = [data_labels]
 
     # Coerce into list if needed
     if not isinstance(data_obj, (list, tuple, SpectrumCollection)):
         data_obj = [data_obj]
 
@@ -265,14 +277,20 @@
         the mosviz table.
     data_labels : str, optional
         The label applied to the glue data component.
     ext : int, optional
         The extension in the FITS file that contains the data to be loaded.
     transpose : bool, optional
         Flag to transpose the data array before loading.
+
+    Returns
+    -------
+    n_specs : int
+        Number of data objects loaded.
+
     """
     spectrum_2d_viewer_reference_name = (
         app._jdaviz_helper._default_spectrum_2d_viewer_reference_name
     )
     table_viewer_reference_name = (
         app._jdaviz_helper._default_table_viewer_reference_name
     )
@@ -472,30 +490,44 @@
         table rows. Typically, a list with file names. Used in combination
         with data_obj for fallback
     """
 
     with app.data_collection.delay_link_manager_update():
 
         current_columns = [comp.label for comp in app.data_collection['MOS Table'].main_components]
+        has_1d = "1D Spectra" in current_columns
+
         # source name can be taken from 1d spectra
-        if "1D Spectra" in current_columns:
+        if has_1d:
             names = _get_source_identifiers(app, "1D Spectra", data_obj, ids)
             _add_to_table(app, names, "Identifier")
 
         # metadata taken from 2d spectra
         if "2D Spectra" in current_columns:
             filters = query_metadata_by_component(app, "FILTER", "2D Spectra", FALLBACK_NAME)
             gratings = query_metadata_by_component(app, "GRATING", "2D Spectra", FALLBACK_NAME)
 
             filters_gratings = [(f+'/'+g) for f, g in zip(filters, gratings)]
 
             _add_to_table(app, filters_gratings, "Filter/Grating")
 
-        # source name and coordinates are taken from image headers, if present
-        if "Images" in current_columns:
+        # Grab target sky coordinates from 1D spectrum, if possible.
+        # This has to happen after Filter/Grating because columns are insertion-ordered.
+        if has_1d:
+            ra = query_metadata_by_component(app, "SRCRA", "1D Spectra", False)
+            dec = query_metadata_by_component(app, "SRCDEC", "1D Spectra", False)
+            if all(ra) and all(dec):
+                _add_to_table(app, ra, "R.A.")
+                _add_to_table(app, dec, "Dec.")
+
+        # Refresh current_columns for Images check
+        current_columns = [comp.label for comp in app.data_collection['MOS Table'].main_components]
+
+        # If not in 1D spectrum, source coordinates are taken from image headers, if present.
+        if "R.A." not in current_columns and "Images" in current_columns:
             ra = query_metadata_by_component(app, "OBJ_RA", "Images", FALLBACK_NAME)
             dec = query_metadata_by_component(app, "OBJ_DEC", "Images", FALLBACK_NAME)
             _add_to_table(app, ra, "R.A.")
             _add_to_table(app, dec, "Dec.")
 
 
 def query_metadata_by_component(app, keys, data_type, fallback=FALLBACK_NAME):
@@ -662,15 +694,15 @@
     if catalog_key is None:
         raise ValueError("cat_key must be identified before parsing directory")
 
     for fp in filepaths:
         if fp.is_dir():
             # Potential names of subdirectories where images are stored
             if fp.name in ("cutouts", "mosviz_cutouts", "images"):
-                images = sorted([file_path for file_path in glob.iglob(str(fp / '*'))])
+                images = sorted(fp.glob('*.fits*'))
                 label_dict['Direct Image'] = images
             else:
                 continue
 
         if fp.suffix in ('.fits', '.fits.gz', '.fit', '.fit.gz'):
             # eligible files will have a DATAMODL value in their primary headers
             header = fits.getheader(fp, ext=0)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/row_lock/row_lock.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/slit_overlay/tests/test_slit_overlay.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/plugins/viewers.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/plugins/viewers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,77 @@
+from astropy.coordinates import SkyCoord
+from astropy.table import QTable
 from glue.core import BaseData
 from glue_jupyter.bqplot.image import BqplotImageView
 from glue_jupyter.table import TableViewer
 from specutils import Spectrum1D
 
 from jdaviz.core.events import (AddDataToViewerMessage,
                                 RemoveDataFromViewerMessage,
                                 TableClickMessage)
+from jdaviz.core.astrowidgets_api import AstrowidgetsImageViewerMixin
 from jdaviz.core.registries import viewer_registry
 from jdaviz.core.freezable_state import FreezableBqplotImageViewerState
 from jdaviz.configs.default.plugins.viewers import JdavizViewerMixin
 
 __all__ = ['MosvizImageView', 'MosvizProfile2DView',
            'MosvizTableViewer']
 
 
 @viewer_registry("mosviz-image-viewer", label="Image 2D (Mosviz)")
-class MosvizImageView(JdavizViewerMixin, BqplotImageView):
+class MosvizImageView(JdavizViewerMixin, BqplotImageView, AstrowidgetsImageViewerMixin):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
                     ['jdaviz:boxzoom'],
                     ['jdaviz:panzoom'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     default_class = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.init_astrowidgets_api()
         self._subscribe_to_layers_update()
 
+        self.state.show_axes = False  # Axes are wrong anyway
+        self.figure.fig_margin = {'left': 0, 'bottom': 0, 'top': 0, 'right': 0}
+
     def data(self, cls=None):
         return [layer_state.layer  # .get_object(cls=cls or self.default_class)
                 for layer_state in self.state.layers
                 if hasattr(layer_state, 'layer') and
                 isinstance(layer_state.layer, BaseData)]
 
-    def set_plot_axes(self):
-        self.figure.axes[1].tick_format = None
-        self.figure.axes[0].tick_format = None
-
-        self.figure.axes[1].label = "y: pixels"
-        self.figure.axes[0].label = "x: pixels"
-
-        # Make it so y axis label is not covering tick numbers.
-        self.figure.axes[1].label_offset = "-50"
+    # NOTE: This is currently only for debugging. It is not used in app.
+    def _mark_targets(self):
+        table_data = self.jdaviz_app.data_collection['MOS Table']
+
+        if ("R.A." not in table_data.component_ids() or
+                "Dec." not in table_data.component_ids()):
+            return
+
+        ra = table_data["R.A."]
+        dec = table_data["Dec."]
+        sky = SkyCoord(ra, dec, unit='deg')
+        t = QTable({'coord': sky})
+        self.add_markers(t, use_skycoord=True, marker_name='Targets')
 
 
 @viewer_registry("mosviz-profile-2d-viewer", label="Spectrum 2D (Mosviz)")
 class MosvizProfile2DView(JdavizViewerMixin, BqplotImageView):
     # Due to limitations in CCDData and 2D data that has spectral and spatial
     #  axes, the default conversion class must handle cubes
     default_class = Spectrum1D
 
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
-                    ['jdaviz:boxzoom', 'jdaviz:xrangezoom'],
+                    ['jdaviz:boxzoom', 'jdaviz:xrangezoom', 'jdaviz:yrangezoom'],
                     ['jdaviz:panzoom', 'jdaviz:panzoom_x'],
                     ['bqplot:xrange'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     _state_cls = FreezableBqplotImageViewerState
 
@@ -130,15 +141,15 @@
         # might be added inplace to the dataset.
 
         if self.figure_widget.data is None:
             self.figure_widget.hidden_components = []
         else:
             components_str = [cid.label for cid in self.figure_widget.data.main_components]
             hidden = []
-            for colname in ['Images', '1D Spectra', '2D Spectra']:
+            for colname in ('Images', '1D Spectra', '2D Spectra'):
                 if colname in components_str:
                     hidden.append(self.figure_widget.data.id[colname])
             self.figure_widget.hidden_components = hidden
 
         super().redraw()
 
     @property
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_data_loading.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_data_loading.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,17 @@
 
     assert isinstance(data[label], Spectrum1D)
 
     with pytest.raises(AttributeError):
         mosviz_helper.load_1d_spectra([1, 2, 3])
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_load_image(mosviz_helper, mos_image):
     label = "Test Image"
-    mosviz_helper.load_images(mos_image, data_labels=label)
+    mosviz_helper.load_images(mos_image, data_labels=label, add_redshift_column=True)
 
     assert len(mosviz_helper.app.data_collection) == 2
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == f"{label} 0"
     assert PRIHDR_KEY not in dc_1.meta
     assert dc_1.meta['RADESYS'] == 'ICRS'
@@ -51,15 +50,15 @@
     dataval = data[f"{label} 0"]
     assert isinstance(dataval, CCDData)
     assert dataval.shape == (55, 55)
 
 
 def test_load_spectrum_collection(mosviz_helper, spectrum_collection):
     labels = [f"Test Spectrum Collection {i}" for i in range(5)]
-    mosviz_helper.load_1d_spectra(spectrum_collection, data_labels=labels)
+    mosviz_helper.load_1d_spectra(spectrum_collection, data_labels=labels, add_redshift_column=True)
 
     # +1 for the table viewer
     assert len(mosviz_helper.app.data_collection) == len(spectrum_collection) + 1
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == labels[0]
     assert dc_1.meta['uncertainty_type'] == 'std'
@@ -72,15 +71,15 @@
     assert isinstance(data[labels[0]], Spectrum1D)
 
 
 def test_load_list_of_spectrum1d(mosviz_helper, spectrum1d):
     spectra = [spectrum1d] * 3
 
     labels = [f"Test Spectrum 1D {i}" for i in range(3)]
-    mosviz_helper.load_1d_spectra(spectra, data_labels=labels)
+    mosviz_helper.load_1d_spectra(spectra, data_labels=labels, add_redshift_column=True)
 
     assert len(mosviz_helper.app.data_collection) == 4
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
     dc_1 = mosviz_helper.app.data_collection[1]
     assert dc_1.label == labels[0]
     assert dc_1.meta['uncertainty_type'] == 'std'
 
@@ -88,15 +87,14 @@
     table.widget_table.vue_on_row_clicked(0)
 
     data = mosviz_helper.app.get_data_from_viewer('spectrum-viewer')
 
     assert isinstance(data[labels[0]], Spectrum1D)
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_load_mos_spectrum2d(mosviz_helper, mos_spectrum2d):
 
     label = "Test 2D Spectrum"
     mosviz_helper.load_data(spectra_2d=mos_spectrum2d, spectra_2d_label=label)
 
     assert len(mosviz_helper.app.data_collection) == 2
     assert mosviz_helper.app.data_collection[0].label == "MOS Table"
@@ -108,15 +106,14 @@
     table.widget_table.vue_on_row_clicked(0)
 
     data = mosviz_helper.app.get_data_from_viewer('spectrum-2d-viewer')
 
     assert data[label].shape == (1024, 15)
 
 
-@pytest.mark.filterwarnings('ignore')
 @pytest.mark.parametrize('label', [None, "Test Label"])
 def test_load_multi_image_spec(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d, label):
     spectra1d = [spectrum1d] * 3
     spectra2d = [mos_spectrum2d] * 3
     images = [mos_image] * 3
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=images, images_label=label)
@@ -165,15 +162,15 @@
     label_mouseover._viewer_mouse_event(image_viewer, {'event': 'mousemove',
                                                        'domain': {'x': 0, 'y': 0}})
     assert label_mouseover.as_text() == ('', '', '')
 
     # Test that loading is still possible after previous crash:
     # https://github.com/spacetelescope/jdaviz/issues/364
     with pytest.raises(ValueError, match="incompatible with the dimensions of this data:"):
-        mosviz_helper.load_data(spectra1d, spectra2d, images=[])
+        mosviz_helper.load_data(spectra1d, spectra2d, images=[mos_image, mos_image])
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=mos_image, images_label=label)
 
     assert mosviz_helper.app.get_viewer("table-viewer").figure_widget.highlighted == 0
     assert len(mosviz_helper.app.data_collection) == 8
 
     qtable = mosviz_helper.to_table()
@@ -208,30 +205,38 @@
     label_mouseover._viewer_mouse_event(image_viewer, {'event': 'mouseleave'})
     assert label_mouseover.as_text() == ('', '', '')
     assert label_mouseover.icon == ''
 
     label_mouseover._viewer_mouse_event(spec2d_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 10, 'y': 100}})
     assert label_mouseover.as_text() == ('Pixel x=00010.0 y=00100.0 Value +8.12986e-01', '', '')
-    assert label_mouseover.icon == 'b'
+    assert label_mouseover.icon == 'c'
 
     # need to trigger a mouseleave or mouseover to reset the traitlets
     label_mouseover._viewer_mouse_event(spec1d_viewer, {'event': 'mouseenter'})
     label_mouseover._viewer_mouse_event(spec1d_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 7000, 'y': 170}})
     assert label_mouseover.as_text() == ('Cursor 7.00000e+03, 1.70000e+02',
                                          'Wave 6.88889e+03 Angstrom (4 pix)',
                                          'Flux 1.35436e+01 Jy')
-    assert label_mouseover.icon == 'c'
+    assert label_mouseover.icon == 'b'
 
 
 def test_zip_error(mosviz_helper, tmp_path):
     '''
     Zipfiles are explicitly and intentionally not supported. This test confirms a TypeError is
     raised if the user tries to supply a Zipfile and expects Mosviz to autoextract.
     '''
     zip_path = tmp_path / "jdaviz_test_zip.zip"
     zip = ZipFile(zip_path, mode='w')
     zip.close()
 
     with pytest.raises(TypeError, match="Please extract"):
         mosviz_helper.load_data(directory=str(zip_path))
+
+
+def test_invalid_inputs(mosviz_helper):
+    with pytest.raises(NotImplementedError, match=r".*not a directory"):
+        mosviz_helper.load_data(directory="foo")
+
+    with pytest.raises(NotImplementedError, match="Please set valid values"):
+        mosviz_helper.load_data()
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_helper.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 
 import csv
 import pytest
 from numpy.testing import assert_allclose
 from jdaviz.configs.specviz2d.helper import Specviz2d
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_viewer_axis_link(mosviz_helper, mos_spectrum1d, mos_spectrum2d):
     label1d = "Test 1D Spectrum"
     mosviz_helper.load_1d_spectra(mos_spectrum1d, data_labels=label1d)
 
     label2d = "Test 2D Spectrum"
-    mosviz_helper.load_2d_spectra(mos_spectrum2d, data_labels=label2d)
+    mosviz_helper.load_2d_spectra(mos_spectrum2d, data_labels=label2d, add_redshift_column=True)
 
     table = mosviz_helper.app.get_viewer('table-viewer')
     table.widget_table.vue_on_row_clicked(0)
 
     scale_2d = mosviz_helper.app.get_viewer('spectrum-2d-viewer').scales['x']
     scale_1d = mosviz_helper.app.get_viewer('spectrum-viewer').scales['x']
 
@@ -26,15 +25,15 @@
 
     scale_1d.max = 7564
     assert scale_2d.max == 800.0
 
 
 def test_to_csv(tmp_path, mosviz_helper, spectrum_collection):
     labels = [f"Test Spectrum Collection {i}" for i in range(5)]
-    mosviz_helper.load_1d_spectra(spectrum_collection, data_labels=labels)
+    mosviz_helper.load_1d_spectra(spectrum_collection, data_labels=labels, add_redshift_column=True)
 
     mosviz_helper.to_csv(filename=str(tmp_path / "MOS_data.csv"))
 
     found_rows = 0
     found_index_label = False
 
     with open(tmp_path / "MOS_data.csv", "r") as f:
@@ -45,15 +44,14 @@
             else:
                 found_rows += 1
 
     assert found_index_label
     assert found_rows == 5
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_table_scrolling(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d):
     spectra1d = [spectrum1d] * 2
     spectra2d = [mos_spectrum2d] * 2
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=mos_image)
 
     table = mosviz_helper.app.get_viewer('table-viewer')
@@ -65,15 +63,14 @@
     table.next_row()
     # with only 2 rows, this should wrap back to 0
     assert table.widget_table.highlighted == 0
     table.prev_row()
     assert table.widget_table.highlighted == 1
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_column_visibility(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d):
     spectra1d = [spectrum1d] * 2
     spectra2d = [mos_spectrum2d] * 2
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=mos_image)
 
     with pytest.raises(
@@ -88,15 +85,14 @@
     mosviz_helper.show_column('Redshift')
     assert 'Redshift' in mosviz_helper.get_column_names(True)
 
     mosviz_helper.hide_column('Redshift')
     assert 'Redshift' not in mosviz_helper.get_column_names(True)
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_custom_columns(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d):
     spectra1d = [spectrum1d] * 2
     spectra2d = [mos_spectrum2d] * 2
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=mos_image)
 
     mosviz_helper.add_column('custom_name')
@@ -118,27 +114,27 @@
 
     mosviz_helper.show_column("Redshift")
     assert "Redshift" in mosviz_helper.get_column_names(True)
     mosviz_helper.set_visible_columns()
     assert "Redshift" not in mosviz_helper.get_column_names(True)
 
 
-@pytest.mark.filterwarnings('ignore')
 def test_redshift_column(mosviz_helper, mos_image, spectrum1d, mos_spectrum2d):
     spectra1d = [spectrum1d] * 2
     spectra2d = [mos_spectrum2d] * 2
 
     mosviz_helper.load_data(spectra1d, spectra2d, images=mos_image)
 
     mosviz_helper.update_column("Redshift", 0.1, row=0)
-    assert_allclose(list(mosviz_helper.specviz.get_spectra().values())[0].redshift.value, 0.1)
+    all_spectra = mosviz_helper.specviz.get_spectra(apply_slider_redshift=True)
+    assert_allclose(list(all_spectra.values())[0].redshift.value, 0.1)
     assert isinstance(mosviz_helper.specviz2d, Specviz2d)
-    assert_allclose(mosviz_helper.get_spectrum_1d().redshift.value, 0.1)
-    assert_allclose(mosviz_helper.get_spectrum_2d().redshift.value, 0.1)
-    assert_allclose(mosviz_helper.get_spectrum_1d(row=1).redshift.value, 0.0)
+    assert_allclose(mosviz_helper.get_spectrum_1d(apply_slider_redshift=True).redshift.value, 0.1)
+    assert_allclose(mosviz_helper.get_spectrum_2d(apply_slider_redshift=True).redshift.value, 0.1)
+    assert_allclose(mosviz_helper.get_spectrum_1d(apply_slider_redshift=True, row=1).redshift.value, 0.0)  # noqa: E501
 
 
 def test_plugin_user_apis(mosviz_helper):
     for plugin_name, plugin_api in mosviz_helper.plugins.items():
         plugin = plugin_api._obj
         for attr in plugin_api._expose:
             assert hasattr(plugin, attr)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_parsers.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import pytest
 from numpy.testing import assert_allclose
 from astropy.utils.data import download_file
 
 from jdaviz.utils import PRIHDR_KEY, COMMENTCARD_KEY
 
 
-@pytest.mark.filterwarnings('ignore')
 @pytest.mark.remote_data
 @pytest.mark.parametrize('instrument_arg', ('nirspec', None))
 def test_nirspec_parser(mosviz_helper, tmp_path, instrument_arg):
     '''
     Tests loading our default MosvizExample notebook data
     Also tests no instrument keyword fallback, and IntraRow linking
     '''
@@ -79,15 +78,14 @@
     assert mosviz_helper.app.data_collection[data_label].meta['mosviz_row'] != table.current_row
 
     with pytest.raises(NotImplementedError, match='Intra-row plotting not supported'):
         mosviz_helper.app.add_data_to_viewer(viewer_reference='spectrum-viewer',
                                              data_label=data_label)
 
 
-@pytest.mark.filterwarnings('ignore')
 @pytest.mark.remote_data
 def test_nirspec_level2_parser(mosviz_helper, tmp_path):
     '''
     Tests loading our default MosvizExample notebook data
     Also tests no instrument keyword fallback, and IntraRow linking
     '''
 
@@ -101,15 +99,14 @@
     data_dir = level3_path
     mosviz_helper.load_data(directory=data_dir, instrument='nirspec')
 
     assert len(mosviz_helper.app.data_collection) == 75
 
 
 @pytest.mark.remote_data
-@pytest.mark.filterwarnings('ignore', match="'(MJy/sr)^2' did not parse as fits unit")
 def test_niriss_parser(mosviz_helper, tmp_path):
     '''
     Tests loading a NIRISS dataset
     This data set is a shortened version of the ERS program GLASS (Program 1324)
     provided by Camilla Pacifici. This is in-flight, "real" JWST data
 
     The spectra are jw01324001001_15101_00001_nis
@@ -173,15 +170,14 @@
             assert int(spec1d.meta['mosviz_row']) == int(spec2d.meta['mosviz_row'])
 
             for spec in (spec1d, spec2d):
                 assert spec.meta['SOURCEID'] == sourceid
 
 
 @pytest.mark.remote_data
-@pytest.mark.filterwarnings('ignore', match="'(MJy/sr)^2' did not parse as fits unit")
 def test_nircam_parser(mosviz_helper, tmp_path):
     '''
     Tests loading a NIRCam dataset
     '''
 
     # Download data
     test_data = 'https://stsci.box.com/shared/static/itk7pav073nubwn58pig002m9796qzpw.zip'
@@ -212,16 +208,14 @@
 
     SRCTYPE is required for Mosviz. We do not want to rely on the JWST x1d parser's
     default behavior of overwriting with "POINT" if it doesn't exist, as all NIRISS data
     should have this populated; missing SRCTYPE indicates something went wrong.
 
     This dataset was our original simulated NIRISS dataset that is missing SRCTYPE.
 
-    NOTE: Under some conditions, a warning is raised when TemporaryDirectory attempts to
-    clean itself up. Most likely a race condition between TempDir and pytest
     '''
 
     # Download data
     test_data = 'https://stsci.box.com/shared/static/l2azhcqd3tvzhybdlpx2j2qlutkaro3z.zip'
     fn = download_file(test_data, cache=True, timeout=30)
 
     # Extract to a known, temporary folder
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py` & `jdaviz-3.5.0/jdaviz/configs/mosviz/tests/test_source_identifier_extract.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/helper.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
 
 from astropy import units as u
+from regions.core.core import Region
 from glue.core.subset_group import GroupedSubset
 from specutils import SpectralRegion, Spectrum1D
 
 from jdaviz.core.helpers import ConfigHelper
 from jdaviz.core.events import RedshiftMessage
 from jdaviz.configs.default.plugins.line_lists.line_list_mixin import LineListMixin
 
@@ -72,36 +73,45 @@
 
         """
         spectra = {}
         # Just to save line length
         get_data_method = self.app._jdaviz_helper.get_data
         viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
         function_kwargs = {'function': getattr(viewer.state, "function")} if self.app.config == 'cubeviz' else {}  # noqa
+        all_subsets = self.app.get_subsets(object_only=True)
 
         if data_label is not None:
             spectrum = get_data_method(data_label=data_label,
-                                       subset_to_apply=subset_to_apply,
+                                       spectral_subset=subset_to_apply,
                                        cls=Spectrum1D)
             spectra[data_label] = spectrum
         else:
             for layer_state in viewer.state.layers:
                 lyr = layer_state.layer
                 if subset_to_apply is not None:
                     if lyr.label == subset_to_apply:
                         spectrum = get_data_method(data_label=lyr.data.label,
-                                                   subset_to_apply=subset_to_apply,
+                                                   spectral_subset=subset_to_apply,
                                                    cls=Spectrum1D,
                                                    **function_kwargs)
                         spectra[lyr.data.label] = spectrum
                     else:
                         continue
                 else:
-                    if isinstance(lyr, GroupedSubset):
+                    if (isinstance(lyr, GroupedSubset) and lyr.label in all_subsets.keys() and
+                            isinstance(all_subsets[lyr.label][0], Region)):
                         spectrum = get_data_method(data_label=lyr.data.label,
-                                                   subset_to_apply=lyr.label,
+                                                   spatial_subset=lyr.label,
+                                                   cls=Spectrum1D,
+                                                   **function_kwargs)
+                        spectra[f'{lyr.data.label} ({lyr.label})'] = spectrum
+                    elif (isinstance(lyr, GroupedSubset) and lyr.label in all_subsets.keys() and
+                            isinstance(all_subsets[lyr.label], SpectralRegion)):
+                        spectrum = get_data_method(data_label=lyr.data.label,
+                                                   spectral_subset=lyr.label,
                                                    cls=Spectrum1D,
                                                    **function_kwargs)
                         spectra[f'{lyr.data.label} ({lyr.label})'] = spectrum
                     else:
                         spectrum = get_data_method(data_label=lyr.label,
                                                    cls=Spectrum1D,
                                                    **function_kwargs)
@@ -135,17 +145,15 @@
 
         Returns
         -------
         spec_regs : dict
             Mapping from the names of the subsets to the subsets expressed
             as `specutils.SpectralRegion` objects.
         """
-        return self.app.get_subsets_from_viewer(
-            self._default_spectrum_viewer_reference_name, subset_type="spectral"
-        )
+        return self.app.get_subsets(spectral_only=True)
 
     def x_limits(self, x_min=None, x_max=None):
         """Sets the limits of the x-axis
 
         Parameters
         ----------
         x_min
@@ -269,39 +277,49 @@
             return
 
         # Examples of values for fmt are '0.1e' or '0.2f'
         self.app.get_viewer(
             self._default_spectrum_viewer_reference_name
         ).figure.axes[axis].tick_format = fmt
 
-    def get_data(self, data_label=None, cls=None, subset_to_apply=None):
+    def get_data(self, data_label=None, spectral_subset=None, cls=None, **kwargs):
         """
         Returns data with name equal to data_label of type cls with subsets applied from
         subset_to_apply.
 
         Parameters
         ----------
         data_label : str, optional
             Provide a label to retrieve a specific data set from data_collection.
+        spectral_subset : str, optional
+            Spectral subset applied to data.
         cls : `~specutils.Spectrum1D`, optional
             The type that data will be returned as.
-        subset_to_apply : str, optional
-            Subset that is to be applied to data before it is returned.
 
         Returns
         -------
         data : cls
             Data is returned as type cls with subsets applied.
 
         """
+        spatial_subset = kwargs.pop("spatial_subset", None)
+        function = kwargs.pop("function", None)
+        if len(kwargs) > 0:
+            raise ValueError(f'kwargs {[x for x in kwargs.keys()]} are not valid')
+
         if self.app.config == 'cubeviz':
             # then this is a specviz instance inside cubeviz and we want to default to the
             # viewer's collapse function
             default_sp_viewer = self.app.get_viewer(self._default_spectrum_viewer_reference_name)
-            function = getattr(default_sp_viewer.state, 'function', None)
+            if function is True or function is None:
+                function = getattr(default_sp_viewer.state, 'function', None)
+
             if cls is None:
                 cls = Spectrum1D
+        elif spatial_subset or function:
+            raise ValueError('kwargs spatial subset and function are not valid in specviz')
         else:
+            spatial_subset = None
             function = None
 
-        return self._get_data(data_label=data_label, cls=cls, subset_to_apply=subset_to_apply,
-                              function=function)
+        return self._get_data(data_label=data_label, spatial_subset=spatial_subset,
+                              spectral_subset=spectral_subset, function=function, cls=cls)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,21 +326,21 @@
         spectral_axis = full_spectrum.spectral_axis
 
         if self.continuum_subset_selected == self.spectral_subset_selected:
             # already raised a validation error in the UI
             self.update_results(None)
             return
 
-        sr = self.app.get_subsets_from_viewer(self._default_spectrum_viewer_reference_name,
-                                              subset_type="spectral").get(self.spectral_subset_selected) # noqa
-
+        sr = self.app.get_subsets().get(self.spectral_subset_selected)
         if self.spectral_subset_selected == "Entire Spectrum":
             spectrum = full_spectrum
         else:
             spectrum = extract_region(full_spectrum, sr, return_single_spectrum=True)
+            sr_lower = spectrum.spectral_axis[spectrum.spectral_axis.value >= sr.lower.value][0]
+            sr_upper = spectrum.spectral_axis[spectrum.spectral_axis.value <= sr.upper.value][-1]
 
         # compute continuum
         if self.continuum_subset_selected == "Surrounding" and self.spectral_subset_selected == "Entire Spectrum": # noqa
             # we know we'll just use the endpoints, so let's be efficient and not even
             # try extracting from the region
             continuum_mask = np.array([0, len(spectral_axis)-1])
             mark_x = {'left': np.array([]),
@@ -351,63 +351,61 @@
             # self.spectral_subset_selected != "Entire Spectrum"
             if self.width > 10 or self.width < 1:
                 # DEV NOTE: if changing the limits, make sure to also update the form validation
                 # rules in line_analysis.vue
                 self.update_results(None)
                 return
 
-            spectral_region_width = sr.upper - sr.lower
+            spectral_region_width = sr_upper - sr_lower
             # convert width from total relative width, to width per "side"
             width = (self.width - 1) / 2
-            left, = np.where((spectral_axis < sr.lower) &
-                             (spectral_axis > sr.lower - spectral_region_width*width))
-
+            left, = np.where((spectral_axis < sr_lower) &
+                             (spectral_axis > sr_lower - spectral_region_width*width))
             if not len(left):
                 # then no points matching the width are available outside the line region,
                 # so we'll default to the left-most point of the line region.
                 left, = np.where(spectral_axis == min(spectrum.spectral_axis))
 
-            right, = np.where((spectral_axis > sr.upper) &
-                              (spectral_axis < sr.upper + spectral_region_width*width))
-
+            right, = np.where((spectral_axis > sr_upper) &
+                              (spectral_axis < sr_upper + spectral_region_width*width))
             if not len(right):
                 # then no points matching the width are available outside the line region,
                 # so we'll default to the right-most point of the line region.
                 right, = np.where(spectral_axis == max(spectrum.spectral_axis))
 
             continuum_mask = np.concatenate((left, right))
-            mark_x = {'left': np.array([min(spectral_axis.value[continuum_mask]), sr.lower.value]),
-                      'center': np.array([sr.lower.value, sr.upper.value]),
-                      'right': np.array([sr.upper.value, max(spectral_axis.value[continuum_mask])])}
+            mark_x = {'left': np.array([min(spectral_axis.value[continuum_mask]), sr_lower.value]),
+                      'center': np.array([sr_lower.value, sr_upper.value]),
+                      'right': np.array([sr_upper.value, max(spectral_axis.value[continuum_mask])])}
 
         else:
             # we'll access the mask of the continuum and then apply that to the spectrum.  For a
             # spatially-collapsed spectrum in cubeviz, this will access the mask from the full
             # cube, but still apply that to the spatially-collapsed spectrum.
             continuum_mask = ~self._specviz_helper.get_data(
                 self.dataset.selected,
-                subset_to_apply=self.continuum_subset_selected).mask
+                spectral_subset=self.continuum_subset_selected).mask
             spectral_axis_nanmasked = spectral_axis.value.copy()
             spectral_axis_nanmasked[~continuum_mask] = np.nan
             if self.spectral_subset_selected == "Entire Spectrum":
                 mark_x = {'left': spectral_axis_nanmasked,
                           'center': spectral_axis.value,
                           'right': []}
             else:
-                mark_x = {'left': spectral_axis_nanmasked[spectral_axis.value < sr.lower.value],
-                          'right': spectral_axis_nanmasked[spectral_axis.value > sr.upper.value]}
+                mark_x = {'left': spectral_axis_nanmasked[spectral_axis.value < sr_lower.value],
+                          'right': spectral_axis_nanmasked[spectral_axis.value > sr_upper.value]}
                 # Center should extend (at least) across the line region between the full
                 # range defined by the continuum subset(s).
                 # OK for mark_x to be all NaNs.
                 with warnings.catch_warnings():
                     warnings.simplefilter('ignore', category=RuntimeWarning)
                     mark_x_min = np.nanmin(mark_x['left'])
                     mark_x_max = np.nanmax(mark_x['right'])
-                left_min = np.nanmin([mark_x_min, sr.lower.value])
-                right_max = np.nanmax([mark_x_max, sr.upper.value])
+                left_min = np.nanmin([mark_x_min, sr_lower.value])
+                right_max = np.nanmax([mark_x_max, sr_upper.value])
                 mark_x['center'] = np.array([left_min, right_max])
 
         continuum_x = spectral_axis[continuum_mask].value
         min_x = min(spectral_axis.value)
         continuum_y = full_spectrum.flux[continuum_mask].value
         # DEV NOTE: could replace this with internal calls to the model fitting infrastructure
         # to enable other model-types and to give visual feedback (by labeling the model
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/line_analysis.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_line_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,12 +423,12 @@
     assert plugin.dataset == 'right_spectrum'
     assert plugin.spectral_subset == 'Entire Spectrum'
     assert plugin._obj.spectral_subset_valid
 
     plugin.spectral_subset = 'Subset 1'
     assert not plugin._obj.spectral_subset_valid
 
-    with pytest.raises(ValueError, match=r"spectral subset 'Subset 1' \(5000.0, 5888.888888888889\) is outside data range of 'right_spectrum' \(6000.0, 8000.0\)"):  # noqa
+    with pytest.raises(ValueError, match=r"spectral subset 'Subset 1' \(5000.0, 6000.0\) is outside data range of 'right_spectrum' \(6000.0, 8000.0\)"):  # noqa
         plugin.get_results()
 
     plugin.dataset = 'left_spectrum'
     assert plugin._obj.spectral_subset_valid
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/line_analysis/tests/test_lineflux.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/parsers.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/tests/test_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/unit_conversion/unit_conversion.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/plugins/viewers.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/plugins/viewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @viewer_registry("specviz-profile-viewer", label="Profile 1D (Specviz)")
 class SpecvizProfileView(JdavizViewerMixin, BqplotProfileView):
     # categories: zoom resets, zoom, pan, subset, select tools, shortcuts
     tools_nested = [
                     ['jdaviz:homezoom', 'jdaviz:prevzoom'],
-                    ['jdaviz:boxzoom', 'jdaviz:xrangezoom'],
+                    ['jdaviz:boxzoom', 'jdaviz:xrangezoom', 'jdaviz:yrangezoom'],
                     ['jdaviz:panzoom', 'jdaviz:panzoom_x', 'jdaviz:panzoom_y'],
                     ['bqplot:xrange'],
                     ['jdaviz:selectline'],
                     ['jdaviz:sidebar_plot', 'jdaviz:sidebar_export']
                 ]
 
     default_class = Spectrum1D
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/specviz.yaml` & `jdaviz-3.5.0/jdaviz/configs/specviz/specviz.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz/tests/test_helper.py` & `jdaviz-3.5.0/jdaviz/configs/specviz/tests/test_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from zipfile import ZipFile
 
 import numpy as np
 import pytest
 from astropy import units as u
 from astropy.tests.helper import assert_quantity_allclose
 from glue.core.roi import XRangeROI
-from glue.core.edit_subset_mode import OrMode
+from glue.core.edit_subset_mode import OrMode, AndMode, AndNotMode
 from specutils import Spectrum1D, SpectrumList, SpectrumCollection
 from astropy.utils.data import download_file
 
 from jdaviz.app import Application
 from jdaviz.configs.specviz.plugins.unit_conversion import unit_conversion as uc
 from jdaviz.core.marks import LineUncertainties
 from jdaviz import Specviz
@@ -132,36 +132,97 @@
         spec_region = self.spec_app.get_spectral_regions()
 
         assert len(spec_region['Subset 1'].subregions) == 3
         # Assert correct values for test with 3 subregions
         assert_quantity_allclose(spec_region['Subset 1'].subregions[0][0].value,
                                  6000., atol=1e-5)
         assert_quantity_allclose(spec_region['Subset 1'].subregions[0][1].value,
-                                 6222.22222222, atol=1e-5)
+                                 6400., atol=1e-5)
 
         assert_quantity_allclose(spec_region['Subset 1'].subregions[1][0].value,
-                                 6666.66666667, atol=1e-5)
+                                 6600., atol=1e-5)
         assert_quantity_allclose(spec_region['Subset 1'].subregions[1][1].value,
-                                 6888.88888889, atol=1e-5)
+                                 7000., atol=1e-5)
 
         assert_quantity_allclose(spec_region['Subset 1'].subregions[2][0].value,
-                                 7333.33333333, atol=1e-5)
+                                 7300., atol=1e-5)
         assert_quantity_allclose(spec_region['Subset 1'].subregions[2][1].value,
-                                 7777.77777778, atol=1e-5)
+                                 7800., atol=1e-5)
 
-    def test_get_spectral_regions_raise_value_error(self):
-        with pytest.raises(ValueError):
-            spectrum_viewer = self.spec_app.app.get_viewer("spectrum-viewer")
-
-            spectrum_viewer.session.edit_subset_mode._mode = OrMode
-            # Selecting ROIs that are not part of the actual spectrum raises an error
-            self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(1, 3))
-            self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(4, 6))
+    def test_get_spectral_regions_does_not_raise_value_error(self):
+        spectrum_viewer = self.spec_app.app.get_viewer("spectrum-viewer")
+
+        spectrum_viewer.session.edit_subset_mode._mode = OrMode
+        # Selecting ROIs that are not part of the actual spectrum no longer raises an error
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(1, 3))
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(4, 6))
+
+        spec_region = self.spec_app.get_spectral_regions()
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[0][0].value,
+                                 1, atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[0][1].value,
+                                 3, atol=1e-5)
+
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[1][0].value,
+                                 4, atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[1][1].value,
+                                 6, atol=1e-5)
+
+    def test_get_spectral_regions_composite_region(self):
+        spectrum_viewer = self.spec_app.app.get_viewer("spectrum-viewer")
+
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6000, 7400))
+
+        spectrum_viewer.session.edit_subset_mode._mode = AndNotMode
+
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6600, 7000))
+
+        spectrum_viewer.session.edit_subset_mode._mode = AndMode
+
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(7300, 7800))
+
+        spec_region = self.spec_app.get_spectral_regions()
+
+        assert len(spec_region['Subset 1'].subregions) == 1
+        # Assert correct values for test with 3 subregions
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[0][0].value,
+                                 7300., atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[0][1].value,
+                                 7400., atol=1e-5)
+
+    def test_get_spectral_regions_composite_region_multiple_and_nots(self):
+        spectrum_viewer = self.spec_app.app.get_viewer("spectrum-viewer")
+
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6000, 7800))
+
+        spectrum_viewer.session.edit_subset_mode._mode = AndNotMode
+
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6200, 6600))
+
+        spectrum_viewer.session.edit_subset_mode._mode = AndNotMode
+
+        self.spec_app.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(7300, 7700))
+
+        spec_region = self.spec_app.get_spectral_regions()
+
+        assert len(spec_region['Subset 1'].subregions) == 3
+        # Assert correct values for test with 3 subregions
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[0][0].value,
+                                 6000., atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[0][1].value,
+                                 6200., atol=1e-5)
 
-            self.spec_app.get_spectral_regions()
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[1][0].value,
+                                 6600., atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[1][1].value,
+                                 7300., atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[2][0].value,
+                                 7700., atol=1e-5)
+        assert_quantity_allclose(spec_region['Subset 1'].subregions[2][1].value,
+                                 7800., atol=1e-5)
 
 
 def test_get_spectra_no_spectra(specviz_helper, spectrum1d):
     with pytest.warns(UserWarning, match='Applying the value from the redshift slider'):
         spectra = specviz_helper.get_spectra()
 
     assert spectra == {}
@@ -196,16 +257,16 @@
     # Ensure units we put in are the same as the units we get out
     specviz_helper.load_spectrum(spectrum1d)
     specviz_helper.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(6200, 7000))
 
     subsets = specviz_helper.get_spectral_regions()
     reg = subsets.get('Subset 1')
 
-    assert spectrum1d.wavelength.unit == reg.lower.unit
-    assert spectrum1d.wavelength.unit == reg.upper.unit
+    assert spectrum1d.spectral_axis.unit == reg.lower.unit
+    assert spectrum1d.spectral_axis.unit == reg.upper.unit
 
 
 def test_get_spectral_regions_unit_conversion(specviz_helper, spectrum1d):
     spec_viewer = specviz_helper.app.get_viewer('spectrum-viewer')
 
     # Mouseover without data should not crash.
     label_mouseover = specviz_helper.app.session.application._tools['g-coords-info']
@@ -242,20 +303,21 @@
     specviz_helper.app.add_data(converted_spectrum, "Converted Spectrum")
     specviz_helper.app.add_data_to_viewer("spectrum-viewer",
                                           "Converted Spectrum",
                                           clear_other_data=True)
 
     specviz_helper.app.get_viewer("spectrum-viewer").apply_roi(XRangeROI(0.6, 0.7))
 
+    # TODO: Is this test still relevant with the upcoming glue unit conversion changes?
     # Retrieve the Subset
-    subsets = specviz_helper.get_spectral_regions()
-    reg = subsets.get('Subset 1')
-
-    assert reg.lower.unit == u.Unit(new_spectral_axis)
-    assert reg.upper.unit == u.Unit(new_spectral_axis)
+    # subsets = specviz_helper.get_spectral_regions()
+    # reg = subsets.get('Subset 1')
+    #
+    # assert reg.lower.unit == u.Unit(new_spectral_axis)
+    # assert reg.upper.unit == u.Unit(new_spectral_axis)
 
     # Coordinates info panel should show new unit
     label_mouseover._viewer_mouse_event(spec_viewer,
                                         {'event': 'mousemove', 'domain': {'x': 0.61, 'y': 12.5}})
     label_mouseover.as_text() == ('Cursor 6.10000e-01, 1.25000e+01',
                                   'Wave 6.00000e-01 micron (0 pix)',
                                   'Flux 1.24967e+01 Jy')
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/helper.py` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -234,7 +234,29 @@
             Whether to load into the spectrum-2d-viewer.
         """
         self.app.add_data(trace, data_label=data_label)
         if show_in_viewer:
             self.app.add_data_to_viewer(
                 self._default_spectrum_2d_viewer_reference_name, data_label
             )
+
+    def get_data(self, data_label=None, spectral_subset=None, cls=None):
+        """
+        Returns data with name equal to data_label of type cls with subsets applied from
+        spectral_subset.
+
+        Parameters
+        ----------
+        data_label : str, optional
+            Provide a label to retrieve a specific data set from data_collection.
+        spectral_subset : str, optional
+            Spectral subset applied to data.
+        cls : `~specutils.Spectrum1D`, `~astropy.nddata.CCDData`, optional
+            The type that data will be returned as.
+
+        Returns
+        -------
+        data : cls
+            Data is returned as type cls with subsets applied.
+
+        """
+        return self._get_data(data_label=data_label, spectral_subset=spectral_subset, cls=cls)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/parsers.py` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/spectral_extraction.vue`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/plugins/spectral_extraction/tests/test_spectral_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
     pext.export_bg_sub(add_data=True)
     assert 'override label 2' in pext.ext_dataset.choices
 
     # test setting auto label
     pext.bg_sub_add_results.auto = True
 
 
+@pytest.mark.skip(reason='filenames changed')
 @pytest.mark.remote_data
 @pytest.mark.skipif(GWCS_LT_0_18_1, reason='Needs GWCS 0.18.1 or later')
 def test_spectrum_on_top(specviz2d_helper):
     fn = download_file('https://mast.stsci.edu/api/v0.1/Download/file/?uri=mast:jwst/product/jw01529-o004_t002_miri_p750l_s2d.fits', cache=True)  # noqa
 
     specviz2d_helper.load_data(spectrum_2d=fn)
```

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/specviz2d.yaml` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/specviz2d.yaml`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/tests/test_helper.py` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/configs/specviz2d/tests/test_parsers.py` & `jdaviz-3.5.0/jdaviz/configs/specviz2d/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/conftest.py` & `jdaviz-3.5.0/jdaviz/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,32 +175,43 @@
                                 uncertainty=uncertainty, meta=meta)
 
         sc.append(spectrum1d)
 
     return SpectrumList(sc)
 
 
-def _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, shape=(2, 2, 4)):
+def _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, shape=(2, 2, 4), with_uncerts=False):
 
     flux = np.arange(np.prod(shape)).reshape(shape) * fluxunit
     wcs_dict = {"CTYPE1": "RA---TAN", "CTYPE2": "DEC--TAN", "CTYPE3": "WAVE-LOG",
                 "CRVAL1": 205, "CRVAL2": 27, "CRVAL3": 4.622e-7,
                 "CDELT1": -0.0001, "CDELT2": 0.0001, "CDELT3": 8e-11,
                 "CRPIX1": 0, "CRPIX2": 0, "CRPIX3": 0}
     w = WCS(wcs_dict)
+    if with_uncerts:
+        uncert = StdDevUncertainty(np.abs(np.random.normal(flux) * u.Jy))
 
-    return Spectrum1D(flux=flux, wcs=w)
+        return Spectrum1D(flux=flux,
+                          uncertainty=uncert,
+                          wcs=w)
+    else:
+        return Spectrum1D(flux=flux, wcs=w)
 
 
 @pytest.fixture
 def spectrum1d_cube():
     return _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy)
 
 
 @pytest.fixture
+def spectrum1d_cube_with_uncerts():
+    return _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, with_uncerts=True)
+
+
+@pytest.fixture
 def spectrum1d_cube_larger():
     return _create_spectrum1d_cube_with_fluxunit(fluxunit=u.Jy, shape=(SPECTRUM_SIZE, 2, 4))
 
 
 @pytest.fixture
 def spectrum1d_cube_custom_fluxunit():
     return _create_spectrum1d_cube_with_fluxunit
@@ -306,9 +317,10 @@
     PYTEST_HEADER_MODULES['ipysplitpanes'] = 'ipysplitpanes'
     PYTEST_HEADER_MODULES['ipygoldenlayout'] = 'ipygoldenlayout'
     PYTEST_HEADER_MODULES['voila'] = 'voila'
     PYTEST_HEADER_MODULES['vispy'] = 'vispy'
     PYTEST_HEADER_MODULES['gwcs'] = 'gwcs'
     PYTEST_HEADER_MODULES['asdf'] = 'asdf'
     PYTEST_HEADER_MODULES['stdatamodels'] = 'stdatamodels'
+    PYTEST_HEADER_MODULES['roman_datamodels'] = 'roman_datamodels'
 
     TESTED_VERSIONS['jdaviz'] = __version__
```

### Comparing `jdaviz-3.4.0/jdaviz/container.vue` & `jdaviz-3.5.0/jdaviz/container.vue`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,27 @@
       :stack="child"
       :key="index"
       :data_items="data_items"
       :app_settings="app_settings"
       :icons="icons"
       :viewer_icons="viewer_icons"
       :layer_icons="layer_icons"
-      @resize="$emit('resize')"
+      @resize="(e) => $emit('resize', e)"
       :closefn="closefn"
       @data-item-visibility="$emit('data-item-visibility', $event)"
       @data-item-unload="$emit('data-item-unload', $event)"
       @data-item-remove="$emit('data-item-remove', $event)"
       @call-viewer-method="$emit('call-viewer-method', $event)"
     ></g-viewer-tab>
     <gl-component
       v-for="(viewer, index) in stack.viewers"
       :key="viewer.id"
-      :title="viewer.config === 'cubeviz' ? viewer.reference : viewer.id"
+      :title="viewer.reference || viewer.id"
       :tab-id="viewer.id"
-      @resize="$emit('resize')"
+      @resize="(e) => $emit('resize', e)"
       @destroy="destroy($event, viewer.id)"
       style="display: flex; flex-flow: column; height: 100%; overflow-y: auto; overflow-x: hidden"
     >
         <div>
           <v-row dense style="background-color: #205f76; margin: 0px" class="jdaviz-viewer-toolbar">
             <j-viewer-data-select
               :data_items="data_items" 
@@ -54,15 +54,15 @@
             <j-play-pause-widget v-if="viewer.reference == 'table-viewer'" @event="$emit('call-viewer-method', {'id': viewer.id, 'method': 'next_row'})"></j-play-pause-widget>
             <v-spacer></v-spacer>
             <jupyter-widget class='jdaviz-nested-toolbar' :widget="viewer.toolbar"></jupyter-widget>
           </v-row>
 
         </div>
 
-        <v-card tile flat style="flex: 1; margin-top: -2px; overflow-y: hidden;">
+        <v-card tile flat style="flex: 1; margin-top: -2px; overflow: hidden;">
           <div v-if="app_settings.viewer_labels" class='viewer-label-container'>
             <div v-if="Object.keys(viewer_icons).length > 1" class="viewer-label invert-if-dark">
               <j-tooltip span_style="white-space: nowrap">
                 <j-layer-viewer-icon span_style="float: right;" :icon="viewer_icons[viewer.id]"></j-layer-viewer-icon>
               </j-tooltip>
               <span class="invert-if-dark" style="margin-left: 24px; margin-right: 32px; line-height: 24px">{{viewer.reference || viewer.id}}</span>
             </div>
@@ -76,15 +76,19 @@
                   {{layer_info.prefix_icon}}
                 </v-icon>
                 {{layer_name}}{{layer_info.suffix_label}}
               </span>
             </div>
           </div>
 
-          <jupyter-widget :widget="viewer.widget" style="width: 100%; height: 100%"></jupyter-widget>
+          <jupyter-widget
+            :widget="viewer.widget"
+            :ref="'viewer-widget-'+viewer.id"
+            :style="'width: 100%; height: 100%; overflow: hidden; transform: rotateY('+viewer_rotateY(viewer.canvas_flip_horizontal)+') rotate('+viewer.canvas_angle+'deg)'"
+          ></jupyter-widget>
         </v-card>
     </gl-component>
   </component>
 </template>
 
 <style>
 .viewer-label-container {
@@ -107,34 +111,50 @@
 }
 .viewer-label:hover {
   background-color: #e5e5e5;
   width: auto;
   border-bottom-left-radius: 4px; 
   border-top-left-radius: 4px;
 }
+.imviz div.v-card.v-card--flat.v-sheet.v-sheet--tile {
+  /* black background beyond edges of canvas for canvas rotation */
+  background-color: black
+}
 </style>
 
 <script>
 module.exports = {
   name: "g-viewer-tab",
   props: ["stack", "data_items", "closefn", "app_settings", "icons", "viewer_icons", "layer_icons"],
   created() {
     this.$parent.childMe = () => {
       return this.$children[0];
     };
   },
+  watch: {
+    stack(new_stack, old_stack) {
+      this.$emit('resize')
+    }
+  },
   methods: {
     computeChildrenPath() {
       return this.$parent.computeChildrenPath();
     },
     destroy(source, viewerId) {
       /* There seems to be no close event provided by vue-golden-layout, so we can't distinguish
        * between a user closing a tab or a re-render. However, when the user closes a tab, the
        * source of the event is a vue component. We can use that distinction as a close signal. */
       source.$root && this.closefn(viewerId);
+    },
+    viewer_rotateY(canvas_flip_horizontal) {
+      if (canvas_flip_horizontal) {
+        return '180deg'
+      } else {
+        return '0deg'
+      }
     }
   },
   computed: {
     parentMe() {
       return this.$parent;
     },
     childMe() {
```

### Comparing `jdaviz-3.4.0/jdaviz/core/astrowidgets_api.py` & `jdaviz-3.5.0/jdaviz/core/astrowidgets_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import gwcs
 import numpy as np
+import os
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.wcs import NoConvergence
 from echo import delay_callback
 from glue.config import colormaps
 from glue.core import Data
 
@@ -33,18 +34,32 @@
         # Markers
         self._marktags = set()
         self._default_mark_tag_name = 'default-marker-name'
         # marker shape not settable: https://github.com/glue-viz/glue/issues/2202
         self.marker = {'color': 'red', 'alpha': 1.0, 'markersize': 5}
 
     def save(self, filename):
-        """Save out the current image view to given PNG filename."""
+        """Save out the current image view to given PNG filename.
+
+        Parameters
+        ----------
+        filename : str
+            PNG filename. If the given file already exists, it will be
+            silently overwritten.
+
+        """
         if not filename.lower().endswith('.png'):
             filename = filename + '.png'
-        self.figure.save_png(filename=filename)
+
+        # https://github.com/bqplot/bqplot/pull/1397
+        def on_png_received(data):
+            with open(os.path.expanduser(filename), 'bw') as f:
+                f.write(data)
+
+        self.figure.get_png_data(on_png_received)
 
     def center_on(self, point):
         """Centers the view on a particular point on the top visible layer.
         The data label of the top visible layer can be queried using the viewer's
         `~jdaviz.configs.imviz.plugins.viewers.ImvizImageView.top_visible_data_label`
         property.
```

### Comparing `jdaviz-3.4.0/jdaviz/core/config.py` & `jdaviz-3.5.0/jdaviz/core/config.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/custom_traitlets.py` & `jdaviz-3.5.0/jdaviz/core/custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/events.py` & `jdaviz-3.5.0/jdaviz/core/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __all__ = ['NewViewerMessage', 'ViewerAddedMessage', 'ViewerRemovedMessage', 'LoadDataMessage',
            'AddDataMessage', 'SnackbarMessage', 'RemoveDataMessage',
            'AddLineListMessage', 'RowLockMessage',
            'SliceSelectSliceMessage',
            'SliceToolStateMessage',
            'TableClickMessage', 'LinkUpdatedMessage', 'ExitBatchLoadMessage',
-           'MarkersChangedMessage']
+           'MarkersChangedMessage', 'CanvasRotationChangedMessage']
 
 
 class NewViewerMessage(Message):
     """Message to trigger viewer creation in the application."""
     def __init__(self, cls, data, x_attr=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -312,7 +312,28 @@
     def __init__(self, has_markers, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._has_markers = has_markers
 
     @property
     def has_markers(self):
         return self._has_markers
+
+
+class CanvasRotationChangedMessage(Message):
+    '''Message generated by canvas rotation plugin'''
+    def __init__(self, viewer_id, angle, flip_horizontal, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._viewer_id = viewer_id
+        self._angle = angle
+        self._flip_horizontal = flip_horizontal
+
+    @property
+    def viewer_id(self):
+        return self._viewer_id
+
+    @property
+    def angle(self):
+        return self._angle
+
+    @property
+    def flip_horizontal(self):
+        return self._flip_horizontal
```

### Comparing `jdaviz-3.4.0/jdaviz/core/freezable_state.py` & `jdaviz-3.5.0/jdaviz/core/freezable_state.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/helpers.py` & `jdaviz-3.5.0/jdaviz/core/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 from contextlib import contextmanager
 from inspect import isclass
 
 import numpy as np
 import astropy.units as u
 from astropy.wcs.wcsapi import BaseHighLevelWCS
 from astropy.nddata import CCDData
+from regions.core.core import Region
 from glue.core import HubListener
 from glue.core.edit_subset_mode import NewMode
 from glue.core.message import SubsetCreateMessage, SubsetDeleteMessage
 from glue.core.subset import Subset, MaskSubsetState
 from glue.config import data_translator
 from ipywidgets.widgets import widget_serialization
-from specutils import Spectrum1D
+from specutils import Spectrum1D, SpectralRegion
 
 
 from jdaviz.app import Application
 from jdaviz.core.events import SnackbarMessage, ExitBatchLoadMessage
 from jdaviz.core.template_mixin import show_widget
 
 __all__ = ['ConfigHelper', 'ImageConfigHelper']
@@ -227,25 +228,31 @@
         if models and model_label:
             models = self.get_models(models=models, model_label=model_label, x=x, y=y)
         elif models is None and model_label:
             models = self.get_models(model_label=model_label, x=x, y=y)
         elif models is None:
             models = self.fitted_models
 
+        data_shapes = {}
+        for label in models:
+            data_label = label.split(" (")[0]
+            if data_label not in data_shapes:
+                data_shapes[data_label] = self.app.data_collection[data_label].data.shape
+
         param_dict = {}
         parameters_cube = {}
         param_x_y = {}
         param_units = {}
 
         for label in models:
             # 3d models take the form of "Model (1,2)" so this if statement
             # looks for that style and separates out the pertinent information.
             if " (" in label:
                 label_split = label.split(" (")
-                model_name = label_split[0] + "_3d"
+                model_name = label_split[0]
                 x = int(label_split[1].split(", ")[0])
                 y = int(label_split[1].split(", ")[1][:-1])
 
                 # x and y values are added to this dict where they will be used
                 # to convert the models of each spaxel into a single
                 # coordinate in the parameters_cube dictionary.
                 if model_name not in param_x_y:
@@ -264,29 +271,26 @@
 
         # This adds another dictionary as the value of
         # parameters_cube[model_name] where the key is the parameter name
         # and the value is either a 2d array of zeros or a single value, depending
         # on whether the model in question is 3d or 1d, respectively.
         for model_name in param_dict:
             if model_name in param_x_y:
-                x_size = len(param_x_y[model_name]['x'])
-                y_size = len(param_x_y[model_name]['y'])
-
-                parameters_cube[model_name] = {x: np.zeros(shape=(x_size, y_size))
+                parameters_cube[model_name] = {x: np.zeros(shape=data_shapes[model_name][:2])
                                                for x in param_dict[model_name]}
             else:
                 parameters_cube[model_name] = {x: 0
                                                for x in param_dict[model_name]}
 
         # This loop handles the actual placement of param.values and
         # param.units into the parameter_cubes dictionary.
         for label in models:
             if " (" in label:
                 label_split = label.split(" (")
-                model_name = label_split[0] + "_3d"
+                model_name = label_split[0]
 
                 # If the get_models method is used to build a dictionary of
                 # models and a value is set for the x or y parameters, that
                 # will mean that only one x or y value is present in the
                 # models.
                 if len(param_x_y[model_name]['x']) == 1:
                     x = 0
@@ -403,37 +407,50 @@
         Preserved for backwards compatibility
         Shows Jdaviz in a sidecar in a new tab to the right
         """
         warnings.warn('show_in_new_tab has been replaced with show(loc="sidecar:tab-after")',
                       DeprecationWarning)
         return self.show(loc="sidecar:tab-after", title=title)
 
-    def _get_data(self, data_label=None, cls=None, subset_to_apply=None, function=None):
+    def _get_data(self, data_label=None, spatial_subset=None, spectral_subset=None,
+                  mask_subset=None, function=None, cls=None):
+        # Start validity checks
         list_of_valid_function_values = ('minimum', 'maximum', 'mean',
                                          'median', 'sum')
         if function and function not in list_of_valid_function_values:
             raise ValueError(f"function {function} not in list of valid"
                              f" function values {list_of_valid_function_values}")
 
         list_of_valid_subset_names = [x.label for x in self.app.data_collection.subset_groups]
-        if subset_to_apply and subset_to_apply not in list_of_valid_subset_names:
-            raise ValueError(f"Subset {subset_to_apply} not in list of valid"
-                             f" subset names {list_of_valid_subset_names}")
+        for subset in (spatial_subset, spectral_subset, mask_subset):
+            if subset and subset not in list_of_valid_subset_names:
+                raise ValueError(f"Subset {subset} not in list of valid"
+                                 f" subset names {list_of_valid_subset_names}")
 
         if data_label and data_label not in self.app.data_collection.labels:
             raise ValueError(f'{data_label} not in {self.app.data_collection.labels}.')
         elif not data_label and len(self.app.data_collection) > 1:
             raise ValueError('data_label must be set if more than'
                              ' one data exists in data_collection.')
         elif not data_label and len(self.app.data_collection) == 1:
             data_label = self.app.data_collection[0].label
 
         if cls is not None and not isclass(cls):
             raise TypeError(
                 "cls in get_data must be a class or None.")
+
+        if spectral_subset:
+            if mask_subset is not None:
+                raise ValueError("cannot use both mask_subset and spectral_subset")
+            # spectral_subset is applied as a mask, the only difference is that it has
+            # its own set of validity checks (whereas mask_subset can be used by downstream
+            # apps which would then need to do their own type checks, if necessary)
+            mask_subset = spectral_subset
+
+        # End validity checks and start data retrieval
         data = self.app.data_collection[data_label]
 
         if not cls:
             if 'Trace' in data.meta:
                 cls = None
             elif data.ndim == 2 and self.app.config == "specviz2d":
                 cls = Spectrum1D
@@ -442,68 +459,100 @@
             elif data.ndim in [1, 3]:
                 cls = Spectrum1D
 
         object_kwargs = {}
         if cls == Spectrum1D:
             object_kwargs['statistic'] = function
 
-        if not subset_to_apply:
+        if not spatial_subset and not mask_subset:
             if 'Trace' in data.meta:
                 if cls is not None:  # pragma: no cover
                     raise ValueError("cls not supported for Trace object")
                 data = data.get_object()
             else:
                 data = data.get_object(cls=cls, **object_kwargs)
 
             return data
 
-        if not cls and subset_to_apply:
+        if not cls and spatial_subset:
             raise AttributeError(f"A valid cls must be provided to"
-                                 f" apply subset {subset_to_apply} to data. "
+                                 f" apply subset {spatial_subset} to data. "
                                  f"Instead, {cls} was given.")
+        elif not cls and mask_subset:
+            raise AttributeError(f"A valid cls must be provided to"
+                                 f" apply subset {mask_subset} to data. "
+                                 f"Instead, {cls} was given.")
+
+        # Now we work on applying subsets to the data
+        all_subsets = self.app.get_subsets(object_only=True)
+
+        # Handle spatial subset
+        if spatial_subset and not isinstance(all_subsets[spatial_subset][0],
+                                             Region):
+            raise ValueError(f"{spatial_subset} is not a spatial subset.")
+        elif spatial_subset:
+            real_spatial = [sub for subsets in self.app.data_collection.subset_groups
+                            for sub in subsets.subsets
+                            if sub.data.label == data_label and subsets.label == spatial_subset][0]
+            handler, _ = data_translator.get_handler_for(cls)
+            try:
+                data = handler.to_object(real_spatial, **object_kwargs)
+            except Exception as e:
+                warnings.warn(f"Not able to get {data_label} returned with"
+                              f" subset {spatial_subset} applied of type {cls}."
+                              f" Exception: {e}")
+        elif function:
+            # This covers the case where cubeviz.get_data is called using a spectral_subset
+            # with function set.
+            data = data.get_object(cls=cls, **object_kwargs)
+
+        # Handle spectral subset, including case where spatial subset is also set
+        if spectral_subset and not isinstance(all_subsets[spectral_subset],
+                                              SpectralRegion):
+            raise ValueError(f"{spectral_subset} is not a spectral subset.")
+
+        if mask_subset:
+            real_spectral = [sub for subsets in self.app.data_collection.subset_groups
+                             for sub in subsets.subsets
+                             if sub.data.label == data_label and subsets.label == mask_subset][0] # noqa
+
+            handler, _ = data_translator.get_handler_for(cls)
+            try:
+                spec_subset = handler.to_object(real_spectral, **object_kwargs)
+            except Exception as e:
+                warnings.warn(f"Not able to get {data_label} returned with"
+                              f" subset {mask_subset} applied of type {cls}."
+                              f" Exception: {e}")
+            if spatial_subset or function:
+                # Return collapsed Spectrum1D object with spectral subset mask applied
+                data.mask = spec_subset.mask
+            else:
+                data = spec_subset
 
-        # Loop through each subset
-        for subsets in self.app.data_collection.subset_groups:
-            # If name matches the name in subsets_to_apply, continue
-            if subsets.label.lower() == subset_to_apply.lower():
-                # Loop through each data a subset applies to
-                for subset in subsets.subsets:
-                    # If the subset applies to data with the same name as data_label, continue
-                    if subset.data.label == data_label:
-
-                        handler, _ = data_translator.get_handler_for(cls)
-                        try:
-                            data = handler.to_object(subset, **object_kwargs)
-                        except Exception as e:
-                            warnings.warn(f"Not able to get {data_label} returned with"
-                                          f" subset {subsets.label} applied of type {cls}."
-                                          f" Exception: {e}")
         return data
 
-    def get_data(self, data_label=None, cls=None, subset_to_apply=None):
+    def get_data(self, data_label=None, cls=None):
         """
-        Returns data with name equal to data_label of type cls with subsets applied from
-        subset_to_apply.
+        Returns data with name equal to data_label of type cls.
 
         Parameters
         ----------
         data_label : str, optional
             Provide a label to retrieve a specific data set from data_collection.
         cls : `~specutils.Spectrum1D`, `~astropy.nddata.CCDData`, optional
             The type that data will be returned as.
-        subset_to_apply : str, optional
-            Subset that is to be applied to data before it is returned.
 
         Returns
         -------
         data : cls
-            Data is returned as type cls with subsets applied.
+            Data is returned as type cls.
 
         """
-        return self._get_data(data_label=data_label, cls=cls, subset_to_apply=subset_to_apply)
+        return self._get_data(data_label=data_label, spatial_subset=None,
+                              spectral_subset=None, function=None, cls=None)
 
 
 class ImageConfigHelper(ConfigHelper):
     """`ConfigHelper` that uses an image viewer as its primary viewer.
     For example, Imviz and Cubeviz.
     """
```

### Comparing `jdaviz-3.4.0/jdaviz/core/linelists.py` & `jdaviz-3.5.0/jdaviz/core/linelists.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/marks.py` & `jdaviz-3.5.0/jdaviz/core/marks.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/region_translators.py` & `jdaviz-3.5.0/jdaviz/core/region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/registries.py` & `jdaviz-3.5.0/jdaviz/core/registries.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/template_mixin.py` & `jdaviz-3.5.0/jdaviz/core/template_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
            'Table', 'TableMixin',
            'AutoTextField', 'AutoTextFieldMixin',
            'AddResults', 'AddResultsMixin',
            'PlotOptionsSyncState',
            'SPATIAL_DEFAULT_TEXT']
 
 SPATIAL_DEFAULT_TEXT = "Entire Cube"
+GLUE_STATES_WITH_HELPERS = ('size_att', 'cmap_att')
 
 
 def show_widget(widget, loc, title):  # pragma: no cover
     from IPython import get_ipython
     from IPython.display import display
 
     # Check if the user is running Jdaviz in the correct environments.
@@ -456,15 +457,15 @@
 
         if default_mode != 'empty' and self.selected == '':
             self._apply_default_selection()
 
     def __repr__(self):
         if hasattr(self, 'multiselect'):
             return f"<selected={self.selected} multiselect={self.multiselect} choices={self.choices}>"  # noqa
-        return f"<selected={self.selected} choices={self.choices}>"
+        return f"<selected='{self.selected}' choices={self.choices}>"
 
     def __eq__(self, other):
         return self.selected == other
 
     def __hash__(self):
         # defining __eq__ without defining __hash__ makes the object unhashable
         return super().__hash__()
@@ -1027,16 +1028,17 @@
     def selected_subset_state(self):
         subset_group = [s for s in self.app.data_collection.subset_groups if
                         s.label == self.selected][0]
         return subset_group.subset_state
 
     @property
     def selected_subset_mask(self):
-        get_data_kwargs = {'data_label': self.plugin.dataset.selected,
-                           'subset_to_apply': self.selected}
+        get_data_kwargs = {'data_label': self.plugin.dataset.selected}
+        if self._allowed_type:
+            get_data_kwargs[f'{self._allowed_type}_subset'] = self.selected
 
         if self.app.config == 'cubeviz' and self._allowed_type == 'spectral':
             viewer_ref = getattr(self.plugin,
                                  '_default_spectrum_viewer_reference_name',
                                  self.viewers[0].reference_id)
             get_data_kwargs['function'] = self.app.get_viewer(viewer_ref).state.function
 
@@ -1407,15 +1409,15 @@
             the name of the items traitlet defined in ``plugin``
         selected : str
             the name of the selected traitlet defined in ``plugin``
         default_text : str or None
             the text to show for no selection.  If not provided or None, no entry will be provided
             in the dropdown for no selection.
         manual_options: list
-            list of options to provide that are not automatically populated by subsets.  If
+            list of options to provide that are not automatically populated by datasets.  If
             ``default`` text is provided but not in ``manual_options`` it will still be included as
             the first item in the list.
         """
         super().__init__(plugin, items=items, selected=selected, filters=filters,
                          default_text=default_text, manual_options=manual_options,
                          default_mode=default_mode)
         self._cached_properties += ["selected_dc_item"]
@@ -1483,15 +1485,15 @@
         # from the data collection
         return self.get_object(cls=self.default_data_cls)
 
     def selected_spectrum_for_spatial_subset(self, spatial_subset=SPATIAL_DEFAULT_TEXT):
         if spatial_subset == SPATIAL_DEFAULT_TEXT:
             spatial_subset = None
         return self.plugin._specviz_helper.get_data(data_label=self.selected,
-                                                    subset_to_apply=spatial_subset)
+                                                    spatial_subset=spatial_subset)
 
     def _is_valid_item(self, data):
         def not_from_plugin(data):
             return data.meta.get('Plugin', None) is None
 
         def not_from_plugin_model_fitting(data):
             return data.meta.get('Plugin', None) != 'ModelFitting'
@@ -1949,17 +1951,18 @@
         self.add_observe(viewer_select._plugin_traitlets['selected'], self._on_viewer_layer_changed)
         self.add_observe(layer_select._plugin_traitlets['selected'], self._on_viewer_layer_changed)
         self.add_observe(value, self._on_value_changed)
         self._on_viewer_layer_changed()
 
     def __repr__(self):
         choices = self.choices
+        glue_name = self._glue_name if isinstance(self._glue_name, str) else ''
         if len(choices):
-            return f"<PlotOptionsSyncState {self._glue_name}={self.value} choices={self.choices} (linked_states: {len(self.linked_states)}/{len(self.subscribed_states)})>"  # noqa
-        return f"<PlotOptionsSyncState {self._glue_name}={self.value} (linked_states: {len(self.linked_states)}/{len(self.subscribed_states)})>"  # noqa
+            return f"<PlotOptionsSyncState {glue_name}={self.value} choices={self.choices} (linked_states: {len(self.linked_states)}/{len(self.subscribed_states)})>"  # noqa
+        return f"<PlotOptionsSyncState {glue_name}={self.value} (linked_states: {len(self.linked_states)}/{len(self.subscribed_states)})>"  # noqa
 
     @property
     def user_api(self):
         expose = ['value', 'unmix_state', 'linked_states']
         if len(self.choices):
             expose += ['choices', 'text']
         return UserApiWrapper(self, expose=expose)
@@ -1986,14 +1989,20 @@
         return [choice['text'] for choice in self.sync.get('choices', {})]
 
     def state_filter(self, state):
         if self._state_filter is None:
             return True
         return self._state_filter(state)
 
+    def glue_name(self, state):
+        if isinstance(self._glue_name, str):
+            return self._glue_name
+        # also support a callable that takes the state as input and returns a string
+        return self._glue_name(state)
+
     @property
     def subscribed_viewers(self):
         viewers = self._viewer_select.selected_obj
         if not isinstance(viewers, list):
             # which is the case for single-select
             viewers = [viewers]
         return viewers
@@ -2048,67 +2057,77 @@
 
     @property
     def linked_states(self):
         # access glue state objects for which the callbacks are currently connected
         return self._linked_states
 
     def _get_glue_value(self, state):
-        if self._glue_name == 'cmap':
-            return getattr(state, self._glue_name).name
-        if self._glue_name in ['contour_visible', 'bitmap_visible']:
+        glue_name = self.glue_name(state)
+        if glue_name == 'cmap':
+            return getattr(state, glue_name).name
+        if glue_name in GLUE_STATES_WITH_HELPERS:
+            return str(getattr(state, glue_name))
+        if glue_name in ('contour_visible', 'bitmap_visible'):
             # return False if the layer itself is not visible.  Setting this object
             # to True will then set both glue_name and visible to True.
-            return getattr(state, self._glue_name) and getattr(state, 'visible')
-        return getattr(state, self._glue_name)
+            return getattr(state, glue_name) and getattr(state, 'visible')
+
+        return getattr(state, glue_name)
 
     def _get_glue_choices(self, state):
-        if self._glue_name == 'cmap':
+        glue_name = self.glue_name(state)
+        if glue_name == 'cmap':
             return [{'text': cmap[0], 'value': cmap[1].name} for cmap in colormaps.members]
-        elif self._glue_name == 'color_mode':
+        if glue_name in GLUE_STATES_WITH_HELPERS:
+            helper = getattr(state, f'{glue_name}_helper')
+            return [{'text': str(choice), 'value': str(choice)} for choice in helper.choices]
+        if glue_name == 'color_mode':
             return [{'text': 'Colormap', 'value': 'Colormaps'},
                     {'text': 'Monochromatic', 'value': 'One color per layer'}]
-        else:
-            values, labels = _get_glue_choices(state, self._glue_name)
-            return [{'text': l, 'value': v} for v, l in zip(values, labels)]
+
+        values, labels = _get_glue_choices(state, glue_name)
+        return [{'text': l, 'value': v} for v, l in zip(values, labels)]
 
     def _on_viewer_layer_changed(self, msg=None):
         self._clear_cache(*self._cached_properties)
 
         # clear existing callbacks - we'll re-create those we need later
         for state in self.linked_states:
-            state.remove_callback(self._glue_name, self._on_glue_value_changed)
-            if self._glue_name in ['contour_visible', 'bitmap_visible']:
+            glue_name = self.glue_name(state)
+            state.remove_callback(glue_name, self._on_glue_value_changed)
+            if glue_name in ['contour_visible', 'bitmap_visible']:
                 state.remove_callback('visible', self._on_glue_layer_visible_changed)
 
         in_subscribed_states = False
         icons = []
         current_glue_values = []
         self._linked_states = []
         for states, icon in zip(self.subscribed_states, self.subscribed_icons):
             if not isinstance(states, list):
                 states = [states]
 
             for state in states:
                 if state is None or not self.state_filter(state):
                     continue
-                if self._glue_name is None or not hasattr(state, self._glue_name):
+                glue_name = self.glue_name(state)
+                if glue_name is None or not hasattr(state, glue_name):
                     continue
 
                 in_subscribed_states = True
                 if icon not in icons:
                     icons.append(icon)
                 current_glue_values.append(self._get_glue_value(state))
                 self._linked_states.append(state)  # these will be iterated when value is set
-                state.add_callback(self._glue_name, self._on_glue_value_changed)
-                if self._glue_name in ['contour_visible', 'bitmap_visible']:
+                state.add_callback(glue_name, self._on_glue_value_changed)
+                if glue_name in ['contour_visible', 'bitmap_visible']:
                     state.add_callback('visible', self._on_glue_layer_visible_changed)
 
                 if self.sync.get('choices') is None and \
-                        (hasattr(getattr(type(state), self._glue_name), 'get_display_func')
-                         or self._glue_name == 'cmap'):
+                        (hasattr(getattr(type(state), glue_name), 'get_display_func')
+                         or glue_name == 'cmap'):
                     # then we can access and populate the choices.  We are assuming here
                     # that each state-instance with this same name will have the same
                     # choices and that those will not change.  If we ever hookup options
                     # with changing choices, we'll need additional logic to sync to those
                     # and handle mixed state in the choices...
                     self.sync = {**self.sync, 'choices': self._get_glue_choices(state)}
 
@@ -2137,25 +2156,30 @@
             return
 
         if self._spinner is not None:
             setattr(self.plugin, self._spinner, True)
 
         self._processing_change_to_glue = True
         for glue_state in self.linked_states:
-            if self._glue_name == 'cmap':
+            glue_name = self.glue_name(glue_state)
+            if glue_name == 'cmap':
                 cmap = None
                 for member in colormaps.members:
                     if member[1].name == msg['new']:
                         cmap = member[1]
                         break
-                setattr(glue_state, self._glue_name, cmap)
+                setattr(glue_state, glue_name, cmap)
+            elif glue_name in GLUE_STATES_WITH_HELPERS:
+                helper = getattr(glue_state, f'{glue_name}_helper')
+                value = [choice for choice in helper.choices if str(choice) == msg['new']][0]
+                setattr(glue_state, glue_name, value)
             else:
-                setattr(glue_state, self._glue_name, msg['new'])
+                setattr(glue_state, glue_name, msg['new'])
 
-            if self._glue_name in ['bitmap_visible', 'contour_visible'] and msg['new'] is True:
+            if glue_name in ['bitmap_visible', 'contour_visible'] and msg['new'] is True:
                 # ensure that the layer is also visible
                 if not glue_state.visible:
                     setattr(glue_state, 'visible', msg['new'])
 
         # need to recompute mixed state
         self._update_mixed_state()
         self._processing_change_to_glue = False
@@ -2187,14 +2211,16 @@
 
         if self._processing_change_to_glue:
             return
 
         self._processing_change_from_glue = True
         if "Colormap" in value.__class__.__name__:
             value = value.name
+        elif self._glue_name in GLUE_STATES_WITH_HELPERS:
+            value = str(value)
         elif isinstance(self.value, (int, float)) and self._glue_name != 'percentile':
             # glue might pass us ints for float or vice versa, but our traitlets care
             # so let's cast to the type expected by the traitlet to avoid having to
             # use Any traitlets for all of these.  We skip percentile as that needs
             # to be an Any traitlet in order to handle "Custom"
             value = type(self.value)(value)
         self.value = value
@@ -2289,22 +2315,39 @@
     To render in the plugin's vue file::
 
       <jupyter-widget :widget="table_widget"></jupyter-widget>
 
     """
     template_file = __file__, "../components/plugin_table.vue"
 
+    _default_values_by_colname = {}
+
     headers_visible = List([]).tag(sync=True)  # list of strings
     headers_avail = List([]).tag(sync=True)   # list of strings
     items = List().tag(sync=True)  # list of dictionaries, pass single dict to add_row
 
     def __init__(self, plugin, *args, **kwargs):
         self._qtable = None
         super().__init__(plugin, 'Table', *args, **kwargs)
 
+    def default_value_for_column(self, colname=None, value=None):
+        if colname in self._default_values_by_colname:
+            return self._default_values_by_colname.get(colname)
+        if isinstance(value, (tuple, list)):
+            return [self.default_value_for_column(value=v) for v in value]
+        if isinstance(value, (float, int)):
+            return np.nan
+        if isinstance(value, str):
+            return ''
+        return None
+
+    @staticmethod
+    def _new_col_visible(colname):
+        return True
+
     def add_item(self, item):
         """
         Add an item/row to the table.
 
         Parameters
         ----------
         item : QTable, QTableRow, or dictionary of row-name, value pairs
@@ -2347,18 +2390,29 @@
             # Row does not have .items() implemented
             item = {k: v for k, v in zip(item.keys(), item.values())}
 
         # save original sent values to the cached QTable object
         if self._qtable is None:
             self._qtable = QTable([item])
         else:
-            # NOTE: this does not support adding columns that did not exist in the first
-            # call to add_row since the last call to clear_table
+            # add any missing columns with a default value for all previous rows
+            for colname, value in item.items():
+                if colname in self._qtable.colnames:
+                    continue
+                default_value = self.default_value_for_column(colname=colname,
+                                                              value=value)
+                self._qtable.add_column(default_value, name=colname)
+
             self._qtable.add_row(item)
 
+        missing_headers = [k for k in item.keys() if k not in self.headers_avail]
+        if len(missing_headers):
+            self.headers_avail = self.headers_avail + missing_headers
+            self.headers_visible = self.headers_visible + [m for m in missing_headers if self._new_col_visible(m)]  # noqa
+
         # clean data to show in the UI
         self.items = self.items + [{k: json_safe(k, v) for k, v in item.items()}]
 
     def clear_table(self):
         """
         Clear all entries/markers from the current table.
         """
```

### Comparing `jdaviz-3.4.0/jdaviz/core/tests/test_custom_traitlets.py` & `jdaviz-3.5.0/jdaviz/core/tests/test_custom_traitlets.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/tests/test_helpers.py` & `jdaviz-3.5.0/jdaviz/core/tests/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
          ('Test 1D Spectrum 2', 'Subset 2',
           [False, True, True, True, True, True, True, True, True, True]),
          ('Test 1D Spectrum 2', 'Subset 3',
           [True, True, True, True, True, True, False, False, False, True])])
     def test_get_data_with_one_subset_per_data(self, specviz_helper, label, subset_name, answer):
 
         results = specviz_helper.get_data(data_label=label,
-                                          subset_to_apply=subset_name)
+                                          spectral_subset=subset_name)
         assert list(results.mask) == answer
 
     def test_get_data_no_label_multiple_in_dc(self, specviz_helper):
         with pytest.raises(ValueError, match='data_label must be set if more'):
             specviz_helper.get_data()
 
     def test_get_data_label_not_in_dc(self, specviz_helper):
@@ -84,8 +84,8 @@
     def test_get_data_invald_cls_class(self, specviz_helper):
         specviz_helper.app.data_collection.remove(specviz_helper.app.data_collection[self.label2])
         with pytest.raises(TypeError, match="cls in get_data must be a class or None."):
             specviz_helper.get_data('Test 1D Spectrum', cls=42)
 
     def test_get_data_invald_subset_name(self, specviz_helper):
         with pytest.raises(ValueError, match="not in list of valid subset names"):
-            specviz_helper.get_data('Test 1D Spectrum', subset_to_apply="Fail")
+            specviz_helper.get_data('Test 1D Spectrum', spectral_subset="Fail")
```

### Comparing `jdaviz-3.4.0/jdaviz/core/tests/test_region_translators.py` & `jdaviz-3.5.0/jdaviz/core/tests/test_region_translators.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/tests/test_template_mixin.py` & `jdaviz-3.5.0/jdaviz/core/tests/test_template_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     assert p.spectral_subset_selected_has_subregions is False
     assert p.spectral_subset.selected_obj is None
     p.spectral_subset_selected = 'Subset 1'
     assert p.spectral_subset_selected_has_subregions is False
     assert p.spectral_subset.selected_obj is not None
     expected_min = spectrum1d.spectral_axis[spectrum1d.spectral_axis.value >= 6500][0]
     expected_max = spectrum1d.spectral_axis[spectrum1d.spectral_axis.value <= 7400][-1]
-    assert p.spectral_subset.selected_min_max(spectrum1d) == (expected_min, expected_max)
+    np.testing.assert_allclose(expected_min.value, 6666.66666667, atol=1e-5)
+    np.testing.assert_allclose(expected_max.value, 7333.33333333, atol=1e-5)
+    assert p.spectral_subset.selected_min_max(spectrum1d) == (6500 * u.AA, 7400 * u.AA)
 
     # check selected subset mask available via API:
     expected_mask_with_spectral_subset = (
         (spectrum1d.wavelength.to(u.AA).value < 6500) |
         (spectrum1d.wavelength.to(u.AA).value > 7400)
     )
     assert np.all(
```

### Comparing `jdaviz-3.4.0/jdaviz/core/tools.py` & `jdaviz-3.5.0/jdaviz/core/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,35 @@
             # let's ignore and reset the tool
             return
 
         self.viewer.state.x_min, self.viewer.state.x_max = self.interact.selected
 
 
 @viewer_tool
+class YRangeZoom(_BaseSelectZoom):
+    icon = os.path.join(ICON_DIR, 'zoom_yrange.svg')
+    tool_id = 'jdaviz:yrangezoom'
+    action_text = 'Vertical zoom'
+    tool_tip = 'Zoom to a drawn vertical region'
+
+    def _new_interact(self):
+        return BrushIntervalSelector(orientation='vertical',
+                                     scale=self.viewer.scale_y,
+                                     color=INTERACT_COLOR)
+
+    def on_update_zoom(self):
+        if self.interact.selected is None:
+            # a valid region was not drawn, perhaps just a click with no drag!
+            # let's ignore and reset the tool
+            return
+
+        self.viewer.state.y_min, self.viewer.state.y_max = self.interact.selected
+
+
+@viewer_tool
 class SelectLine(CheckableTool, HubListener):
     icon = os.path.join(ICON_DIR, 'line_select.svg')
     tool_id = 'jdaviz:selectline'
     action_text = 'Select/identify spectral line'
     tool_tip = 'Select/identify spectral line'
 
     def __init__(self, viewer, **kwargs):
```

### Comparing `jdaviz-3.4.0/jdaviz/core/user_api.py` & `jdaviz-3.5.0/jdaviz/core/user_api.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/core/validunits.py` & `jdaviz-3.5.0/jdaviz/core/validunits.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/checktoradial.svg` & `jdaviz-3.5.0/jdaviz/data/icons/checktoradial.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/compass.svg` & `jdaviz-3.5.0/jdaviz/data/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/line_select.svg` & `jdaviz-3.5.0/jdaviz/data/icons/line_select.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/line_select_disabled.svg` & `jdaviz-3.5.0/jdaviz/data/icons/line_select_disabled.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/pan.svg` & `jdaviz-3.5.0/jdaviz/data/icons/pan.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/pan2.svg` & `jdaviz-3.5.0/jdaviz/data/icons/pan2.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/panzoom_match.svg` & `jdaviz-3.5.0/jdaviz/data/icons/panzoom_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/pixelspectra.svg` & `jdaviz-3.5.0/jdaviz/data/icons/pixelspectra.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/radialtocheck.svg` & `jdaviz-3.5.0/jdaviz/data/icons/radialtocheck.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/select_circle.svg` & `jdaviz-3.5.0/jdaviz/data/icons/select_circle.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/select_ellipse.svg` & `jdaviz-3.5.0/jdaviz/data/icons/select_ellipse.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/select_lasso.svg` & `jdaviz-3.5.0/jdaviz/data/icons/select_lasso.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/select_single_pixel.svg` & `jdaviz-3.5.0/jdaviz/data/icons/select_single_pixel.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/select_xy.svg` & `jdaviz-3.5.0/jdaviz/data/icons/select_xy.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/slice.svg` & `jdaviz-3.5.0/jdaviz/data/icons/slice.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/spectral_range.svg` & `jdaviz-3.5.0/jdaviz/data/icons/spectral_range.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/zoom_box_match.svg` & `jdaviz-3.5.0/jdaviz/data/icons/zoom_box_match.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/zoom_xrange.svg` & `jdaviz-3.5.0/jdaviz/data/icons/zoom_yrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/icons/zoom_yrange.svg` & `jdaviz-3.5.0/jdaviz/data/icons/zoom_xrange.svg`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Atomic-ISO.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Atomic-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Atomic-Ionic.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Atomic-Ionic_FineStructure.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/CO.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/CO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_2000A-11000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Common_Galactic_700A-2000A.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Common_nebular.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Common_nebular.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/Common_stellar.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/Common_stellar.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/DEV_NOTES.txt` & `jdaviz-3.5.0/jdaviz/data/linelists/DEV_NOTES.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/H-He.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/H-He.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/H-Paschen-Brackett.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/H-Paschen-Brackett.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/H2-ISO.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/H2-ISO.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/H2-alt.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/H2-alt.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/H2.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/H2.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/HeI-HeII.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/HeI-HeII.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/JWST_line_list_original.txt` & `jdaviz-3.5.0/jdaviz/data/linelists/JWST_line_list_original.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/PAH.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/PAH.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/SDSS-IV.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/SDSS-IV.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/SDSS.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/SDSS.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/UV_linelist_vacuum.csv` & `jdaviz-3.5.0/jdaviz/data/linelists/UV_linelist_vacuum.csv`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/data/linelists/linelist_metadata.json` & `jdaviz-3.5.0/jdaviz/data/linelists/linelist_metadata.json`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/jdaviz_cli.ipynb` & `jdaviz-3.5.0/jdaviz/jdaviz_cli.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/models/physical_models.py` & `jdaviz-3.5.0/jdaviz/models/physical_models.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/tests/coveragerc` & `jdaviz-3.5.0/jdaviz/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/tests/test_app.py` & `jdaviz-3.5.0/jdaviz/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/tests/test_data_formats.py` & `jdaviz-3.5.0/jdaviz/tests/test_data_formats.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/tests/test_metadata.py` & `jdaviz-3.5.0/jdaviz/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/tests/test_utils.py` & `jdaviz-3.5.0/jdaviz/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/tests/test_viewer_ids.py` & `jdaviz-3.5.0/jdaviz/tests/test_viewer_ids.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz/utils.py` & `jdaviz-3.5.0/jdaviz/utils.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/jdaviz.egg-info/PKG-INFO` & `jdaviz-3.5.0/jdaviz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: jdaviz
-Version: 3.4.0
+Version: 3.5.0
 Summary: Astronomical data analysis development leveraging the Jupyter platform
-Home-page: https://jdaviz.readthedocs.io/en/latest/
-Author: JDADF Developers
-Author-email: rosteen@stsci.edu
-License: BSD 3-Clause
+Author-email: JDADF Developers <rosteen@stsci.edu>
+Project-URL: Homepage, https://jdaviz.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: roman
 License-File: LICENSE.rst
 
 .. image:: docs/logos/jdaviz.svg
     :width: 400
     :alt: Jdaviz logo
     :align: center
 
@@ -106,18 +105,22 @@
 The power of ``jdaviz`` is that it can integrated into your Jupyter notebook workflow:
 
 .. code-block:: python
 
     from jdaviz import Specviz
 
     specviz = Specviz()
-    specviz.app
+    specviz.show()
 
 To learn more about the various ``jdaviz`` application configurations and loading data, see the
-`specviz <https://jdaviz.readthedocs.io/en/latest/specviz/import_data.html>`_, `cubeviz <https://jdaviz.readthedocs.io/en/latest/cubeviz/import_data.html>`_, `mosviz <https://jdaviz.readthedocs.io/en/latest/mosviz/import_data.html>`_, or `imviz <https://jdaviz.readthedocs.io/en/latest/imviz/import_data.html>`_ tools.
+`Specviz <https://jdaviz.readthedocs.io/en/latest/specviz/import_data.html>`_,
+`Cubeviz <https://jdaviz.readthedocs.io/en/latest/cubeviz/import_data.html>`_,
+`Mosviz <https://jdaviz.readthedocs.io/en/latest/mosviz/import_data.html>`_,
+`Imviz <https://jdaviz.readthedocs.io/en/latest/imviz/import_data.html>`_,
+or `Specviz2D <https://jdaviz.readthedocs.io/en/latest/specviz2d/import_data.html>`_ tools.
 
 ``jdaviz`` also provides a directory of `sample notebooks <https://jdaviz.readthedocs.io/en/latest/sample_notebooks.html>`_ to test the application, located in the ``notebooks`` sub-directory
 of the git repository.  ``CubevizExample.ipynb`` is provided as an example that loads a JWST data cube with the
 ``Cubeviz`` configuration.  To run the provided example, start the Jupyter kernel with the notebook path:
 
 .. code-block:: bash
 
@@ -127,14 +130,19 @@
 ----
 
 If you uncover any issues or bugs, you can
 `open a GitHub issue <https://github.com/spacetelescope/jdaviz/issues/new/choose>`_
 if they are not already reported. For faster responses, however, we encourage you to
 submit a `JWST Help Desk Ticket <https://jwsthelp.stsci.edu>`_.
 
+Recordings and instructional notebooks from live Jdaviz tutorials (as part of the JWebbinars series)
+can be found at `the JWebbinar website <https://www.stsci.edu/jwst/science-execution/jwebbinars>`_
+under the "Materials and Videos" expandable section. Scroll down to the bottom of that section to
+find materials from the most recent session (JWebbinar 24, March 2023).
+
 License & Attribution
 ---------------------
 
 This project is Copyright (c) JDADF Developers and licensed under
 the terms of the BSD 3-Clause license. This package is based upon
 the `Astropy package template <https://github.com/astropy/package-template>`_
 which is licensed under the BSD 3-clause licence. See the
@@ -142,15 +150,15 @@
 folder for more information.
 
 Cite ``jdaviz`` via our Zenodo record: https://doi.org/10.5281/zenodo.5513927.
 
 Contributing
 ------------
 
-We love contributions! jdaviz is open source,
+We love contributions! ``jdaviz`` is open source,
 built on open source, and we'd love to have you hang out in our community.
 
 **Imposter syndrome disclaimer**: We want your help. No, really.
 
 There may be a little voice inside your head that is telling you that you're not
 ready to be an open source contributor; that your skills aren't nearly good
 enough to contribute. What could you possibly offer a project like this one?
```

### Comparing `jdaviz-3.4.0/jdaviz.egg-info/SOURCES.txt` & `jdaviz-3.5.0/jdaviz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .bandit.yaml
+.flake8
 .gitignore
 .readthedocs.yaml
 CHANGES.rst
 CITATION.cff
 CODE_OF_CONDUCT.md
 LICENSE.rst
 MANIFEST.in
 README.rst
 conftest.py
+licenses
 pyproject.toml
-setup.cfg
 setup.py
 tox.ini
 .github/CODEOWNERS
 .github/PULL_REQUEST_TEMPLATE.md
 .github/labeler.yml
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
@@ -177,31 +178,38 @@
 jdaviz/configs/imviz/plugins/image_viewer_creator/image_viewer_creator.vue
 jdaviz/configs/imviz/plugins/line_profile_xy/__init__.py
 jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.py
 jdaviz/configs/imviz/plugins/line_profile_xy/line_profile_xy.vue
 jdaviz/configs/imviz/plugins/links_control/__init__.py
 jdaviz/configs/imviz/plugins/links_control/links_control.py
 jdaviz/configs/imviz/plugins/links_control/links_control.vue
+jdaviz/configs/imviz/plugins/rotate_canvas/__init__.py
+jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.py
+jdaviz/configs/imviz/plugins/rotate_canvas/rotate_canvas.vue
+jdaviz/configs/imviz/plugins/rotate_canvas/tests/__init__.py
+jdaviz/configs/imviz/plugins/rotate_canvas/tests/test_rotate_canvas.py
 jdaviz/configs/imviz/tests/__init__.py
 jdaviz/configs/imviz/tests/test_astrowidgets_api.py
 jdaviz/configs/imviz/tests/test_catalogs.py
 jdaviz/configs/imviz/tests/test_helper.py
 jdaviz/configs/imviz/tests/test_line_profile_xy.py
 jdaviz/configs/imviz/tests/test_linking.py
 jdaviz/configs/imviz/tests/test_links_control.py
 jdaviz/configs/imviz/tests/test_parser.py
+jdaviz/configs/imviz/tests/test_parser_roman.py
 jdaviz/configs/imviz/tests/test_regions.py
 jdaviz/configs/imviz/tests/test_simple_aper_phot.py
 jdaviz/configs/imviz/tests/test_subset_centroid.py
 jdaviz/configs/imviz/tests/test_tools.py
 jdaviz/configs/imviz/tests/test_viewer_tools.py
 jdaviz/configs/imviz/tests/test_viewers.py
 jdaviz/configs/imviz/tests/test_wcs_utils.py
 jdaviz/configs/imviz/tests/utils.py
 jdaviz/configs/imviz/tests/data/miri_i2d_lonlat_gwcs.asdf
+jdaviz/configs/imviz/tests/data/roman_wfi_image_model.asdf
 jdaviz/configs/mosviz/__init__.py
 jdaviz/configs/mosviz/helper.py
 jdaviz/configs/mosviz/mosviz.yaml
 jdaviz/configs/mosviz/plugins/__init__.py
 jdaviz/configs/mosviz/plugins/parsers.py
 jdaviz/configs/mosviz/plugins/viewers.py
 jdaviz/configs/mosviz/plugins/row_lock/__init__.py
@@ -257,14 +265,15 @@
 jdaviz/core/events.py
 jdaviz/core/freezable_state.py
 jdaviz/core/helpers.py
 jdaviz/core/linelists.py
 jdaviz/core/marks.py
 jdaviz/core/region_translators.py
 jdaviz/core/registries.py
+jdaviz/core/style_widget.py
 jdaviz/core/template_mixin.py
 jdaviz/core/tools.py
 jdaviz/core/user_api.py
 jdaviz/core/validunits.py
 jdaviz/core/tests/__init__.py
 jdaviz/core/tests/test_custom_traitlets.py
 jdaviz/core/tests/test_data_menu.py
@@ -274,23 +283,25 @@
 jdaviz/core/tests/test_tools.py
 jdaviz/data/icons/blink.svg
 jdaviz/data/icons/checktoradial.svg
 jdaviz/data/icons/compass.svg
 jdaviz/data/icons/contrast.svg
 jdaviz/data/icons/home.svg
 jdaviz/data/icons/image.svg
+jdaviz/data/icons/left-east.svg
 jdaviz/data/icons/line_select.svg
 jdaviz/data/icons/line_select_disabled.svg
 jdaviz/data/icons/pan.svg
 jdaviz/data/icons/pan2.svg
 jdaviz/data/icons/pan_x.svg
 jdaviz/data/icons/pan_y.svg
 jdaviz/data/icons/panzoom_match.svg
 jdaviz/data/icons/pixelspectra.svg
 jdaviz/data/icons/radialtocheck.svg
+jdaviz/data/icons/right-east.svg
 jdaviz/data/icons/select_circle.svg
 jdaviz/data/icons/select_ellipse.svg
 jdaviz/data/icons/select_lasso.svg
 jdaviz/data/icons/select_single_pixel.svg
 jdaviz/data/icons/select_x.svg
 jdaviz/data/icons/select_xy.svg
 jdaviz/data/icons/select_y.svg
@@ -359,14 +370,15 @@
 notebooks/concepts/imviz_compass_mpl.ipynb
 notebooks/concepts/imviz_custom_colormap.ipynb
 notebooks/concepts/imviz_dithered_gwcs.ipynb
 notebooks/concepts/imviz_edit_subset_programmatic.ipynb
 notebooks/concepts/imviz_line_profiles.ipynb
 notebooks/concepts/imviz_load_3d_slices.ipynb
 notebooks/concepts/imviz_load_fits_hdu.ipynb
+notebooks/concepts/imviz_roman_asdf.ipynb
 notebooks/concepts/imviz_simple_aper_phot.ipynb
 notebooks/concepts/mosviz_concept.ipynb
 notebooks/concepts/mosviz_generate_photometry.ipynb
 notebooks/concepts/mosviz_niriss_parser.ipynb
 notebooks/concepts/mosviz_overplot_slit.ipynb
 notebooks/concepts/pypi_metrics.ipynb
 notebooks/concepts/specviz_from_list.ipynb
```

### Comparing `jdaviz-3.4.0/jdaviz.egg-info/requires.txt` & `jdaviz-3.5.0/jdaviz.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 packaging
 astropy>=4.3
 matplotlib
 traitlets>=5.0.5
-bqplot>=0.12.36
+bqplot>=0.12.37
 bqplot-image-gl>=1.4.11
-glue-core>=1.6.0
+glue-core!=1.10,!=1.9.0,>=1.6.0
 glue-jupyter>=0.15.0
 echo>=0.5.0
 ipykernel>=6.19.4
 ipyvue>=1.6
 ipyvuetify>=1.7.0
 ipysplitpanes>=0.1.0
 ipygoldenlayout>=0.3.0
-ipywidgets<8.0.5,>=8
+ipywidgets>=8.0.6
 voila>=0.4
 pyyaml>=5.4.1
 specutils>=1.9
 specreduce<1.4.0,>=1.3.0
 photutils>=1.4
 glue-astronomy>=0.7
 asteval>=0.9.23
@@ -34,11 +34,17 @@
 [:python_version == "3.9"]
 y_py<0.5.5
 
 [docs]
 sphinx-rtd-theme
 sphinx-astropy
 
+[docs:python_version < "3.11"]
+tomli
+
+[roman]
+roman_datamodels>=0.14.2
+
 [test]
 pytest
 pytest-astropy
 pytest-tornasync
```

### Comparing `jdaviz-3.4.0/licenses/GINGA_LICENSE.txt` & `jdaviz-3.5.0/licenses/GINGA_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/licenses/IMEXAM_LICENSE.txt` & `jdaviz-3.5.0/licenses/IMEXAM_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/licenses/IPYFILECHOOSER_LICENSE.rst` & `jdaviz-3.5.0/licenses/IPYFILECHOOSER_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/licenses/TEMPLATE_LICENCE.rst` & `jdaviz-3.5.0/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/CubevizExample.ipynb` & `jdaviz-3.5.0/notebooks/CubevizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/ImvizDitheredExample.ipynb` & `jdaviz-3.5.0/notebooks/ImvizDitheredExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/ImvizExample.ipynb` & `jdaviz-3.5.0/notebooks/ImvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/MosvizExample.ipynb` & `jdaviz-3.5.0/notebooks/MosvizExample.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971007799671593%*

 * *Differences: {"'cells'": "{18: {'source': {insert: [(2, '# On the last data loader call, also add redshift "*

 * *            "column.\\n'), (6, 'mosviz.load_images(images, add_redshift_column=True)\\n'), (7, "*

 * *            "'mosviz.load_metadata(images)')], delete: [6, 3]}}, 22: {'source': {insert: [(2, '# "*

 * *            "On the last data loader call, also add redshift column.\\n'), (5, "*

 * *            "'mosviz_no_images.load_2d_spectra(spectra_2d, add_redshift_column=True)')], delete: "*

 * *            '[4]}}}',*

 * * "'metadata'": "{' […]*

```diff
@@ -197,19 +197,20 @@
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 "# *** OR ***\n",
                 "# Enable and run this cell if you want to load them separately.\n",
+                "# On the last data loader call, also add redshift column.\n",
                 "\n",
-                "mosviz.load_metadata(images)    \n",
                 "mosviz.load_1d_spectra(spectra_1d)\n",
                 "mosviz.load_2d_spectra(spectra_2d)\n",
-                "mosviz.load_images(images)"
+                "mosviz.load_images(images, add_redshift_column=True)\n",
+                "mosviz.load_metadata(images)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If no images are provided, Mosviz can still display the spectra."
@@ -236,17 +237,18 @@
         },
         {
             "cell_type": "raw",
             "metadata": {},
             "source": [
                 "# *** OR ***\n",
                 "# Enable and run this cell if you want to load them separately.\n",
+                "# On the last data loader call, also add redshift column.\n",
                 "\n",
                 "mosviz_no_images.load_1d_spectra(spectra_1d)\n",
-                "mosviz_no_images.load_2d_spectra(spectra_2d)"
+                "mosviz_no_images.load_2d_spectra(spectra_2d, add_redshift_column=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Images can be added later."
@@ -309,13 +311,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.10.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `jdaviz-3.4.0/notebooks/MosvizNIRISSExample.ipynb` & `jdaviz-3.5.0/notebooks/MosvizNIRISSExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/Specviz2dExample.ipynb` & `jdaviz-3.5.0/notebooks/Specviz2dExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/SpecvizExample.ipynb` & `jdaviz-3.5.0/notebooks/SpecvizExample.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_contour_overlay.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_contour_overlay.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_data_interactions.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_data_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_fitting.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_ndarray_gif.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_fitting.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_spectral_spatial_interactions.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb` & `jdaviz-3.5.0/notebooks/concepts/cubeviz_wfc3ir_ramp.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb` & `jdaviz-3.5.0/notebooks/concepts/default_programmatic_viewers_from_blank.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_color_display.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_color_display.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_compass_mpl.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_compass_mpl.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_custom_colormap.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_custom_colormap.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_dithered_gwcs.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_dithered_gwcs.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_edit_subset_programmatic.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_line_profiles.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_line_profiles.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_load_3d_slices.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_load_3d_slices.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_load_fits_hdu.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_load_fits_hdu.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/imviz_simple_aper_phot.ipynb` & `jdaviz-3.5.0/notebooks/concepts/imviz_simple_aper_phot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/mosviz_concept.ipynb` & `jdaviz-3.5.0/notebooks/concepts/mosviz_concept.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/mosviz_generate_photometry.ipynb` & `jdaviz-3.5.0/notebooks/concepts/mosviz_generate_photometry.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/mosviz_niriss_parser.ipynb` & `jdaviz-3.5.0/notebooks/concepts/mosviz_niriss_parser.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/mosviz_overplot_slit.ipynb` & `jdaviz-3.5.0/notebooks/concepts/mosviz_overplot_slit.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/pypi_metrics.ipynb` & `jdaviz-3.5.0/notebooks/concepts/pypi_metrics.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/specviz_from_list.ipynb` & `jdaviz-3.5.0/notebooks/concepts/specviz_from_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/specviz_from_splot.ipynb` & `jdaviz-3.5.0/notebooks/concepts/specviz_from_splot.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/specviz_line_lists.ipynb` & `jdaviz-3.5.0/notebooks/concepts/specviz_line_lists.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/specviz_minimal.ipynb` & `jdaviz-3.5.0/notebooks/concepts/specviz_minimal.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/specviz_spectrum_list.ipynb` & `jdaviz-3.5.0/notebooks/concepts/specviz_spectrum_list.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/notebooks/concepts/specviz_unit_conversion.ipynb` & `jdaviz-3.5.0/notebooks/concepts/specviz_unit_conversion.ipynb`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/setup.py` & `jdaviz-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js` & `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/ansi.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html` & `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/app.html`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2` & `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js` & `jdaviz-3.5.0/share/jupyter/nbconvert/templates/jdaviz-default/util.js`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2` & `jdaviz-3.5.0/share/jupyter/voila/templates/jdaviz-default/index.html.j2`

 * *Files identical despite different names*

### Comparing `jdaviz-3.4.0/tox.ini` & `jdaviz-3.5.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{38,39,310,311}-test{,-alldeps,-devdeps,-predeps}{,-cov}
+    py{38,39,310,311}-test{,-alldeps,-devdeps,-predeps}{-romandeps}{,-cov}
     linkcheck
     codestyle
     pep517
     securityaudit
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
@@ -32,49 +32,52 @@
 #
 #     tox -l -v
 #
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
+    romandeps: with dependencies specific to supporting Roman
     cov: and test coverage
 
 # The following provides some specific pinnings for key packages
 deps =
     # NOTE: Add/remove as needed
     devdeps: scipy>=0.0.dev0
     devdeps: numpy>=0.0.dev0
     devdeps: git+https://github.com/astropy/regions.git
     devdeps: git+https://github.com/astropy/specutils.git
     devdeps: git+https://github.com/astropy/photutils.git
     devdeps: git+https://github.com/spacetelescope/gwcs.git
     devdeps: git+https://github.com/asdf-format/asdf.git
-    devdeps: git+https://github.com/spacetelescope/stdatamodels.git
+    devdeps: git+https://github.com/astropy/asdf-astropy.git
+    # FIXME: https://github.com/spacetelescope/stdatamodels/issues/159
+    #devdeps: git+https://github.com/spacetelescope/stdatamodels.git
     devdeps: git+https://github.com/bqplot/bqplot.git@0.12.x
     devdeps: git+https://github.com/glue-viz/glue.git
     devdeps: git+https://github.com/voila-dashboards/voila.git
-    # FIXME: https://github.com/glue-viz/bqplot-image-gl/issues/99
-    #devdeps: git+https://github.com/glue-viz/bqplot-image-gl.git
+    devdeps: git+https://github.com/glue-viz/bqplot-image-gl.git
     devdeps: git+https://github.com/glue-viz/glue-jupyter.git
     devdeps: git+https://github.com/glue-viz/glue-astronomy.git
     # TODO: Enable this when specreduce becomes stable.
     #devdeps: git+https://github.com/astropy/specreduce.git
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
+    romandeps: roman
     # Uncomment when we have all again in setup.cfg
     #alldeps: all
 
 commands =
     devdeps: pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
     jupyter --paths
     pip freeze
     !cov: pytest --pyargs jdaviz {toxinidir}/docs {posargs}
-    cov: pytest --pyargs jdaviz {toxinidir}/docs --cov jdaviz --cov-config={toxinidir}/setup.cfg {posargs}
+    cov: pytest --pyargs jdaviz {toxinidir}/docs --cov jdaviz --cov-config={toxinidir}/pyproject.toml {posargs}
     cov: coverage xml -o {toxinidir}/coverage.xml
 
 pip_pre =
     predeps: true
     !predeps: false
 
 [testenv:linkcheck]
```

