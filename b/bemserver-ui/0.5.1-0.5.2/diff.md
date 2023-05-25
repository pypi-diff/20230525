# Comparing `tmp/bemserver-ui-0.5.1.tar.gz` & `tmp/bemserver-ui-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-ui-0.5.1.tar", last modified: Thu Apr 27 15:02:13 2023, max compression
+gzip compressed data, was "bemserver-ui-0.5.2.tar", last modified: Thu May 25 08:25:46 2023, max compression
```

## Comparing `bemserver-ui-0.5.1.tar` & `bemserver-ui-0.5.2.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/common/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/common/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/campaign_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/flask_es6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/jinja_custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-areas.json
--rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-full.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-regions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/services/weather_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/internal_api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.570421 bemserver-ui-0.5.1/bemserver_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.ico
--rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.578421 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/accordionList.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/dropZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/eventLevel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/filterSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/flash.js
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/itemsCount.js
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/modalConfirm.js
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/spinner.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
--rw-r--r--   0 runner    (1001) docker     (123)    32394 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/tree.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/userGroup/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/flashTimer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/formController.js
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/notifications.js
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/sidebar.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/array.js
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/dict.js
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/fetcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/flaskES6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/parser.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/time.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.570421 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaignScopes/
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.582422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/list.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/weatherData/
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
--rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
--rw-r--r--   0 runner    (1001) docker     (123)    52668 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/dragndrop.css
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/main.css
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/signin.css
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/static/styles/tree.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.570421 bemserver-ui-0.5.1/bemserver_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/campaigns/selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_admin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_services.html
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/user_group_available.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.586422 bemserver-ui-0.5.1/bemserver_ui/templates/components/users/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_for_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/structural_element_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/ts_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/flash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/macros/partners.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/degree_days.html
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/energy_consumption.html
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/setup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/weather_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/weather_data/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.590422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/explore.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/completeness.html
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/semantic_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.594422 bemserver-ui-0.5.1/bemserver_ui/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/campaigns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/events/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/services/weather_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/bemserver_ui/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.574422 bemserver-ui-0.5.1/bemserver_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 15:02:13.000000 bemserver-ui-0.5.1/bemserver_ui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-27 15:02:13.598422 bemserver-ui-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 15:01:54.000000 bemserver-ui-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/campaign_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/flask_es6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/jinja_custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-areas.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-full.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/weather_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/accordionList.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/dropZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/eventLevel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/filterSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/flash.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/itemsCount.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/modalConfirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/spinner.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32482 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/tree.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/userGroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/flashTimer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/formController.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/notifications.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/sidebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/dict.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/fetcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/flaskES6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/time.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaignScopes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/list.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/weatherData/
+-rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/dragndrop.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/signin.css
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/tree.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/templates/components/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/campaigns/selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_admin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_services.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/user_group_available.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/components/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_for_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/structural_element_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/ts_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/flash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/partners.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/degree_days.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/energy_consumption.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/setup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/weather_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/weather_data/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/explore.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/completeness.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/semantic_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.741495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.741495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.741495 bemserver-ui-0.5.2/bemserver_ui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/campaigns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/events/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/weather_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-25 08:25:46.749496 bemserver-ui-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/tox.ini
```

### Comparing `bemserver-ui-0.5.1/LICENSE` & `bemserver-ui-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/PKG-INFO` & `bemserver-ui-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.1
+Version: 0.5.2
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -85,10 +85,10 @@
                         },
                         "text": "The Python micro framework for building web applications."
                     }
                 }
             ]
 
     *(optional)* **BEMSERVER_UI_PLUGINS = None**
-        List of absolute folder paths that locate the ``__init__.py`` file from each UI plugin package to load
+        List of absolute file paths that locate the ``__init__.py`` file from each UI plugin package to load
```

### Comparing `bemserver-ui-0.5.1/README.rst` & `bemserver-ui-0.5.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -63,8 +63,8 @@
                         },
                         "text": "The Python micro framework for building web applications."
                     }
                 }
             ]
 
     *(optional)* **BEMSERVER_UI_PLUGINS = None**
-        List of absolute folder paths that locate the ``__init__.py`` file from each UI plugin package to load
+        List of absolute file paths that locate the ``__init__.py`` file from each UI plugin package to load
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/__init__.py` & `bemserver-ui-0.5.2/bemserver_ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import flask
 
 from . import extensions
 from . import internal_api
 from . import views
 
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 
 def create_app(config_override=None):
     """Create application"""
     app = flask.Flask(__name__)
     app.config.from_object("bemserver_ui.settings.Config")
     app.config.from_envvar("BEMSERVER_UI_SETTINGS_FILE", silent=True)
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/common/time.py` & `bemserver-ui-0.5.2/bemserver_ui/common/time.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/common/tree.py` & `bemserver-ui-0.5.2/bemserver_ui/common/tree.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/__init__.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/api_client.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/auth.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/campaign_context.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/campaign_context.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/error_handlers.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/error_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     BEMServerAPINotFoundError,
     BEMServerAPIValidationError,
     BEMServerAPIPreconditionError,
     BEMServerAPINotModified,
     BEMServerAPIConflictError,
 )
 
-from bemserver_ui.extensions.campaign_context import (  # noqa: F401
+from bemserver_ui.extensions.campaign_context import (
     IGNORE_CAMPAIGN_CONTEXT_QUERY_ARG_NAME,
 )
 
 
 def _is_from_internal_api():
     if flask.request.endpoint is not None:
         return flask.request.endpoint.startswith("api.")
@@ -61,15 +61,17 @@
     if _should_handle_error(exc, http_status_code):
         message = "Incorrect or missing credentials"
         if _is_from_internal_api():
             return _handle_for_internal_api(http_status_code, message)
         flask.session.clear()
         flask.flash(message, "error")
         return flask.redirect(
-            flask.url_for("auth.signin", IGNORE_CAMPAIGN_CONTEXT_QUERY_ARG_NAME=True)
+            flask.url_for(
+                "auth.signin", **{IGNORE_CAMPAIGN_CONTEXT_QUERY_ARG_NAME: True}
+            )
         )
 
 
 def _handle_403(exc):
     http_status_code = 403
     if _should_handle_error(exc, http_status_code):
         message = "Insufficient permissions"
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/flask_es6.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/flask_es6.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/jinja_custom_filters.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/jinja_custom_filters.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/partners.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/partners.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/plugins.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/plugins.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/__init__.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-areas.json` & `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-areas.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones-full.json` & `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-full.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/extensions/timezones/timezones.py` & `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/__init__.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/completeness.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/degree_days.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/analysis/energy_consumption.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/campaign_scopes.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/campaigns.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/events.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/notifications.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/__init__.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/consumption.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/energy/production.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/production.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/semantics/weather.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/weather.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,25 +27,30 @@
     filters = {}
     if "site" in flask.request.args:
         filters["site_id"] = flask.request.args["site"]
     if "parameter" in flask.request.args:
         filters["parameter"] = flask.request.args["parameter"]
     if "timeseries" in flask.request.args:
         filters["timeseries_id"] = flask.request.args["timeseries"]
+    if "forecast" in flask.request.args:
+        filters["forecast"] = flask.request.args["forecast"]
     ts_weather_resp = flask.g.api_client.weather_ts_by_sites.getall(**filters)
     json_data = ts_weather_resp.toJSON()
     for param in json_data["data"]:
         param = _extend_data(param)
     return flask.jsonify(json_data)
 
 
 @blp.route("/", methods=["POST"])
 @auth.signin_required(roles=[Roles.admin])
 def create():
-    ts_weather_resp = flask.g.api_client.weather_ts_by_sites.create(flask.request.json)
+    payload = flask.request.json
+    if "forecast" not in payload:
+        payload["forecast"] = False
+    ts_weather_resp = flask.g.api_client.weather_ts_by_sites.create(payload)
 
     json_data = ts_weather_resp.toJSON()
     json_data["data"] = _extend_data(json_data["data"])
     return flask.jsonify(json_data)
 
 
 @blp.route("/<int:id>")
@@ -57,16 +62,19 @@
     json_data["data"] = _extend_data(json_data["data"])
     return flask.jsonify(json_data)
 
 
 @blp.route("/<int:id>", methods=["PUT"])
 @auth.signin_required(roles=[Roles.admin])
 def update(id):
+    payload = flask.request.json
+    if "forecast" not in payload:
+        payload["forecast"] = False
     ts_weather_resp = flask.g.api_client.weather_ts_by_sites.update(
-        id, flask.request.json, etag=flask.request.headers["ETag"]
+        id, payload, etag=flask.request.headers["ETag"]
     )
 
     json_data = ts_weather_resp.toJSON()
     json_data["data"] = _extend_data(json_data["data"])
     return flask.jsonify(json_data)
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/services/cleanup.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/services/missing_data.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/services/outlier_data.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/structural_elements.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/data.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Timeseries data internal API"""
 from io import StringIO
 import csv
 import zoneinfo
+import datetime as dt
 import flask
 
 from bemserver_api_client.enums import DataFormat, Aggregation, BucketWidthUnit
 from bemserver_ui.extensions import auth, ensure_campaign_context
 from bemserver_ui.common.time import (
     convert_html_form_datetime,
     convert_from_iso,
@@ -220,17 +221,20 @@
         ts_ids,
         timezone=tz_name,
     )
 
     data_stats = ts_data_stats_resp.data["stats"]
 
     tz = zoneinfo.ZoneInfo(tz_name)
+    dt_now = dt.datetime.now(tz=tz)
     for ts_stats in data_stats.values():
         try:
             dt_first = convert_from_iso(ts_stats["first_timestamp"], tz=tz)
             dt_last = convert_from_iso(ts_stats["last_timestamp"], tz=tz)
-            ts_stats["elapsed_time"] = strfdelta(dt_last - dt_first)
+            ts_stats["period_duration"] = strfdelta(dt_last - dt_first)
+            ts_stats["last_data_since"] = strfdelta(dt_now - dt_last)
         except BEMServerUICommonInvalidDatetimeError:
             # Exception raised if timestamps are None.
-            ts_stats["elapsed_time"] = None
+            ts_stats["period_duration"] = None
+            ts_stats["last_data_since"] = None
 
     return flask.jsonify(data_stats)
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/timeseries/timeseries.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/user_groups.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/internal_api/users.py` & `bemserver-ui-0.5.2/bemserver_ui/internal_api/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-ico.svg` & `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-ico.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver-min.svg` & `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-min.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.ico` & `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.ico`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/images/bemserver.svg` & `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/app.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/app.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/accordionList.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/accordionList.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/dropZone.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/dropZone.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/eventLevel.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/eventLevel.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/filterSelect.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/filterSelect.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/flash.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/flash.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/itemsCount.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/itemsCount.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/modalConfirm.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/modalConfirm.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/pagination.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/pagination.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/spinner.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/spinner.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -255,14 +255,24 @@
         this.#updateDateAndTime();
         this.#updateTzInfo();
         this.#updateStyle();
 
         this.#initEventListeners();
     }
 
+    focus(options = {
+        focusOnTime: false
+    }) {
+        if (options.focusOnTime) {
+            this.#timeInputElmt.focus();
+        } else {
+            this.#dateInputElmt.focus();
+        }
+    }
+
     reset(options = {
         ignoreDate: false,
         ignoreTime: false
     }) {
         if (!options.ignoreDate) {
             this.#date = null;
             this.#dateMin = null;
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/time/tzPicker.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/tzPicker.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/timeseries/selector.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/selector.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -672,17 +672,19 @@
 
     #createSelectedItemElement(tsData, afterRemoveSelectedCallback = null) {
         let selectedItem = new SelectedItem(tsData);
         selectedItem.addEventListener("remove", (event) => {
             event.preventDefault();
 
             let searchResultItem = this.#searchResultsContainerElmt.querySelector(`button[data-ts-id="${tsData.id.toString()}"]`);
+            if (searchResultItem == null) {
+                searchResultItem = this.#createSearchResultItemElement(tsData);
+            }
             searchResultItem.isActive = false;
 
-            this.#updateSelectedItemsContainer();
             afterRemoveSelectedCallback?.();
         });
 
         return selectedItem
     }
 
     #createSearchResultItemElement(tsData, afterRemoveSelectedCallback = null) {
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/tree.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/tree.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/flashTimer.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/flashTimer.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/formController.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/formController.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/notifications.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/notifications.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/sidebar.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/sidebar.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/array.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/array.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/fetcher.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/fetcher.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/flaskES6.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/flaskES6.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/parser.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/parser.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/time.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/time.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/tools/uuid.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/uuid.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/campaigns/selector.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaigns/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/edit.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/edit.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/events/list.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/explore.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/notifications/setup.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/setup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/list.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,600 +1,727 @@
 import {
     InternalAPIRequest
-} from "/static/scripts/modules/tools/fetcher.js";
+} from "../../tools/fetcher.js";
 import {
     flaskES6,
     signedUser
-} from "/static/scripts/app.js";
+} from "../../../app.js";
+import {
+    Spinner
+} from "../../components/spinner.js";
+import "../../components/itemsCount.js";
+import "../../components/pagination.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "/static/scripts/modules/components/flash.js";
+} from "../../components/flash.js";
 import {
-    Spinner
-} from "../../../components/spinner.js";
+    TimeDisplay
+} from "../../tools/time.js";
 import {
-    FilterSelect
-} from "/static/scripts/modules/components/filterSelect.js";
-import "/static/scripts/modules/components/itemsCount.js";
-import "/static/scripts/modules/components/time/datetimePicker.js";
+    EventLevelBadge
+} from "../../components/eventLevel.js";
+import "../../components/tree.js";
 
 
-class WeatherDataServiceManageView {
-
-    #internalAPIRequester = null;
-    #listReqID = null;
-    #updateStateReqID = null;
-    #getSvcEtagReqID = null;
-    #getSemanticsReqID = null;
+export class StructuralElementsExploreView {
 
+    #tzName = "UTC";
     #messagesElmt = null;
 
-    #filtersContainerElmt = null;
-    #siteNameSearchElmt = null;
-    #serviceStateFilterElmt = null;
-    #removeFiltersBtnElmt = null;
-
-    #itemsCountElmt = null;
-    #serviceStatesContainerElmt = null;
-
-    #fetchDataModalElmt = null;
-    #fetchDataModal = null;
-    #fetchDataSiteIdElmt = null;
-    #fetchDataDatetimeStartElmt = null;
-    #fetchDataDatetimeEndElmt = null;
-    #fetchDataBtnElmt = null;
-    #fetchDataModalParamsContainerElmt = null;
+    #internalAPIRequester = null;
+    #generalReqID = null;
+    #propertiesReqID = null;
+    #tsReqID = null;
+    #eventsReqID = null;
+    #sitesTreeReqID = null;
+    #zonesTreeReqID = null;
+
+    #tabSitesElmts = null;
+    #tabPropertiesElmts = null;
+    #generalTabContentElmt = null;
+    #propertiesTabContentElmt = null;
+
+    #tsSearchElmt = null;
+    #tsClearSearchBtnElmt = null;
+    #tsRecurseSwitchElmt = null;
+    #tsPageSizeElmt = null;
+    #tsCountElmt = null;
+    #tsPaginationElmt = null;
+    #tsListElmt = null;
+
+    #eventsSearchElmt = null;
+    #eventsClearSearchBtnElmt = null;
+    #eventsRecurseSwitchElmt = null;
+    #eventsPageSizeElmt = null;
+    #eventsCountElmt = null;
+    #eventsPaginationElmt = null;
+    #eventsListElmt = null;
+
+    #tabSitesSelected = null;
+    #tabPropertiesSelected = null;
+
+    #selectedItemsPerTab = {};
+    #renderPerTab = {
+        "general-tab": this.#renderGeneral.bind(this),
+        "properties-tab": this.#renderProperties.bind(this),
+        "timeseries-tab": this.#renderTimeseries.bind(this),
+        "events-tab": this.#renderEvents.bind(this),
+    }
+    #alreadyLoadedPerTab = {};
+
+    #sitesTreeElmt = null;
+    #zonesTreeElmt = null;
 
-    constructor() {
+    constructor(options = {}) {
         this.#internalAPIRequester = new InternalAPIRequest();
 
+        this.#loadOptions(options);
         this.#cacheDOM();
-        this.#initFilters();
         this.#initEventListeners();
+
+        this.#updateTsSearchState();
+        this.#updateEventsSearchState();
+    }
+
+    #loadOptions(options = {}) {
+        this.#tzName = options.timezone || "UTC";
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
-        this.#filtersContainerElmt = document.getElementById("filtersContainer");
-        this.#siteNameSearchElmt = document.getElementById("siteNameSearch");
-        this.#removeFiltersBtnElmt = document.getElementById("removeFiltersBtn");
+        this.#tabSitesElmts = [].slice.call(document.querySelectorAll("#tabSites button[data-bs-toggle='tab']"));
+        this.#tabPropertiesElmts = [].slice.call(document.querySelectorAll("#tabProperties button[data-bs-toggle='tab']"));
+        this.#generalTabContentElmt = document.getElementById("general-tabcontent");
+        this.#propertiesTabContentElmt = document.getElementById("properties-tabcontent");
+
+        this.#tsSearchElmt = document.getElementById("tsSearch");
+        this.#tsClearSearchBtnElmt = document.getElementById("tsClear");
+        this.#tsRecurseSwitchElmt = document.getElementById("tsRecurseSwitch");
+        this.#tsPageSizeElmt = document.getElementById("tsPageSize");
+        this.#tsCountElmt = document.getElementById("tsCount");
+        this.#tsPaginationElmt = document.getElementById("tsPagination");
+        this.#tsListElmt = document.getElementById("tsList");
+
+        this.#eventsSearchElmt = document.getElementById("eventsSearch");
+        this.#eventsClearSearchBtnElmt = document.getElementById("eventsClear");
+        this.#eventsRecurseSwitchElmt = document.getElementById("eventsRecurseSwitch");
+        this.#eventsPageSizeElmt = document.getElementById("eventsPageSize");
+        this.#eventsCountElmt = document.getElementById("eventsCount");
+        this.#eventsPaginationElmt = document.getElementById("eventsPagination");
+        this.#eventsListElmt = document.getElementById("eventsList");
 
-        this.#itemsCountElmt = document.getElementById("itemsCount");
-        this.#serviceStatesContainerElmt = document.getElementById("serviceStatesContainer");
+        this.#sitesTreeElmt = document.getElementById("sitesTree");
+        this.#zonesTreeElmt = document.getElementById("zonesTree");
+    }
 
-        if (signedUser.is_admin) {
-            this.#fetchDataModalElmt = document.getElementById("fetchDataModal");
-            this.#fetchDataModal = new bootstrap.Modal(this.#fetchDataModalElmt);
-            this.#fetchDataSiteIdElmt = document.getElementById("fetchDataSiteId");
-            this.#fetchDataDatetimeStartElmt = document.getElementById("fetchDataDatetimeStart");
-            this.#fetchDataDatetimeEndElmt = document.getElementById("fetchDataDatetimeEnd");
-            this.#fetchDataBtnElmt = document.getElementById("fetchDataBtn");
-            this.#fetchDataModalParamsContainerElmt = document.getElementById("fetchDataModalParamsContainer");
+    #initEventListeners() {
+        for (let tabElmt of this.#tabSitesElmts) {
+            if (tabElmt.classList.contains("active")) {
+                this.#tabSitesSelected = tabElmt;
+            }
+            this.#selectedItemsPerTab[tabElmt.id] = null;
+            tabElmt.addEventListener("shown.bs.tab", (event) => {
+                // newly activated tab is `event.target` ; previous active tab is `event.relatedTarget`
+                this.#tabSitesSelected = event.target;
+                for (let tabPropertyElmt of this.#tabPropertiesElmts) {
+                    this.#alreadyLoadedPerTab[tabPropertyElmt.id] = false;
+                }
+                this.#refreshTabs();
+            });
         }
-    }
 
-    #initFilters() {
-        this.#serviceStateFilterElmt = new FilterSelect();
-        this.#filtersContainerElmt.insertBefore(this.#serviceStateFilterElmt, this.#removeFiltersBtnElmt);
-        this.#serviceStateFilterElmt.load([{
-            value: "all",
-            text: "All"
-        }, {
-            value: "on",
-            text: "ON"
-        }, {
-            value: "off",
-            text: "OFF"
-        }, ]);
-        this.#serviceStateFilterElmt.setAttribute("data-default", "all");
-    }
+        for (let tabElmt of this.#tabPropertiesElmts) {
+            if (tabElmt.classList.contains("active")) {
+                this.#tabPropertiesSelected = tabElmt;
+            }
+            this.#alreadyLoadedPerTab[tabElmt.id] = false;
+            tabElmt.addEventListener("shown.bs.tab", (event) => {
+                // newly activated tab is `event.target` ; previous active tab is `event.relatedTarget`
+                this.#tabPropertiesSelected = event.target;
+                this.#refreshTabs();
+            });
+        }
 
-    #initEventListeners() {
-        this.#siteNameSearchElmt.addEventListener("input", (event) => {
+        this.#tsSearchElmt.addEventListener("input", (event) => {
             event.preventDefault();
 
-            this.#updateSiteNameSearch();
-            this.#refreshList();
+            this.#updateTsSearchState();
+
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#tsPaginationElmt.page = 1;
+            this.#refreshTabs();
         });
 
-        this.#serviceStateFilterElmt.addEventListener("change", (event) => {
+        this.#tsClearSearchBtnElmt.addEventListener("click", (event) => {
             event.preventDefault();
 
-            this.#refreshList();
+            this.#tsSearchElmt.value = "";
+            this.#updateTsSearchState();
+
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#refreshTabs();
         });
 
-        this.#removeFiltersBtnElmt.addEventListener("click", (event) => {
+        this.#tsRecurseSwitchElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            let hasFilterChanged = false;
-            if (this.#siteNameSearchElmt.value != "") {
-                this.#siteNameSearchElmt.value = "";
-                this.#updateSiteNameSearch();
-                hasFilterChanged = true;
-            }
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#refreshTabs();
+        });
 
-            let serviceStateFilterDefault = this.#serviceStateFilterElmt.getAttribute("data-default");
-            if (this.#serviceStateFilterElmt.value != serviceStateFilterDefault) {
-                this.#serviceStateFilterElmt.reset();
-                hasFilterChanged = true;
-            }
+        this.#tsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
+            event.preventDefault();
 
-            if (hasFilterChanged) {
-                this.#refreshList();
+            if (event.detail.newValue != event.detail.oldValue) {
+                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+                this.#tsPaginationElmt.page = 1;
+                this.#refreshTabs();
             }
         });
 
-        if (signedUser.is_admin) {
-            this.#fetchDataDatetimeStartElmt.addEventListener("datetimeChange", (event) => {
-                event.preventDefault();
+        this.#tsPaginationElmt.addEventListener("pageItemClick", (event) => {
+            event.preventDefault();
 
-                this.#fetchDataDatetimeEndElmt.dateMin = this.#fetchDataDatetimeStartElmt.date;
-                this.#updateFetchDataBtn();
-            });
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#refreshTabs();
+        });
 
-            this.#fetchDataDatetimeEndElmt.addEventListener("datetimeChange", (event) => {
-                event.preventDefault();
+        this.#eventsSearchElmt.addEventListener("input", (event) => {
+            event.preventDefault();
 
-                this.#fetchDataDatetimeStartElmt.dateMax = this.#fetchDataDatetimeEndElmt.date;
-                this.#updateFetchDataBtn();
-            });
+            this.#updateEventsSearchState();
 
-            this.#fetchDataBtnElmt.addEventListener("click", () => {
-                this.#internalAPIRequester.put(
-                    flaskES6.urlFor(`api.structural_elements.fetch_weather_data`, {
-                        id: this.#fetchDataSiteIdElmt.value
-                    }), {
-                        "start_date": this.#fetchDataDatetimeStartElmt.date,
-                        "start_time": this.#fetchDataDatetimeStartElmt.time,
-                        "end_date": this.#fetchDataDatetimeEndElmt.date,
-                        "end_time": this.#fetchDataDatetimeEndElmt.time,
-                    },
-                    null,
-                    () => {
-                        let flashMsgElmt = new FlashMessage({
-                            type: FlashMessageTypes.INFO,
-                            text: `Command sent with success. Weather data will be fetched soon.`,
-                            isDismissible: true
-                        });
-                        this.#messagesElmt.appendChild(flashMsgElmt);
-
-                        this.#fetchDataModal.hide();
-                    },
-                    (error) => {
-                        let flashMsgElmt = new FlashMessage({
-                            type: FlashMessageTypes.ERROR,
-                            text: error.toString(),
-                            isDismissible: true
-                        });
-                        this.#messagesElmt.appendChild(flashMsgElmt);
-
-                        this.#fetchDataModal.hide();
-                    },
-                );
-            });
-        }
-    }
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#eventsPaginationElmt.page = 1;
+            this.#refreshTabs();
+        });
 
-    #updateSiteNameSearch() {
-        if (this.#siteNameSearchElmt.value == "") {
-            this.#siteNameSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
-        } else if (!this.#siteNameSearchElmt.classList.contains("border-info")) {
-            this.#siteNameSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
-        }
-    }
+        this.#eventsClearSearchBtnElmt.addEventListener("click", (event) => {
+            event.preventDefault();
 
-    #updateFetchDataBtn() {
-        if (this.#fetchDataDatetimeStartElmt.date != null && this.#fetchDataDatetimeStartElmt.time != null && this.#fetchDataDatetimeEndElmt.date != null && this.#fetchDataDatetimeEndElmt.time != null) {
-            this.#fetchDataBtnElmt.removeAttribute("disabled");
-        } else {
-            this.#fetchDataBtnElmt.setAttribute("disabled", true);
-        }
-    }
+            this.#eventsSearchElmt.value = "";
+            this.#updateEventsSearchState();
 
-    #createEntryElement(serviceStateData) {
-        let trElmt = document.createElement("tr");
-        trElmt.classList.add("align-middle");
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#refreshTabs();
+        });
 
-        let thElmt = document.createElement("th");
-        thElmt.classList.add("text-break");
-        thElmt.setAttribute("scope", "row");
-        thElmt.innerText = serviceStateData.site_name;
-        trElmt.appendChild(thElmt);
+        this.#eventsRecurseSwitchElmt.addEventListener("change", (event) => {
+            event.preventDefault();
 
-        let svcCtrlElmt = document.createElement("div");
-        svcCtrlElmt.classList.add("d-flex", "gap-1", "my-auto", "placeholder-glow");
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#refreshTabs();
+        });
 
-        if (signedUser.is_admin) {
-            let svcEtagInputElmt = document.createElement("input");
-            svcEtagInputElmt.setAttribute("type", "hidden");
-            svcCtrlElmt.appendChild(svcEtagInputElmt);
-
-            let svcOnInputElmt = document.createElement("input");
-            svcOnInputElmt.id = `radio-svc-state-${serviceStateData.site_id}-on`;
-            svcOnInputElmt.name = `radio-svc-state-${serviceStateData.site_id}`;
-            svcOnInputElmt.classList.add("btn-check");
-            svcOnInputElmt.setAttribute("type", "radio");
-            svcOnInputElmt.setAttribute("autocomplete", "off");
-            svcCtrlElmt.appendChild(svcOnInputElmt);
-
-            let svcOnLabelElmt = document.createElement("label");
-            svcOnLabelElmt.classList.add("btn", "btn-sm", "btn-outline-success");
-            svcOnLabelElmt.setAttribute("for", svcOnInputElmt.id);
-            svcOnLabelElmt.setAttribute("title", "Enable service");
-            svcOnLabelElmt.innerText = "ON";
-            svcCtrlElmt.appendChild(svcOnLabelElmt);
-
-            let svcOffInputElmt = document.createElement("input");
-            svcOffInputElmt.id = `radio-svc-state-${serviceStateData.site_id}-off`;
-            svcOffInputElmt.name = `radio-svc-state-${serviceStateData.site_id}`;
-            svcOffInputElmt.classList.add("btn-check");
-            svcOffInputElmt.setAttribute("type", "radio");
-            svcOffInputElmt.setAttribute("autocomplete", "off");
-            svcCtrlElmt.appendChild(svcOffInputElmt);
-
-            let svcOffLabelElmt = document.createElement("label");
-            svcOffLabelElmt.classList.add("btn", "btn-sm", "btn-outline-danger");
-            svcOffLabelElmt.setAttribute("for", svcOffInputElmt.id);
-            svcOffLabelElmt.setAttribute("title", "Disable service");
-            svcOffLabelElmt.innerText = "OFF";
-            svcCtrlElmt.appendChild(svcOffLabelElmt);
-
-            let updateSvcInputState = () => {
-                if (serviceStateData.is_enabled) {
-                    svcOffInputElmt.removeAttribute("checked");
-                    svcOnInputElmt.setAttribute("checked", "true");
-                } else {
-                    svcOnInputElmt.removeAttribute("checked");
-                    svcOffInputElmt.setAttribute("checked", "true");
-                }
+        this.#eventsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
+            event.preventDefault();
 
-                svcOnLabelElmt.classList.remove("placeholder");
-                svcOffLabelElmt.classList.remove("placeholder");
+            if (event.detail.newValue != event.detail.oldValue) {
+                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+                this.#eventsPaginationElmt.page = 1;
+                this.#refreshTabs();
             }
+        });
 
+        this.#eventsPaginationElmt.addEventListener("pageItemClick", (event) => {
+            event.preventDefault();
+
+            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
+            this.#refreshTabs();
+        });
 
-            updateSvcInputState();
+        this.#sitesTreeElmt.addEventListener("treeNodeSelect", (event) => {
+            this.render(event.detail.id, event.detail.type, event.detail.path);
+        });
 
+        this.#zonesTreeElmt.addEventListener("treeNodeSelect", (event) => {
+            this.render(event.detail.id, event.detail.type, event.detail.path);
+        });
+    }
 
-            let updateServiceState = (isEnabled) => {
-                svcOnLabelElmt.classList.add("placeholder");
-                svcOffLabelElmt.classList.add("placeholder");
+    #updateTsSearchState() {
+        if (this.#tsSearchElmt.value != "") {
+            this.#tsSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
+            this.#tsClearSearchBtnElmt.classList.remove("d-none", "invisible");
+        } else {
+            this.#tsSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
+            this.#tsClearSearchBtnElmt.classList.add("d-none", "invisible");
+        }
+    }
 
-                if (this.#updateStateReqID != null) {
-                    this.#internalAPIRequester.abort(this.#updateStateReqID);
-                    this.#updateStateReqID = null;
-                }
+    #updateEventsSearchState() {
+        if (this.#eventsSearchElmt.value != "") {
+            this.#eventsSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
+            this.#eventsClearSearchBtnElmt.classList.remove("d-none", "invisible");
+        } else {
+            this.#eventsSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
+            this.#eventsClearSearchBtnElmt.classList.add("d-none", "invisible");
+        }
+    }
 
-                if (serviceStateData.id == null) {
-                    if (isEnabled) {
-                        // Enable weather data service for site.
-                        this.#updateStateReqID = this.#internalAPIRequester.post(
-                            flaskES6.urlFor(`api.services.weather_data.enable`), {
-                                site_id: serviceStateData.site_id,
-                                is_enabled: isEnabled
-                            },
-                            (data) => {
-                                serviceStateData = data.data;
-                                svcEtagInputElmt.value = data.etag;
-                                updateSvcInputState();
-
-                                let flashMsgElmt = new FlashMessage({
-                                    type: FlashMessageTypes.INFO,
-                                    text: "Weather data service enabled!",
-                                    isDismissible: true
-                                });
-                                this.#messagesElmt.appendChild(flashMsgElmt);
-                            },
-                            (error) => {
-                                let flashMsgElmt = new FlashMessage({
-                                    type: FlashMessageTypes.ERROR,
-                                    text: error.toString(),
-                                    isDismissible: true
-                                });
-                                this.#messagesElmt.appendChild(flashMsgElmt);
-
-                                svcOnLabelElmt.classList.remove("placeholder");
-                                svcOffLabelElmt.classList.remove("placeholder");
-                            },
-                        );
-                    }
-                } else {
-                    let _updateSvcState = (isEnabled) => {
-                        // Update weather data service state for site.
-                        this.#updateStateReqID = this.#internalAPIRequester.put(
-                            flaskES6.urlFor(`api.services.weather_data.update_state`, {
-                                id: serviceStateData.id
-                            }), {
-                                is_enabled: isEnabled
-                            },
-                            svcEtagInputElmt.value,
-                            (data) => {
-                                serviceStateData = data.data;
-                                svcEtagInputElmt.value = data.etag;
-                                updateSvcInputState();
-
-                                let flashMsgElmt = new FlashMessage({
-                                    type: FlashMessageTypes.INFO,
-                                    text: `Weather data service ${isEnabled ? "en": "dis"}abled!`,
-                                    isDismissible: true
-                                });
-                                this.#messagesElmt.appendChild(flashMsgElmt);
-                            },
-                            (error) => {
-                                let flashMsgElmt = new FlashMessage({
-                                    type: FlashMessageTypes.ERROR,
-                                    text: error.toString(),
-                                    isDismissible: true
-                                });
-                                this.#messagesElmt.appendChild(flashMsgElmt);
-
-                                updateSvcInputState();
-                            },
-                        );
-                    }
-
-                    if (svcEtagInputElmt.value == "") {
-                        if (this.#getSvcEtagReqID != null) {
-                            this.#internalAPIRequester.abort(this.#getSvcEtagReqID);
-                            this.#getSvcEtagReqID = null;
-                        }
-
-                        this.#getSvcEtagReqID = this.#internalAPIRequester.get(
-                            flaskES6.urlFor(`api.services.weather_data.retrieve_one`, {
-                                id: serviceStateData.id
-                            }),
-                            (data) => {
-                                svcEtagInputElmt.value = data.etag;
-                                _updateSvcState(true);
-                            },
-                            (error) => {
-                                let flashMsgElmt = new FlashMessage({
-                                    type: FlashMessageTypes.ERROR,
-                                    text: error.toString(),
-                                    isDismissible: true
-                                });
-                                this.#messagesElmt.appendChild(flashMsgElmt);
-
-                                updateSvcInputState();
-                            },
-                        );
-                    } else {
-                        _updateSvcState(isEnabled);
-                    }
-                }
+    #getEditBtnHTML(type, id, tab = null) {
+        if (signedUser.is_admin) {
+            let editUrlParams = {
+                type: type,
+                id: id
             };
+            if (tab != null) {
+                editUrlParams["tab"] = tab;
+            }
+            try {
+                let editUrl = flaskES6.urlFor(`structural_elements.edit`, editUrlParams);
+                return `<a class="btn btn-sm btn-outline-primary text-nowrap" href="${editUrl}" role="button" title="Edit ${type}"><i class="bi bi-pencil"></i> Edit</a>`;
+            } catch (error) {
+                let flashMsgElmt = new FlashMessage({
+                    type: FlashMessageTypes.ERROR,
+                    text: error,
+                    isDismissible: true
+                });
+                this.#messagesElmt.appendChild(flashMsgElmt);
+            }
+        }
+        return ``;
+    }
 
+    #getGeneralHTML(data, path) {
+        let htmlContent = `<div class="d-flex justify-content-between align-items-start gap-3 mb-3">
+    <div>
+        <h5 class="text-break">${data.structural_element.name}</h5>
+        <h6 class="text-break">${path}</h6>
+    </div>
+    ${this.#getEditBtnHTML(data.type, data.structural_element.id)}
+</div>
+<p class="fst-italic text-muted text-break">${data.structural_element.description}</p>
+<div class="row">
+    <dl class="col">
+        <dt>IFC ID</dt>
+        <dd>${(data.structural_element.ifc_id != null && data.structural_element.ifc_id != "") ? data.structural_element.ifc_id : "-"}</dd>
+    </dl>
+</div>`;
+
+        if (data.type == "site") {
+            htmlContent += `<div class="row">
+    <dl class="col">
+        <dt>Latitude <small class="text-muted">[°]</small></dt>
+        <dd>${data.structural_element.latitude != null ? data.structural_element.latitude : "-"}</dd>
+    </dl>
+    <dl class="col">
+        <dt>Longitude <small class="text-muted">[°]</small></dt>
+        <dd>${data.structural_element.longitude != null ? data.structural_element.longitude : "-"}</dd>
+    </dl>
+</div>`;
+        }
 
-            svcOnInputElmt.addEventListener("change", () => {
-                if (svcOnInputElmt.checked) {
-                    updateServiceState(true);
-                }
-            });
+        return htmlContent;
+    }
 
-            svcOffInputElmt.addEventListener("change", () => {
-                if (svcOffInputElmt.checked) {
-                    updateServiceState(false);
-                }
-            });
-        } else {
-            let spanStateElmt = document.createElement("span");
-            spanStateElmt.classList.add("fw-bold", "text-opacity-75");
-            if (serviceStateData.is_enabled) {
-                spanStateElmt.classList.add("text-success");
-                spanStateElmt.innerText = "ON";
-            } else {
-                spanStateElmt.classList.add("text-danger");
-                spanStateElmt.innerText = "OFF";
-            }
-            svcCtrlElmt.appendChild(spanStateElmt);
+    #getItemHelpHTML(itemDescription, withSpace = true) {
+        let ret = ``;
+        if (itemDescription?.length > 0) {
+            let abbrElmt = document.createElement("abbr");
+            abbrElmt.title = itemDescription != null ? itemDescription : "";
+            let abbrContentElmt = document.createElement("i");
+            abbrContentElmt.classList.add("bi", "bi-question-diamond");
+            abbrElmt.appendChild(abbrContentElmt);
+            ret = `<sup${withSpace ? ` class="ms-1"`: ``}>${abbrElmt.outerHTML}</sup>`;
         }
+        return ret;
+    }
 
-        let tdStateElmt = document.createElement("td");
-        tdStateElmt.classList.add("d-flex", "gap-4");
-        tdStateElmt.appendChild(svcCtrlElmt);
-        trElmt.appendChild(tdStateElmt);
-
-        if (signedUser.is_admin) {
-            if (serviceStateData.id == null) {
-                let warnAlertElmt = this.#createWarnAlertElement("Never launched yet");
-                tdStateElmt.appendChild(warnAlertElmt);
+    #getPropertiesHTML(data, id) {
+        let propertyDataHTML = ``;
+        if (data.properties.length > 0) {
+            for (let property of data.properties) {
+                let unitSymbol = (property.unit_symbol != null && property.unit_symbol.length > 0) ? `<small class="text-muted ms-1">[${property.unit_symbol}]</small>` : ``;
+                propertyDataHTML += `<dl>
+    <dt>${property.name}${unitSymbol}${this.#getItemHelpHTML(property.description)}</dt>
+    <dd>${(property.value !== "" && property.value != null) ? property.value : "-"}</dd>
+</dl>`;
             }
+        } else {
+            propertyDataHTML = `<p class="fst-italic">No data</p>`;
+        }
 
-            // Verify that the site has long/lat coordinates.
-            let warnSiteCoordElmt = null;
-            this.#internalAPIRequester.get(
-                flaskES6.urlFor(`api.structural_elements.retrieve_data`, {
-                    type: "site",
-                    id: serviceStateData.site_id
-                }),
-                (data) => {
-                    if (data.structural_element.latitude == null || data.structural_element.longitude == null) {
-                        warnSiteCoordElmt = this.#createWarnAlertElement("Site latitude/longitude coordinates are not defined!");
-                        tdStateElmt.appendChild(warnSiteCoordElmt);
-                    }
-                },
-                (error) => {
-                    let flashMsgElmt = new FlashMessage({
-                        type: FlashMessageTypes.ERROR,
-                        text: error.toString(),
-                        isDismissible: true
-                    });
-                    this.#messagesElmt.appendChild(flashMsgElmt);
-                },
-            );
-
-            let tdFetchElmt = document.createElement("td");
-            trElmt.appendChild(tdFetchElmt);
-
-            let fetchLinkElmt = document.createElement("a");
-            fetchLinkElmt.classList.add("btn", "btn-sm", "btn-outline-primary");
-            fetchLinkElmt.setAttribute("role", "button");
-            fetchLinkElmt.setAttribute("title", "Fetch weather data from external service");
-            fetchLinkElmt.setAttribute("data-bs-toggle", "modal");
-            fetchLinkElmt.setAttribute("data-bs-target", `#${this.#fetchDataModalElmt.id}`);
-            tdFetchElmt.appendChild(fetchLinkElmt);
-
-            let fetchIconElmt = document.createElement("i");
-            fetchIconElmt.classList.add("bi", "bi-cloud-download");
-            fetchLinkElmt.appendChild(fetchIconElmt);
-
-            fetchLinkElmt.addEventListener("click", () => {
-                this.#fetchDataSiteIdElmt.value = serviceStateData.site_id.toString();
-                this.#fetchDataDatetimeStartElmt.reset({
-                    ignoreTime: true
-                });
-                this.#fetchDataDatetimeEndElmt.reset({
-                    ignoreTime: true
-                });
-                this.#updateFetchDataBtn();
+        return `<div class="d-flex justify-content-between align-items-start mb-3">
+    <div class="d-flex gap-4">
+        ${propertyDataHTML}
+    </div>
+    ${this.#getEditBtnHTML(data.type, id, "properties")}
+</div>`;
+    }
+
+    #getErrorHTML(error) {
+        return `<div class="alert alert-danger" role="alert">
+    <i class="bi bi-x-octagon me-2"></i>
+    ${error}
+</div>`;
+    }
+
+    #renderGeneral(id, type, path) {
+        this.#generalTabContentElmt.innerHTML = "";
+        this.#generalTabContentElmt.appendChild(new Spinner());
+
+        if (this.#generalReqID != null) {
+            this.#internalAPIRequester.abort(this.#generalReqID);
+            this.#generalReqID = null;
+        }
+        this.#generalReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.structural_elements.retrieve_data`, {
+                type: type,
+                id: id
+            }),
+            (data) => {
+                this.#generalTabContentElmt.innerHTML = this.#getGeneralHTML(data, path);
+            },
+            (error) => {
+                this.#generalTabContentElmt.innerHTML = this.#getErrorHTML(error.message);
+            },
+        );
+    }
 
-                this.#fetchDataModalParamsContainerElmt.innerHTML = "";
-                this.#fetchDataModalParamsContainerElmt.appendChild(new Spinner());
+    #renderProperties(id, type, path) {
+        this.#propertiesTabContentElmt.innerHTML = "";
+        this.#propertiesTabContentElmt.appendChild(new Spinner());
+
+        if (this.#propertiesReqID != null) {
+            this.#internalAPIRequester.abort(this.#propertiesReqID);
+            this.#propertiesReqID = null;
+        }
+        this.#propertiesReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.structural_elements.retrieve_property_data`, {
+                type: type,
+                id: id
+            }),
+            (data) => {
+                this.#propertiesTabContentElmt.innerHTML = this.#getPropertiesHTML(data, id);
+            },
+            (error) => {
+                this.#propertiesTabContentElmt.innerHTML = this.#getErrorHTML(error.message);
+            },
+        );
+    }
 
-                if (this.#getSemanticsReqID != null) {
-                    this.#internalAPIRequester.abort(this.#getSemanticsReqID);
-                    this.#getSemanticsReqID = null;
+    #populateTimeseriesList(tsList) {
+        this.#tsListElmt.innerHTML = "";
+        if (tsList.length > 0) {
+            for (let tsData of tsList) {
+                let tsElmt = document.createElement("div");
+                tsElmt.classList.add("list-group-item");
+
+                let tsHeaderElmt = document.createElement("div");
+                tsHeaderElmt.classList.add("d-flex", "gap-1");
+
+                let iconElmt = document.createElement("i");
+                iconElmt.classList.add("bi", "bi-clock-history", "me-1");
+                tsHeaderElmt.appendChild(iconElmt);
+
+                let nameSpanElmt = document.createElement("span");
+                nameSpanElmt.classList.add("fw-bold", "text-break");
+                nameSpanElmt.innerText = tsData.name;
+                tsHeaderElmt.appendChild(nameSpanElmt);
+
+                if (tsData.unit_symbol) {
+                    let unitSpanElmt = document.createElement("span");
+                    unitSpanElmt.classList.add("text-muted");
+                    unitSpanElmt.innerText = `[${tsData.unit_symbol}]`;
+                    tsHeaderElmt.appendChild(unitSpanElmt);
                 }
 
-                this.#getSemanticsReqID = this.#internalAPIRequester.get(
-                    flaskES6.urlFor(`api.semantics.weather.list`, {
-                        site: serviceStateData.site_id
-                    }),
-                    (data) => {
-                        this.#fetchDataModalParamsContainerElmt.innerHTML = "";
-
-                        if (data.data.length > 0) {
-                            let weatherParamsTitleElmt = document.createElement("h6");
-                            weatherParamsTitleElmt.innerText = `${data.data.length} weather parameter${data.data.length > 1 ? "s" : ""} will be fetched:`;
-                            this.#fetchDataModalParamsContainerElmt.appendChild(weatherParamsTitleElmt);
-
-                            let weatherParamsListElmt = document.createElement("dl");
-                            weatherParamsListElmt.classList.add("d-flex", "flex-wrap", "gap-3");
-                            this.#fetchDataModalParamsContainerElmt.appendChild(weatherParamsListElmt);
-                            for (let weatherParam of data.data) {
-                                let weatherParamsListItemElmt = document.createElement("div");
-                                weatherParamsListElmt.appendChild(weatherParamsListItemElmt);
-
-                                let weatherParamsListItemTitleElmt = document.createElement("dt");
-                                weatherParamsListItemTitleElmt.innerText = `${weatherParam["parameter_label"]}`;
-                                weatherParamsListItemElmt.appendChild(weatherParamsListItemTitleElmt);
-
-                                let weatherParamsListItemTextElmt = document.createElement("dd");
-                                weatherParamsListItemTextElmt.innerText = `${weatherParam["timeseries"]["name"]}${weatherParam["timeseries"]["unit_symbol"] != null ? ` [${weatherParam["timeseries"]["unit_symbol"]}]` : ""}`;
-                                weatherParamsListItemElmt.appendChild(weatherParamsListItemTextElmt);
-                            }
-                        } else {
-                            let warnAlertElmt = this.#createWarnAlertElement("No weather parameter to fetch. You should set timeseries semantics for weather parameters.");
-                            this.#fetchDataModalParamsContainerElmt.appendChild(warnAlertElmt);
-                        }
-
-                        if (warnSiteCoordElmt != null) {
-                            this.#fetchDataModalParamsContainerElmt.appendChild(warnSiteCoordElmt);
-                        }
-                    },
-                    (error) => {
-                        let flashMsgElmt = new FlashMessage({
-                            type: FlashMessageTypes.ERROR,
-                            text: error.toString(),
-                            isDismissible: true
-                        });
-                        this.#messagesElmt.appendChild(flashMsgElmt);
-                    },
-                );
-            });
+                tsElmt.appendChild(tsHeaderElmt);
+
+                let tsDescElmt = document.createElement("small");
+                tsDescElmt.classList.add("fst-italic", "text-muted");
+                tsDescElmt.innerText = tsData.description != null ? tsData.description : "-";
+                tsElmt.appendChild(tsDescElmt);
+
+                this.#tsListElmt.appendChild(tsElmt);
+            }
+        } else {
+            let nodataSpanElmt = document.createElement("span");
+            nodataSpanElmt.classList.add("fst-italic", "text-muted", "text-center");
+            nodataSpanElmt.innerText = "No data";
+            this.#tsListElmt.appendChild(nodataSpanElmt);
         }
+    }
+
+    #populateEventList(eventsList) {
+        this.#eventsListElmt.innerHTML = "";
+        if (eventsList.length > 0) {
+            for (let eventData of eventsList) {
+                let eventElmt = document.createElement("div");
+                eventElmt.classList.add("list-group-item");
+
+                let eventHeaderElmt = document.createElement("div");
+                eventHeaderElmt.classList.add("d-flex", "align-items-center", "gap-1", "w-100");
+                eventElmt.appendChild(eventHeaderElmt);
+
+                let iconElmt = document.createElement("i");
+                iconElmt.classList.add("bi", "bi-journal-x", "me-1");
+                eventHeaderElmt.appendChild(iconElmt);
+
+                let headerContentElmt = document.createElement("div");
+                headerContentElmt.classList.add("d-flex", "justify-content-between", "align-items-center", "gap-2", "w-100");
+                eventHeaderElmt.appendChild(headerContentElmt);
+
+                let timestampElmt = document.createElement("h6");
+                timestampElmt.classList.add("text-nowrap", "mb-0");
+                timestampElmt.innerText = TimeDisplay.toLocaleString(new Date(eventData.timestamp), {
+                    timezone: this.#tzName
+                });
+                headerContentElmt.appendChild(timestampElmt);
+
+                let levelBadgeElmt = new EventLevelBadge();
+                levelBadgeElmt.setAttribute("level", eventData.level.toUpperCase());
+                headerContentElmt.appendChild(levelBadgeElmt);
+
+                let bodyContentElmt = document.createElement("div");
+                bodyContentElmt.classList.add("d-flex", "justify-content-between", "align-items-start", "gap-2");
+                eventElmt.appendChild(bodyContentElmt);
+
+                let eventDescElmt = document.createElement("small");
+                eventDescElmt.classList.add("fst-italic", "text-muted");
+                eventDescElmt.innerText = eventData.description;
+                bodyContentElmt.appendChild(eventDescElmt);
+
+                let sourceElmt = document.createElement("span");
+                sourceElmt.classList.add("text-nowrap");
+                sourceElmt.innerText = eventData.source;
+                bodyContentElmt.appendChild(sourceElmt);
 
-        return trElmt;
+                this.#eventsListElmt.appendChild(eventElmt);
+            }
+        } else {
+            let nodataSpanElmt = document.createElement("span");
+            nodataSpanElmt.classList.add("fst-italic", "text-muted", "text-center");
+            nodataSpanElmt.innerText = "No data";
+            this.#eventsListElmt.appendChild(nodataSpanElmt);
+        }
     }
 
-    #createWarnAlertElement(text) {
-        let warnContainerElmt = document.createElement("div");
-        warnContainerElmt.classList.add("alert", "alert-warning", "border", "border-warning", "mb-0", "py-1");
-        warnContainerElmt.setAttribute("role", "alert");
+    #renderTimeseries(id, type, path) {
+        this.#tsCountElmt.setLoading();
+        this.#tsListElmt.innerHTML = "";
+        this.#tsListElmt.appendChild(new Spinner());
+
+        if (this.#tsReqID != null) {
+            this.#internalAPIRequester.abort(this.#tsReqID);
+            this.#tsReqID = null;
+        }
 
-        let warnIconElmt = document.createElement("i");
-        warnIconElmt.classList.add("bi", "bi-exclamation-triangle", "me-1");
-        warnContainerElmt.appendChild(warnIconElmt);
+        if (["space", "zone"].includes(type)) {
+            this.#tsRecurseSwitchElmt.checked = false;
+            this.#tsRecurseSwitchElmt.setAttribute("disabled", true);
+        } else {
+            this.#tsRecurseSwitchElmt.removeAttribute("disabled");
+        }
 
-        let warnTextElmt = document.createElement("span");
-        warnTextElmt.classList.add("fst-italic");
-        warnTextElmt.innerText = text;
-        warnContainerElmt.appendChild(warnTextElmt);
+        let tsOptions = {
+            "page_size": this.#tsPageSizeElmt.current,
+            "page": this.#tsPaginationElmt.page,
+        };
+        tsOptions[`${this.#tsRecurseSwitchElmt.checked ? "recurse_" : ""}${type}_id`] = id;
+        if (this.#tsSearchElmt.value != "") {
+            tsOptions["search"] = this.#tsSearchElmt.value;
+        }
 
-        return warnContainerElmt;
-    }
+        this.#tsReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.timeseries.retrieve_list`, tsOptions),
+            (data) => {
+                let tsPaginationOpts = {
+                    pageSize: this.#tsPageSizeElmt.current,
+                    totalItems: data.pagination.total,
+                    totalPages: data.pagination.total_pages,
+                    page: data.pagination.page,
+                    firstPage: data.pagination.first_page,
+                    lastPage: data.pagination.last_page,
+                    previousPage: data.pagination.previous_page,
+                    nextPage: data.pagination.next_page,
+                }
+                this.#tsPaginationElmt.reload(tsPaginationOpts);
+                this.#tsCountElmt.update({
+                    totalCount: this.#tsPaginationElmt.totalItems,
+                    firstItem: this.#tsPaginationElmt.startItem,
+                    lastItem: this.#tsPaginationElmt.endItem
+                });
 
-    #setListLoading() {
-        let loadingContainerElmt = document.createElement("td");
-        loadingContainerElmt.setAttribute("colspan", "3");
-        loadingContainerElmt.classList.add("text-center", "p-4", "w-100");
-        loadingContainerElmt.appendChild(new Spinner());
-        this.#serviceStatesContainerElmt.appendChild(loadingContainerElmt);
+                this.#populateTimeseriesList(data.data);
+            },
+            (error) => {
+                let flashMsgElmt = new FlashMessage({
+                    type: FlashMessageTypes.ERROR,
+                    text: error,
+                    isDismissible: true
+                });
+                this.#messagesElmt.appendChild(flashMsgElmt);
+            },
+        );
     }
 
-    #refreshList() {
-        this.#itemsCountElmt.setLoading();
-        this.#serviceStatesContainerElmt.innerHTML = "";
-        this.#setListLoading();
-
-        if (this.#listReqID != null) {
-            this.#internalAPIRequester.abort(this.#listReqID);
-            this.#listReqID = null;
+    #renderEvents(id, type, path) {
+        this.#eventsCountElmt.setLoading();
+        this.#eventsListElmt.innerHTML = "";
+        this.#eventsListElmt.appendChild(new Spinner());
+
+        if (this.#eventsReqID != null) {
+            this.#internalAPIRequester.abort(this.#eventsReqID);
+            this.#eventsReqID = null;
         }
 
-        let filters = {};
-        if (this.#siteNameSearchElmt.value != "") {
-            filters["in_site_name"] = this.#siteNameSearchElmt.value;
+        if (["space", "zone"].includes(type)) {
+            this.#eventsRecurseSwitchElmt.checked = false;
+            this.#eventsRecurseSwitchElmt.setAttribute("disabled", true);
+        } else {
+            this.#eventsRecurseSwitchElmt.removeAttribute("disabled");
         }
-        if (this.#serviceStateFilterElmt.value == "on") {
-            filters["is_enabled"] = true;
-        } else if (this.#serviceStateFilterElmt.value == "off") {
-            filters["is_enabled"] = false;
+
+        let eventsOptions = {
+            "page_size": this.#eventsPageSizeElmt.current,
+            "page": this.#eventsPaginationElmt.page,
+        };
+        eventsOptions[`${this.#eventsRecurseSwitchElmt.checked ? "recurse_" : ""}${type}_id`] = id;
+        if (this.#eventsSearchElmt.value != "") {
+            eventsOptions["in_source"] = this.#eventsSearchElmt.value;
         }
 
-        this.#listReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.services.weather_data.retrieve_list`, filters),
+        this.#eventsReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.events.retrieve_list`, eventsOptions),
             (data) => {
-                this.#serviceStatesContainerElmt.innerHTML = "";
-                if (data.length > 0) {
-                    for (let row of data) {
-                        row.is_enabled = row.is_enabled == null ? false : row.is_enabled;
-                        this.#serviceStatesContainerElmt.appendChild(this.#createEntryElement(row));
-                    }
-                } else {
-                    let noItemElmt = document.createElement("p");
-                    noItemElmt.classList.add("fst-italic", "text-center", "text-muted", "w-100");
-                    noItemElmt.innerText = "No download weather data service states for sites";
-                    this.#serviceStatesContainerElmt.appendChild(noItemElmt);
+                let eventsPaginationOpts = {
+                    pageSize: this.#eventsPageSizeElmt.current,
+                    totalItems: data.pagination.total,
+                    totalPages: data.pagination.total_pages,
+                    page: data.pagination.page,
+                    firstPage: data.pagination.first_page,
+                    lastPage: data.pagination.last_page,
+                    previousPage: data.pagination.previous_page,
+                    nextPage: data.pagination.next_page,
                 }
-
-                this.#itemsCountElmt.update({
-                    firstItem: data.length > 0 ? 1 : 0,
-                    lastItem: data.length,
-                    totalCount: data.length
+                this.#eventsPaginationElmt.reload(eventsPaginationOpts);
+                this.#eventsCountElmt.update({
+                    totalCount: this.#eventsPaginationElmt.totalItems,
+                    firstItem: this.#eventsPaginationElmt.startItem,
+                    lastItem: this.#eventsPaginationElmt.endItem
                 });
+
+                this.#populateEventList(data.data);
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
-                    text: error.toString(),
+                    text: error,
                     isDismissible: true
                 });
                 this.#messagesElmt.appendChild(flashMsgElmt);
             },
         );
     }
 
-    mount() {
-        this.#refreshList();
+    #loadSitesTreeData() {
+        this.#sitesTreeElmt.showLoading();
+
+        if (this.#sitesTreeReqID != null) {
+            this.#internalAPIRequester.abort(this.#sitesTreeReqID);
+            this.#sitesTreeReqID = null;
+        }
+
+        this.#sitesTreeReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.structural_elements.retrieve_tree_sites`),
+            (data) => {
+                this.#sitesTreeElmt.load(data.data);
+                this.#sitesTreeElmt.collapseAll();
+            },
+            (error) => {
+                let flashMsgElmt = new FlashMessage({
+                    type: FlashMessageTypes.ERROR,
+                    text: error,
+                    isDismissible: true
+                });
+                this.#messagesElmt.appendChild(flashMsgElmt);
+            },
+        );
     }
-}
 
+    #loadZonesTreeData() {
+        this.#zonesTreeElmt.showLoading();
 
-document.addEventListener("DOMContentLoaded", () => {
+        if (this.#zonesTreeReqID != null) {
+            this.#internalAPIRequester.abort(this.#zonesTreeReqID);
+            this.#zonesTreeReqID = null;
+        }
 
-    let view = new WeatherDataServiceManageView();
-    view.mount();
+        this.#zonesTreeReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.structural_elements.retrieve_tree_zones`),
+            (data) => {
+                this.#zonesTreeElmt.load(data.data);
+                this.#zonesTreeElmt.collapseAll();
+            },
+            (error) => {
+                let flashMsgElmt = new FlashMessage({
+                    type: FlashMessageTypes.ERROR,
+                    text: error,
+                    isDismissible: true
+                });
+                this.#messagesElmt.appendChild(flashMsgElmt);
+            },
+        );
+    }
+
+    #generateHelpElement(helpContext) {
+        let helpContainerElmt = document.createElement("div");
+        helpContainerElmt.classList.add("alert", "alert-info", "mb-0", "pb-0");
+
+        let helpIconElmt = document.createElement("i");
+        helpIconElmt.classList.add("bi", "bi-question-diamond", "me-2");
+        helpContainerElmt.appendChild(helpIconElmt);
+
+        let helpTitleElmt = document.createElement("span");
+        helpTitleElmt.classList.add("fw-bold");
+        helpTitleElmt.innerText = "Help";
+        helpContainerElmt.appendChild(helpTitleElmt);
+
+        let helpTextElmt = document.createElement("p");
+        helpTextElmt.innerHTML = `Select a <span class="fw-bold">location (site, building...)</span> in the tree to see its <span class="fw-bold">${helpContext}</span>.`;
+        helpContainerElmt.appendChild(helpTextElmt);
+
+        return helpContainerElmt;
+    }
+
+    #refreshTabs() {
+        let selectedItemData = this.#selectedItemsPerTab[this.#tabSitesSelected.id];
+        if (selectedItemData != null) {
+            if (!this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id]) {
+                this.#renderPerTab[this.#tabPropertiesSelected.id]?.call(this, selectedItemData.id, selectedItemData.type, selectedItemData.path);
+                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = true;
+            }
+        } else {
+            this.#generalTabContentElmt.innerHTML = "";
+            this.#generalTabContentElmt.appendChild(this.#generateHelpElement("description"));
+            this.#propertiesTabContentElmt.innerHTML = "";
+            this.#propertiesTabContentElmt.appendChild(this.#generateHelpElement("properties"));
+            this.#tsListElmt.innerHTML = "";
+            this.#tsListElmt.appendChild(this.#generateHelpElement("related timeseries"));
+            this.#eventsListElmt.innerHTML = "";
+            this.#eventsListElmt.appendChild(this.#generateHelpElement("related events"));
+        }
+    }
 
-});
+    render(id, type, path) {
+        this.#selectedItemsPerTab[this.#tabSitesSelected.id] = {
+            id: id,
+            type: type,
+            path: path
+        };
+        for (let tabElmt of this.#tabPropertiesElmts) {
+            this.#alreadyLoadedPerTab[tabElmt.id] = false;
+        }
+        this.#tsPaginationElmt.reload();
+        this.#refreshTabs();
+    }
+
+    refresh() {
+        this.#loadSitesTreeData();
+        this.#loadZonesTreeData();
+        this.#refreshTabs();
+    }
+}
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,727 +1,688 @@
 import {
     InternalAPIRequest
-} from "../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
     flaskES6,
     signedUser
-} from "../../../app.js";
-import {
-    Spinner
-} from "../../components/spinner.js";
-import "../../components/itemsCount.js";
-import "../../components/pagination.js";
+} from "/static/scripts/app.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 import {
-    TimeDisplay
-} from "../../tools/time.js";
+    Spinner
+} from "../../../components/spinner.js";
 import {
-    EventLevelBadge
-} from "../../components/eventLevel.js";
-import "../../components/tree.js";
+    FilterSelect
+} from "/static/scripts/modules/components/filterSelect.js";
+import "/static/scripts/modules/components/itemsCount.js";
+import "/static/scripts/modules/components/time/datetimePicker.js";
 
 
-export class StructuralElementsExploreView {
-
-    #tzName = "UTC";
-    #messagesElmt = null;
+class WeatherDataServiceManageView {
 
     #internalAPIRequester = null;
-    #generalReqID = null;
-    #propertiesReqID = null;
-    #tsReqID = null;
-    #eventsReqID = null;
-    #sitesTreeReqID = null;
-    #zonesTreeReqID = null;
-
-    #tabSitesElmts = null;
-    #tabPropertiesElmts = null;
-    #generalTabContentElmt = null;
-    #propertiesTabContentElmt = null;
-
-    #tsSearchElmt = null;
-    #tsClearSearchBtnElmt = null;
-    #tsRecurseSwitchElmt = null;
-    #tsPageSizeElmt = null;
-    #tsCountElmt = null;
-    #tsPaginationElmt = null;
-    #tsListElmt = null;
-
-    #eventsSearchElmt = null;
-    #eventsClearSearchBtnElmt = null;
-    #eventsRecurseSwitchElmt = null;
-    #eventsPageSizeElmt = null;
-    #eventsCountElmt = null;
-    #eventsPaginationElmt = null;
-    #eventsListElmt = null;
-
-    #tabSitesSelected = null;
-    #tabPropertiesSelected = null;
-
-    #selectedItemsPerTab = {};
-    #renderPerTab = {
-        "general-tab": this.#renderGeneral.bind(this),
-        "properties-tab": this.#renderProperties.bind(this),
-        "timeseries-tab": this.#renderTimeseries.bind(this),
-        "events-tab": this.#renderEvents.bind(this),
-    }
-    #alreadyLoadedPerTab = {};
+    #weatherListReqID = null;
+    #forecastWeatherListReqID = null;
+    #updateStateReqID = null;
+    #getSvcEtagReqID = null;
+    #getSemanticsReqID = null;
+
+    #messagesElmt = null;
 
-    #sitesTreeElmt = null;
-    #zonesTreeElmt = null;
+    #filtersContainerElmt = null;
+    #siteNameSearchElmt = null;
+    #serviceStateFilterElmt = null;
+    #removeFiltersBtnElmt = null;
+
+    #weatherItemsCountElmt = null;
+    #weatherServiceStatesContainerElmt = null;
+
+    #forecastWeatherItemsCountElmt = null;
+    #forecastWeatherServiceStatesContainerElmt = null;
+
+    #fetchDataModalElmt = null;
+    #fetchDataModal = null;
+    #fetchDataModalBodyElmt = null;
+    #fetchDataSiteIdElmt = null;
+    #fetchDataDatetimeStartElmt = null;
+    #fetchDataDatetimeEndElmt = null;
+    #fetchDataBtnElmt = null;
+    #fetchDataModalParamsContainerElmt = null;
 
-    constructor(options = {}) {
+    constructor() {
         this.#internalAPIRequester = new InternalAPIRequest();
 
-        this.#loadOptions(options);
         this.#cacheDOM();
+        this.#initFilters();
         this.#initEventListeners();
-
-        this.#updateTsSearchState();
-        this.#updateEventsSearchState();
-    }
-
-    #loadOptions(options = {}) {
-        this.#tzName = options.timezone || "UTC";
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
-        this.#tabSitesElmts = [].slice.call(document.querySelectorAll("#tabSites button[data-bs-toggle='tab']"));
-        this.#tabPropertiesElmts = [].slice.call(document.querySelectorAll("#tabProperties button[data-bs-toggle='tab']"));
-        this.#generalTabContentElmt = document.getElementById("general-tabcontent");
-        this.#propertiesTabContentElmt = document.getElementById("properties-tabcontent");
-
-        this.#tsSearchElmt = document.getElementById("tsSearch");
-        this.#tsClearSearchBtnElmt = document.getElementById("tsClear");
-        this.#tsRecurseSwitchElmt = document.getElementById("tsRecurseSwitch");
-        this.#tsPageSizeElmt = document.getElementById("tsPageSize");
-        this.#tsCountElmt = document.getElementById("tsCount");
-        this.#tsPaginationElmt = document.getElementById("tsPagination");
-        this.#tsListElmt = document.getElementById("tsList");
-
-        this.#eventsSearchElmt = document.getElementById("eventsSearch");
-        this.#eventsClearSearchBtnElmt = document.getElementById("eventsClear");
-        this.#eventsRecurseSwitchElmt = document.getElementById("eventsRecurseSwitch");
-        this.#eventsPageSizeElmt = document.getElementById("eventsPageSize");
-        this.#eventsCountElmt = document.getElementById("eventsCount");
-        this.#eventsPaginationElmt = document.getElementById("eventsPagination");
-        this.#eventsListElmt = document.getElementById("eventsList");
+        this.#filtersContainerElmt = document.getElementById("filtersContainer");
+        this.#siteNameSearchElmt = document.getElementById("siteNameSearch");
+        this.#removeFiltersBtnElmt = document.getElementById("removeFiltersBtn");
 
-        this.#sitesTreeElmt = document.getElementById("sitesTree");
-        this.#zonesTreeElmt = document.getElementById("zonesTree");
-    }
+        this.#weatherItemsCountElmt = document.getElementById("weatherItemsCount");
+        this.#weatherServiceStatesContainerElmt = document.getElementById("weatherServiceStatesContainer");
 
-    #initEventListeners() {
-        for (let tabElmt of this.#tabSitesElmts) {
-            if (tabElmt.classList.contains("active")) {
-                this.#tabSitesSelected = tabElmt;
-            }
-            this.#selectedItemsPerTab[tabElmt.id] = null;
-            tabElmt.addEventListener("shown.bs.tab", (event) => {
-                // newly activated tab is `event.target` ; previous active tab is `event.relatedTarget`
-                this.#tabSitesSelected = event.target;
-                for (let tabPropertyElmt of this.#tabPropertiesElmts) {
-                    this.#alreadyLoadedPerTab[tabPropertyElmt.id] = false;
-                }
-                this.#refreshTabs();
-            });
-        }
+        this.#forecastWeatherItemsCountElmt = document.getElementById("weatherForecastItemsCount");
+        this.#forecastWeatherServiceStatesContainerElmt = document.getElementById("weatherForecastServiceStatesContainer");
 
-        for (let tabElmt of this.#tabPropertiesElmts) {
-            if (tabElmt.classList.contains("active")) {
-                this.#tabPropertiesSelected = tabElmt;
-            }
-            this.#alreadyLoadedPerTab[tabElmt.id] = false;
-            tabElmt.addEventListener("shown.bs.tab", (event) => {
-                // newly activated tab is `event.target` ; previous active tab is `event.relatedTarget`
-                this.#tabPropertiesSelected = event.target;
-                this.#refreshTabs();
-            });
+        if (signedUser.is_admin) {
+            this.#fetchDataModalElmt = document.getElementById("fetchDataModal");
+            this.#fetchDataModal = new bootstrap.Modal(this.#fetchDataModalElmt);
+            this.#fetchDataModalBodyElmt = document.getElementById("fetchDataModalBody");
+            this.#fetchDataSiteIdElmt = document.getElementById("fetchDataSiteId");
+            this.#fetchDataDatetimeStartElmt = document.getElementById("fetchDataDatetimeStart");
+            this.#fetchDataDatetimeEndElmt = document.getElementById("fetchDataDatetimeEnd");
+            this.#fetchDataBtnElmt = document.getElementById("fetchDataBtn");
+            this.#fetchDataModalParamsContainerElmt = document.getElementById("fetchDataModalParamsContainer");
         }
+    }
 
-        this.#tsSearchElmt.addEventListener("input", (event) => {
-            event.preventDefault();
-
-            this.#updateTsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#tsPaginationElmt.page = 1;
-            this.#refreshTabs();
-        });
+    #initFilters() {
+        this.#serviceStateFilterElmt = new FilterSelect();
+        this.#filtersContainerElmt.insertBefore(this.#serviceStateFilterElmt, this.#removeFiltersBtnElmt);
+        this.#serviceStateFilterElmt.load([{
+            value: "all",
+            text: "All"
+        }, {
+            value: "on",
+            text: "ON"
+        }, {
+            value: "off",
+            text: "OFF"
+        }, ]);
+        this.#serviceStateFilterElmt.setAttribute("data-default", "all");
+    }
 
-        this.#tsClearSearchBtnElmt.addEventListener("click", (event) => {
+    #initEventListeners() {
+        this.#siteNameSearchElmt.addEventListener("input", (event) => {
             event.preventDefault();
 
-            this.#tsSearchElmt.value = "";
-            this.#updateTsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+            this.#updateSiteNameSearch();
+            this.#refreshWeatherList();
+            this.#refreshForecastWeatherList();
         });
 
-        this.#tsRecurseSwitchElmt.addEventListener("change", (event) => {
+        this.#serviceStateFilterElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+            this.#refreshWeatherList();
+            this.#refreshForecastWeatherList();
         });
 
-        this.#tsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
+        this.#removeFiltersBtnElmt.addEventListener("click", (event) => {
             event.preventDefault();
 
-            if (event.detail.newValue != event.detail.oldValue) {
-                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-                this.#tsPaginationElmt.page = 1;
-                this.#refreshTabs();
+            let hasFilterChanged = false;
+            if (this.#siteNameSearchElmt.value != "") {
+                this.#siteNameSearchElmt.value = "";
+                this.#updateSiteNameSearch();
+                hasFilterChanged = true;
             }
-        });
-
-        this.#tsPaginationElmt.addEventListener("pageItemClick", (event) => {
-            event.preventDefault();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
-        });
-
-        this.#eventsSearchElmt.addEventListener("input", (event) => {
-            event.preventDefault();
-
-            this.#updateEventsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#eventsPaginationElmt.page = 1;
-            this.#refreshTabs();
-        });
-
-        this.#eventsClearSearchBtnElmt.addEventListener("click", (event) => {
-            event.preventDefault();
 
-            this.#eventsSearchElmt.value = "";
-            this.#updateEventsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
-        });
-
-        this.#eventsRecurseSwitchElmt.addEventListener("change", (event) => {
-            event.preventDefault();
+            let serviceStateFilterDefault = this.#serviceStateFilterElmt.getAttribute("data-default");
+            if (this.#serviceStateFilterElmt.value != serviceStateFilterDefault) {
+                this.#serviceStateFilterElmt.reset();
+                hasFilterChanged = true;
+            }
 
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+            if (hasFilterChanged) {
+                this.#refreshWeatherList();
+                this.#refreshForecastWeatherList();
+            }
         });
 
-        this.#eventsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
-            event.preventDefault();
+        if (signedUser.is_admin) {
+            this.#fetchDataDatetimeStartElmt.addEventListener("datetimeChange", (event) => {
+                event.preventDefault();
 
-            if (event.detail.newValue != event.detail.oldValue) {
-                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-                this.#eventsPaginationElmt.page = 1;
-                this.#refreshTabs();
-            }
-        });
+                this.#fetchDataDatetimeEndElmt.dateMin = this.#fetchDataDatetimeStartElmt.date;
+                this.#updateFetchDataBtn();
+            });
 
-        this.#eventsPaginationElmt.addEventListener("pageItemClick", (event) => {
-            event.preventDefault();
+            this.#fetchDataDatetimeEndElmt.addEventListener("datetimeChange", (event) => {
+                event.preventDefault();
 
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
-        });
+                this.#fetchDataDatetimeStartElmt.dateMax = this.#fetchDataDatetimeEndElmt.date;
+                this.#updateFetchDataBtn();
+            });
 
-        this.#sitesTreeElmt.addEventListener("treeNodeSelect", (event) => {
-            this.render(event.detail.id, event.detail.type, event.detail.path);
-        });
+            this.#fetchDataModalElmt.addEventListener("shown.bs.modal", () => {
+                this.#fetchDataDatetimeStartElmt.focus();
+            });
 
-        this.#zonesTreeElmt.addEventListener("treeNodeSelect", (event) => {
-            this.render(event.detail.id, event.detail.type, event.detail.path);
-        });
+            this.#fetchDataBtnElmt.addEventListener("click", () => {
+                this.#fetchDataBtnElmt.classList.add("placeholder");
+                this.#fetchDataModalBodyElmt.classList.add("placeholder");
+
+                this.#internalAPIRequester.put(
+                    flaskES6.urlFor(`api.structural_elements.fetch_weather_data`, {
+                        id: this.#fetchDataSiteIdElmt.value
+                    }), {
+                        "start_date": this.#fetchDataDatetimeStartElmt.date,
+                        "start_time": this.#fetchDataDatetimeStartElmt.time,
+                        "end_date": this.#fetchDataDatetimeEndElmt.date,
+                        "end_time": this.#fetchDataDatetimeEndElmt.time,
+                    },
+                    null,
+                    () => {
+                        let flashMsgElmt = new FlashMessage({
+                            type: FlashMessageTypes.SUCCESS,
+                            text: `Weather data successfully fetched.`,
+                            isDismissible: true,
+                            isTimed: false
+                        });
+                        this.#messagesElmt.appendChild(flashMsgElmt);
+
+                        this.#fetchDataModal.hide();
+                    },
+                    (error) => {
+                        let flashMsgElmt = new FlashMessage({
+                            type: FlashMessageTypes.ERROR,
+                            text: error.toString(),
+                            isDismissible: true,
+                            isTimed: false
+                        });
+                        this.#messagesElmt.appendChild(flashMsgElmt);
+
+                        this.#fetchDataModal.hide();
+                    },
+                );
+            });
+        }
     }
 
-    #updateTsSearchState() {
-        if (this.#tsSearchElmt.value != "") {
-            this.#tsSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
-            this.#tsClearSearchBtnElmt.classList.remove("d-none", "invisible");
-        } else {
-            this.#tsSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
-            this.#tsClearSearchBtnElmt.classList.add("d-none", "invisible");
+    #updateSiteNameSearch() {
+        if (this.#siteNameSearchElmt.value == "") {
+            this.#siteNameSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
+        } else if (!this.#siteNameSearchElmt.classList.contains("border-info")) {
+            this.#siteNameSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
         }
     }
 
-    #updateEventsSearchState() {
-        if (this.#eventsSearchElmt.value != "") {
-            this.#eventsSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
-            this.#eventsClearSearchBtnElmt.classList.remove("d-none", "invisible");
+    #updateFetchDataBtn() {
+        if (this.#fetchDataBtnElmt.classList.contains("placeholder")) {
+            this.#fetchDataBtnElmt.classList.remove("placeholder");
+        }
+        if (this.#fetchDataModalBodyElmt.classList.contains("placeholder")) {
+            this.#fetchDataModalBodyElmt.classList.remove("placeholder");
+        }
+
+        if (this.#fetchDataDatetimeStartElmt.date != null && this.#fetchDataDatetimeStartElmt.time != null && this.#fetchDataDatetimeEndElmt.date != null && this.#fetchDataDatetimeEndElmt.time != null) {
+            this.#fetchDataBtnElmt.removeAttribute("disabled");
         } else {
-            this.#eventsSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
-            this.#eventsClearSearchBtnElmt.classList.add("d-none", "invisible");
+            this.#fetchDataBtnElmt.setAttribute("disabled", true);
         }
     }
 
-    #getEditBtnHTML(type, id, tab = null) {
+    #createEntryElement(serviceStateData, forecast = false) {
+        let suffixId = `${forecast ? "forecast-" : ""}${serviceStateData.site_id}`;
+
+        let trElmt = document.createElement("tr");
+        trElmt.classList.add("align-middle");
+
+        let thElmt = document.createElement("th");
+        thElmt.classList.add("text-break");
+        thElmt.setAttribute("scope", "row");
+        thElmt.innerText = serviceStateData.site_name;
+        trElmt.appendChild(thElmt);
+
+        let svcCtrlElmt = document.createElement("div");
+        svcCtrlElmt.classList.add("d-flex", "gap-1", "my-auto", "placeholder-glow");
+
         if (signedUser.is_admin) {
-            let editUrlParams = {
-                type: type,
-                id: id
-            };
-            if (tab != null) {
-                editUrlParams["tab"] = tab;
-            }
-            try {
-                let editUrl = flaskES6.urlFor(`structural_elements.edit`, editUrlParams);
-                return `<a class="btn btn-sm btn-outline-primary text-nowrap" href="${editUrl}" role="button" title="Edit ${type}"><i class="bi bi-pencil"></i> Edit</a>`;
-            } catch (error) {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error,
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-            }
-        }
-        return ``;
-    }
+            let svcEtagInputElmt = document.createElement("input");
+            svcEtagInputElmt.setAttribute("type", "hidden");
+            svcCtrlElmt.appendChild(svcEtagInputElmt);
+
+            let svcOnInputElmt = document.createElement("input");
+            svcOnInputElmt.id = `radio-svc-state-${suffixId}-on`;
+            svcOnInputElmt.name = `radio-svc-state-${suffixId}`;
+            svcOnInputElmt.classList.add("btn-check");
+            svcOnInputElmt.setAttribute("type", "radio");
+            svcOnInputElmt.setAttribute("autocomplete", "off");
+            svcCtrlElmt.appendChild(svcOnInputElmt);
+
+            let svcOnLabelElmt = document.createElement("label");
+            svcOnLabelElmt.classList.add("btn", "btn-sm", "btn-outline-success");
+            svcOnLabelElmt.setAttribute("for", svcOnInputElmt.id);
+            svcOnLabelElmt.setAttribute("title", "Enable service");
+            svcOnLabelElmt.innerText = "ON";
+            svcCtrlElmt.appendChild(svcOnLabelElmt);
+
+            let svcOffInputElmt = document.createElement("input");
+            svcOffInputElmt.id = `radio-svc-state-${suffixId}-off`;
+            svcOffInputElmt.name = `radio-svc-state-${suffixId}`;
+            svcOffInputElmt.classList.add("btn-check");
+            svcOffInputElmt.setAttribute("type", "radio");
+            svcOffInputElmt.setAttribute("autocomplete", "off");
+            svcCtrlElmt.appendChild(svcOffInputElmt);
+
+            let svcOffLabelElmt = document.createElement("label");
+            svcOffLabelElmt.classList.add("btn", "btn-sm", "btn-outline-danger");
+            svcOffLabelElmt.setAttribute("for", svcOffInputElmt.id);
+            svcOffLabelElmt.setAttribute("title", "Disable service");
+            svcOffLabelElmt.innerText = "OFF";
+            svcCtrlElmt.appendChild(svcOffLabelElmt);
+
+            let updateSvcInputState = () => {
+                if (serviceStateData.is_enabled) {
+                    svcOffInputElmt.removeAttribute("checked");
+                    svcOnInputElmt.setAttribute("checked", "true");
+                } else {
+                    svcOnInputElmt.removeAttribute("checked");
+                    svcOffInputElmt.setAttribute("checked", "true");
+                }
 
-    #getGeneralHTML(data, path) {
-        let htmlContent = `<div class="d-flex justify-content-between align-items-start gap-3 mb-3">
-    <div>
-        <h5 class="text-break">${data.structural_element.name}</h5>
-        <h6 class="text-break">${path}</h6>
-    </div>
-    ${this.#getEditBtnHTML(data.type, data.structural_element.id)}
-</div>
-<p class="fst-italic text-muted text-break">${data.structural_element.description}</p>
-<div class="row">
-    <dl class="col">
-        <dt>IFC ID</dt>
-        <dd>${(data.structural_element.ifc_id != null && data.structural_element.ifc_id != "") ? data.structural_element.ifc_id : "-"}</dd>
-    </dl>
-</div>`;
-
-        if (data.type == "site") {
-            htmlContent += `<div class="row">
-    <dl class="col">
-        <dt>Latitude <small class="text-muted">[°]</small></dt>
-        <dd>${data.structural_element.latitude != null ? data.structural_element.latitude : "-"}</dd>
-    </dl>
-    <dl class="col">
-        <dt>Longitude <small class="text-muted">[°]</small></dt>
-        <dd>${data.structural_element.longitude != null ? data.structural_element.longitude : "-"}</dd>
-    </dl>
-</div>`;
-        }
-
-        return htmlContent;
-    }
-
-    #getItemHelpHTML(itemDescription, withSpace = true) {
-        let ret = ``;
-        if (itemDescription?.length > 0) {
-            let abbrElmt = document.createElement("abbr");
-            abbrElmt.title = itemDescription != null ? itemDescription : "";
-            let abbrContentElmt = document.createElement("i");
-            abbrContentElmt.classList.add("bi", "bi-question-diamond");
-            abbrElmt.appendChild(abbrContentElmt);
-            ret = `<sup${withSpace ? ` class="ms-1"`: ``}>${abbrElmt.outerHTML}</sup>`;
-        }
-        return ret;
-    }
-
-    #getPropertiesHTML(data, id) {
-        let propertyDataHTML = ``;
-        if (data.properties.length > 0) {
-            for (let property of data.properties) {
-                let unitSymbol = (property.unit_symbol != null && property.unit_symbol.length > 0) ? `<small class="text-muted ms-1">[${property.unit_symbol}]</small>` : ``;
-                propertyDataHTML += `<dl>
-    <dt>${property.name}${unitSymbol}${this.#getItemHelpHTML(property.description)}</dt>
-    <dd>${(property.value !== "" && property.value != null) ? property.value : "-"}</dd>
-</dl>`;
+                svcOnLabelElmt.classList.remove("placeholder");
+                svcOffLabelElmt.classList.remove("placeholder");
             }
-        } else {
-            propertyDataHTML = `<p class="fst-italic">No data</p>`;
-        }
 
-        return `<div class="d-flex justify-content-between align-items-start mb-3">
-    <div class="d-flex gap-4">
-        ${propertyDataHTML}
-    </div>
-    ${this.#getEditBtnHTML(data.type, id, "properties")}
-</div>`;
-    }
 
-    #getErrorHTML(error) {
-        return `<div class="alert alert-danger" role="alert">
-    <i class="bi bi-x-octagon me-2"></i>
-    ${error}
-</div>`;
-    }
+            updateSvcInputState();
 
-    #renderGeneral(id, type, path) {
-        this.#generalTabContentElmt.innerHTML = "";
-        this.#generalTabContentElmt.appendChild(new Spinner());
 
-        if (this.#generalReqID != null) {
-            this.#internalAPIRequester.abort(this.#generalReqID);
-            this.#generalReqID = null;
-        }
-        this.#generalReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.structural_elements.retrieve_data`, {
-                type: type,
-                id: id
-            }),
-            (data) => {
-                this.#generalTabContentElmt.innerHTML = this.#getGeneralHTML(data, path);
-            },
-            (error) => {
-                this.#generalTabContentElmt.innerHTML = this.#getErrorHTML(error.message);
-            },
-        );
-    }
+            let updateServiceState = (isEnabled) => {
+                svcOnLabelElmt.classList.add("placeholder");
+                svcOffLabelElmt.classList.add("placeholder");
 
-    #renderProperties(id, type, path) {
-        this.#propertiesTabContentElmt.innerHTML = "";
-        this.#propertiesTabContentElmt.appendChild(new Spinner());
-
-        if (this.#propertiesReqID != null) {
-            this.#internalAPIRequester.abort(this.#propertiesReqID);
-            this.#propertiesReqID = null;
-        }
-        this.#propertiesReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.structural_elements.retrieve_property_data`, {
-                type: type,
-                id: id
-            }),
-            (data) => {
-                this.#propertiesTabContentElmt.innerHTML = this.#getPropertiesHTML(data, id);
-            },
-            (error) => {
-                this.#propertiesTabContentElmt.innerHTML = this.#getErrorHTML(error.message);
-            },
-        );
-    }
+                if (this.#updateStateReqID != null) {
+                    this.#internalAPIRequester.abort(this.#updateStateReqID);
+                    this.#updateStateReqID = null;
+                }
 
-    #populateTimeseriesList(tsList) {
-        this.#tsListElmt.innerHTML = "";
-        if (tsList.length > 0) {
-            for (let tsData of tsList) {
-                let tsElmt = document.createElement("div");
-                tsElmt.classList.add("list-group-item");
-
-                let tsHeaderElmt = document.createElement("div");
-                tsHeaderElmt.classList.add("d-flex", "gap-1");
-
-                let iconElmt = document.createElement("i");
-                iconElmt.classList.add("bi", "bi-clock-history", "me-1");
-                tsHeaderElmt.appendChild(iconElmt);
-
-                let nameSpanElmt = document.createElement("span");
-                nameSpanElmt.classList.add("fw-bold", "text-break");
-                nameSpanElmt.innerText = tsData.name;
-                tsHeaderElmt.appendChild(nameSpanElmt);
-
-                if (tsData.unit_symbol) {
-                    let unitSpanElmt = document.createElement("span");
-                    unitSpanElmt.classList.add("text-muted");
-                    unitSpanElmt.innerText = `[${tsData.unit_symbol}]`;
-                    tsHeaderElmt.appendChild(unitSpanElmt);
+                if (serviceStateData.id == null) {
+                    if (isEnabled) {
+                        // Enable weather data service for site.
+                        this.#updateStateReqID = this.#internalAPIRequester.post(
+                            flaskES6.urlFor(`api.services.weather_data.${forecast ? "forecast_": ""}enable`), {
+                                site_id: serviceStateData.site_id,
+                                is_enabled: isEnabled
+                            },
+                            (data) => {
+                                serviceStateData = data.data;
+                                svcEtagInputElmt.value = data.etag;
+                                updateSvcInputState();
+
+                                let flashMsgElmt = new FlashMessage({
+                                    type: FlashMessageTypes.INFO,
+                                    text: `${forecast ? "Forecast w": "W"}eather data service enabled!`,
+                                    isDismissible: true
+                                });
+                                this.#messagesElmt.appendChild(flashMsgElmt);
+                            },
+                            (error) => {
+                                let flashMsgElmt = new FlashMessage({
+                                    type: FlashMessageTypes.ERROR,
+                                    text: error.toString(),
+                                    isDismissible: true
+                                });
+                                this.#messagesElmt.appendChild(flashMsgElmt);
+
+                                svcOnLabelElmt.classList.remove("placeholder");
+                                svcOffLabelElmt.classList.remove("placeholder");
+                            },
+                        );
+                    }
+                } else {
+                    let _updateSvcState = (_isEnabled) => {
+                        // Update weather data service state for site.
+                        this.#updateStateReqID = this.#internalAPIRequester.put(
+                            flaskES6.urlFor(`api.services.weather_data.${forecast ? "forecast_": ""}update_state`, {
+                                id: serviceStateData.id
+                            }), {
+                                is_enabled: _isEnabled
+                            },
+                            svcEtagInputElmt.value,
+                            (data) => {
+                                serviceStateData = data.data;
+                                svcEtagInputElmt.value = data.etag;
+                                updateSvcInputState();
+
+                                let flashMsgElmt = new FlashMessage({
+                                    type: FlashMessageTypes.INFO,
+                                    text: `${forecast ? "Forecast w": "W"}eather data service ${isEnabled ? "en": "dis"}abled!`,
+                                    isDismissible: true
+                                });
+                                this.#messagesElmt.appendChild(flashMsgElmt);
+                            },
+                            (error) => {
+                                let flashMsgElmt = new FlashMessage({
+                                    type: FlashMessageTypes.ERROR,
+                                    text: error.toString(),
+                                    isDismissible: true
+                                });
+                                this.#messagesElmt.appendChild(flashMsgElmt);
+
+                                updateSvcInputState();
+                            },
+                        );
+                    }
+
+                    if (svcEtagInputElmt.value == "") {
+                        if (this.#getSvcEtagReqID != null) {
+                            this.#internalAPIRequester.abort(this.#getSvcEtagReqID);
+                            this.#getSvcEtagReqID = null;
+                        }
+
+                        this.#getSvcEtagReqID = this.#internalAPIRequester.get(
+                            flaskES6.urlFor(`api.services.weather_data.retrieve_${forecast ? "forecast_": ""}one`, {
+                                id: serviceStateData.id
+                            }),
+                            (data) => {
+                                svcEtagInputElmt.value = data.etag;
+                                _updateSvcState(isEnabled);
+                            },
+                            (error) => {
+                                let flashMsgElmt = new FlashMessage({
+                                    type: FlashMessageTypes.ERROR,
+                                    text: error.toString(),
+                                    isDismissible: true
+                                });
+                                this.#messagesElmt.appendChild(flashMsgElmt);
+
+                                updateSvcInputState();
+                            },
+                        );
+                    } else {
+                        _updateSvcState(isEnabled);
+                    }
                 }
+            };
 
-                tsElmt.appendChild(tsHeaderElmt);
 
-                let tsDescElmt = document.createElement("small");
-                tsDescElmt.classList.add("fst-italic", "text-muted");
-                tsDescElmt.innerText = tsData.description != null ? tsData.description : "-";
-                tsElmt.appendChild(tsDescElmt);
+            svcOnInputElmt.addEventListener("change", () => {
+                if (svcOnInputElmt.checked) {
+                    updateServiceState(true);
+                }
+            });
 
-                this.#tsListElmt.appendChild(tsElmt);
-            }
+            svcOffInputElmt.addEventListener("change", () => {
+                if (svcOffInputElmt.checked) {
+                    updateServiceState(false);
+                }
+            });
         } else {
-            let nodataSpanElmt = document.createElement("span");
-            nodataSpanElmt.classList.add("fst-italic", "text-muted", "text-center");
-            nodataSpanElmt.innerText = "No data";
-            this.#tsListElmt.appendChild(nodataSpanElmt);
+            let spanStateElmt = document.createElement("span");
+            spanStateElmt.classList.add("fw-bold", "text-opacity-75");
+            if (serviceStateData.is_enabled) {
+                spanStateElmt.classList.add("text-success");
+                spanStateElmt.innerText = "ON";
+            } else {
+                spanStateElmt.classList.add("text-danger");
+                spanStateElmt.innerText = "OFF";
+            }
+            svcCtrlElmt.appendChild(spanStateElmt);
         }
-    }
 
-    #populateEventList(eventsList) {
-        this.#eventsListElmt.innerHTML = "";
-        if (eventsList.length > 0) {
-            for (let eventData of eventsList) {
-                let eventElmt = document.createElement("div");
-                eventElmt.classList.add("list-group-item");
-
-                let eventHeaderElmt = document.createElement("div");
-                eventHeaderElmt.classList.add("d-flex", "align-items-center", "gap-1", "w-100");
-                eventElmt.appendChild(eventHeaderElmt);
-
-                let iconElmt = document.createElement("i");
-                iconElmt.classList.add("bi", "bi-journal-x", "me-1");
-                eventHeaderElmt.appendChild(iconElmt);
-
-                let headerContentElmt = document.createElement("div");
-                headerContentElmt.classList.add("d-flex", "justify-content-between", "align-items-center", "gap-2", "w-100");
-                eventHeaderElmt.appendChild(headerContentElmt);
-
-                let timestampElmt = document.createElement("h6");
-                timestampElmt.classList.add("text-nowrap", "mb-0");
-                timestampElmt.innerText = TimeDisplay.toLocaleString(new Date(eventData.timestamp), {
-                    timezone: this.#tzName
-                });
-                headerContentElmt.appendChild(timestampElmt);
+        let tdStateElmt = document.createElement("td");
+        tdStateElmt.classList.add("d-flex", "gap-4");
+        tdStateElmt.appendChild(svcCtrlElmt);
+        trElmt.appendChild(tdStateElmt);
 
-                let levelBadgeElmt = new EventLevelBadge();
-                levelBadgeElmt.setAttribute("level", eventData.level.toUpperCase());
-                headerContentElmt.appendChild(levelBadgeElmt);
-
-                let bodyContentElmt = document.createElement("div");
-                bodyContentElmt.classList.add("d-flex", "justify-content-between", "align-items-start", "gap-2");
-                eventElmt.appendChild(bodyContentElmt);
-
-                let eventDescElmt = document.createElement("small");
-                eventDescElmt.classList.add("fst-italic", "text-muted");
-                eventDescElmt.innerText = eventData.description;
-                bodyContentElmt.appendChild(eventDescElmt);
-
-                let sourceElmt = document.createElement("span");
-                sourceElmt.classList.add("text-nowrap");
-                sourceElmt.innerText = eventData.source;
-                bodyContentElmt.appendChild(sourceElmt);
+        if (signedUser.is_admin) {
+            if (serviceStateData.id == null) {
+                let warnAlertElmt = this.#createWarnAlertElement("Never launched yet");
+                tdStateElmt.appendChild(warnAlertElmt);
+            }
 
-                this.#eventsListElmt.appendChild(eventElmt);
+            // Verify that the site has long/lat coordinates.
+            let siteHasCoord = true;
+            this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.structural_elements.retrieve_data`, {
+                    type: "site",
+                    id: serviceStateData.site_id
+                }),
+                (data) => {
+                    if (data.structural_element.latitude == null || data.structural_element.longitude == null) {
+                        siteHasCoord = false;
+                        let warnSiteCoordElmt = this.#createWarnAlertElement("Site latitude/longitude coordinates are not defined!");
+                        tdStateElmt.appendChild(warnSiteCoordElmt);
+                    }
+                },
+                (error) => {
+                    let flashMsgElmt = new FlashMessage({
+                        type: FlashMessageTypes.ERROR,
+                        text: error.toString(),
+                        isDismissible: true
+                    });
+                    this.#messagesElmt.appendChild(flashMsgElmt);
+                },
+            );
+
+            if (!forecast) {
+                let tdFetchElmt = document.createElement("td");
+                trElmt.appendChild(tdFetchElmt);
+
+                let fetchLinkElmt = document.createElement("a");
+                fetchLinkElmt.classList.add("btn", "btn-sm", "btn-outline-primary");
+                fetchLinkElmt.setAttribute("role", "button");
+                fetchLinkElmt.setAttribute("title", "Fetch weather data from external service");
+                fetchLinkElmt.setAttribute("data-bs-toggle", "modal");
+                fetchLinkElmt.setAttribute("data-bs-target", `#${this.#fetchDataModalElmt.id}`);
+                tdFetchElmt.appendChild(fetchLinkElmt);
+
+                let fetchIconElmt = document.createElement("i");
+                fetchIconElmt.classList.add("bi", "bi-cloud-download");
+                fetchLinkElmt.appendChild(fetchIconElmt);
+
+                fetchLinkElmt.addEventListener("click", () => {
+                    this.#fetchDataSiteIdElmt.value = serviceStateData.site_id.toString();
+                    this.#fetchDataDatetimeStartElmt.reset({
+                        ignoreTime: true
+                    });
+                    this.#fetchDataDatetimeEndElmt.reset({
+                        ignoreTime: true
+                    });
+                    this.#updateFetchDataBtn();
+
+                    this.#fetchDataModalParamsContainerElmt.innerHTML = "";
+                    this.#fetchDataModalParamsContainerElmt.appendChild(new Spinner());
+
+                    if (this.#getSemanticsReqID != null) {
+                        this.#internalAPIRequester.abort(this.#getSemanticsReqID);
+                        this.#getSemanticsReqID = null;
+                    }
+
+                    this.#getSemanticsReqID = this.#internalAPIRequester.get(
+                        flaskES6.urlFor(`api.semantics.weather.list`, {
+                            site: serviceStateData.site_id
+                        }),
+                        (data) => {
+                            this.#fetchDataModalParamsContainerElmt.innerHTML = "";
+
+                            if (data.data.length > 0) {
+                                let weatherParamsTitleElmt = document.createElement("h6");
+                                weatherParamsTitleElmt.innerText = `${data.data.length} weather parameter${data.data.length > 1 ? "s" : ""} will be fetched:`;
+                                this.#fetchDataModalParamsContainerElmt.appendChild(weatherParamsTitleElmt);
+
+                                let weatherParamsListElmt = document.createElement("dl");
+                                weatherParamsListElmt.classList.add("d-flex", "flex-wrap", "gap-3");
+                                this.#fetchDataModalParamsContainerElmt.appendChild(weatherParamsListElmt);
+                                for (let weatherParam of data.data) {
+                                    let weatherParamsListItemElmt = document.createElement("div");
+                                    weatherParamsListElmt.appendChild(weatherParamsListItemElmt);
+
+                                    let weatherParamsListItemTitleElmt = document.createElement("dt");
+                                    weatherParamsListItemTitleElmt.innerText = `${weatherParam["parameter_label"]}`;
+                                    weatherParamsListItemElmt.appendChild(weatherParamsListItemTitleElmt);
+
+                                    let weatherParamsListItemTextElmt = document.createElement("dd");
+                                    weatherParamsListItemTextElmt.innerText = `${weatherParam["timeseries"]["name"]}${weatherParam["timeseries"]["unit_symbol"] != null ? ` [${weatherParam["timeseries"]["unit_symbol"]}]` : ""}`;
+                                    weatherParamsListItemElmt.appendChild(weatherParamsListItemTextElmt);
+                                }
+                            } else {
+                                let warnAlertElmt = this.#createWarnAlertElement("No weather parameter to fetch. You should set timeseries semantics for weather parameters.");
+                                this.#fetchDataModalParamsContainerElmt.appendChild(warnAlertElmt);
+                            }
+
+                            if (!siteHasCoord) {
+                                let warnSiteCoordElmt = this.#createWarnAlertElement("Site latitude/longitude coordinates are not defined!");
+                                this.#fetchDataModalParamsContainerElmt.appendChild(warnSiteCoordElmt);
+                            }
+                        },
+                        (error) => {
+                            let flashMsgElmt = new FlashMessage({
+                                type: FlashMessageTypes.ERROR,
+                                text: error.toString(),
+                                isDismissible: true
+                            });
+                            this.#messagesElmt.appendChild(flashMsgElmt);
+                        },
+                    );
+                });
             }
-        } else {
-            let nodataSpanElmt = document.createElement("span");
-            nodataSpanElmt.classList.add("fst-italic", "text-muted", "text-center");
-            nodataSpanElmt.innerText = "No data";
-            this.#eventsListElmt.appendChild(nodataSpanElmt);
         }
+
+        return trElmt;
     }
 
-    #renderTimeseries(id, type, path) {
-        this.#tsCountElmt.setLoading();
-        this.#tsListElmt.innerHTML = "";
-        this.#tsListElmt.appendChild(new Spinner());
+    #createWarnAlertElement(text) {
+        let warnContainerElmt = document.createElement("div");
+        warnContainerElmt.classList.add("alert", "alert-warning", "border", "border-warning", "mb-0", "py-1");
+        warnContainerElmt.setAttribute("role", "alert");
 
-        if (this.#tsReqID != null) {
-            this.#internalAPIRequester.abort(this.#tsReqID);
-            this.#tsReqID = null;
-        }
+        let warnIconElmt = document.createElement("i");
+        warnIconElmt.classList.add("bi", "bi-exclamation-triangle", "me-1");
+        warnContainerElmt.appendChild(warnIconElmt);
 
-        if (["space", "zone"].includes(type)) {
-            this.#tsRecurseSwitchElmt.checked = false;
-            this.#tsRecurseSwitchElmt.setAttribute("disabled", true);
-        } else {
-            this.#tsRecurseSwitchElmt.removeAttribute("disabled");
-        }
+        let warnTextElmt = document.createElement("span");
+        warnTextElmt.classList.add("fst-italic");
+        warnTextElmt.innerText = text;
+        warnContainerElmt.appendChild(warnTextElmt);
 
-        let tsOptions = {
-            "page_size": this.#tsPageSizeElmt.current,
-            "page": this.#tsPaginationElmt.page,
-        };
-        tsOptions[`${this.#tsRecurseSwitchElmt.checked ? "recurse_" : ""}${type}_id`] = id;
-        if (this.#tsSearchElmt.value != "") {
-            tsOptions["search"] = this.#tsSearchElmt.value;
-        }
-
-        this.#tsReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.timeseries.retrieve_list`, tsOptions),
-            (data) => {
-                let tsPaginationOpts = {
-                    pageSize: this.#tsPageSizeElmt.current,
-                    totalItems: data.pagination.total,
-                    totalPages: data.pagination.total_pages,
-                    page: data.pagination.page,
-                    firstPage: data.pagination.first_page,
-                    lastPage: data.pagination.last_page,
-                    previousPage: data.pagination.previous_page,
-                    nextPage: data.pagination.next_page,
-                }
-                this.#tsPaginationElmt.reload(tsPaginationOpts);
-                this.#tsCountElmt.update({
-                    totalCount: this.#tsPaginationElmt.totalItems,
-                    firstItem: this.#tsPaginationElmt.startItem,
-                    lastItem: this.#tsPaginationElmt.endItem
-                });
+        return warnContainerElmt;
+    }
 
-                this.#populateTimeseriesList(data.data);
-            },
-            (error) => {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error,
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-            },
-        );
+    #getListLoadingElement() {
+        let loadingContainerElmt = document.createElement("td");
+        loadingContainerElmt.setAttribute("colspan", "3");
+        loadingContainerElmt.classList.add("text-center", "p-4", "w-100");
+        loadingContainerElmt.appendChild(new Spinner());
+        return loadingContainerElmt;
     }
 
-    #renderEvents(id, type, path) {
-        this.#eventsCountElmt.setLoading();
-        this.#eventsListElmt.innerHTML = "";
-        this.#eventsListElmt.appendChild(new Spinner());
-
-        if (this.#eventsReqID != null) {
-            this.#internalAPIRequester.abort(this.#eventsReqID);
-            this.#eventsReqID = null;
-        }
+    #refreshWeatherList() {
+        this.#weatherItemsCountElmt.setLoading();
+        this.#weatherServiceStatesContainerElmt.innerHTML = "";
+        this.#weatherServiceStatesContainerElmt.appendChild(this.#getListLoadingElement());
 
-        if (["space", "zone"].includes(type)) {
-            this.#eventsRecurseSwitchElmt.checked = false;
-            this.#eventsRecurseSwitchElmt.setAttribute("disabled", true);
-        } else {
-            this.#eventsRecurseSwitchElmt.removeAttribute("disabled");
+        if (this.#weatherListReqID != null) {
+            this.#internalAPIRequester.abort(this.#weatherListReqID);
+            this.#weatherListReqID = null;
         }
 
-        let eventsOptions = {
-            "page_size": this.#eventsPageSizeElmt.current,
-            "page": this.#eventsPaginationElmt.page,
-        };
-        eventsOptions[`${this.#eventsRecurseSwitchElmt.checked ? "recurse_" : ""}${type}_id`] = id;
-        if (this.#eventsSearchElmt.value != "") {
-            eventsOptions["in_source"] = this.#eventsSearchElmt.value;
+        let filters = {};
+        if (this.#siteNameSearchElmt.value != "") {
+            filters["in_site_name"] = this.#siteNameSearchElmt.value;
+        }
+        if (this.#serviceStateFilterElmt.value == "on") {
+            filters["is_enabled"] = true;
+        } else if (this.#serviceStateFilterElmt.value == "off") {
+            filters["is_enabled"] = false;
         }
 
-        this.#eventsReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.events.retrieve_list`, eventsOptions),
+        this.#weatherListReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.services.weather_data.retrieve_list`, filters),
             (data) => {
-                let eventsPaginationOpts = {
-                    pageSize: this.#eventsPageSizeElmt.current,
-                    totalItems: data.pagination.total,
-                    totalPages: data.pagination.total_pages,
-                    page: data.pagination.page,
-                    firstPage: data.pagination.first_page,
-                    lastPage: data.pagination.last_page,
-                    previousPage: data.pagination.previous_page,
-                    nextPage: data.pagination.next_page,
+                this.#weatherServiceStatesContainerElmt.innerHTML = "";
+                if (data.length > 0) {
+                    for (let row of data) {
+                        row.is_enabled = row.is_enabled == null ? false : row.is_enabled;
+                        this.#weatherServiceStatesContainerElmt.appendChild(this.#createEntryElement(row));
+                    }
+                } else {
+                    let noItemElmt = document.createElement("p");
+                    noItemElmt.classList.add("fst-italic", "text-center", "text-muted", "w-100");
+                    noItemElmt.innerText = "No download weather data service states for sites";
+                    this.#weatherServiceStatesContainerElmt.appendChild(noItemElmt);
                 }
-                this.#eventsPaginationElmt.reload(eventsPaginationOpts);
-                this.#eventsCountElmt.update({
-                    totalCount: this.#eventsPaginationElmt.totalItems,
-                    firstItem: this.#eventsPaginationElmt.startItem,
-                    lastItem: this.#eventsPaginationElmt.endItem
-                });
 
-                this.#populateEventList(data.data);
+                this.#weatherItemsCountElmt.update({
+                    firstItem: data.length > 0 ? 1 : 0,
+                    lastItem: data.length,
+                    totalCount: data.length
+                });
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
-                    text: error,
+                    text: error.toString(),
                     isDismissible: true
                 });
                 this.#messagesElmt.appendChild(flashMsgElmt);
             },
         );
     }
 
-    #loadSitesTreeData() {
-        this.#sitesTreeElmt.showLoading();
+    #refreshForecastWeatherList() {
+        this.#forecastWeatherItemsCountElmt.setLoading();
+        this.#forecastWeatherServiceStatesContainerElmt.innerHTML = "";
+        this.#forecastWeatherServiceStatesContainerElmt.appendChild(this.#getListLoadingElement());
 
-        if (this.#sitesTreeReqID != null) {
-            this.#internalAPIRequester.abort(this.#sitesTreeReqID);
-            this.#sitesTreeReqID = null;
+        if (this.#forecastWeatherListReqID != null) {
+            this.#internalAPIRequester.abort(this.#forecastWeatherListReqID);
+            this.#forecastWeatherListReqID = null;
         }
 
-        this.#sitesTreeReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.structural_elements.retrieve_tree_sites`),
-            (data) => {
-                this.#sitesTreeElmt.load(data.data);
-                this.#sitesTreeElmt.collapseAll();
-            },
-            (error) => {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error,
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-            },
-        );
-    }
-
-    #loadZonesTreeData() {
-        this.#zonesTreeElmt.showLoading();
-
-        if (this.#zonesTreeReqID != null) {
-            this.#internalAPIRequester.abort(this.#zonesTreeReqID);
-            this.#zonesTreeReqID = null;
+        let filters = {};
+        if (this.#siteNameSearchElmt.value != "") {
+            filters["in_site_name"] = this.#siteNameSearchElmt.value;
+        }
+        if (this.#serviceStateFilterElmt.value == "on") {
+            filters["is_enabled"] = true;
+        } else if (this.#serviceStateFilterElmt.value == "off") {
+            filters["is_enabled"] = false;
         }
 
-        this.#zonesTreeReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.structural_elements.retrieve_tree_zones`),
+        this.#forecastWeatherListReqID = this.#internalAPIRequester.get(
+            flaskES6.urlFor(`api.services.weather_data.retrieve_forecast_list`, filters),
             (data) => {
-                this.#zonesTreeElmt.load(data.data);
-                this.#zonesTreeElmt.collapseAll();
+                this.#forecastWeatherServiceStatesContainerElmt.innerHTML = "";
+                if (data.length > 0) {
+                    for (let row of data) {
+                        row.is_enabled = row.is_enabled == null ? false : row.is_enabled;
+                        this.#forecastWeatherServiceStatesContainerElmt.appendChild(this.#createEntryElement(row, true));
+                    }
+                } else {
+                    let noItemElmt = document.createElement("p");
+                    noItemElmt.classList.add("fst-italic", "text-center", "text-muted", "w-100");
+                    noItemElmt.innerText = "No download weather data service states for sites";
+                    this.#forecastWeatherServiceStatesContainerElmt.appendChild(noItemElmt);
+                }
+
+                this.#forecastWeatherItemsCountElmt.update({
+                    firstItem: data.length > 0 ? 1 : 0,
+                    lastItem: data.length,
+                    totalCount: data.length
+                });
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
-                    text: error,
+                    text: error.toString(),
                     isDismissible: true
                 });
                 this.#messagesElmt.appendChild(flashMsgElmt);
             },
         );
     }
 
-    #generateHelpElement(helpContext) {
-        let helpContainerElmt = document.createElement("div");
-        helpContainerElmt.classList.add("alert", "alert-info", "mb-0", "pb-0");
-
-        let helpIconElmt = document.createElement("i");
-        helpIconElmt.classList.add("bi", "bi-question-diamond", "me-2");
-        helpContainerElmt.appendChild(helpIconElmt);
-
-        let helpTitleElmt = document.createElement("span");
-        helpTitleElmt.classList.add("fw-bold");
-        helpTitleElmt.innerText = "Help";
-        helpContainerElmt.appendChild(helpTitleElmt);
-
-        let helpTextElmt = document.createElement("p");
-        helpTextElmt.innerHTML = `Select a <span class="fw-bold">location (site, building...)</span> in the tree to see its <span class="fw-bold">${helpContext}</span>.`;
-        helpContainerElmt.appendChild(helpTextElmt);
-
-        return helpContainerElmt;
-    }
-
-    #refreshTabs() {
-        let selectedItemData = this.#selectedItemsPerTab[this.#tabSitesSelected.id];
-        if (selectedItemData != null) {
-            if (!this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id]) {
-                this.#renderPerTab[this.#tabPropertiesSelected.id]?.call(this, selectedItemData.id, selectedItemData.type, selectedItemData.path);
-                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = true;
-            }
-        } else {
-            this.#generalTabContentElmt.innerHTML = "";
-            this.#generalTabContentElmt.appendChild(this.#generateHelpElement("description"));
-            this.#propertiesTabContentElmt.innerHTML = "";
-            this.#propertiesTabContentElmt.appendChild(this.#generateHelpElement("properties"));
-            this.#tsListElmt.innerHTML = "";
-            this.#tsListElmt.appendChild(this.#generateHelpElement("related timeseries"));
-            this.#eventsListElmt.innerHTML = "";
-            this.#eventsListElmt.appendChild(this.#generateHelpElement("related events"));
-        }
+    mount() {
+        this.#refreshWeatherList();
+        this.#refreshForecastWeatherList();
     }
+}
 
-    render(id, type, path) {
-        this.#selectedItemsPerTab[this.#tabSitesSelected.id] = {
-            id: id,
-            type: type,
-            path: path
-        };
-        for (let tabElmt of this.#tabPropertiesElmts) {
-            this.#alreadyLoadedPerTab[tabElmt.id] = false;
-        }
-        this.#tsPaginationElmt.reload();
-        this.#refreshTabs();
-    }
-
-    refresh() {
-        this.#loadSitesTreeData();
-        this.#loadZonesTreeData();
-        this.#refreshTabs();
-    }
-}
+
+document.addEventListener("DOMContentLoaded", () => {
+
+    let view = new WeatherDataServiceManageView();
+    view.mount();
+
+});
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/delete.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/delete.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/list.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/list.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -285,26 +285,27 @@
         };
 
         let timestampsCardElmt = document.createElement("div");
         timestampsCardElmt.classList.add("card", "mb-auto");
         statsContainerElmt.appendChild(timestampsCardElmt);
         let timestampsCardHeaderElmt = document.createElement("div");
         timestampsCardHeaderElmt.classList.add("card-header", "fw-bold");
-        timestampsCardHeaderElmt.innerText = "Timestamp bounds";
+        timestampsCardHeaderElmt.innerText = "Timestamps statistics";
         timestampsCardElmt.appendChild(timestampsCardHeaderElmt);
         let timestampsBoundsListElmt = document.createElement("ul");
         timestampsBoundsListElmt.classList.add("list-group", "list-group-flush");
         timestampsCardElmt.appendChild(timestampsBoundsListElmt);
         timestampsBoundsListElmt.appendChild(createListGroupItemElmt("First", tsDataStats["first_timestamp"] != null ? TimeDisplay.toLocaleString(new Date(tsDataStats["first_timestamp"]), {
             timezone: this.#tzName
         }) : "-"));
         timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Last", tsDataStats["last_timestamp"] != null ? TimeDisplay.toLocaleString(new Date(tsDataStats["last_timestamp"]), {
             timezone: this.#tzName
         }) : "-"));
-        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Elapsed", tsDataStats["elapsed_time"] || "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Period duration", tsDataStats["period_duration"] || "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Last data since", tsDataStats["last_data_since"] || "-"));
 
         let statsCardElmt = document.createElement("div");
         statsCardElmt.classList.add("card", "mb-auto");
         statsContainerElmt.appendChild(statsCardElmt);
         let statsCardHeaderElmt = document.createElement("div");
         statsCardHeaderElmt.classList.add("card-header", "fw-bold");
         statsCardHeaderElmt.innerText = "Values statistics";
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -22,33 +22,41 @@
 
 
 export class TimeseriesSemanticSetupView {
 
     #internalAPIRequester = null;
     #sitesTreeReqID = null;
     #weatherSetupGetReqID = null;
+    #forecastWeatherSetupGetReqID = null;
     #energyProdSetupGetReqID = null;
     #energyConsSetupGetReqID = null;
     #postReqIDByTab = {};
     #putReqIDByTab = {};
     #deleteReqIDByTab = {};
 
     #messagesElmt = null;
 
     #sitesTreeElmt = null;
     #weatherTabElmt = null;
+    #forecastWeatherTabElmt = null;
     #energyProdTabElmt = null;
     #energyConsTabElmt = null;
 
     #weatherSetupHelpElmt = null;
     #weatherSetupTableElmt = null;
     #weatherSetupItemsCountElmt = null;
     #weatherAddParamBtnElmt = null;
     #weatherAddParamMenuElmt = null;
 
+    #forecastWeatherSetupHelpElmt = null;
+    #forecastWeatherSetupTableElmt = null;
+    #forecastWeatherSetupItemsCountElmt = null;
+    #forecastWeatherAddParamBtnElmt = null;
+    #forecastWeatherAddParamMenuElmt = null;
+
     #energyProdSetupHelpElmt = null;
     #energyProdSetupTableElmt = null;
     #energyProdSetupItemsCountElmt = null;
     #energyProdAddEnergyBtnElmt = null;
     #energyProdAddEnergyMenuElmt = null;
 
     #energyConsSetupHelpElmt = null;
@@ -69,21 +77,24 @@
     #weatherParams = {};
     #energyProdTechs = {};
 
     #structuralElementType = null;
     #structuralElementId = null;
     // Weather setup (parameter <-> timeseries) by weather parameter.
     #weatherSetupByParam = {};
+    // Forecast weather setup (parameter <-> timeseries) by weather parameter.
+    #forecastWeatherSetupByParam = {};
     // Energy production setup by energy and production techno (energy <-> prod techno <-> timeseries).
     #energyProdSetupByEnergyAndTech = {};
     // Energy consumption setup by energy and energy use (energy <-> energy use <-> timeseries).
     #energyConsSetupByEnergyAndUses = {};
 
     #selectedTab = null;
     #weatherParamEdited = null;
+    #forecastWeatherParamEdited = null;
     #energyEdited = null;
     #endUseEdited = null;
     #prodTechEdited = null;
 
     constructor(energies, energyEndUses, weatherParams, energyProdTechs, isEditable) {
         this.#energies = energies;
         this.#energyEndUses = energyEndUses;
@@ -105,23 +116,30 @@
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
         this.#sitesTreeElmt = document.getElementById("sitesTree");
         this.#weatherTabElmt = document.getElementById("weather-tab");
+        this.#forecastWeatherTabElmt = document.getElementById("weatherForecast-tab");
         this.#energyProdTabElmt = document.getElementById("energyProd-tab");
         this.#energyConsTabElmt = document.getElementById("energyCons-tab");
 
         this.#weatherSetupHelpElmt = document.getElementById("weatherSetupHelp");
         this.#weatherSetupTableElmt = document.getElementById("weatherSetupTable");
         this.#weatherSetupItemsCountElmt = document.getElementById("weatherItemsCount");
         this.#weatherAddParamBtnElmt = document.getElementById("weatherAddParamBtn");
         this.#weatherAddParamMenuElmt = this.#weatherAddParamBtnElmt?.parentElement.querySelector("ul.dropdown-menu");
 
+        this.#forecastWeatherSetupHelpElmt = document.getElementById("weatherForecastSetupHelp");
+        this.#forecastWeatherSetupTableElmt = document.getElementById("weatherForecastSetupTable");
+        this.#forecastWeatherSetupItemsCountElmt = document.getElementById("weatherForecastItemsCount");
+        this.#forecastWeatherAddParamBtnElmt = document.getElementById("weatherForecastAddParamBtn");
+        this.#forecastWeatherAddParamMenuElmt = this.#forecastWeatherAddParamBtnElmt?.parentElement.querySelector("ul.dropdown-menu");
+
         this.#energyProdSetupHelpElmt = document.getElementById("energyProdSetupHelp");
         this.#energyProdSetupTableElmt = document.getElementById("energyProdSetupTable");
         this.#energyProdSetupItemsCountElmt = document.getElementById("energyProdItemsCount");
         this.#energyProdAddEnergyBtnElmt = document.getElementById("energyProdAddEnergyBtn");
         this.#energyProdAddEnergyMenuElmt = this.#energyProdAddEnergyBtnElmt?.parentElement.querySelector("ul.dropdown-menu");
 
         this.#energyConsSetupHelpElmt = document.getElementById("energyConsSetupHelp");
@@ -146,22 +164,27 @@
 
             let filters = {};
             filters[this.#structuralElementType] = this.#structuralElementId;
             this.#tsSelector.setFilters(filters);
             this.#tsSelector.clearAllSelection();
 
             this.#loadWeatherParametersSetup();
+            this.#loadForecastWeatherParametersSetup();
             this.#loadEnergyProductionSetup();
             this.#loadEnergyConsumptionSetup();
         });
 
         this.#weatherTabElmt.addEventListener("show.bs.tab", () => {
             this.#selectedTab = this.#weatherTabElmt;
         });
 
+        this.#forecastWeatherTabElmt.addEventListener("show.bs.tab", () => {
+            this.#selectedTab = this.#forecastWeatherTabElmt;
+        });
+
         this.#energyProdTabElmt.addEventListener("show.bs.tab", () => {
             this.#selectedTab = this.#energyProdTabElmt;
         });
 
         this.#energyConsTabElmt.addEventListener("show.bs.tab", () => {
             this.#selectedTab = this.#energyConsTabElmt;
         });
@@ -176,14 +199,15 @@
             event.preventDefault();
 
             this.#saveSelectedTimeseries();
         });
 
         this.#selectTimeseriesModalElmt?.addEventListener("hide.bs.modal", () => {
             this.#weatherParamEdited = null;
+            this.#forecastWeatherParamEdited = null;
             this.#energyEdited = null;
             this.#prodTechEdited = null;
             this.#endUseEdited = null;
         });
     }
 
     #internalApiErrorCallback(error) {
@@ -234,14 +258,15 @@
                 this.#selectTimeseriesModal.hide();
             };
 
             let payload = {
                 parameter: this.#weatherParamEdited,
                 site_id: this.#structuralElementId,
                 timeseries_id: this.#tsSelector.selectedItems[0].id,
+                forecast: false,
             };
 
             let weatherData = this.#weatherSetupByParam[this.#weatherParamEdited];
             if (weatherData.id == null) {
                 // Create setup (post call).
                 this.#postReqIDByTab[this.#selectedTab] = this.#internalAPIRequester.post(
                     flaskES6.urlFor(`api.semantics.weather.create`),
@@ -263,14 +288,69 @@
                     updateSetupDoneCallback,
                 );
             } else {
                 // Nothing to do but just hide timeseries selection modal.
                 this.#selectTimeseriesModal.hide();
             }
         }
+        // Forecast weather parameter tab case.
+        if (this.#selectedTab == this.#forecastWeatherTabElmt) {
+            let updateSetupCallback = (data) => {
+                let updatedData = data.data;
+                updatedData.etag = data.etag;
+                this.#forecastWeatherSetupByParam[updatedData.parameter] = updatedData;
+                this.#refreshSetup(updatedData.timeseries, `weatherForecast-${updatedData.parameter}`);
+            };
+            let updateSetupDoneCallback = () => {
+                let weatherData = this.#forecastWeatherSetupByParam[this.#forecastWeatherParamEdited];
+
+                let flashMsgElmt = new FlashMessage({
+                    type: FlashMessageTypes.SUCCESS,
+                    text: `${weatherData.parameter_label} weather parameter setup saved!`,
+                    isDismissible: true
+                });
+                this.#messagesElmt.appendChild(flashMsgElmt);
+
+                this.#selectTimeseriesModal.hide();
+            };
+
+            let payload = {
+                parameter: this.#forecastWeatherParamEdited,
+                site_id: this.#structuralElementId,
+                timeseries_id: this.#tsSelector.selectedItems[0].id,
+                forecast: true,
+            };
+
+            let weatherData = this.#forecastWeatherSetupByParam[this.#forecastWeatherParamEdited];
+            if (weatherData.id == null) {
+                // Create setup (post call).
+                this.#postReqIDByTab[this.#selectedTab] = this.#internalAPIRequester.post(
+                    flaskES6.urlFor(`api.semantics.weather.create`),
+                    payload,
+                    updateSetupCallback,
+                    this.#internalApiErrorCallback,
+                    updateSetupDoneCallback,
+                );
+            } else if (weatherData.timeseries_id != this.#tsSelector.selectedItems[0].id) {
+                // Update setup (put call).
+                this.#putReqIDByTab[this.#selectedTab] = this.#internalAPIRequester.put(
+                    flaskES6.urlFor(`api.semantics.weather.update`, {
+                        id: weatherData.id
+                    }),
+                    payload,
+                    weatherData.etag,
+                    updateSetupCallback,
+                    this.#internalApiErrorCallback,
+                    updateSetupDoneCallback,
+                );
+            } else {
+                // Nothing to do but just hide timeseries selection modal.
+                this.#selectTimeseriesModal.hide();
+            }
+        }
         // Energy production tab case.
         else if (this.#selectedTab == this.#energyProdTabElmt) {
             let updateSetupCallback = (data) => {
                 let updatedData = data.data;
                 updatedData.etag = data.etag;
                 this.#energyProdSetupByEnergyAndTech[updatedData.energy_id][updatedData.prod_tech_id] = updatedData;
                 this.#refreshSetup(updatedData.timeseries, `energyProd-${updatedData.energy_id}-${updatedData.prod_tech_id}`);
@@ -535,55 +615,63 @@
 
         return tdElmt;
     }
 
     #createWeatherParamRowElement(data) {
         let rowElmt = this.#createRowElement(data.parameter_label);
 
-        let suffixId = `weather-${data.parameter}`;
+        let suffixId = `weather${data.forecast ? "Forecast" : ""}-${data.parameter}`;
 
         let tdElmt = this.#createTimeseriesSetupCellElement(
             suffixId,
             `${data.timeseries_id != null ? `${data.timeseries.name}${data.timeseries.unit_symbol ? ` [${data.timeseries.unit_symbol}]` : ""}` : "none"}`,
             data.timeseries_id != null,
             () => {
-                this.#selectTimeseriesTargetTextElmt.innerText = `${data.parameter_label} weather parameter`;
+                this.#selectTimeseriesTargetTextElmt.innerText = `${data.parameter_label.toLowerCase()} weather parameter`;
                 this.#tsSelector.clearAllSelection();
                 this.#updateSaveBtnState();
 
                 // In update case, get resource etag if not known.
                 this.#reloadWeatherParameterSetupForEtag(
-                    data.parameter,
+                    data,
                     () => {
                         // Get up-to-date setup data.
-                        let dataToEdit = this.#weatherSetupByParam[data.parameter];
+                        let dataToEdit = data.forecast ? this.#forecastWeatherSetupByParam[data.parameter] : this.#weatherSetupByParam[data.parameter];
                         if (dataToEdit.timeseries_id != null) {
                             this.#tsSelector.select(dataToEdit.timeseries_id, () => {
                                 this.#updateSaveBtnState();
                             });
                         }
                     },
                 );
 
-                this.#weatherParamEdited = data.parameter;
+                if (!data.forecast) {
+                    this.#weatherParamEdited = data.parameter;
+                } else {
+                    this.#forecastWeatherParamEdited = data.parameter;
+                }
             },
             `Remove <mark>${data.parameter_label}</mark> weather parameter setup`,
             () => {
-                let dataToDelete = this.#weatherSetupByParam[data.parameter];
+                let dataToDelete = data.forecast ? this.#forecastWeatherSetupByParam[data.parameter] : this.#weatherSetupByParam[data.parameter];
                 this.#deleteReqIDByTab[this.#selectedTab] = this.#internalAPIRequester.delete(
                     flaskES6.urlFor(`api.semantics.weather.delete`, {
                         id: dataToDelete.id
                     }),
                     dataToDelete.etag,
                     () => {
                         dataToDelete.id = null;
                         dataToDelete.timeseries_id = null;
                         dataToDelete.timeseries = null;
                         dataToDelete.etag = null;
-                        this.#weatherSetupByParam[dataToDelete.parameter] = dataToDelete;
+                        if (!dataToDelete.forecast) {
+                            this.#weatherSetupByParam[dataToDelete.parameter] = dataToDelete;
+                        } else {
+                            this.#forecastWeatherSetupByParam[dataToDelete.parameter] = dataToDelete;
+                        }
 
                         this.#refreshSetup(dataToDelete.timeseries, suffixId);
                     },
                     this.#internalApiErrorCallback,
                     () => {
                         let flashMsgElmt = new FlashMessage({
                             type: FlashMessageTypes.SUCCESS,
@@ -593,37 +681,45 @@
                         this.#messagesElmt.appendChild(flashMsgElmt);
                     },
                 );
             },
             () => {
                 // In delete case, get resource etag if not known.
                 this.#reloadWeatherParameterSetupForEtag(
-                    data.parameter,
+                    data,
                     () => {
-                        this.#weatherParamEdited = data.parameter;
+                        if (!data.forecast) {
+                            this.#weatherParamEdited = data.parameter;
+                        } else {
+                            this.#forecastWeatherParamEdited = data.parameter;
+                        }
                     },
                 );
             },
         );
         rowElmt.appendChild(tdElmt);
 
         return rowElmt;
     }
 
-    #reloadWeatherParameterSetupForEtag(weatherParam, afterEtagLoadedCallback = null) {
-        let weatherData = this.#weatherSetupByParam[weatherParam];
+    #reloadWeatherParameterSetupForEtag(weatherTsData, afterEtagLoadedCallback = null) {
+        let weatherData = weatherTsData.forecast ? this.#forecastWeatherSetupByParam[weatherTsData.parameter] : this.#weatherSetupByParam[weatherTsData.parameter];
         if (weatherData.id != null && weatherData.etag == null) {
             this.#internalAPIRequester.get(
                 flaskES6.urlFor(`api.semantics.weather.retrieve_one`, {
                     id: weatherData.id
                 }),
                 (data) => {
                     weatherData = data.data;
                     weatherData.etag = data.etag;
-                    this.#weatherSetupByParam[weatherParam] = weatherData;
+                    if (!weatherData.forecast) {
+                        this.#weatherSetupByParam[weatherTsData.parameter] = weatherData;
+                    } else {
+                        this.#forecastWeatherSetupByParam[weatherTsData.parameter] = weatherData;
+                    }
 
                     afterEtagLoadedCallback?.();
                 },
                 this.#internalApiErrorCallback,
             );
         } else {
             afterEtagLoadedCallback?.();
@@ -646,15 +742,16 @@
             if (this.#weatherSetupGetReqID != null) {
                 this.#internalAPIRequester.abort(this.#weatherSetupGetReqID);
                 this.#weatherSetupGetReqID = null;
             }
 
             this.#weatherSetupGetReqID = this.#internalAPIRequester.get(
                 flaskES6.urlFor(`api.semantics.weather.list`, {
-                    site: this.#structuralElementId
+                    site: this.#structuralElementId,
+                    forecast: false
                 }),
                 (data) => {
                     tableBodyElmt.innerHTML = "";
                     if (data.data.length > 0) {
                         for (let row of data.data) {
                             this.#weatherSetupByParam[row.parameter] = row;
                             let itemElmt = this.#createWeatherParamRowElement(row);
@@ -686,14 +783,15 @@
                                     let weatherParamSetup = {
                                         "id": null,
                                         "parameter": weatherParamID,
                                         "parameter_label": weatherParamLabel,
                                         "timeseries": null,
                                         "site_id": this.#structuralElementId,
                                         "timeseries_id": null,
+                                        "forecast": false,
                                     };
 
                                     if (Object.keys(this.#weatherSetupByParam).length <= 0) {
                                         tableBodyElmt.innerHTML = "";
                                     }
                                     let rowElmt = this.#createWeatherParamRowElement(weatherParamSetup);
                                     tableBodyElmt.appendChild(rowElmt);
@@ -724,27 +822,127 @@
         this.#weatherSetupItemsCountElmt.update({
             totalCount: totalCount,
             firstItem: totalCount > 0 ? 1 : 0,
             lastItem: totalCount
         });
     }
 
-    #createEnergyProdRowElement(energyID, energyName, energyProdSetup) {
+    #loadForecastWeatherParametersSetup() {
+        this.#forecastWeatherSetupByParam = {};
+
+        if (this.#structuralElementType == "site") {
+            this.#forecastWeatherSetupHelpElmt.classList.add("d-none", "invisible");
+            this.#forecastWeatherSetupTableElmt.parentElement.classList.remove("d-none", "invisible");
+            this.#forecastWeatherAddParamBtnElmt.parentElement.classList.remove("d-none", "invisible");
+
+            let tableBodyElmt = this.#forecastWeatherSetupTableElmt.querySelector("tbody");
+            tableBodyElmt.innerHTML = "";
+            tableBodyElmt.appendChild(new Spinner());
+            this.#forecastWeatherSetupItemsCountElmt.setLoading();
+
+            if (this.#forecastWeatherSetupGetReqID != null) {
+                this.#internalAPIRequester.abort(this.#forecastWeatherSetupGetReqID);
+                this.#forecastWeatherSetupGetReqID = null;
+            }
+
+            this.#forecastWeatherSetupGetReqID = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.semantics.weather.list`, {
+                    site: this.#structuralElementId,
+                    forecast: true
+                }),
+                (data) => {
+                    tableBodyElmt.innerHTML = "";
+                    if (data.data.length > 0) {
+                        for (let row of data.data) {
+                            this.#forecastWeatherSetupByParam[row.parameter] = row;
+                            let itemElmt = this.#createWeatherParamRowElement(row);
+                            tableBodyElmt.appendChild(itemElmt);
+                        }
+                    } else {
+                        let trElmt = document.createElement("tr");
+                        tableBodyElmt.appendChild(trElmt);
+
+                        let tdElmt = document.createElement("td");
+                        tdElmt.setAttribute("colspan", 2);
+                        trElmt.appendChild(tdElmt);
+
+                        let noItemElmt = document.createElement("p");
+                        noItemElmt.classList.add("fst-italic", "text-center", "text-muted", "pt-2", "w-100");
+                        noItemElmt.innerText = "Nothing configured yet";
+                        tdElmt.appendChild(noItemElmt);
+                    }
+
+                    this.#updateForecastWeatherItemsCount();
+
+                    let definedWeatherParamIDs = Object.keys(this.#forecastWeatherSetupByParam);
+                    this.#forecastWeatherAddParamMenuElmt.innerHTML = "";
+                    for (let [weatherParamID, weatherParamLabel] of Object.entries(this.#weatherParams)) {
+                        if (!definedWeatherParamIDs.includes(weatherParamID)) {
+                            let menuItemElmt = this.#createDropDownMenuItemElement(
+                                weatherParamLabel,
+                                () => {
+                                    let weatherParamSetup = {
+                                        "id": null,
+                                        "parameter": weatherParamID,
+                                        "parameter_label": weatherParamLabel,
+                                        "timeseries": null,
+                                        "site_id": this.#structuralElementId,
+                                        "timeseries_id": null,
+                                        "forecast": true,
+                                    };
+
+                                    if (Object.keys(this.#forecastWeatherSetupByParam).length <= 0) {
+                                        tableBodyElmt.innerHTML = "";
+                                    }
+                                    let rowElmt = this.#createWeatherParamRowElement(weatherParamSetup);
+                                    tableBodyElmt.appendChild(rowElmt);
+
+                                    this.#forecastWeatherSetupByParam[weatherParamID] = weatherParamSetup;
+
+                                    this.#updateForecastWeatherItemsCount();
+
+                                    if (this.#forecastWeatherAddParamMenuElmt.childElementCount <= 0) {
+                                        this.#forecastWeatherAddParamBtnElmt.parentElement.classList.add("d-none", "invisible");
+                                    }
+                                },
+                            );
+                            this.#forecastWeatherAddParamMenuElmt.appendChild(menuItemElmt);
+                        }
+                    }
+                },
+                this.#internalApiErrorCallback,
+            );
+        } else {
+            this.#forecastWeatherSetupHelpElmt.classList.remove("d-none", "invisible");
+            this.#forecastWeatherSetupTableElmt.parentElement.classList.add("d-none", "invisible");
+        }
+    }
+
+    #updateForecastWeatherItemsCount() {
+        let totalCount = Object.keys(this.#forecastWeatherSetupByParam).length;
+        this.#forecastWeatherSetupItemsCountElmt.update({
+            totalCount: totalCount,
+            firstItem: totalCount > 0 ? 1 : 0,
+            lastItem: totalCount
+        });
+    }
+
+    #createEnergyProdRowElement(energ7261530yID, energyName, energyProdSetup) {
         let rowElmt = this.#createRowElement(energyName);
 
         for (let energyProdTechSetup of Object.values(energyProdSetup)) {
             let suffixId = `energyProd-${energyProdTechSetup.energy_id}-${energyProdTechSetup.prod_tech_id}`;
             let prodTechName = this.#energyProdTechs[energyProdTechSetup.prod_tech_id];
 
             let tdElmt = this.#createTimeseriesSetupCellElement(
                 suffixId,
                 `${energyProdTechSetup.timeseries_id != null ? `${energyProdTechSetup.timeseries.name}${energyProdTechSetup.timeseries.unit_symbol ? ` [${energyProdTechSetup.timeseries.unit_symbol}]` : ""}` : "none"}`,
                 energyProdTechSetup.timeseries_id != null,
                 () => {
-                    this.#selectTimeseriesTargetTextElmt.innerText = `[${energyName} - ${prodTechName}] energy production`;
+                    this.#selectTimeseriesTargetTextElmt.innerText = `${energyName.toLowerCase()} energy production of ${prodTechName.toLowerCase()} system`;
                     this.#tsSelector.clearAllSelection();
                     this.#updateSaveBtnState();
 
                     // In update case, get resource etag if not known.
                     this.#reloadEnergyProdSetupForEtag(
                         energyProdTechSetup.energy_id,
                         energyProdTechSetup.prod_tech_id,
@@ -957,15 +1155,15 @@
             let endUseName = this.#energyEndUses[energyConsEndUseSetup.end_use_id];
 
             let tdElmt = this.#createTimeseriesSetupCellElement(
                 suffixId,
                 `${energyConsEndUseSetup.timeseries_id != null ? `${energyConsEndUseSetup.timeseries.name}${energyConsEndUseSetup.timeseries.unit_symbol ? ` [${energyConsEndUseSetup.timeseries.unit_symbol}]` : ""}` : "none"}`,
                 energyConsEndUseSetup.timeseries_id != null,
                 () => {
-                    this.#selectTimeseriesTargetTextElmt.innerText = `[${energyName} - ${endUseName}] energy consumption`;
+                    this.#selectTimeseriesTargetTextElmt.innerText = `${energyName.toLowerCase()} energy consumption of ${endUseName.toLowerCase()} end use`;
                     this.#tsSelector.clearAllSelection();
                     this.#updateSaveBtnState();
 
                     // In update case, get resource etag if not known.
                     this.#reloadEnergyConsSetupForEtag(
                         energyConsEndUseSetup.energy_id,
                         energyConsEndUseSetup.end_use_id,
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/list.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/scripts/modules/views/users/manageGroups.js` & `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/styles/app.css` & `bemserver-ui-0.5.2/bemserver_ui/static/styles/app.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/styles/main.css` & `bemserver-ui-0.5.2/bemserver_ui/static/styles/main.css`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,26 @@
 
 input:invalid:not(:focus) {
     border-color: var(--bs-danger);
     border-left-width: 8px;
     background-color: rgba(var(--bs-danger-rgb), 0.05);
 }
 
+/* Firefow */
+input[type=number].hide-arrows {
+    -moz-appearance: textfield;
+    appearance: textfield;
+}
+/* Chrome, Safari, Edge, Opera */
+input[type=number].hide-arrows::-webkit-outer-spin-button,
+input[type=number].hide-arrows::-webkit-inner-spin-button {
+  -webkit-appearance: none;
+  margin: 0;
+}
+
 .vr {
     color: var(--app-gray) !important;
 }
 
 .badge.bg-primary {
     background-color: rgba(var(--app-blue-rgb), var(--bs-bg-opacity)) !important;
 }
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/styles/signin.css` & `bemserver-ui-0.5.2/bemserver_ui/static/styles/signin.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/static/styles/tree.css` & `bemserver-ui-0.5.2/bemserver_ui/static/styles/tree.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/campaigns/selector.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/campaigns/selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/header.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/header.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_admin.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_admin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_analysis.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_analysis.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_services.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_services.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/user_groups/user_group_available.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/user_group_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_available.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/components/users/user_for_group.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_for_group.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/sidebar.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/structural_element_selector.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/structural_element_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/macros/components/ts_selector.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/ts_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/macros/flash.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/macros/flash.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/macros/partners.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/macros/partners.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/about.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/about.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/degree_days.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/degree_days.html`

 * *Files 1% similar despite different names*

```diff
@@ -91,10 +91,10 @@
     </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
 {% filter indent(width=8, first=True) %}
-<script type="module" src="{{ url_for('static', filename='scripts/modules/views/analysis/degreeDays.js') }}" async></script>
+<script type="module" src="{{ url_for('static', filename='scripts/modules/views/analysis/degreeDays.js') }}" defer></script>
 {% endfilter %}
 {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/analysis/energy_consumption.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/energy_consumption.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/base.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/base.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaign_scopes/view.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/manage_groups.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/manage_groups.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/campaigns/view.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/categories/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/events/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/home.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/explore.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/notifications/setup.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/cleanup/manage.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/missing_data/manage.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/outlier_data/manage.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/services/weather_data/manage.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,99 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Weather data service" %}
+{% set title = "User group" %}
+{% set subtitle = "Manage users" %}
+
+{% block main_toolbar %}
+{{ super() -}}
+{% filter indent(width=20, first=True) %}
+<div class="d-lg-flex d-grid gap-2">
+    <a href="{{ url_for('user_groups.view', id=user_group.id) }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage user group"><i class="bi bi-arrow-return-left"></i> Back to user group</a>
+    <div class="vr d-none d-lg-block mx-2"></div>
+    <div class="hstack gap-2 ms-auto">
+        {% if signed_user.is_admin %}
+        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; user group">
+            <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
+            <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
+        </form>
+        {% endif %}
+        <a href="{{ url_for('user_groups.edit', id=user_group.id) }}" class="btn btn-sm btn-outline-primary text-nowrap" role="button" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
+    </div>
+</div>
+{% endfilter %}
+{% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
-    <div class="row g-5 mb-3">
-        <div class="col-auto">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if g.campaign_ctxt.campaign.state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ g.campaign_ctxt.campaign.state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ g.campaign_ctxt.name }}</p>
-        </div>
+    <div class="row mb-3">
         <div class="col">
-            <div class="alert alert-info border border-info mb-0" role="alert">
-                <i class="bi bi-info-square me-1"></i>
-                For each site, {% if signed_user.is_admin %}by using the ON/OFF buttons below, {% endif %}weather data can be fetched automatically from <a href="https://oikolab.com/" target="_blank">oikolab</a> web service.
-                {% if signed_user.is_admin %}
-                <p class="mb-0">You can also do it manually using the fetch data button (<i class="bi bi-cloud-download text-primary"></i>), weither the automatic fetch service is enabled or not.</p>
-                {% endif %}
-            </div>
+            <h5>Group</h5>
+            <p class="text-break">{{ user_group.name }}</p>
         </div>
     </div>
-    <div class="row mb-2">
-        <div class="col">
-            <div class="accordion" id="accordionFilters">
-                <div class="accordion-item">
-                    <h2 class="accordion-header" id="headingFilters">
-                        <button class="accordion-button{% if not is_filtered %} collapsed{% endif %}" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFilters" aria-controls="collapseFilters" aria-expanded="{{ is_filtered | lower }}">
-                            <span class="fw-bold text-secondary"><i class="bi bi-funnel"></i> Filters</span>
-                        </button>
-                    </h2>
-                    <div id="collapseFilters" class="accordion-collapse collapse{% if is_filtered %} show{% endif %}" aria-labelledby="headingFilters" data-bs-parent="#accordionFilters">
-                        <div class="accordion-body">
-                            <div id="filtersContainer" class="d-sm-flex d-grid align-items-center gap-2">
-                                <input type="text" class="form-control form-control-sm" id="siteNameSearch" placeholder="Site..." aria-label="Site name search" aria-describedby="siteNameSearch" autofocus>
-                                <a id="removeFiltersBtn" class="btn btn-sm btn-outline-secondary text-nowrap my-auto" role="button" title="Remove filters"><i class="bi bi-eraser"></i> Remove</a>
-                            </div>
-                        </div>
-                    </div>
+    <div class="row">
+        <div class="col pb-3 pb-lg-0">
+            <h5>
+                Members <span class="badge bg-secondary">{{ users|length }}</span>
+                {% if users|length > 0 %}
+                <sup><a class="link-secondary" title="Help" role="button" data-bs-toggle="collapse" data-bs-target="#helpMembers" aria-expanded="false" aria-controls="helpMembers"><i class="bi bi-question-diamond"></i></a></sup>
+                {% endif %}
+            </h5>
+            {% if users|length > 0 %}
+            <div class="collapse mb-3" id="helpMembers">
+                <div class="alert alert-info pb-0" role="alert">
+                    <span class="fw-bold"><i class="bi bi-question-diamond"></i> Help</span>
+                    <p class="ms-3">Click on <span class="btn btn-sm btn-outline-danger px-1 py-0"><i class="bi bi-x-lg"></i></span> button to remove a user from <span class="fw-bold fst-italic">{{ user_group.name }}</span></p>
                 </div>
             </div>
+            <div class="d-flex flex-wrap mt-2 gap-2">
+                {% for user in users %}
+                {% filter indent(width=16) %}
+                {% include "components/users/user_for_group.html" %}
+                {% endfilter %}
+                {% endfor %}
+            </div>
+            {% else %}
+            <span class="fst-italic text-muted">none</span>
+            {% endif %}
         </div>
-    </div>
-    <div class="row">
-        <div class="table-responsive-xl">
-            <table class="table table-sm table-hover caption-top">
-                <caption class="text-end">
-                    <small class="text-nowrap text-muted"><app-items-count id="itemsCount"></app-items-count></small>
-                </caption>
-                <thead>
-                    <tr>
-                        <th scope="col">Site</th>
-                        <th scope="col">State</th>
-                        {% if signed_user.is_admin %}
-                        <th scope="col">Fetch data</th>
+        <div class="w-100 d-lg-none d-block"></div>
+        <div class="col">
+            <div class="hstack">
+                <div class="vr d-none d-lg-block me-lg-4"></div>
+                <div class="w-100">
+                    <h5>
+                        Available users <span class="badge bg-secondary">{{ available_users|length }}</span>
+                        {% if available_users|length > 0 %}
+                        <sup><a class="link-secondary" title="Help" role="button" data-bs-toggle="collapse" data-bs-target="#helpAvailable" aria-expanded="false" aria-controls="helpAvailable"><i class="bi bi-question-diamond"></i></a></sup>
                         {% endif %}
-                    </tr>
-                </thead>
-                <tbody class="table-group-divider" id="serviceStatesContainer">
-                </tbody>
-            </table>
-        </div>
-    </div>
-</div>
-{% if signed_user.is_admin %}
-<div class="modal fade" id="fetchDataModal" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="fetchDataModalLabel" aria-hidden="true">
-    <div class="modal-dialog modal-lg modal-dialog-centered">
-        <div class="modal-content">
-            <div class="modal-header">
-                <h5 class="modal-title" id="fetchDataModalLabel">Fetch weather data</h5>
-                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
-            </div>
-            <div class="modal-body">
-                <input type="hidden" id="fetchDataSiteId">
-                <div class="row d-xl-flex d-grid mb-4">
-                    <div class="col pb-2 pb-xl-0">
-                        <div is="app-datetime-picker" id="fetchDataDatetimeStart" title="From" time="00:00" tzname="{{ g.campaign_ctxt.tz_name }}" required>
-                            <div is="app-spinner"></div>
+                    </h5>
+                    {% if available_users|length > 0 %}
+                    <div class="collapse mb-3" id="helpAvailable">
+                        <div class="alert alert-info pb-0" role="alert">
+                            <span class="fw-bold"><i class="bi bi-question-diamond"></i> Help</span>
+                            <ol>
+                                <li>Click on the users below to select/unselect them</li>
+                                <li>Click on <div class="btn btn-sm btn-primary">Set users</div> button to set selected users as members of <span class="fw-bold fst-italic">{{ user_group.name }}</span></li>
+                            </ol>
                         </div>
                     </div>
-                    <div class="col">
-                        <div is="app-datetime-picker" id="fetchDataDatetimeEnd" title="Until" time="00:00" tzname="{{ g.campaign_ctxt.tz_name }}" required>
-                            <div is="app-spinner"></div>
-                        </div>
-                        <small class="fst-italic text-muted">(excluded from the interval)</small>
+                    <form id="addUsersForm" class="d-flex flex-wrap gap-2" action="{{ url_for('user_groups.manage', id=user_group.id) }}" method="POST">
+                        {% for user in available_users %}
+                        {% filter indent(width=16) %}
+                        {% include "components/users/user_available.html" %}
+                        {% endfilter %}
+                        {% endfor %}
+                    </form>
+                    <div class="d-flex justify-content-end gap-2 mt-3">
+                        <button class="btn btn-sm btn-primary" type="submit" form="addUsersForm" title="Save">Set users</button>
                     </div>
+                    {% else %}
+                    <span class="fst-italic text-muted">none</span>
+                    {% endif %}
                 </div>
-                <div id="fetchDataModalParamsContainer"></div>
-            </div>
-            <div class="modal-footer d-flex justify-content-end gap-2">
-                <button type="button" class="btn btn-sm btn-outline-secondary" data-bs-dismiss="modal">Cancel</button>
-                <button id="fetchDataBtn" type="button" class="btn btn-sm btn-primary" disabled><i class="bi bi-cloud-download"></i> Fetch</button>
             </div>
         </div>
     </div>
 </div>
-{% endif %}
-{% endblock main_content %}
-
-{% block body_scripts %}
-{{ super() -}}
-{% filter indent(width=8, first=True) %}
-<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/weatherData/manage.js') }}"></script>
-{% endfilter %}
-{% endblock body_scripts %}
+{% endblock main_content %}
```

#### html2text {}

```diff
@@ -1,22 +1,32 @@
-{% extends "pages/base.html" %} {% set title = "Weather data service" %} {%
-block main_content %} {{ super() -}}
-** Campaign **
-[{{ g.campaign_ctxt.campaign.state | upper }}]
-{{ g.campaign_ctxt.name }}
- For each site, {% if signed_user.is_admin %}by using the ON/OFF buttons below,
-{% endif %}weather data can be fetched automatically from oikolab web service.
+{% extends "pages/base.html" %} {% set title = "User group" %} {% set subtitle
+= "Manage users" %} {% block main_toolbar %} {{ super() -}} {% filter indent
+(width=20, first=True) %}
+ Back_to_user_group
 {% if signed_user.is_admin %}
-You can also do it manually using the fetch data button (), weither the
-automatic fetch service is enabled or not.
+  Delete
 {% endif %}
-  Filters
-[                    ]
- Remove
-Site State Fetch data
-{% if signed_user.is_admin %}
-** Fetch weather data **
-(excluded from the interval)
-Cancel  Fetch
-{% endif %} {% endblock main_content %} {% block body_scripts %} {{ super() -}}
-{% filter indent(width=8, first=True) %}
- {% endfilter %} {% endblock body_scripts %}
+ Edit
+{% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
+-}}
+** Group **
+{{ user_group.name }}
+Members {{ users|length }} {% if users|length > 0 %}  {% endif %}
+{% if users|length > 0 %}
+ Help
+Click on  button to remove a user from {{ user_group.name }}
+{% for user in users %} {% filter indent(width=16) %} {% include "components/
+users/user_for_group.html" %} {% endfilter %} {% endfor %}
+{% else %} none {% endif %}
+Available users {{ available_users|length }} {% if available_users|length > 0
+%}  {% endif %}
+{% if available_users|length > 0 %}
+ Help
+   1. Click on the users below to select/unselect them
+   2. Click on
+      Set users
+      button to set selected users as members of {{ user_group.name }}
+{% for user in available_users %} {% filter indent(width=16) %} {% include
+"components/users/user_available.html" %} {% endfilter %} {% endfor %}
+Set users
+{% else %} none {% endif %}
+{% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/signin.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/signin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/skeleton.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/skeleton.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/create.html`

 * *Files 3% similar despite different names*

```diff
@@ -32,32 +32,34 @@
                         </select>
                     </div>
                     {% endif %}
                     <div class="mb-3">
                         <label class="form-label" for="name">Name</label>
                         <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
                     </div>
+                    {% if type == 'site' %}
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
+                            <input type="number" class="form-control hide-arrows" id="latitude" name="latitude" min="-90" max="90" step="any">
+                        </div>
+                        <div class="col">
+                            <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
+                            <input type="number" class="form-control hide-arrows" id="longitude" name="longitude" min="-180" max="180" step="any">
+                        </div>
+                    </div>
+                    {% endif %}
                     <div class="mb-3">
                         <label class="form-label" for="description">Description</label>
                         <textarea class="form-control" id="description" name="description" maxlength="500" rows="3"></textarea>
                     </div>
                     <div class="mb-3">
                         <label class="form-label" for="ifc_id">IFC ID</label>
                         <input type="text" class="form-control" id="ifc_id" name="ifc_id" maxlength="22">
                     </div>
-                    {% if type == 'site' %}
-                    <div class="mb-3">
-                        <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
-                        <input type="number" class="form-control" id="latitude" name="latitude" min="-90" max="90" step="0.00001">
-                    </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
-                        <input type="number" class="form-control" id="longitude" name="longitude" min="-180" max="180" step="0.00001">
-                    </div>
-                    {% endif %}
                 </fieldset>
                 <div class="d-flex justify-content-end gap-2">
                     <a href="{{ url_for('structural_elements.explore') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                     <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"{% if has_no_parents %} disabled{% endif %}><i class="bi bi-save"></i> Save</button>
                 </div>
             </form>
         </div>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 % if has_no_parents %} disabled{% endif %}> {{ type|capitalize }} general
 informations {% if parent_type is not none and parents|length > 0 %}
 {% for x in parents %}
 {{ x.name }}
 {% endfor %}
 {% endif %}
 Name [name                ]
-IFC ID [ifc_id              ]
 {% if type == 'site' %}
 Latitude [Â°] [Unknown INPUT type]
 Longitude [Â°] [Unknown INPUT type]
 {% endif %}
+IFC ID [ifc_id              ]
 Cancel
 % if has_no_parents %} disabled{% endif %}> Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/edit.html`

 * *Files 2% similar despite different names*

```diff
@@ -32,32 +32,34 @@
                 <div class="tab-pane fade{% if tab == 'general' %} show active{% endif %} p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab">
                     <fieldset>
                         <legend class="invisible d-none">{{ type|capitalize }} general informations</legend>
                         <div class="mb-3">
                             <label class="form-label" for="name">Name</label>
                             <input type="text" form="editForm" class="form-control" id="name" name="name" value="{{ structural_element.name }}" minlength="1" maxlength="80" required autofocus>
                         </div>
+                        {% if type == "site" %}
+                        <div class="row mb-3">
+                            <div class="col">
+                                <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
+                                <input type="number" form="editForm" class="form-control hide-arrows" id="latitude" name="latitude" min="-90" max="90" step="any" value="{{ structural_element.latitude }}">
+                            </div>
+                            <div class="col">
+                                <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
+                                <input type="number" form="editForm" class="form-control hide-arrows" id="longitude" name="longitude" min="-180" max="180" step="any" value="{{ structural_element.longitude }}">
+                            </div>
+                        </div>
+                        {% endif %}
                         <div class="mb-3">
                             <label class="form-label" for="description">Description</label>
                             <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ structural_element.description }}</textarea>
                         </div>
                         <div class="mb-3">
                             <label class="form-label" for="ifc_id">IFC ID</label>
                             <input type="text" form="editForm" class="form-control" id="ifc_id" name="ifc_id" value="{{ structural_element.ifc_id }}" maxlength="22">
                         </div>
-                        {% if type == "site" %}
-                        <div class="mb-3">
-                            <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
-                            <input type="number" form="editForm" class="form-control" id="latitude" name="latitude" min="-90" max="90" step="0.00001" value="{{ structural_element.latitude }}">
-                        </div>
-                        <div class="mb-3">
-                            <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
-                            <input type="number" form="editForm" class="form-control" id="longitude" name="longitude" min="-180" max="180" step="0.00001" value="{{ structural_element.longitude }}">
-                        </div>
-                        {% endif %}
                     </fieldset>
                 </div>
                 <div class="tab-pane fade{% if tab == 'properties' %} show active{% endif %} p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab">
                     <fieldset>
                         <legend class="invisible d-none">{{ type|capitalize }} properties</legend>
                         {% for property_id, property_data in properties.items() %}
                         <div class="mb-3">
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/explore.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/properties/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/structural_elements/upload.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/completeness.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/completeness.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/delete.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/delete.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/explore.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/data/upload.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/datastates/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/properties/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/semantic_setup.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/semantic_setup.html`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         <div class="col">
             <h5 class="text-secondary"><i class="bi bi-clock-history"></i> Timeseries semantic setup</h5>
             <ul class="nav nav-tabs app-tabs" role="tablist">
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'weather' %} active{% endif %}" id="weather-tab" data-bs-toggle="tab" data-bs-target="#weather-tabcontent" type="button" role="tab" aria-controls="weather-tabcontent" aria-selected="{% if tab == 'weather' %}true{% else %}false{% endif %}">Weather</button>
                 </li>
                 <li class="nav-item" role="presentation">
+                    <button class="nav-link{% if tab == 'weather_forecast' %} active{% endif %}" id="weatherForecast-tab" data-bs-toggle="tab" data-bs-target="#weatherForecast-tabcontent" type="button" role="tab" aria-controls="weatherForecast-tabcontent" aria-selected="{% if tab == 'weather_forecast' %}true{% else %}false{% endif %}">Weather forecast</button>
+                </li>
+                <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'energy_prod' %} active{% endif %}" id="energyProd-tab" data-bs-toggle="tab" data-bs-target="#energyProd-tabcontent" type="button" role="tab" aria-controls="energyProd-tabcontent" aria-selected="{% if tab == 'energy_prod' %}true{% else %}false{% endif %}">Energy production</button>
                 </li>
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'energy_cons' %} active{% endif %}" id="energyCons-tab" data-bs-toggle="tab" data-bs-target="#energyCons-tabcontent" type="button" role="tab" aria-controls="energyCons-tabcontent" aria-selected="{% if tab == 'energy_cons' %}true{% else %}false{% endif %}">Energy consumption</button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white mb-3">
@@ -65,14 +68,48 @@
                                             </div>
                                             {% endif %}
                                         </div>
                                     </th>
                                     <th scope="col" class="text-center align-middle">Timeseries</th>
                                 </tr>
                             </thead>
+                            <tbody class="table-group-divider">
+                            </tbody>
+                        </table>
+                    </div>
+                </div>
+                <div class="tab-pane{% if tab == 'weather_forecast' %} show active{% endif %} p-3" id="weatherForecast-tabcontent" role="tabpanel" aria-labelledby="weatherForecast-tab">
+                    <div class="alert alert-info mb-0 pb-0" id="weatherForecastSetupHelp">
+                        <i class="bi bi-question-diamond me-2"></i>
+                        <span class="fw-bold">Help</span>
+                        <p>Select a <span class="fw-bold">site</span> in the tree to see its <span class="fw-bold">weather forecast parameters</span> setup.</p>
+                    </div>
+                    <div class="table-responsive-xl d-none invisible">
+                        <table class="table table-sm table-bordered caption-top" id="weatherForecastSetupTable">
+                            <caption class="text-end">
+                                <small><app-items-count id="weatherForecastItemsCount"></app-items-count></small>
+                            </caption>
+                            <thead>
+                                <tr>
+                                    <th scope="col" class="align-middle w-25">
+                                        <div class="hstack justify-content-center align-items-center gap-2">
+                                            <span>Weather parameter</span>
+                                            {% if is_editable %}
+                                            <div class="dropdown my-2">
+                                                <button class="btn btn-sm btn-outline-primary dropdown-toggle" type="button" id="weatherForecastAddParamBtn" data-bs-toggle="dropdown" aria-expanded="false" title="Define a forecast weather parameter">
+                                                    <i class="bi bi-plus-circle"></i>
+                                                </button>
+                                                <ul class="dropdown-menu" aria-labelledby="weatherForecastAddParamBtn"></ul>
+                                            </div>
+                                            {% endif %}
+                                        </div>
+                                    </th>
+                                    <th scope="col" class="text-center align-middle">Timeseries</th>
+                                </tr>
+                            </thead>
                             <tbody class="table-group-divider">
                             </tbody>
                         </table>
                     </div>
                 </div>
                 <div class="tab-pane{% if tab == 'energy_prod' %} show active{% endif %} p-3" id="energyProd-tabcontent" role="tabpanel" aria-labelledby="energyProd-tab">
                     <div class="alert alert-info mb-0 pb-0" id="energyProdSetupHelp">
```

#### html2text {}

```diff
@@ -5,22 +5,28 @@
 {% filter indent(width=20, first=True) %}
  Back_to_timeseries
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
  Sites and buildings
  Timeseries semantic setup
     * Weather
+    * Weather forecast
     * Energy production
     * Energy consumption
  Help
 Select a site in the tree to see its weather parameters setup.
 Weather parameter {% if is_editable %}
                                        Timeseries
 {% endif %}
  Help
+Select a site in the tree to see its weather forecast parameters setup.
+Weather parameter {% if is_editable %}
+                                       Timeseries
+{% endif %}
+ Help
 Select a site or a building in the tree to see its energy production setup.
 Energy {% if is_editable %} Production technologies
                             {{ energy_prod_techno_name }}
 {% endif %}
  Help
 Select a site or a building in the tree to see its energy consumption setup.
 Energy {% if is_editable %} Energy end uses
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/timeseries/upload.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/manage_campaigns.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaigns.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/user_groups/view.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/create.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/edit.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/list.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/templates/pages/users/view.html` & `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/__init__.py` & `bemserver-ui-0.5.2/bemserver_ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/analysis/degree_days.py` & `bemserver-ui-0.5.2/bemserver_ui/views/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/auth.py` & `bemserver-ui-0.5.2/bemserver_ui/views/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Auth views (sign in/out)"""
 import flask
 
 from bemserver_ui.extensions import auth
-from bemserver_ui.extensions.campaign_context import (  # noqa: F401
+from bemserver_ui.extensions.campaign_context import (
     IGNORE_CAMPAIGN_CONTEXT_QUERY_ARG_NAME,
 )
 
 
 blp = flask.Blueprint("auth", __name__, url_prefix="/auth")
 
 
@@ -37,15 +37,15 @@
         # XXX: Little trick to "adapt" response data.
         user_json = user_resp.toJSON()
         user_json["data"] = user_json["data"][0]
         flask.session["user"] = user_json
         flask.flash(f"Welcome back {user_json['data']['name']}!", "message")
         url_redir = flask.url_for(
             "main.index",
-            IGNORE_CAMPAIGN_CONTEXT_QUERY_ARG_NAME=True,
+            **{IGNORE_CAMPAIGN_CONTEXT_QUERY_ARG_NAME: True},
         )
         return flask.redirect(url_redir)
 
     # Render sign in form.
     return flask.render_template("pages/signin.html")
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/campaign_scopes.py` & `bemserver-ui-0.5.2/bemserver_ui/views/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/campaigns.py` & `bemserver-ui-0.5.2/bemserver_ui/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/events/categories.py` & `bemserver-ui-0.5.2/bemserver_ui/views/events/categories.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/events/events.py` & `bemserver-ui-0.5.2/bemserver_ui/views/events/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/main.py` & `bemserver-ui-0.5.2/bemserver_ui/views/main.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/notifications.py` & `bemserver-ui-0.5.2/bemserver_ui/views/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/services/cleanup.py` & `bemserver-ui-0.5.2/bemserver_ui/views/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/services/missing_data.py` & `bemserver-ui-0.5.2/bemserver_ui/views/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/services/outlier_data.py` & `bemserver-ui-0.5.2/bemserver_ui/views/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/properties.py` & `bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/structural_elements/structural_elements.py` & `bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/data.py` & `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/datastates.py` & `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/datastates.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/properties.py` & `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/timeseries/timeseries.py` & `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/user_groups.py` & `bemserver-ui-0.5.2/bemserver_ui/views/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui/views/users.py` & `bemserver-ui-0.5.2/bemserver_ui/views/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/bemserver_ui.egg-info/PKG-INFO` & `bemserver-ui-0.5.2/bemserver_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.1
+Version: 0.5.2
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -85,10 +85,10 @@
                         },
                         "text": "The Python micro framework for building web applications."
                     }
                 }
             ]
 
     *(optional)* **BEMSERVER_UI_PLUGINS = None**
-        List of absolute folder paths that locate the ``__init__.py`` file from each UI plugin package to load
+        List of absolute file paths that locate the ``__init__.py`` file from each UI plugin package to load
```

### Comparing `bemserver-ui-0.5.1/bemserver_ui.egg-info/SOURCES.txt` & `bemserver-ui-0.5.2/bemserver_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.1/requirements/dev.txt` & `bemserver-ui-0.5.2/requirements/dev.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via virtualenv
 identify==2.5.0
     # via pre-commit
 nodeenv==1.6.0
     # via pre-commit
 platformdirs==2.5.2
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.2
     # via -r requirements/dev.in
 pyyaml==6.0
     # via pre-commit
 six==1.16.0
     # via virtualenv
 virtualenv==20.14.1
     # via pre-commit
```

### Comparing `bemserver-ui-0.5.1/requirements/install.txt` & `bemserver-ui-0.5.2/requirements/install.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/install.txt --resolver=backtracking setup.py
 #
-bemserver-api-client==0.18.0
+bemserver-api-client==0.19.1
     # via bemserver-ui (setup.py)
 certifi==2021.10.8
     # via requests
 charset-normalizer==2.0.12
     # via requests
 click==8.1.3
     # via flask
@@ -22,19 +22,19 @@
     # via flask
 jinja2==3.1.2
     # via flask
 markupsafe==2.1.1
     # via
     #   jinja2
     #   werkzeug
-packaging==23.0
+packaging==23.1
     # via bemserver-api-client
 python-dotenv==1.0.0
     # via bemserver-ui (setup.py)
-requests==2.28.2
+requests==2.31.0
     # via bemserver-api-client
 urllib3==1.26.9
     # via requests
 werkzeug==2.2.2
     # via flask
 zipp==3.8.0
     # via importlib-metadata
```

### Comparing `bemserver-ui-0.5.1/setup.py` & `bemserver-ui-0.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="bemserver-ui",
-    version="0.5.1",
+    version="0.5.2",
     description="BEMServer web interface",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/BEMServer/bemserver-ui",
     author="NOBATEK/INEF4",
     author_email="dfrederique@nobatek.inef4.com",
     license="AGPLv3+",
@@ -44,13 +44,13 @@
             "GNU Affero General Public License v3 or later (AGPLv3+)"
         ),
     ],
     python_requires=">=3.9",
     install_requires=[
         "flask>=2.2.3,<3.0.0",
         "python-dotenv>=1.0.0,<2.0.0",
-        "bemserver-api-client>=0.18.0,<0.19.0",
+        "bemserver-api-client>=0.19.1,<0.20.0",
     ],
     extras_require=EXTRAS_REQUIRE,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
 )
```

