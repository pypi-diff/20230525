# Comparing `tmp/popmon-1.4.0.tar.gz` & `tmp/popmon-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popmon-1.4.0.tar", last modified: Wed Oct 19 14:33:32 2022, max compression
+gzip compressed data, was "popmon-1.4.3.tar", last modified: Thu May 25 16:40:55 2023, max compression
```

## Comparing `popmon-1.4.0.tar` & `popmon-1.4.3.tar`

### file list

```diff
@@ -1,126 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.880771 popmon-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2022-10-19 14:33:29.000000 popmon-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2022-10-19 14:33:29.000000 popmon-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3792 2022-10-19 14:33:29.000000 popmon-1.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    21392 2022-10-19 14:33:32.880771 popmon-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20785 2022-10-19 14:33:29.000000 popmon-1.4.0/README.rst
--rw-r--r--   0 root         (0) root         (0)       24 2022-10-19 14:33:30.000000 popmon-1.4.0/extras.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.860771 popmon-1.4.0/popmon/
--rw-r--r--   0 root         (0) root         (0)     1902 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.860771 popmon-1.4.0/popmon/alerting/
--rw-r--r--   0 root         (0) root         (0)     1626 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/alerting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4198 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/alerting/alerts_summary.py
--rw-r--r--   0 root         (0) root         (0)    18583 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/alerting/compute_tl_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/analysis/
--rw-r--r--   0 root         (0) root         (0)     1283 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13978 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/apply_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/analysis/comparison/
--rw-r--r--   0 root         (0) root         (0)     1593 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/comparison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8805 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/comparison/comparisons.py
--rw-r--r--   0 root         (0) root         (0)    15479 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/comparison/hist_comparer.py
--rw-r--r--   0 root         (0) root         (0)    19248 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/functions.py
--rw-r--r--   0 root         (0) root         (0)    18600 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/hist_numpy.py
--rw-r--r--   0 root         (0) root         (0)     2478 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/merge_statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/analysis/profiling/
--rw-r--r--   0 root         (0) root         (0)     1490 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/profiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8235 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/profiling/hist_profiler.py
--rw-r--r--   0 root         (0) root         (0)     6876 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/profiling/profiles.py
--rw-r--r--   0 root         (0) root         (0)    11316 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/analysis/profiling/pull_calculator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/base/
--rw-r--r--   0 root         (0) root         (0)     1223 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6982 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/base/module.py
--rw-r--r--   0 root         (0) root         (0)     3001 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/base/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     4783 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/base/registry.py
--rw-r--r--   0 root         (0) root         (0)    14509 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/decorators/
--rw-r--r--   0 root         (0) root         (0)     1221 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/decorators/pandas.py
--rw-r--r--   0 root         (0) root         (0)     1737 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/decorators/spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/extensions/
--rw-r--r--   0 root         (0) root         (0)     1250 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1637 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/extensions/extension.py
--rw-r--r--   0 root         (0) root         (0)     2488 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/extensions/profile_diptest.py
--rw-r--r--   0 root         (0) root         (0)     1645 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/extensions/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/hist/
--rw-r--r--   0 root         (0) root         (0)     1193 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/hist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.864771 popmon-1.4.0/popmon/hist/filling/
--rw-r--r--   0 root         (0) root         (0)     1755 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/hist/filling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6569 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/hist/hist_splitter.py
--rw-r--r--   0 root         (0) root         (0)    10915 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/hist/hist_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.868771 popmon-1.4.0/popmon/io/
--rw-r--r--   0 root         (0) root         (0)     1293 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/io/file_reader.py
--rw-r--r--   0 root         (0) root         (0)     3294 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/io/file_writer.py
--rw-r--r--   0 root         (0) root         (0)     1721 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/io/json_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.868771 popmon-1.4.0/popmon/notebooks/
--rw-r--r--   0 root         (0) root         (0)    19461 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/notebooks/popmon_tutorial_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)     5777 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/notebooks/popmon_tutorial_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    11902 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
--rw-r--r--   0 root         (0) root         (0)    11762 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/notebooks/popmon_tutorial_reports.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.868771 popmon-1.4.0/popmon/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1117 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2418 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/amazing_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5224 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/dataset_splitter.py
--rw-r--r--   0 root         (0) root         (0)     7066 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/metrics.py
--rw-r--r--   0 root         (0) root         (0)    16535 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/metrics_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    11188 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/report.py
--rw-r--r--   0 root         (0) root         (0)     9099 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/report_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     1756 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/pipeline/timing.py
--rw-r--r--   0 root         (0) root         (0)     4585 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.868771 popmon-1.4.0/popmon/stats/
--rw-r--r--   0 root         (0) root         (0)     1222 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11180 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/stats/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.868771 popmon-1.4.0/popmon/stitching/
--rw-r--r--   0 root         (0) root         (0)     1238 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/stitching/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20218 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/stitching/hist_stitcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.872771 popmon-1.4.0/popmon/test_data/
--rw-r--r--   0 root         (0) root         (0)    73043 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/data_generator_hists.json.gz
--rw-r--r--   0 root         (0) root         (0)      128 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/example.json
--rw-r--r--   0 root         (0) root         (0)    15152 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/example_histogram.json
--rw-r--r--   0 root         (0) root         (0)   696816 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/flight_delays.csv.gz
--rw-r--r--   0 root         (0) root         (0)   692782 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/flight_delays_reference.csv.gz
--rw-r--r--   0 root         (0) root         (0)    79082 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/synthetic_histograms.json
--rw-r--r--   0 root         (0) root         (0)    64368 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/test_data/test.csv.gz
--rw-r--r--   0 root         (0) root         (0)     2687 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/utils.py
--rw-r--r--   0 root         (0) root         (0)       66 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.872771 popmon-1.4.0/popmon/visualization/
--rw-r--r--   0 root         (0) root         (0)     1670 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6260 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/alert_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    15423 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/histogram_section.py
--rw-r--r--   0 root         (0) root         (0)     8494 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/overview_section.py
--rw-r--r--   0 root         (0) root         (0)     3068 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/report_generator.py
--rw-r--r--   0 root         (0) root         (0)    10768 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/section_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.872771 popmon-1.4.0/popmon/visualization/templates/
--rw-r--r--   0 root         (0) root         (0)      835 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/aggregated-overview.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.860771 popmon-1.4.0/popmon/visualization/templates/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.872771 popmon-1.4.0/popmon/visualization/templates/assets/css/
--rw-r--r--   0 root         (0) root         (0)   155712 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)     2090 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/css/custom-style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.880771 popmon-1.4.0/popmon/visualization/templates/assets/js/
--rw-r--r--   0 root         (0) root         (0)    78586 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)     2943 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/js/custom-script.js
--rwxr-xr-x   0 root         (0) root         (0)     2532 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/js/jquery.easing.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)  3682474 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/js/plotly.js
--rw-r--r--   0 root         (0) root         (0)      927 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/assets/js/scrolling-nav.js
--rw-r--r--   0 root         (0) root         (0)     2453 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/card.html
--rw-r--r--   0 root         (0) root         (0)     1003 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/core.html
--rw-r--r--   0 root         (0) root         (0)      942 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/footer.html
--rw-r--r--   0 root         (0) root         (0)      782 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/header.html
--rw-r--r--   0 root         (0) root         (0)      988 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/modal-popup.html
--rw-r--r--   0 root         (0) root         (0)      178 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/notebook_iframe.html
--rw-r--r--   0 root         (0) root         (0)     2739 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/section.html
--rw-r--r--   0 root         (0) root         (0)     1401 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/templates/table.html
--rw-r--r--   0 root         (0) root         (0)     7243 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/traffic_light_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    26132 2022-10-19 14:33:30.000000 popmon-1.4.0/popmon/visualization/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-19 14:33:32.860771 popmon-1.4.0/popmon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21392 2022-10-19 14:33:32.000000 popmon-1.4.0/popmon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3458 2022-10-19 14:33:32.000000 popmon-1.4.0/popmon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-19 14:33:32.000000 popmon-1.4.0/popmon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       69 2022-10-19 14:33:32.000000 popmon-1.4.0/popmon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      163 2022-10-19 14:33:32.000000 popmon-1.4.0/popmon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-19 14:33:32.000000 popmon-1.4.0/popmon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      398 2022-10-19 14:33:30.000000 popmon-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      144 2022-10-19 14:33:30.000000 popmon-1.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-19 14:33:32.880771 popmon-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2022 2022-10-19 14:33:30.000000 popmon-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.803537 popmon-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-25 16:40:44.000000 popmon-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-25 16:40:44.000000 popmon-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3792 2023-05-25 16:40:44.000000 popmon-1.4.3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    23345 2023-05-25 16:40:55.803537 popmon-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21523 2023-05-25 16:40:44.000000 popmon-1.4.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-25 16:40:44.000000 popmon-1.4.3/extras.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.775536 popmon-1.4.3/popmon/
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/alerting/
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/alerting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/alerting/alerts_summary.py
+-rw-r--r--   0 root         (0) root         (0)    18616 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/alerting/compute_tl_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/apply_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/analysis/comparison/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/comparison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/comparison/comparisons.py
+-rw-r--r--   0 root         (0) root         (0)    15490 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/comparison/hist_comparer.py
+-rw-r--r--   0 root         (0) root         (0)    19311 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/functions.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/hist_numpy.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/merge_statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/analysis/profiling/
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8232 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/hist_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    11323 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/analysis/profiling/pull_calculator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/base/
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6973 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/module.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/base/registry.py
+-rw-r--r--   0 root         (0) root         (0)    14500 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.779537 popmon-1.4.3/popmon/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/decorators/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/decorators/spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/extensions/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/extensions/extension.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/extensions/profile_diptest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/hist/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/hist/filling/
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/filling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6570 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/hist_splitter.py
+-rw-r--r--   0 root         (0) root         (0)    10908 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/hist/hist_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/io/
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/file_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/file_writer.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/io/json_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.783537 popmon-1.4.3/popmon/notebooks/
+-rw-r--r--   0 root         (0) root         (0)    19461 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11902 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/notebooks/popmon_tutorial_reports.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.787537 popmon-1.4.3/popmon/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/amazing_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5208 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/dataset_splitter.py
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    16465 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/metrics_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    11202 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/report.py
+-rw-r--r--   0 root         (0) root         (0)     9117 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/report_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/pipeline/timing.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.787537 popmon-1.4.3/popmon/stats/
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11198 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stats/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.787537 popmon-1.4.3/popmon/stitching/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stitching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20217 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/stitching/hist_stitcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.791537 popmon-1.4.3/popmon/test_data/
+-rw-r--r--   0 root         (0) root         (0)    73043 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/data_generator_hists.json.gz
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/example.json
+-rw-r--r--   0 root         (0) root         (0)    15152 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/example_histogram.json
+-rw-r--r--   0 root         (0) root         (0)   696816 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/flight_delays.csv.gz
+-rw-r--r--   0 root         (0) root         (0)   692782 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/flight_delays_reference.csv.gz
+-rw-r--r--   0 root         (0) root         (0)    79082 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/synthetic_histograms.json
+-rw-r--r--   0 root         (0) root         (0)    64368 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/test_data/test.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-25 16:40:45.000000 popmon-1.4.3/popmon/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.795537 popmon-1.4.3/popmon/visualization/
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/alert_section_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15429 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/histogram_section.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/overview_section.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/report_generator.py
+-rw-r--r--   0 root         (0) root         (0)    10829 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/section_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.795537 popmon-1.4.3/popmon/visualization/templates/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/aggregated-overview.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.775536 popmon-1.4.3/popmon/visualization/templates/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.799537 popmon-1.4.3/popmon/visualization/templates/assets/css/
+-rw-r--r--   0 root         (0) root         (0)   155712 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/css/custom-style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.803537 popmon-1.4.3/popmon/visualization/templates/assets/js/
+-rw-r--r--   0 root         (0) root         (0)    78586 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/custom-script.js
+-rwxr-xr-x   0 root         (0) root         (0)     2532 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.easing.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)  3682474 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/plotly.js
+-rw-r--r--   0 root         (0) root         (0)      927 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/assets/js/scrolling-nav.js
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/card.html
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/core.html
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/footer.html
+-rw-r--r--   0 root         (0) root         (0)      782 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/header.html
+-rw-r--r--   0 root         (0) root         (0)      988 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/modal-popup.html
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/notebook_iframe.html
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/section.html
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/templates/table.html
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/traffic_light_section_generator.py
+-rw-r--r--   0 root         (0) root         (0)    26741 2023-05-25 16:40:44.000000 popmon-1.4.3/popmon/visualization/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:40:55.775536 popmon-1.4.3/popmon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23345 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3422 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 16:40:55.000000 popmon-1.4.3/popmon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-05-25 16:40:44.000000 popmon-1.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-25 16:40:44.000000 popmon-1.4.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 16:40:55.803537 popmon-1.4.3/setup.cfg
```

### Comparing `popmon-1.4.0/LICENSE` & `popmon-1.4.3/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 ING Wholesale Banking Advanced Analytics
+Copyright 2023 ING Analytics Wholesale Banking
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
 to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions
```

### Comparing `popmon-1.4.0/NOTICE` & `popmon-1.4.3/NOTICE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/PKG-INFO` & `popmon-1.4.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: popmon
-Version: 1.4.0
-Summary: Monitor the stability of a pandas or spark dataset
-Home-page: https://github.com/ing-bank/popmon
-Author: ING Wholesale Banking Advanced Analytics
-License: MIT
-Keywords: pandas spark data-science data-analysis monitoring statistics python jupyter ipython
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: diptest
-License-File: LICENSE
-License-File: NOTICE
-
 ===========================
 Population Shift Monitoring
 ===========================
 
-|build| |docs| |release| |release_date| |downloads|
+|build| |docs| |release| |release_date| |downloads| |ruff|
 
 |logo|
 
 `popmon` is a package that allows one to check the stability of a dataset.
 `popmon` works with both **pandas** and **spark datasets**.
 
 `popmon` creates histograms of features binned in time-slices,
@@ -205,15 +187,15 @@
 +----------------+---------------+
 | Grafana        | Kibana        |
 +----------------+---------------+
 
 Resources on how to integrate popmon are available in the `examples directory <https://github.com/ing-bank/popmon/tree/master/examples/integrations>`_.
 Contributions of additional or improved integrations are welcome!
 
-.. |grafana_logo| image:: https://upload.wikimedia.org/wikipedia/en/a/a1/Grafana_logo.svg
+.. |grafana_logo| image:: https://upload.wikimedia.org/wikipedia/commons/a/a1/Grafana_logo.svg
     :alt: Grafana logo
     :height: 120
     :target: https://github.com/grafana/grafana
 
 .. |kibana_logo| image:: https://miro.medium.com/max/1400/1*HW_x9ZvIbUkyaqHstsB1ig.png
     :alt: Kibana logo
     :height: 120
@@ -262,34 +244,37 @@
 
 Articles
 --------
 
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | Title                                                                                                                                                                                             | Date             | Author                                      |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
+|`POPMON v1.0.0: The Dataset-Shift Pokémon <https://medium.com/wbaa/popmon-v1-0-0-the-dataset-shift-pok%C3%A9mon-7dea9cb49a71>`_                                                                    | Aug 3, 2022      | Pradyot Patil                               |
++---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`Monitoring Model Drift with Python <https://medium.com/broadhorizon-cmotions/monitoring-model-drift-with-python-b9e15ca16b18>`_                                                                   | April 16, 2022   | Jeanine Schoonemann                         |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`The Statistics Underlying the Popmon Hood <https://www.theanalyticslab.nl/the-statistics-underlying-the-popmon-hood/>`_                                                                           | April 15, 2022   | Jurriaan Nagelkerke and Jeanine Schoonemann |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`popmon: code breakfast session <https://simonbrugman.nl/2021/11/09/popmon-code-breakfast.html>`_                                                                                                  | November 9, 2022 | Simon Brugman                               |       
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | `Population Shift Analysis: Monitoring Data Quality with Popmon <https://www.codemotion.com/magazine/dev-hub/big-data-analyst/popmon-data-quality-monitoring/>`_                                  | May 21, 2021     | Vito Gentile                                |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | `Popmon Open Source Package — Population Shift Monitoring Made Easy <https://medium.com/wbaa/population-monitoring-open-source-1ce3139d8c3a>`_                                                    | May 20, 2020     | Nicole Mpozika                              |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 
+
 Software
 --------
 
 - `Kedro-popmon <https://github.com/stephanecollot/kedro-popmon>`_ is a plugin to integrate popmon reporting with kedro. This plugin allows you to automate the process of popmon feature and output stability monitoring. Package created by `Marian Dabrowski <https://www.linkedin.com/in/marian-dabrowski/>`_ and `Stephane Collot <https://github.com/stephanecollot/>`_.
 
 Project contributors
 ====================
 
-This package was authored by ING Wholesale Banking Advanced Analytics.
+This package was authored by ING Analytics Wholesale Banking (INGA WB).
 Special thanks to the following people who have contributed to the development of this package: `Ahmet Erdem <https://github.com/aerdem4>`_, `Fabian Jansen <https://github.com/faab5>`_, `Nanne Aben <https://github.com/nanne-aben>`_, Mathieu Grimal.
 
 
 Citing popmon
 =============
 If ``popmon`` has been relevant in your work, and you would like to acknowledge the project in your publication, we suggest citing the following paper:
 
@@ -311,32 +296,35 @@
 
 
 Contact and support
 ===================
 
 * Issues & Ideas & Support: https://github.com/ing-bank/popmon/issues
 
-Please note that ING WBAA provides support only on a best-effort basis.
+Please note that INGA WB provides support only on a best-effort basis.
 
 License
 =======
-Copyright ING WBAA. `popmon` is completely free, open-source and licensed under the `MIT license <https://en.wikipedia.org/wiki/MIT_License>`_.
+Copyright INGA WB. `popmon` is completely free, open-source and licensed under the `MIT license <https://en.wikipedia.org/wiki/MIT_License>`_.
 
 .. |logo| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/popmon-logo.png
     :alt: POPMON logo
     :target: https://github.com/ing-bank/popmon
 .. |example| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/report_overview.png
     :alt: Traffic Light Overview
 .. |histograms| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/histogram_inspector.png
     :alt: Histogram inspector
 .. |pipeline| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/pipeline.png
     :alt: Pipeline Visualization
     :target: https://github.com/ing-bank/popmon/files/7417124/pipeline_amazingpipeline_subgraphs_unversioned.pdf
 .. |build| image:: https://github.com/ing-bank/popmon/workflows/build/badge.svg
     :alt: Build status
+.. |ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+    :alt: Ruff
+    :target: https://github.com/charliermarsh/ruff
 .. |docs| image:: https://readthedocs.org/projects/popmon/badge/?version=latest
     :alt: Package docs status
     :target: https://popmon.readthedocs.io
 .. |release| image:: https://img.shields.io/github/v/release/ing-bank/popmon
     :alt: Latest GitHub release
     :target: https://github.com/ing-bank/popmon/releases
 .. |release_date| image:: https://img.shields.io/github/release-date/ing-bank/popmon
@@ -357,9 +345,7 @@
     :target: https://colab.research.google.com/github/ing-bank/popmon/blob/master/popmon/notebooks/popmon_tutorial_reports.ipynb
 .. |downloads| image:: https://pepy.tech/badge/popmon
     :alt: PyPi downloads
     :target: https://pepy.tech/project/popmon
 
 .. _profiles: https://popmon.readthedocs.io/en/latest/profiles.html
 .. _comparisons: https://popmon.readthedocs.io/en/latest/comparisons.html
-
-
```

### Comparing `popmon-1.4.0/README.rst` & `popmon-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,45 @@
+Metadata-Version: 2.1
+Name: popmon
+Version: 1.4.3
+Summary: Monitor the stability of a pandas or spark dataset
+Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
+License: Copyright 2023 ING Analytics Wholesale Banking
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+        documentation files (the "Software"), to deal in the Software without restriction, including without limitation
+        the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
+        to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions
+        of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+        TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+        THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+        CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+        DEALINGS IN THE SOFTWARE.
+        
+Project-URL: repository, https://github.com/ing-bank/popmon
+Keywords: pandas,spark,data-science,data-analysis,monitoring,statistics,python,jupyter,ipython
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: diptest
+License-File: LICENSE
+License-File: NOTICE
+
 ===========================
 Population Shift Monitoring
 ===========================
 
-|build| |docs| |release| |release_date| |downloads|
+|build| |docs| |release| |release_date| |downloads| |ruff|
 
 |logo|
 
 `popmon` is a package that allows one to check the stability of a dataset.
 `popmon` works with both **pandas** and **spark datasets**.
 
 `popmon` creates histograms of features binned in time-slices,
@@ -187,15 +220,15 @@
 +----------------+---------------+
 | Grafana        | Kibana        |
 +----------------+---------------+
 
 Resources on how to integrate popmon are available in the `examples directory <https://github.com/ing-bank/popmon/tree/master/examples/integrations>`_.
 Contributions of additional or improved integrations are welcome!
 
-.. |grafana_logo| image:: https://upload.wikimedia.org/wikipedia/en/a/a1/Grafana_logo.svg
+.. |grafana_logo| image:: https://upload.wikimedia.org/wikipedia/commons/a/a1/Grafana_logo.svg
     :alt: Grafana logo
     :height: 120
     :target: https://github.com/grafana/grafana
 
 .. |kibana_logo| image:: https://miro.medium.com/max/1400/1*HW_x9ZvIbUkyaqHstsB1ig.png
     :alt: Kibana logo
     :height: 120
@@ -244,34 +277,37 @@
 
 Articles
 --------
 
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | Title                                                                                                                                                                                             | Date             | Author                                      |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
+|`POPMON v1.0.0: The Dataset-Shift Pokémon <https://medium.com/wbaa/popmon-v1-0-0-the-dataset-shift-pok%C3%A9mon-7dea9cb49a71>`_                                                                    | Aug 3, 2022      | Pradyot Patil                               |
++---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`Monitoring Model Drift with Python <https://medium.com/broadhorizon-cmotions/monitoring-model-drift-with-python-b9e15ca16b18>`_                                                                   | April 16, 2022   | Jeanine Schoonemann                         |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`The Statistics Underlying the Popmon Hood <https://www.theanalyticslab.nl/the-statistics-underlying-the-popmon-hood/>`_                                                                           | April 15, 2022   | Jurriaan Nagelkerke and Jeanine Schoonemann |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`popmon: code breakfast session <https://simonbrugman.nl/2021/11/09/popmon-code-breakfast.html>`_                                                                                                  | November 9, 2022 | Simon Brugman                               |       
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | `Population Shift Analysis: Monitoring Data Quality with Popmon <https://www.codemotion.com/magazine/dev-hub/big-data-analyst/popmon-data-quality-monitoring/>`_                                  | May 21, 2021     | Vito Gentile                                |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | `Popmon Open Source Package — Population Shift Monitoring Made Easy <https://medium.com/wbaa/population-monitoring-open-source-1ce3139d8c3a>`_                                                    | May 20, 2020     | Nicole Mpozika                              |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 
+
 Software
 --------
 
 - `Kedro-popmon <https://github.com/stephanecollot/kedro-popmon>`_ is a plugin to integrate popmon reporting with kedro. This plugin allows you to automate the process of popmon feature and output stability monitoring. Package created by `Marian Dabrowski <https://www.linkedin.com/in/marian-dabrowski/>`_ and `Stephane Collot <https://github.com/stephanecollot/>`_.
 
 Project contributors
 ====================
 
-This package was authored by ING Wholesale Banking Advanced Analytics.
+This package was authored by ING Analytics Wholesale Banking (INGA WB).
 Special thanks to the following people who have contributed to the development of this package: `Ahmet Erdem <https://github.com/aerdem4>`_, `Fabian Jansen <https://github.com/faab5>`_, `Nanne Aben <https://github.com/nanne-aben>`_, Mathieu Grimal.
 
 
 Citing popmon
 =============
 If ``popmon`` has been relevant in your work, and you would like to acknowledge the project in your publication, we suggest citing the following paper:
 
@@ -293,32 +329,35 @@
 
 
 Contact and support
 ===================
 
 * Issues & Ideas & Support: https://github.com/ing-bank/popmon/issues
 
-Please note that ING WBAA provides support only on a best-effort basis.
+Please note that INGA WB provides support only on a best-effort basis.
 
 License
 =======
-Copyright ING WBAA. `popmon` is completely free, open-source and licensed under the `MIT license <https://en.wikipedia.org/wiki/MIT_License>`_.
+Copyright INGA WB. `popmon` is completely free, open-source and licensed under the `MIT license <https://en.wikipedia.org/wiki/MIT_License>`_.
 
 .. |logo| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/popmon-logo.png
     :alt: POPMON logo
     :target: https://github.com/ing-bank/popmon
 .. |example| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/report_overview.png
     :alt: Traffic Light Overview
 .. |histograms| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/histogram_inspector.png
     :alt: Histogram inspector
 .. |pipeline| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/pipeline.png
     :alt: Pipeline Visualization
     :target: https://github.com/ing-bank/popmon/files/7417124/pipeline_amazingpipeline_subgraphs_unversioned.pdf
 .. |build| image:: https://github.com/ing-bank/popmon/workflows/build/badge.svg
     :alt: Build status
+.. |ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+    :alt: Ruff
+    :target: https://github.com/charliermarsh/ruff
 .. |docs| image:: https://readthedocs.org/projects/popmon/badge/?version=latest
     :alt: Package docs status
     :target: https://popmon.readthedocs.io
 .. |release| image:: https://img.shields.io/github/v/release/ing-bank/popmon
     :alt: Latest GitHub release
     :target: https://github.com/ing-bank/popmon/releases
 .. |release_date| image:: https://img.shields.io/github/release-date/ing-bank/popmon
```

### Comparing `popmon-1.4.0/popmon/__init__.py` & `popmon-1.4.3/popmon/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `popmon-1.4.0/popmon/alerting/__init__.py` & `popmon-1.4.3/popmon/alerting/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,16 +14,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..alerting.alerts_summary import AlertsSummary
-from ..alerting.compute_tl_bounds import (
+from popmon.alerting.alerts_summary import AlertsSummary
+from popmon.alerting.compute_tl_bounds import (
     ComputeTLBounds,
     DynamicBounds,
     StaticBounds,
     TrafficLightAlerts,
     collect_traffic_light_bounds,
     pull_bounds,
     traffic_light,
```

### Comparing `popmon-1.4.0/popmon/alerting/alerts_summary.py` & `popmon-1.4.3/popmon/alerting/alerts_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,23 +12,22 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+from __future__ import annotations
 
 import fnmatch
-from typing import Optional
 
 import numpy as np
 import pandas as pd
 
-from ..base import Module
+from popmon.base import Module
 
 
 class AlertsSummary(Module):
     """The module AlertsSummary combines the alerts-summaries of all individual features
 
     It combines the alerts-summaries of all individual features into an artificial feature "_AGGREGATE_".
     """
@@ -55,15 +54,15 @@
         super().__init__()
         self.read_key = read_key
         self.store_key = store_key or self.read_key
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.combined_variable = combined_variable
 
-    def transform(self, data: dict) -> Optional[dict]:
+    def transform(self, data: dict) -> dict | None:
         # determine all possible features, used for the comparison below
         features = self.get_features(list(data.keys()))
         if len(features) == 0:
             return None
 
         self.logger.info(
             f'Combining alerts into artificial variable "{self.combined_variable}"'
```

### Comparing `popmon-1.4.0/popmon/alerting/compute_tl_bounds.py` & `popmon-1.4.3/popmon/alerting/compute_tl_bounds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,26 +12,26 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+from __future__ import annotations
 
 import copy
 import fnmatch
 from collections import defaultdict
-from typing import Any, Tuple
+from typing import Any
 
 import numpy as np
 import pandas as pd
 
-from ..analysis.apply_func import ApplyFunc
-from ..base import Module, Pipeline
+from popmon.analysis.apply_func import ApplyFunc
+from popmon.base import Module, Pipeline
 
 
 def traffic_light_summary(row, cols=None, prefix=""):
     """Make a summary of traffic light alerts present in the dataframe
 
     Count number of green, yellow and red traffic lights.
 
@@ -57,27 +57,26 @@
     x["n_red"] = (traffic_lights == 2).sum()
     x["n_yellow"] = (traffic_lights == 1).sum()
     x["n_green"] = (traffic_lights == 0).sum()
     return pd.Series(x)
 
 
 def traffic_light(value, red_high, yellow_high, yellow_low=0, red_low=0):
-    """Get corresponding traffic light given a value and traffic light bounds.
+    """Get the corresponding traffic light given a value and traffic light bounds.
 
     :param float value: value to check
     :param float red_high: higher bound of red traffic light
     :param float yellow_high: higher bound of yellow traffic light
     :param float yellow_low: lower bound of yellow traffic light (optional)
     :param float red_low: lower bound of red traffic light (optional)
 
     :return: corresponding traffic light based on the value and traffic light bounds
     """
-    assert (
-        np.diff([red_high, yellow_high, yellow_low, red_low]) > 0
-    ).sum() == 0, "Traffic lights not sorted!"
+    if (np.diff([red_high, yellow_high, yellow_low, red_low]) > 0).sum() != 0:
+        raise ValueError("Traffic lights not sorted!")
 
     if value < red_low or value >= red_high:
         return 2
     elif value < yellow_low or value >= yellow_high:
         return 1
     return 0
 
@@ -91,15 +90,15 @@
     :param dict monitoring_rules: dictionary of defined monitoring rules (bounds)
 
     :return: dict metrics_per_feature (containing features with corresponding metrics),
              list metrics: list of generic metrics
     """
     metrics_per_feature = defaultdict(list)
     metrics = []
-    for pattern in monitoring_rules.keys():
+    for pattern in monitoring_rules:
         psplit = pattern.split(":")
         feature = ":".join(psplit[:-1])
         metric = psplit[-1]
         (metrics_per_feature[feature] if feature else metrics).append(metric)
 
     return metrics_per_feature, metrics
 
@@ -195,15 +194,15 @@
                         "prefix": self.prefix,
                         "suffix": self.suffix,
                         "entire": self.entire,
                         "kwargs": self.kwargs,
                     }
                 )
 
-    def transform(self, test_data: dict) -> Tuple[Any, Any]:
+    def transform(self, test_data: dict) -> tuple[Any, Any]:
         # determine all possible features, used for the comparison below
         features = self.get_features(list(test_data.keys()))
 
         pkeys, nkeys = collect_traffic_light_bounds(self.monitoring_rules)
 
         # loop over features to apply monitoring business rules to
         for feature in features[:]:
```

### Comparing `popmon-1.4.0/popmon/analysis/__init__.py` & `popmon-1.4.3/popmon/analysis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,12 +14,13 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..analysis.apply_func import ApplyFunc
+from popmon.analysis.apply_func import ApplyFunc
+
 from .comparison import Comparisons
 from .profiling import Profiles
 
 __all__ = ["ApplyFunc", "Comparisons", "Profiles"]
```

### Comparing `popmon-1.4.0/popmon/analysis/apply_func.py` & `popmon-1.4.3/popmon/analysis/apply_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -20,16 +20,16 @@
 
 import warnings
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
-from ..base import Module
-from ..utils import parallel
+from popmon.base import Module
+from popmon.utils import parallel
 
 
 class ApplyFunc(Module):
     """This module applies functions to specified feature and metrics.
 
     Extra parameters (kwargs) can be passed to the apply function.
     """
@@ -93,16 +93,16 @@
             raise NotImplementedError
 
     def add_apply_func(
         self,
         func,
         suffix=None,
         prefix=None,
-        metrics=[],
-        features=[],
+        metrics=None,
+        features=None,
         entire=None,
         *args,
         **kwargs,
     ):
         """Add function to be applied to dataframe.
 
         Can call this function after module instantiation to add new functions.
@@ -113,14 +113,18 @@
         :param features: (list, optional) features the function is applied to. Overwrites features above
         :param metrics: (list, optional) metrics the function is applied to. Overwrites metrics above
         :param entire: (boolean, optional) apply function to the entire feature's dataframe of metrics?
         :param args: (tuple, optional) args for 'func'
         :param kwargs: (dict, optional) kwargs for 'func'
         """
         # check inputs
+        if features is None:
+            features = []
+        if metrics is None:
+            metrics = []
         if not callable(func):
             raise TypeError("functions in ApplyFunc must be callable objects")
         if suffix is not None and not isinstance(suffix, str):
             raise TypeError("prefix, and suffix in ApplyFunc must be strings or None.")
         if prefix is not None and not isinstance(prefix, str):
             raise TypeError("prefix, and suffix in ApplyFunc must be strings or None.")
         if not isinstance(metrics, list) or not isinstance(features, list):
@@ -248,17 +252,20 @@
     :param str feature: feature currently looping over
     :param list selected_metrics: list of selected metrics to apply to
     :param df: pandas data frame that function in arr is applied to
     :param dict arr: dictionary containing the function to be applied to pandas dataframe.
     :return: dictionary with outputs of applied-to metric pd.Series
     """
     # basic checks of feature
-    if "features" in arr and len(arr["features"]) > 0:
-        if feature not in arr["features"]:
-            return {}
+    if (
+        "features" in arr
+        and len(arr["features"]) > 0
+        and feature not in arr["features"]
+    ):
+        return {}
 
     # get func input
     keys = list(arr.keys())
 
     assert "func" in keys, "function input is insufficient."
     func = arr["func"]
 
@@ -312,15 +319,15 @@
     ) and isinstance(df, pd.DataFrame):
         obj = {"_".join(df.columns): obj}
     elif (
         isinstance(obj, (list, tuple, np.ndarray))
         and isinstance(df, pd.DataFrame)
         and len(df.columns) == len(obj)
     ):
-        obj = {c: o for c, o in zip(df.columns, obj)}
+        obj = dict(zip(df.columns, obj))
     elif (
         isinstance(obj, (list, tuple, np.ndarray))
         and isinstance(df, pd.Series)
         and len(df.index) == len(obj)
     ):
         obj = {df.name: pd.Series(data=obj, index=df.index)}
     elif (
@@ -339,28 +346,23 @@
     elif (
         isinstance(obj, pd.Series)
         and isinstance(df, pd.DataFrame)
         and len(obj) == len(df)
         and all(obj.index == df.index)
     ):
         obj = {"_".join(df.columns): obj}
+    # e.g. output of normalized_hist_mean_cov: a dataframe with one column, actually a series
     elif (
         isinstance(obj, pd.DataFrame)
         and len(obj.columns) == 1
-        and len(obj.index) != len(df.index)
-    ):
-        # e.g. output of normalized_hist_mean_cov: a dataframe with one column, actually a series
-        obj = obj[obj.columns[0]].to_dict()
-    elif (
-        isinstance(obj, pd.DataFrame)
-        and len(obj.columns) == 1
-        and len(obj.index) == len(df.index)
-        and (obj.index != df.index).any()
+        and (
+            len(obj.index) != len(df.index)
+            or (len(obj.index) == len(df.index) and (obj.index != df.index).any())
+        )
     ):
-        # e.g. output of normalized_hist_mean_cov: a dataframe with one column, actually a series
         obj = obj[obj.columns[0]].to_dict()
     elif isinstance(obj, pd.Series):
         # e.g. output of np.mean of np.std: results in one number per column when applied to a dataframe
         obj = obj.to_dict()
     elif isinstance(obj, pd.DataFrame):
         # when apply to one column returns another column
         obj = {c: obj[c] for c in obj.columns}
```

### Comparing `popmon-1.4.0/popmon/analysis/comparison/__init__.py` & `popmon-1.4.3/popmon/analysis/comparison/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,22 +12,23 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from ...analysis.comparison.hist_comparer import (
+from popmon.analysis.comparison.hist_comparer import (
     ExpandingHistComparer,
     ExpandingNormHistComparer,
     ReferenceHistComparer,
     ReferenceNormHistComparer,
     RollingHistComparer,
     RollingNormHistComparer,
 )
+
 from .comparisons import Comparisons
 
 __all__ = [
     "Comparisons",
     "ReferenceHistComparer",
     "RollingHistComparer",
     "ExpandingHistComparer",
```

### Comparing `popmon-1.4.0/popmon/analysis/comparison/comparisons.py` & `popmon-1.4.3/popmon/analysis/comparison/comparisons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -78,15 +78,15 @@
 def ks_test(hist_1, hist_2):
     """KS-test for two histograms with different number of entries
 
     Copyright ROOT:
     Formulas translated from c++ to python, but formulas otherwise not modified.
     Reference: link: https://root.cern.ch/doc/master/classTH1.html#TH1:KolmogorovTest
     GNU license: https://root.cern.ch/license
-    All modifications copyright ING WBAA.
+    All modifications copyright INGA WB.
 
     :param hist_1: 1D array with bin counts of the histogram_1
     :param hist_2: 1D array with bin counts of the histogram_2
 
     :return: ks_score: Kolmogorov-Smirnov Test score
     :rtype: float
     """
@@ -111,15 +111,15 @@
 def ks_prob(testscore):
     """KS-probability corresponding ti KS test score
 
     Copyright ROOT:
     Formulas translated from c++ to python, but formulas otherwise not modified.
     Reference: https://root.cern.ch/doc/master/classTH1.html#TH1:KolmogorovTest
     GNU license: https://root.cern.ch/license
-    All modifications copyright ING WBAA.
+    All modifications copyright INGA WB.
 
     :param float testscore: Kolmogorov-Smirnov test score
 
     :return: approximate pvalue for the Kolmogorov-Smirnov test score
     :rtype: float
     """
     fj = np.array([-2, -8, -18, -32])
@@ -150,15 +150,15 @@
         "Kolmogorov-Smirnov test statistic",
         "p-value of the Kolmogorov-Smirnov test",
         "Z-score of the Kolmogorov-Smirnov test",
     ],
     dim=1,
     htype="num",
 )
-def ks(p, q, *args):
+def ks(p, q, *_):
     # KS-test only properly defined for (ordered) 1D interval variables
     ks_testscore = ks_test(p, q)
     ks_pvalue = ks_prob(ks_testscore)
     ks_zscore = -stats.norm.ppf(ks_pvalue)
     return ks_testscore, ks_pvalue, ks_zscore
 
 
@@ -178,15 +178,15 @@
 
 @Comparisons.register(
     key="pearson",
     description="Pearson correlation coefficient",
     dim=(2,),
     htype="all",
 )
-def pearson(p, q, *args):
+def pearson(p, q, *_):
     # calculate pearson coefficient
     pearson_coeff = np.nan
     if len(p) >= 2:
         same0 = all(p == p[0])
         same1 = all(q == q[0])
         if not same0 and not same1:
             # this avoids std==0, and thereby avoid runtime warnings
@@ -197,15 +197,15 @@
 def uu_chi2(n, m):
     """Normalized Chi^2 formula for two histograms with different number of entries
 
     Copyright ROOT:
     Formulas translated from c++ to python, but formulas otherwise not modified.
     Reference: https://root.cern.ch/doc/master/classTH1.html#a6c281eebc0c0a848e7a0d620425090a5
     GNU License: https://root.cern.ch/license
-    All modifications copyright ING WBAA.
+    All modifications copyright INGA WB.
 
     :param n: 1d array with bin counts of the reference set
     :param m: 1d array with bin counts of the test set
     :return: tuple of floats (chi2_value, chi2_norm, z_score, p_value, res)
     """
 
     def _not_finite_to_zero(x):
@@ -214,16 +214,16 @@
         return res
 
     if len(n) == 0 or len(m) == 0:
         raise ValueError("Input histogram(s) has zero size.")
     if len(n) != len(m):
         raise ValueError("Input histograms have unequal size.")
 
-    N = np.sum(n)
-    M = np.sum(m)
+    N = np.sum(n)  # noqa: N806
+    M = np.sum(m)  # noqa: N806
 
     if N == 0 or M == 0:
         return np.nan, np.nan, np.nan, np.nan, [0] * len(n)
 
     # remove all zero entries in the sum, to present division by zero for individual bins
     z = n + m
     n = n[z != 0]
```

### Comparing `popmon-1.4.0/popmon/analysis/comparison/hist_comparer.py` & `popmon-1.4.3/popmon/analysis/comparison/hist_comparer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -17,31 +17,31 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import numpy as np
 import pandas as pd
 
-from ...analysis.apply_func import ApplyFunc
-from ...analysis.functions import (
+from popmon.analysis.apply_func import ApplyFunc
+from popmon.analysis.functions import (
     expand_norm_hist_mean_cov,
     expanding_hist,
     hist_sum,
     normalized_hist_mean_cov,
     relative_chi_squared,
     roll_norm_hist_mean_cov,
     rolling_hist,
 )
-from ...analysis.hist_numpy import (
+from popmon.analysis.hist_numpy import (
     check_similar_hists,
     get_consistent_numpy_entries,
     get_consistent_numpy_ndgrids,
 )
-from ...base import Pipeline
-from ...hist.hist_utils import COMMON_HIST_TYPES, is_numeric
+from popmon.base import Pipeline
+from popmon.hist.hist_utils import COMMON_HIST_TYPES, is_numeric
 
 
 def hist_compare(row, hist_name1="", hist_name2=""):
     """Function to compare two histograms
 
     Apply statistical tests to compare two input histograms, such as:
     Chi2, KS, Pearson, max probability difference.
@@ -128,15 +128,15 @@
 
         # make reference histogram(s)
         hist_collector = ApplyFunc(
             apply_to_key=read_key,
             assign_to_key=assign_to_key,
         )
         hist_collector.add_apply_func(
-            func=func_hist_collector, entire=True, suffix=suffix, *args, **kwargs
+            *args, func=func_hist_collector, entire=True, suffix=suffix, **kwargs
         )
         # do histogram comparison
         hist_comparer = ApplyFunc(
             apply_to_key=assign_to_key,
             assign_to_key=store_key,
             apply_funcs=[
                 {
@@ -322,15 +322,15 @@
         """
         if assign_to_key is None:
             assign_to_key = read_key
 
         # make reference histogram(s)
         hist_collector = ApplyFunc(apply_to_key=read_key, assign_to_key=assign_to_key)
         hist_collector.add_apply_func(
-            func=func_hist_collector, hist_name=hist_col, suffix="", *args, **kwargs
+            *args, func=func_hist_collector, hist_name=hist_col, suffix="", **kwargs
         )
 
         # do histogram comparison
         hist_comparer = ApplyFunc(
             apply_to_key=assign_to_key,
             assign_to_key=store_key,
             apply_funcs=[
```

### Comparing `popmon-1.4.0/popmon/analysis/functions.py` & `popmon-1.4.3/popmon/analysis/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -20,22 +20,22 @@
 
 import numpy as np
 import pandas as pd
 from numpy.lib.stride_tricks import as_strided
 from scipy import linalg, stats
 from scipy.stats import linregress, norm
 
-from ..analysis.hist_numpy import (
+from popmon.analysis.hist_numpy import (
     check_similar_hists,
     get_consistent_numpy_2dgrids,
     get_consistent_numpy_entries,
     set_2dgrid,
 )
-from ..hist.hist_utils import COMMON_HIST_TYPES, is_numeric
-from ..stats.numpy import probability_distribution_mean_covariance
+from popmon.hist.hist_utils import COMMON_HIST_TYPES, is_numeric
+from popmon.stats.numpy import probability_distribution_mean_covariance
 
 
 def pull(row, suffix_mean="_mean", suffix_std="_std", cols=None):
     """Calculate normalized residual (pull) for list of cols
 
     Function can be used by ApplyFunc module.
 
@@ -53,23 +53,25 @@
         cols = [
             m
             for m in set(indices)
             if all(r in indices for r in [m + suffix_mean, m + suffix_std])
         ]
 
     x = {
-        m: np.nan
-        if (
-            any(
-                r not in rdict or pd.isnull(rdict[r])
-                for r in [m, m + suffix_mean, m + suffix_std]
+        m: (
+            np.nan
+            if (
+                any(
+                    r not in rdict or pd.isnull(rdict[r])
+                    for r in [m, m + suffix_mean, m + suffix_std]
+                )
+                or rdict[m + suffix_std] == 0.0
             )
-            or rdict[m + suffix_std] == 0.0
+            else (rdict[m] - rdict[m + suffix_mean]) / rdict[m + suffix_std]
         )
-        else (rdict[m] - rdict[m + suffix_mean]) / rdict[m + suffix_std]
         for m in cols
     }
 
     return pd.Series(x)
 
 
 def expanding_mean(df, shift=1):
@@ -179,14 +181,15 @@
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int window: size of rolling window.
     :param int shift: size of shift. default is 0.
     :return: df with rolling z-score results of lin_regress() function applied to all columns
     """
+
     # MB 20200420: turn original df.rolling off, it doesn't accept timestamps.
     # raw=True suppresses Future warning
     # return df.shift(shift).rolling(window).apply(func, raw=True)
     def func(x):
         y = pd.Series(index=x.index, dtype=float)
         for name in x.index:
             try:
```

### Comparing `popmon-1.4.0/popmon/analysis/hist_numpy.py` & `popmon-1.4.3/popmon/analysis/hist_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -20,16 +20,16 @@
 
 import warnings
 
 import histogrammar
 import numpy as np
 from histogrammar.util import get_hist_props
 
-from ..hist.hist_utils import get_bin_centers, is_numeric
-from ..stats.numpy import quantile
+from popmon.hist.hist_utils import get_bin_centers, is_numeric
+from popmon.stats.numpy import quantile
 
 used_hist_types = (histogrammar.Bin, histogrammar.SparselyBin, histogrammar.Categorize)
 
 
 def prepare_ndgrid(hist, n_dim):
     """Get lists of all unique combinations of keys
 
@@ -47,28 +47,28 @@
 
     def get_hist_keys(h):
         if hasattr(h, "bins"):
             return set(h.bins.keys())
         elif hasattr(h, "values"):
             return set(range(len(h.values)))
         else:
-            raise TypeError()
+            raise TypeError
 
     # SparselyBin or Categorize
     def keys_recursive(hist, hist_keys, idx):
         hist_keys[idx] |= get_hist_keys(hist)
         if (idx + 1) < len(hist_keys):
             if hasattr(hist, "bins"):
                 for h in hist.bins.values():
                     hist_keys = keys_recursive(h, hist_keys, idx + 1)
             elif hasattr(hist, "values"):
                 for h in hist.values:
                     hist_keys = keys_recursive(h, hist_keys, idx + 1)
             else:
-                raise TypeError()
+                raise TypeError
         return hist_keys
 
     keys = [set() for _ in range(n_dim)]
     keys = keys_recursive(hist, keys, 0)
     keys = [sorted(k) for k in keys]
     return keys
 
@@ -104,33 +104,32 @@
 
     def flatten(histogram, keys, grid, dim=0, prefix=None):
         if prefix is None:
             prefix = []
 
         if len(keys) == len(prefix):
             grid[tuple(prefix)] = histogram.entries
+        elif hasattr(histogram, "bins"):
+            for k, h in histogram.bins.items():
+                if k not in keys[dim]:
+                    continue
+                i = keys[dim].index(k)
+                flatten(h, keys, grid, dim + 1, [i, *prefix])
+        elif hasattr(histogram, "values"):
+            for i, h in enumerate(histogram.values):
+                flatten(h, keys, grid, dim + 1, [i, *prefix])
         else:
-            if hasattr(histogram, "bins"):
-                for k, h in histogram.bins.items():
-                    if k not in keys[dim]:
-                        continue
-                    i = keys[dim].index(k)
-                    flatten(h, keys, grid, dim + 1, [i] + prefix)
-            elif hasattr(histogram, "values"):
-                for i, h in enumerate(histogram.values):
-                    flatten(h, keys, grid, dim + 1, [i] + prefix)
-            else:
-                raise TypeError()
+            raise TypeError
 
     flatten(hist, keys, grid)
     return grid
 
 
 def set_2dgrid(hist, keys):
-    """Set 2d grid of first two dimenstions of input histogram
+    """Set 2d grid of first two dimensions of input histogram
 
     Used as input by get_2dgrid(hist).
 
     :param hist: input histogrammar histogram
     :param list xkeys: list with unique x keys
     :param list ykeys: list with unique y keys
     :return: filled 2d numpy grid
@@ -138,15 +137,15 @@
     return set_ndgrid(hist, keys, n_dim=2)
 
 
 def get_ndgrid(hist, get_bin_labels=False, n_dim=2):
     """Get filled n-d grid of first n dimensions of input histogram
 
     :param hist: input histogrammar histogram
-    :return: grid of first n dimenstions of input histogram
+    :return: grid of first n dimensions of input histogram
     """
     if hist.n_dim < n_dim:
         warnings.warn(
             f"Input histogram only has {hist.n_dim} dimensions (<{n_dim}). Returning empty grid."
         )
         return np.zeros(tuple([0] * n_dim))
 
@@ -159,29 +158,29 @@
     return grid
 
 
 def get_2dgrid(hist, get_bin_labels=False):
     """Get filled x,y grid of first two dimensions of input histogram
 
     :param hist: input histogrammar histogram
-    :return: x,y grid of first two dimenstions of input histogram
+    :return: x,y grid of first two dimensions of input histogram
     """
     return get_ndgrid(hist, get_bin_labels, n_dim=2)
 
 
-def get_consistent_numpy_ndgrids(hist_list=[], get_bin_labels=False, dim=3):
+def get_consistent_numpy_ndgrids(hist_list=None, get_bin_labels=False, dim=3):
     """Get list of consistent x,y grids of first n dimensions of (sparse) input histograms
 
     :param list hist_list: list of input histogrammar histograms
     :param bool get_bin_labels: if true, return x-keys and y-keys describing binnings of 2d-grid.
     :param int dim: number of dimension (>= 3)
     :return: list of consistent x,y grids of first two dimensions of each input histogram in list
     """
     # --- basic checks
-    if len(hist_list) == 0:
+    if hist_list is None or len(hist_list) == 0:
         raise ValueError("Input histogram list has zero length.")
     if hist_list[0].n_dim < dim:
         raise ValueError(
             f"Input histogram only has {hist_list[0].n_dim} dimensions (<{dim}). Cannot compute {dim}d-grid."
         )
     assert_similar_hists(hist_list)
 
@@ -196,21 +195,23 @@
 
     if get_bin_labels:
         return gridnd_list, keys
 
     return gridnd_list
 
 
-def get_consistent_numpy_2dgrids(hist_list=[], get_bin_labels=False):
+def get_consistent_numpy_2dgrids(hist_list=None, get_bin_labels=False):
     """Get list of consistent x,y grids of first two dimensions of (sparse) input histograms
 
     :param list hist_list: list of input histogrammar histograms
     :param bool get_bin_labels: if true, return x-keys and y-keys describing binnings of 2d-grid.
     :return: list of consistent x,y grids of first two dimensions of each input histogram in list
     """
+    if hist_list is None:
+        hist_list = []
     return get_consistent_numpy_ndgrids(hist_list, get_bin_labels, dim=2)
 
 
 def get_consistent_numpy_1dhists(hist_list, get_bin_labels=False, crop_range=False):
     """Get list of consistent numpy hists for list of sparse (or bin) input histograms
 
     Works for sparse and bin histograms.
@@ -385,74 +386,74 @@
     # - datatypes
     # - Bin attributes
     # - SparselyBin attributes
     # - all above for sub-histograms in case of n-dim > 1
 
     # Check generic attributes - filled histograms only
     n_d = [hist.n_dim for hist in hist_list]
-    if not n_d.count(n_d[0]) == len(n_d):
+    if n_d.count(n_d[0]) != len(n_d):
         warnings.warn("Input histograms have inconsistent dimensions.")
         return False
     dts = [hist.datatype for hist in hist_list]
-    if not dts.count(dts[0]) == len(dts):
+    if dts.count(dts[0]) != len(dts):
         warnings.warn(f"Input histograms have inconsistent datatypes: {dts}")
         return False
     # Check generic attributes
     if check_type:
         # E.g. histogrammar.specialized.CategorizeHistogramMethods and
         # histogrammar.primitives.categorize.Categorize are both of type hg.Categorize
         # Make this consistent first.
         types = [get_contentType(hist) for hist in hist_list]
-        if not types.count(types[0]) == len(types):
+        if types.count(types[0]) != len(types):
             warnings.warn(
                 "Input histograms have inconsistent class types: {types}".format(
                     types=types
                 )
             )
             return False
 
     # Check Bin attributes
     if isinstance(hist_list[0], histogrammar.Bin):
         nums = [hist.num for hist in hist_list]
-        if not nums.count(nums[0]) == len(nums):
+        if nums.count(nums[0]) != len(nums):
             warnings.warn(
                 "Input Bin histograms have inconsistent num attributes: {types}".format(
                     types=nums
                 )
             )
             return False
         lows = [hist.low for hist in hist_list]
-        if not lows.count(lows[0]) == len(lows):
+        if lows.count(lows[0]) != len(lows):
             warnings.warn(
                 "Input Bin histograms have inconsistent low attributes: {types}".format(
                     types=lows
                 )
             )
             return False
         highs = [hist.high for hist in hist_list]
-        if not highs.count(highs[0]) == len(highs):
+        if highs.count(highs[0]) != len(highs):
             warnings.warn(
                 "Input histograms have inconsistent high attributes: {types}".format(
                     types=highs
                 )
             )
             return False
 
     # Check SparselyBin attributes
     if isinstance(hist_list[0], histogrammar.SparselyBin):
         origins = [hist.origin for hist in hist_list]
-        if not origins.count(origins[0]) == len(origins):
+        if origins.count(origins[0]) != len(origins):
             warnings.warn(
                 "Input SparselyBin histograms have inconsistent origin attributes: {types}".format(
                     types=origins
                 )
             )
             return False
         bws = [hist.binWidth for hist in hist_list]
-        if not bws.count(bws[0]) == len(bws):
+        if bws.count(bws[0]) != len(bws):
             warnings.warn(
                 "Input SparselyBin histograms have inconsistent binWidth attributes: {types}".format(
                     types=bws
                 )
             )
             return False
```

### Comparing `popmon-1.4.0/popmon/analysis/merge_statistics.py` & `popmon-1.4.3/popmon/analysis/merge_statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,29 +13,28 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-
-from typing import List
+from __future__ import annotations
 
 import pandas as pd
 
-from ..base import Module
+from popmon.base import Module
 
 
 class MergeStatistics(Module):
     """Merging dictionaries of features containing dataframes with statistics as its values."""
 
     _input_keys = ("read_keys",)
     _output_keys = ("store_key",)
 
-    def __init__(self, read_keys: List[str], store_key: str):
+    def __init__(self, read_keys: list[str], store_key: str):
         """Initialize an instance of MergeStatistics.
 
         :param list read_keys: list of keys of input data to read from the datastore
         :param str store_key: key of output data to store in the datastore
         """
         super().__init__()
         self.read_keys = read_keys
```

### Comparing `popmon-1.4.0/popmon/analysis/profiling/__init__.py` & `popmon-1.4.3/popmon/analysis/profiling/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,20 +12,21 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from ...analysis.profiling.hist_profiler import HistProfiler
-from ...analysis.profiling.pull_calculator import (
+from popmon.analysis.profiling.hist_profiler import HistProfiler
+from popmon.analysis.profiling.pull_calculator import (
     ExpandingPullCalculator,
     ReferencePullCalculator,
     RollingPullCalculator,
 )
+
 from .profiles import Profiles
 
 __all__ = [
     "Profiles",
     "HistProfiler",
     "RollingPullCalculator",
     "ReferencePullCalculator",
```

### Comparing `popmon-1.4.0/popmon/analysis/profiling/hist_profiler.py` & `popmon-1.4.3/popmon/analysis/profiling/hist_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -17,16 +17,16 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import numpy as np
 import pandas as pd
 
-from ...base import Module
-from ...hist.hist_utils import get_bin_centers, is_numeric, is_timestamp
+from popmon.base import Module
+from popmon.hist.hist_utils import get_bin_centers, is_numeric, is_timestamp
 
 
 class HistProfiler(Module):
     """Generate profiles of histograms using default statistical functions.
 
     Profiles are:
 
@@ -67,15 +67,15 @@
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.var_timestamp = var_timestamp or []
         self.hist_col = hist_col
         self.index_col = index_col
 
         if stats_functions is not None:
-            raise NotImplementedError()
+            raise NotImplementedError
 
     def _profile_1d_histogram(self, name, hist):
         from popmon.analysis import Profiles
 
         # preprocessing value counts and TS
         is_num = is_numeric(hist)
         is_ts = is_timestamp(hist) or name in self.var_timestamp
```

### Comparing `popmon-1.4.0/popmon/analysis/profiling/profiles.py` & `popmon-1.4.3/popmon/analysis/profiling/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -16,19 +16,18 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import numpy as np
 
+from popmon.analysis.hist_numpy import get_2dgrid
 from popmon.base.registry import Registry
-
-from ...analysis.hist_numpy import get_2dgrid
-from ...hist.hist_utils import sum_entries
-from ...stats import numpy as pm_np
+from popmon.hist.hist_utils import sum_entries
+from popmon.stats import numpy as pm_np
 
 Profiles = Registry()
 
 
 @Profiles.register(
     key=["min", "max", "p01", "p05", "p16", "p50", "p84", "p95", "p99"],
     description=[
@@ -41,29 +40,29 @@
         "84% percentile",
         "95% percentile",
         "99% percentile",
     ],
     dim=1,
     htype="num",
 )
-def profile_quantiles(x, w, bin_width):
+def profile_quantiles(x, w, _):
     return tuple(
         pm_np.quantile(
             x, q=[0.0, 1.0, 0.01, 0.05, 0.16, 0.50, 0.84, 0.95, 0.99], weights=w
         )
     )
 
 
 @Profiles.register(key="mean", description="Mean value", dim=1, htype="num")
-def profile_mean(x, w, bin_width):
+def profile_mean(x, w, _):
     return pm_np.mean(x, w)
 
 
 @Profiles.register(key="std", description="Standard deviation", dim=1, htype="num")
-def profile_std(x, w, bin_width):
+def profile_std(x, w, _):
     return pm_np.std(x, w)
 
 
 @Profiles.register(
     key="nan", description="Number of missing entries (NaN)", dim=1, htype=None
 )
 def profile_nan(hist):
@@ -104,18 +103,15 @@
     dim=2,
     htype=None,
 )
 def profile_phik(hist):
     from phik import phik
 
     # calculate phik correlation
-    try:
-        grid = get_2dgrid(hist)
-    except Exception:
-        raise
+    grid = get_2dgrid(hist)
 
     try:
         phi_k = phik.phik_from_hist2d(observed=grid)
     except ValueError:
         # self.logger.debug(
         #     f"Not enough values in the 2d `{name}` time-split histogram to apply the phik test."
         # )
```

### Comparing `popmon-1.4.0/popmon/analysis/profiling/pull_calculator.py` & `popmon-1.4.3/popmon/analysis/profiling/pull_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -17,24 +17,24 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import numpy as np
 import pandas as pd
 
-from ...analysis.apply_func import ApplyFunc
-from ...analysis.functions import (
+from popmon.analysis.apply_func import ApplyFunc
+from popmon.analysis.functions import (
     expanding_mean,
     expanding_std,
     pull,
     rolling_mean,
     rolling_std,
 )
-from ...base import Pipeline
-from ...stats.numpy import mad
+from popmon.base import Pipeline
+from popmon.stats.numpy import mad
 
 
 class PullCalculator(Pipeline):
     """Base module for pull calculation, based on mean and standard deviation calculation
 
     Steps as performed by ApplyFunc modules:
 
@@ -78,18 +78,18 @@
         if assign_to_key is None:
             assign_to_key = apply_to_key
 
         calc_mean_std = ApplyFunc(
             apply_to_key=apply_to_key, assign_to_key=assign_to_key, features=features
         )
         calc_mean_std.add_apply_func(
-            func_std, suffix=suffix_std, entire=True, *args, **kwargs
+            func_std, *args, suffix=suffix_std, entire=True, **kwargs
         )
         calc_mean_std.add_apply_func(
-            func_mean, suffix=suffix_mean, entire=True, *args, **kwargs
+            func_mean, *args, suffix=suffix_mean, entire=True, **kwargs
         )
 
         calc_pull = ApplyFunc(
             apply_to_key=assign_to_key, assign_to_key=store_key, features=features
         )
         calc_pull.add_apply_func(
             pull,
```

### Comparing `popmon-1.4.0/popmon/base/__init__.py` & `popmon-1.4.3/popmon/base/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,11 +14,11 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..base.module import Module
-from ..base.pipeline import Pipeline
+from popmon.base.module import Module
+from popmon.base.pipeline import Pipeline
 
 __all__ = ["Module", "Pipeline"]
```

### Comparing `popmon-1.4.0/popmon/base/module.py` & `popmon-1.4.3/popmon/base/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `popmon-1.4.0/popmon/base/pipeline.py` & `popmon-1.4.3/popmon/base/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,39 +12,37 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+from __future__ import annotations
 
 import logging
-from abc import ABC
 
 
-class Pipeline(ABC):
-    """Abstract base class used for to run modules in a pipeline."""
+class Pipeline:
+    """Base class used for to run modules in a pipeline."""
 
-    def __init__(self, modules, logger=None):
+    def __init__(self, modules, logger: logging.Logger | None = None):
         """Initialization of the pipeline
 
         :param list modules: modules of the pipeline.
         :param logger: logger to be used by each module.
         """
         self.modules = modules
         self.set_logger(logger)
 
-    def set_logger(self, logger):
+    def set_logger(self, logger: logging.Logger | None):
         """Set the logger to be used by each module
 
         :param logger: input logger
         """
-        self.logger = logger
-        if self.logger is None:
-            self.logger = logging.getLogger()
+        self.logger = logger or logging.getLogger()
         for module in self.modules:
             module.set_logger(self.logger)
 
     def add_modules(self, modules):
         """Add more modules to existing list of modules.
 
         :param list modules: list of more modules
@@ -52,15 +50,15 @@
         if len(modules):
             self.modules.extend(modules)
 
     def transform(self, datastore):
         """Central function of the pipeline.
 
         Calls transform() of each module in the pipeline.
-        Typically transform() of a module takes something from the datastore, does something to it,
+        Typically, transform() of a module takes something from the datastore, does something to it,
         and puts the results back into the datastore again, to be passed on to the next module in the pipeline.
 
         :param dict datastore: input datastore
         :return: updated output datastore
         :rtype: dict
         """
```

### Comparing `popmon-1.4.0/popmon/base/registry.py` & `popmon-1.4.3/popmon/base/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,35 +12,35 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+from __future__ import annotations
 
 from collections import defaultdict
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable
 
 
 class Registry:
     _properties = ("dim", "htype")
 
     def __init__(self):
-        self._keys: List[str] = []
-        self._descriptions: Dict[str, str] = {}
+        self._keys: list[str] = []
+        self._descriptions: dict[str, str] = {}
         self._properties_to_func = defaultdict(lambda: defaultdict(dict))
         self._func_name_to_properties = {}
 
     def register(
         self,
-        key: Union[str, List[str], Tuple[str]],
-        description: Union[str, List[str], Tuple[str]],
+        key: str | list[str] | tuple[str],
+        description: str | list[str] | tuple[str],
         dim: int = -1,
-        htype: Optional[str] = None,
+        htype: str | None = None,
     ):
         # rename for function use, without changing api
         keys = key
         del key
 
         descriptions = description
         del description
@@ -78,40 +78,38 @@
             return func
 
         return f
 
     # Methods
     def _get_func_properties_by_name(
         self, function_name: str
-    ) -> Tuple[int, str, Tuple[str]]:
+    ) -> tuple[int, str, tuple[str]]:
         return self._func_name_to_properties[function_name]
 
     def get_func_by_name(self, function_name: str) -> Callable:
         """
          Get a function by the function name
 
         :param str function_name: name of the original function
         """
         dim, htype, key = self._get_func_properties_by_name(function_name)
         return self._properties_to_func[dim][htype][key]
 
-    def get_func_by_dim_and_htype(self, dim, htype) -> Dict[Tuple[str], Callable]:
+    def get_func_by_dim_and_htype(self, dim, htype) -> dict[tuple[str], Callable]:
         return self._properties_to_func[dim][htype]
 
-    def get_keys(self) -> List[str]:
+    def get_keys(self) -> list[str]:
         """List of keys associated with registered functions"""
         return self._keys
 
-    def get_keys_by_dim_and_htype(self, dim, htype) -> List[str]:
+    def get_keys_by_dim_and_htype(self, dim, htype) -> list[str]:
         """Flat list of keys for a provided dimension and histogram type"""
-        return [
-            v for values in self._properties_to_func[dim][htype].keys() for v in values
-        ]
+        return [v for values in self._properties_to_func[dim][htype] for v in values]
 
-    def get_descriptions(self) -> Dict[str, str]:
+    def get_descriptions(self) -> dict[str, str]:
         """Dictionary of key->description associated with registered functions"""
         return self._descriptions
 
     def update_func(self, name, func) -> None:
         dim, htype, key = self._func_name_to_properties[name]
         self._properties_to_func[dim][htype][key] = func
```

### Comparing `popmon-1.4.0/popmon/config.py` & `popmon-1.4.3/popmon/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `popmon-1.4.0/popmon/decorators/__init__.py` & `popmon-1.4.3/popmon/stats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,11 +14,10 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-# flake8: noqa
+from popmon.stats.numpy import mean, median, quantile, std
 
-# import pandas and spark DataFrame decorators
-from ..decorators import pandas, spark
+__all__ = ["mean", "std", "median", "quantile"]
```

### Comparing `popmon-1.4.0/popmon/decorators/pandas.py` & `popmon-1.4.3/popmon/decorators/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -17,16 +17,16 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 from histogrammar.dfinterface.make_histograms import make_histograms
 from pandas import DataFrame
 
-from ..pipeline.metrics import df_stability_metrics
-from ..pipeline.report import df_stability_report
+from popmon.pipeline.metrics import df_stability_metrics
+from popmon.pipeline.report import df_stability_report
 
 # add function to create histogrammar histograms.
 # pm_make_histograms is kept for bkw compatibility.
 DataFrame.pm_make_histograms = make_histograms
 
 # add function to create stability report
 DataFrame.pm_stability_report = df_stability_report
```

### Comparing `popmon-1.4.0/popmon/decorators/spark.py` & `popmon-1.4.3/popmon/decorators/spark.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `popmon-1.4.0/popmon/extensions/__init__.py` & `popmon-1.4.3/popmon/extensions/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `popmon-1.4.0/popmon/extensions/profile_diptest.py` & `popmon-1.4.3/popmon/extensions/profile_diptest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -63,9 +63,8 @@
         # compute diptest
         dip, pval = diptest(sample_noise)
         return dip, pval
 
 
 class Diptest(Extension):
     name = "diptest"
-    requirements = ["diptest"]
     extension = extension
```

### Comparing `popmon-1.4.0/popmon/extensions/utils.py` & `popmon-1.4.3/popmon/stitching/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,33 +13,11 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-import json
-from pathlib import Path
 
-from popmon.extensions import extensions
+from popmon.stitching.hist_stitcher import HistStitcher, stitch_histograms
 
-
-def get_extras():
-    """Obtain extras from extensions"""
-    extras = {}
-    for extension in extensions:
-        extras.update(extension.extras)
-
-    return extras
-
-
-def write_extras():
-    """Write extras to extras.json for setup.py"""
-    extras = get_extras()
-    file_path = Path(__file__).parent.parent.parent / "extras.json"
-
-    with file_path.open("w") as f:
-        json.dump(extras, f)
-
-
-if __name__ == "__main__":
-    write_extras()
+__all__ = ["HistStitcher", "stitch_histograms"]
```

### Comparing `popmon-1.4.0/popmon/hist/__init__.py` & `popmon-1.4.3/popmon/pipeline/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,12 +12,7 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-from ..hist.hist_splitter import HistSplitter
-
-__all__ = ["HistSplitter"]
```

### Comparing `popmon-1.4.0/popmon/hist/filling/__init__.py` & `popmon-1.4.3/popmon/hist/filling/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,15 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-# MB 20210323: histogrammming code hade been moved to histogrammar v1.0.20+
+# MB 20210323: histogrammming code has been moved to histogrammar v1.0.20+
 #              these imports are kept for backwards compatibility.
 
 from histogrammar.dfinterface.make_histograms import (
     get_bin_specs,
     get_one_time_axis,
     get_time_axes,
     has_one_time_axis,
```

### Comparing `popmon-1.4.0/popmon/hist/hist_splitter.py` & `popmon-1.4.3/popmon/hist/hist_splitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -16,16 +16,16 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import pandas as pd
 
-from ..base import Module
-from ..hist.hist_utils import (
+from popmon.base import Module
+from popmon.hist.hist_utils import (
     get_histogram,
     is_timestamp,
     split_hist_along_first_dimension,
 )
 
 
 class HistSplitter(Module):
```

### Comparing `popmon-1.4.0/popmon/hist/hist_utils.py` & `popmon-1.4.3/popmon/hist/hist_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -280,16 +280,16 @@
     #   datatype, so that the comparison of split-histograms along the x-axis gives inconsistent histograms.
     #   In this step we filter out any such empty sub-histograms, to ensure that
     #   all left-over sub-histograms are consistent with each other.
     if filter_empty_split_hists:
         centers, values = _filter_empty_split_hists(centers, values)
 
     for name, val in zip(centers, values):
-        name = _edit_name(hist, name, xname, yname, convert_time_index, short_keys)
-        hdict[name] = val
+        hname = _edit_name(hist, name, xname, yname, convert_time_index, short_keys)
+        hdict[hname] = val
 
     return hdict
 
 
 def _filter_empty_split_hists(centers, values):
     """Filter empty split histograms from input centers and values
```

### Comparing `popmon-1.4.0/popmon/io/__init__.py` & `popmon-1.4.3/popmon/hist/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,12 +14,10 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..io.file_reader import FileReader
-from ..io.file_writer import FileWriter
-from ..io.json_reader import JsonReader
+from popmon.hist.hist_splitter import HistSplitter
 
-__all__ = ["FileWriter", "FileReader", "JsonReader"]
+__all__ = ["HistSplitter"]
```

### Comparing `popmon-1.4.0/popmon/io/file_reader.py` & `popmon-1.4.3/popmon/io/file_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,62 +13,70 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
+import copy
 from pathlib import Path
-from typing import Callable, Optional, Union
+from typing import Callable
 
-from ..base import Module
+from popmon.base import Module
 
 
-class FileReader(Module):
-    """Module to read contents from a file, transform the contents with a function and write them to the datastore."""
+class FileWriter(Module):
+    """Module transforms specific datastore content and writes it to a file."""
 
-    _input_keys = ()
+    _input_keys = ("read_key",)
     _output_keys = ("store_key",)
 
     def __init__(
         self,
-        store_key: str,
-        file_path: Union[str, Path],
-        apply_func: Optional[Callable] = None,
+        read_key: str,
+        store_key: str | None = None,
+        file_path: str | Path | None = None,
+        apply_func: Callable | None = None,
         **kwargs,
     ):
         """Initialize an instance.
 
-        :param str store_key: key of input data to be stored in the datastore
-        :param str file_path: the file path to read the data from
+        :param str read_key: key of input histogram-dict to read from data store
+        :param str store_key: key of output data to store in data store (optional)
+        :param str file_path: the file path where to output the report (optional)
         :param callable apply_func: function to be used for the transformation of data (optional)
         :param dict kwargs: additional keyword arguments which would be passed to `apply_func`
         """
         super().__init__()
-        if not isinstance(file_path, (str, Path)):
+        if file_path is not None and not isinstance(file_path, (str, Path)):
             raise TypeError("file_path should be of type `str` or `pathlib.Path`")
         if apply_func is not None and not callable(apply_func):
             raise TypeError("transformation function must be a callable object")
+        self.read_key = read_key
+        self.store_key = store_key or read_key
 
-        self.store_key = store_key
         self.file_path = file_path
         self.apply_func = apply_func
         self.kwargs = kwargs
 
     def get_description(self):
         return self.file_path
 
-    def transform(self):
-        with open(self.file_path) as file:
-            data = file.read()
+    def transform(self, data):
+        data = copy.deepcopy(data)
 
         # if a transformation function is provided, transform the data
         if self.apply_func is not None:
             data = self.apply_func(data, **self.kwargs)
 
+        # if file path is provided, write data to a file. Otherwise, write data into the datastore
+        if self.file_path is None:
+            return data
+
+        with open(self.file_path, "w+") as file:
+            file.write(data)
         self.logger.info(
-            f'Object "{self.store_key}" read from file "{self.file_path}".'
+            f'Object "{self.read_key}" written to file "{self.file_path}".'
         )
-
-        # store the transformed/original contents
-        return data
+        return None
```

### Comparing `popmon-1.4.0/popmon/io/file_writer.py` & `popmon-1.4.3/popmon/io/file_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,69 +13,63 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
-import copy
 from pathlib import Path
-from typing import Callable, Optional, Union
+from typing import Callable
 
-from ..base import Module
+from popmon.base import Module
 
 
-class FileWriter(Module):
-    """Module transforms specific datastore content and writes it to a file."""
+class FileReader(Module):
+    """Module to read contents from a file, transform the contents with a function and write them to the datastore."""
 
-    _input_keys = ("read_key",)
+    _input_keys = ()
     _output_keys = ("store_key",)
 
     def __init__(
         self,
-        read_key: str,
-        store_key: Optional[str] = None,
-        file_path: Optional[Union[str, Path]] = None,
-        apply_func: Optional[Callable] = None,
+        store_key: str,
+        file_path: str | Path,
+        apply_func: Callable | None = None,
         **kwargs,
     ):
         """Initialize an instance.
 
-        :param str read_key: key of input histogram-dict to read from data store
-        :param str store_key: key of output data to store in data store (optional)
-        :param str file_path: the file path where to output the report (optional)
+        :param str store_key: key of input data to be stored in the datastore
+        :param str file_path: the file path to read the data from
         :param callable apply_func: function to be used for the transformation of data (optional)
         :param dict kwargs: additional keyword arguments which would be passed to `apply_func`
         """
         super().__init__()
-        if file_path is not None and not isinstance(file_path, (str, Path)):
+        if not isinstance(file_path, (str, Path)):
             raise TypeError("file_path should be of type `str` or `pathlib.Path`")
         if apply_func is not None and not callable(apply_func):
             raise TypeError("transformation function must be a callable object")
-        self.read_key = read_key
-        self.store_key = store_key or read_key
 
+        self.store_key = store_key
         self.file_path = file_path
         self.apply_func = apply_func
         self.kwargs = kwargs
 
     def get_description(self):
         return self.file_path
 
-    def transform(self, data):
-        data = copy.deepcopy(data)
+    def transform(self):
+        with open(self.file_path) as file:
+            data = file.read()
 
         # if a transformation function is provided, transform the data
         if self.apply_func is not None:
             data = self.apply_func(data, **self.kwargs)
 
-        # if file path is provided, write data to a file. Otherwise, write data into the datastore
-        if self.file_path is None:
-            return data
-
-        with open(self.file_path, "w+") as file:
-            file.write(data)
         self.logger.info(
-            f'Object "{self.read_key}" written to file "{self.file_path}".'
+            f'Object "{self.store_key}" read from file "{self.file_path}".'
         )
-        return None
+
+        # store the transformed/original contents
+        return data
```

### Comparing `popmon-1.4.0/popmon/io/json_reader.py` & `popmon-1.4.3/popmon/io/json_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,26 +13,26 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 import json
 from pathlib import Path
-from typing import Union
 
-from ..io import FileReader
+from popmon.io import FileReader
 
 
 class JsonReader(FileReader):
     """Read json file's contents into the datastore."""
 
-    def __init__(self, file_path: Union[str, Path], store_key: str):
+    def __init__(self, file_path: str | Path, store_key: str):
         """Initialize an instance.
 
         :param str store_key: key of input data to be stored in the datastore
         :param str file_path: the file path to read the data from
         """
         super().__init__(store_key, file_path, apply_func=json.loads)
```

### Comparing `popmon-1.4.0/popmon/notebooks/popmon_tutorial_advanced.ipynb` & `popmon-1.4.3/popmon/notebooks/popmon_tutorial_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/notebooks/popmon_tutorial_basic.ipynb` & `popmon-1.4.3/popmon/notebooks/popmon_tutorial_basic.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/notebooks/popmon_tutorial_incremental_data.ipynb` & `popmon-1.4.3/popmon/notebooks/popmon_tutorial_incremental_data.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/notebooks/popmon_tutorial_reports.ipynb` & `popmon-1.4.3/popmon/notebooks/popmon_tutorial_reports.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/pipeline/__init__.py` & `popmon-1.4.3/popmon/decorators/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,7 +12,11 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+# import pandas and spark DataFrame decorators
+from popmon.decorators import pandas, spark  # noqa: F401
```

### Comparing `popmon-1.4.0/popmon/pipeline/amazing_pipeline.py` & `popmon-1.4.3/popmon/pipeline/amazing_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
```

### Comparing `popmon-1.4.0/popmon/pipeline/dataset_splitter.py` & `popmon-1.4.3/popmon/pipeline/dataset_splitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,26 +12,26 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+from __future__ import annotations
 
 from math import floor
-from typing import List, Optional, Union
 
 import pandas as pd
 from typing_extensions import Literal
 
 
 def _split_dataset_pandas(
     dataset,
     split_type: Literal["n_instances", "fraction", "condition"],
-    split: Union[int, float, pd.Series, str],
+    split: int | float | pd.Series | str,
 ):
     if split_type in ["n_instances", "fraction"]:
         if split_type == "fraction":
             n = dataset.shape[0]
             split = floor(split * n)
         reference = dataset.iloc[:split]
         df = dataset.iloc[split:]
@@ -48,30 +48,30 @@
 
     return reference, df
 
 
 def _split_dataset_spark(
     dataset,
     split_type: Literal["n_instances", "fraction", "condition"],
-    split: Union[int, float, pd.Series, str],
+    split: int | float | pd.Series | str,
     time_axis: str,
-    partition_cols: Optional[List[str]] = None,
+    partition_cols: list[str] | None = None,
     persist: bool = True,
 ):
     """
     Split a dataset into a reference and remaining part based on split params using PySpark
     (see `split_dataset`)
 
     :param split_type: meaning of split parameter
     :param split: split parameter
     :param time_axis: time axis
     :param partition_cols: cols to partition by (for performance)
     :param persist: persist or not, enabled by default since we are checking for empty dataframes
     """
-    from pyspark.sql import functions as F
+    from pyspark.sql import functions as F  # noqa: N812
     from pyspark.sql.window import Window
 
     if split_type in ["n_instances", "fraction"]:
         data_win = Window.orderBy(time_axis)
         if partition_cols is not None:
             data_win = data_win.partitionBy(partition_cols)
 
@@ -96,15 +96,15 @@
         raise ValueError(
             "Returned dataframe is empty. Please adjust the `split` argument"
         )
 
     return reference, df
 
 
-def split_dataset(dataset, split: Union[int, float, pd.Series, str], time_axis: str):
+def split_dataset(dataset, split: int | float | pd.Series | str, time_axis: str):
     """Split a dataset into a reference and remaining part based on split params.
 
     :param pd.Dataset|pyspark.sql.Dataset dataset: dataset as input
     :param Any split: split details, meaning depends on the type:
         if integer, then the reference will be the first ``split`` instances
         if float, then ``split`` will be used as ration (e.g. 0.5 returns a 50/50 split)
         otherwise, the ``split`` are interpreted as condition, where the records for which the condition is
```

### Comparing `popmon-1.4.0/popmon/pipeline/metrics.py` & `popmon-1.4.3/popmon/pipeline/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,21 +13,22 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 import logging
 
 from histogrammar.dfinterface.make_histograms import get_bin_specs, make_histograms
 
-from ..config import Settings
-from ..pipeline.metrics_pipelines import create_metrics_pipeline
+from popmon.config import Settings
+from popmon.pipeline.metrics_pipelines import create_metrics_pipeline
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s %(levelname)s [%(module)s]: %(message)s"
 )
 logger = logging.getLogger()
```

### Comparing `popmon-1.4.0/popmon/pipeline/metrics_pipelines.py` & `popmon-1.4.3/popmon/pipeline/metrics_pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,117 +12,115 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from typing import List, Union
+from __future__ import annotations
 
-from ..alerting import (
+from popmon.alerting import (
     AlertsSummary,
     DynamicBounds,
     StaticBounds,
     TrafficLightAlerts,
     traffic_light_summary,
 )
-from ..analysis.apply_func import ApplyFunc
-from ..analysis.comparison.hist_comparer import (
+from popmon.analysis.apply_func import ApplyFunc
+from popmon.analysis.comparison.hist_comparer import (
     ExpandingHistComparer,
     PreviousHistComparer,
     ReferenceHistComparer,
     RollingHistComparer,
 )
-from ..analysis.functions import rolling_lr_zscore
-from ..analysis.profiling import HistProfiler
-from ..analysis.profiling.pull_calculator import (
+from popmon.analysis.functions import rolling_lr_zscore
+from popmon.analysis.profiling import HistProfiler
+from popmon.analysis.profiling.pull_calculator import (
     ExpandingPullCalculator,
     ReferencePullCalculator,
     RefMedianMadPullCalculator,
     RollingPullCalculator,
 )
-from ..base import Module, Pipeline
-from ..config import Settings
-from ..hist.hist_splitter import HistSplitter
+from popmon.base import Module, Pipeline
+from popmon.config import Settings
+from popmon.hist.hist_splitter import HistSplitter
+
 from .timing import Timing
 
 
 def get_metrics_pipeline_class(reference_type, reference):
     _metrics_pipeline_register = {
         "self": SelfReferenceMetricsPipeline,
         "external": ExternalReferenceMetricsPipeline,
         "self_split": ExternalReferenceMetricsPipeline,
         "rolling": RollingReferenceMetricsPipeline,
         "expanding": ExpandingReferenceMetricsPipeline,
     }
 
     if reference_type not in _metrics_pipeline_register:
         raise ValueError(
-            f"reference_type should be in {str(_metrics_pipeline_register.keys())}'."
+            f"reference_type should be in {_metrics_pipeline_register.keys()!s}'."
         )
     if (
         reference_type in ["external", "self_split"]
         and not isinstance(reference, dict)
         and reference is not None
     ):
         raise TypeError("reference should be a dict of histogrammar histograms.")
 
     return _metrics_pipeline_register[reference_type]
 
 
 def create_metrics_pipeline(
     settings: Settings,
-    reference_type="self",
     reference=None,
     hists_key="hists",
     **kwargs,
 ):
     # configuration and datastore for report pipeline
     cfg = {
         "hists_key": hists_key,
         "settings": settings,
         **kwargs,
     }
 
     # execute reporting pipeline
-    cls = get_metrics_pipeline_class(reference_type, reference)
+    cls = get_metrics_pipeline_class(settings.reference_type, reference)
     pipeline = cls(**cfg)
     return pipeline
 
 
-def get_timing_module(key: str) -> List[Module]:
+def get_timing_module(key: str) -> list[Module]:
     return [Timing(store_key=key)]
 
 
-def get_splitting_modules(
-    hists_key, features, time_axis
-) -> List[Union[Module, Pipeline]]:
+def get_splitting_modules(hists_key, features, time_axis) -> list[Module | Pipeline]:
     """
     Splitting of test histograms. For each histogram with datetime i, comparison of histogram i with histogram i-1,
     results in chi2 comparison of histograms
     """
-    modules: List[Union[Module, Pipeline]] = [
+    modules: list[Module | Pipeline] = [
         HistSplitter(
             read_key=hists_key,
             store_key="split_hists",
             features=features,
             feature_begins_with=f"{time_axis}:",
         ),
         PreviousHistComparer(read_key="split_hists", store_key="comparisons"),
         HistProfiler(read_key="split_hists", store_key="profiles"),
     ]
     return modules
 
 
-def get_traffic_light_modules(monitoring_rules) -> List[Union[Module, Pipeline]]:
+def get_traffic_light_modules(monitoring_rules) -> list[Module | Pipeline]:
     """
     Expand all (wildcard) static traffic light bounds and apply them.
     Applied to both profiles and comparisons datasets
     """
-    modules: List[Union[Module, Pipeline]] = [
+    modules: list[Module | Pipeline] = [
         TrafficLightAlerts(
             read_key="profiles",
             rules=monitoring_rules,
             store_key="traffic_lights",
             expanded_rules_key="static_bounds",
         ),
         TrafficLightAlerts(
@@ -138,20 +136,20 @@
             msg="Generating traffic light alerts summary.",
         ),
         AlertsSummary(read_key="alerts"),
     ]
     return modules
 
 
-def get_static_bound_modules(pull_rules) -> List[Union[Module, Pipeline]]:
+def get_static_bound_modules(pull_rules) -> list[Module | Pipeline]:
     """
     generate dynamic traffic light boundaries, based on traffic lights for normalized residuals, used for
     plotting in popmon_profiles report.
     """
-    modules: List[Union[Module, Pipeline]] = [
+    modules: list[Module | Pipeline] = [
         StaticBounds(
             read_key="profiles",
             rules=pull_rules,
             store_key="dynamic_bounds",
             suffix_mean="_mean",
             suffix_std="_std",
         ),
@@ -162,20 +160,20 @@
             suffix_mean="_mean",
             suffix_std="_std",
         ),
     ]
     return modules
 
 
-def get_dynamic_bound_modules(pull_rules) -> List[Union[Module, Pipeline]]:
+def get_dynamic_bound_modules(pull_rules) -> list[Module | Pipeline]:
     """
     Generate dynamic traffic light boundaries, based on traffic lights for normalized residuals, used for
     plotting in popmon_profiles report.
     """
-    modules: List[Union[Module, Pipeline]] = [
+    modules: list[Module | Pipeline] = [
         DynamicBounds(
             read_key="profiles",
             rules=pull_rules,
             store_key="dynamic_bounds",
             suffix_mean="_mean",
             suffix_std="_std",
         ),
@@ -186,17 +184,17 @@
             suffix_mean="_mean",
             suffix_std="_std",
         ),
     ]
     return modules
 
 
-def get_trend_modules(window) -> List[Union[Module, Pipeline]]:
+def get_trend_modules(window) -> list[Module | Pipeline]:
     """Looking for significant rolling linear trends in selected features/metrics"""
-    modules: List[Union[Module, Pipeline]] = [
+    modules: list[Module | Pipeline] = [
         ApplyFunc(
             apply_to_key="profiles",
             assign_to_key="comparisons",
             apply_funcs=[
                 {
                     "func": rolling_lr_zscore,
                     "suffix": f"_trend{window}_zscore",
@@ -221,15 +219,15 @@
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled self reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
 
         reference_prefix = "ref"
-        reference_modules: List[Union[Module, Pipeline]] = [
+        reference_modules: list[Module | Pipeline] = [
             # 3. Comparison of with profiled test histograms, results in chi2 comparison of histograms
             ReferenceHistComparer(
                 reference_key="split_hists",
                 assign_to_key="split_hists",
                 store_key="comparisons",
             ),
             RefMedianMadPullCalculator(
@@ -279,15 +277,15 @@
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :param str ref_hists_key: key to reference histograms in datastore. default is 'ref_hists'
         :return: assembled external reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
 
         reference_prefix = "ref"
-        reference_modules: List[Union[Module, Pipeline]] = [
+        reference_modules: list[Module | Pipeline] = [
             # 3. Profiling of split reference histograms, then chi2 comparison with test histograms
             HistSplitter(
                 read_key=ref_hists_key,
                 store_key="split_ref_hists",
                 features=settings.features,
                 feature_begins_with=f"{settings.time_axis}:",
             ),
@@ -340,15 +338,15 @@
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled rolling reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
 
         reference_prefix = "roll"
-        reference_modules: List[Union[Module, Pipeline]] = [
+        reference_modules: list[Module | Pipeline] = [
             # 3. profiling of reference histograms, then comparison of with profiled test histograms
             #        results in chi2 comparison of histograms
             RollingHistComparer(
                 read_key="split_hists",
                 window=settings.comparison.window,
                 shift=settings.comparison.shift,
                 store_key="comparisons",
@@ -399,15 +397,15 @@
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled expanding reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
 
         reference_prefix = "expanding"
-        reference_modules: List[Union[Module, Pipeline]] = [
+        reference_modules: list[Module | Pipeline] = [
             # 3. profiling of reference histograms, then comparison of with profiled test histograms
             #    results in chi2 comparison of histograms
             ExpandingHistComparer(
                 read_key="split_hists",
                 shift=settings.comparison.shift,
                 store_key="comparisons",
             ),
```

### Comparing `popmon-1.4.0/popmon/pipeline/report.py` & `popmon-1.4.3/popmon/pipeline/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,34 +13,34 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 import logging
-from typing import Optional
 
 from histogrammar.dfinterface.make_histograms import get_bin_specs, make_histograms
 
-from ..config import Settings
-from ..pipeline.dataset_splitter import split_dataset
-from ..pipeline.report_pipelines import ReportPipe, get_report_pipeline_class
-from ..resources import templates_env
+from popmon.config import Settings
+from popmon.pipeline.dataset_splitter import split_dataset
+from popmon.pipeline.report_pipelines import ReportPipe, get_report_pipeline_class
+from popmon.resources import templates_env
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s %(levelname)s [%(module)s]: %(message)s"
 )
 logger = logging.getLogger()
 
 
 def stability_report(
     hists,
-    settings: Optional[Settings] = None,
+    settings: Settings | None = None,
     reference=None,
     **kwargs,
 ):
     """Create a data stability monitoring html report for given dict of input histograms.
 
     :param dict hists: input histograms to be profiled and monitored over time.
     :param popmon.config.Settings settings: popmon configuration object
@@ -125,15 +125,15 @@
 
     if (
         reference is not None
         and not isinstance(reference, dict)
         and settings.time_axis not in reference.columns
     ):
         raise ValueError(
-            f'time_axis  "{settings.time_axis}" not found in columns of reference dataframe.'
+            f'time_axis "{settings.time_axis}" not found in columns of reference dataframe.'
         )
 
     if settings.features is not None:
         # by now time_axis is defined. ensure that all histograms start with it.
         settings._ensure_features_time_axis()
 
     # interpret time_width and time_offset
```

### Comparing `popmon-1.4.0/popmon/pipeline/report_pipelines.py` & `popmon-1.4.3/popmon/pipeline/report_pipelines.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -18,31 +18,31 @@
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 from pathlib import Path
 
 from typing_extensions import Literal
 
-from ..base import Pipeline
-from ..config import Settings
-from ..io import FileWriter
-from ..pipeline.metrics_pipelines import (
+from popmon.base import Pipeline
+from popmon.config import Settings
+from popmon.io import FileWriter
+from popmon.pipeline.metrics_pipelines import (
     ExpandingReferenceMetricsPipeline,
     ExternalReferenceMetricsPipeline,
     RollingReferenceMetricsPipeline,
     SelfReferenceMetricsPipeline,
 )
-from ..visualization import (
+from popmon.visualization import (
     AlertSectionGenerator,
     HistogramSection,
     ReportGenerator,
     SectionGenerator,
     TrafficLightSectionGenerator,
 )
-from ..visualization.overview_section import OverviewSectionGenerator
+from popmon.visualization.overview_section import OverviewSectionGenerator
 
 
 def get_report_pipeline_class(
     reference_type: Literal["self", "external", "rolling", "expanding", "self_split"],
     reference,
 ):
     _report_pipeline = {
@@ -50,15 +50,15 @@
         "external": ExternalReference,
         "rolling": RollingReference,
         "expanding": ExpandingReference,
         "self_split": ExternalReference,
     }
     reference_types = list(_report_pipeline.keys())
     if reference_type not in reference_types:
-        raise ValueError(f"reference_type should be one of {str(reference_types)}.")
+        raise ValueError(f"reference_type should be one of {reference_types!s}.")
     if reference_type == "external" and not isinstance(reference, dict):
         raise TypeError("reference should be a dict of histogrammar histograms.")
 
     return _report_pipeline[reference_type]
 
 
 class SelfReference(Pipeline):
```

### Comparing `popmon-1.4.0/popmon/pipeline/timing.py` & `popmon-1.4.3/popmon/pipeline/timing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,15 +14,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from datetime import datetime
 
-from ..base import Module
+from popmon.base import Module
 
 
 class Timing(Module):
     """Module to add the current timestamp to the datastore."""
 
     _input_keys = ()
     _output_keys = ("store_key",)
```

### Comparing `popmon-1.4.0/popmon/resources.py` & `popmon-1.4.3/popmon/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -44,15 +44,16 @@
 # Resource types
 _RESOURCES = {"data": _DATA, "notebook": _NOTEBOOK}
 
 # Environment for visualization templates' directory
 _TEMPLATES_ENV = Environment(
     loader=FileSystemLoader(
         resource_filename(popmon.__name__, "visualization/templates")
-    )
+    ),
+    autoescape=True,
 )
 _TEMPLATES_ENV.filters["fmt_metric"] = lambda x: x.replace("_", " ")
 
 
 def _js_list(encoder, data):
     pairs = [_js_val(encoder, v) for v in data]
     return "[" + ", ".join(pairs) + "]"
```

### Comparing `popmon-1.4.0/popmon/stats/__init__.py` & `popmon-1.4.3/popmon/io/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,10 +14,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..stats.numpy import mean, median, quantile, std
+from popmon.io.file_reader import FileReader
+from popmon.io.file_writer import FileWriter
+from popmon.io.json_reader import JsonReader
 
-__all__ = ["mean", "std", "median", "quantile"]
+__all__ = ["FileWriter", "FileReader", "JsonReader"]
```

### Comparing `popmon-1.4.0/popmon/stats/numpy.py` & `popmon-1.4.3/popmon/stats/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -119,16 +119,16 @@
     if weights is None:
         return np.quantile(a, q, axis=axis, keepdims=keepdims)
     elif axis is None:
         raveled_data = np.ravel(a)
         idx = np.argsort(raveled_data)
         sorted_data = raveled_data[idx]
         sorted_weights = np.ravel(weights)[idx]
-        Sn = np.cumsum(sorted_weights)
-        Pn = (Sn - 0.5 * sorted_weights) / Sn[-1]
+        Sn = np.cumsum(sorted_weights)  # noqa: N806
+        Pn = (Sn - 0.5 * sorted_weights) / Sn[-1]  # noqa: N806
         y = np.interp(q, Pn, sorted_data)
         if keepdims:
             y = y.reshape((*y.shape, *(1,) * np.ndim(a)))
 
         return y
     else:
         # Move the dimensions which are reduced to the back
@@ -229,15 +229,15 @@
 
     mad = median(abs(a - median(a)))/c
 
     Copyright statsmodels:
     Kindly taken from statsmodels package and then modified to work with dataframes as well.
     Reference: https://www.statsmodels.org/dev/_modules/statsmodels/robust/scale.html#mad
     License: https://github.com/statsmodels/statsmodels/blob/master/LICENSE.txt
-    All modifications copyright ING WBAA.
+    All modifications copyright INGA WB.
 
     :param a: array_like Input array.
     :param float c: optional. The normalization constant. Defined as scipy.stats.norm.ppf(3/4.),
         which is approximately .6745.
     :param int axis: optional. The default is 0. Can also be None.
     :param center: callable or float. If a callable is provided, such as the default `np.median` then it
         is expected to be called center(a). The axis argument will be applied
```

### Comparing `popmon-1.4.0/popmon/stitching/__init__.py` & `popmon-1.4.3/popmon/visualization/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -14,10 +14,22 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..stitching.hist_stitcher import HistStitcher, stitch_histograms
+from popmon.visualization.alert_section_generator import AlertSectionGenerator
+from popmon.visualization.histogram_section import HistogramSection
+from popmon.visualization.report_generator import ReportGenerator
+from popmon.visualization.section_generator import SectionGenerator
+from popmon.visualization.traffic_light_section_generator import (
+    TrafficLightSectionGenerator,
+)
 
-__all__ = ["HistStitcher", "stitch_histograms"]
+__all__ = [
+    "SectionGenerator",
+    "HistogramSection",
+    "ReportGenerator",
+    "TrafficLightSectionGenerator",
+    "AlertSectionGenerator",
+]
```

### Comparing `popmon-1.4.0/popmon/stitching/hist_stitcher.py` & `popmon-1.4.3/popmon/stitching/hist_stitcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -17,16 +17,16 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import histogrammar as hg
 import numpy as np
 
-from ..analysis.hist_numpy import assert_similar_hists
-from ..base import Module
+from popmon.analysis.hist_numpy import assert_similar_hists
+from popmon.base import Module
 
 
 class HistStitcher(Module):
     """Module stitches histograms by date"""
 
     _input_keys = ("read_key", "delta_key")
     _output_keys = ("store_key",)
@@ -337,25 +337,26 @@
         # consistency checks on histogram definitions
         if not hasattr(hbasis, "bins"):
             raise ValueError(
                 "basis histogram does not have bins attribute. cannot insert."
             )
         if len(hbasis.bins) > 0:
             hbk0 = list(hbasis.bins.values())[0]
-            assert_similar_hists([hbk0] + hdelta_list)
+            assert_similar_hists([hbk0, *hdelta_list])
         else:
             assert_similar_hists(hdelta_list)
 
         # check consistency of hbasis and time-value type
         if isinstance(time_bin_idx[0], str):
             if not isinstance(hbasis, hg.Categorize):
                 raise TypeError("hbasis does not accept string time-values.")
-        elif isinstance(time_bin_idx[0], (int, np.integer)):
-            if not isinstance(hbasis, hg.SparselyBin):
-                raise TypeError("hbasis does not accept integer time-values.")
+        elif isinstance(time_bin_idx[0], (int, np.integer)) and not isinstance(
+            hbasis, hg.SparselyBin
+        ):
+            raise TypeError("hbasis does not accept integer time-values.")
 
         # stitch all the hdeltas into hbasis
         hsum = hbasis.copy()
 
         for tv, hdelta in zip(time_bin_idx, hdelta_list):
             if tv in hsum.bins:
                 # replace or sum?
@@ -387,15 +388,15 @@
                 "time_bin_idx not set. should be an (ordered) string or integer."
             )
 
         ht = (
             hg.SparselyBin(binWidth=1.0, origin=0.0, quantity=lambda x: x)
             if isinstance(time_bin_idx, int)
             else hg.Categorize(quantity=lambda x: x)
-        )  # noqa
+        )
         ht.bins[time_bin_idx] = hist
         ht.entries = hist.entries
         return ht
 
     def _stitch_by_update(self, mode, hist_list):
         """Get sum of histograms using h1.bins.update(h2.bins), from first to last hist
```

### Comparing `popmon-1.4.0/popmon/test_data/data_generator_hists.json.gz` & `popmon-1.4.3/popmon/test_data/data_generator_hists.json.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/test_data/example_histogram.json` & `popmon-1.4.3/popmon/test_data/example_histogram.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/test_data/flight_delays.csv.gz` & `popmon-1.4.3/popmon/test_data/flight_delays.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/test_data/flight_delays_reference.csv.gz` & `popmon-1.4.3/popmon/test_data/flight_delays_reference.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/test_data/synthetic_histograms.json` & `popmon-1.4.3/popmon/test_data/synthetic_histograms.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/test_data/test.csv.gz` & `popmon-1.4.3/popmon/test_data/test.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/utils.py` & `popmon-1.4.3/popmon/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,40 +13,43 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
+
 import fnmatch
 from textwrap import shorten
-from typing import Callable, List, Optional
+from typing import Callable
 
 import pandas as pd
 from joblib import Parallel, delayed
 
 
 def short_date(date):
     """
     Shorten date string to length of 22
     """
     if isinstance(date, pd.Timestamp):
         # Drop the time of day when midnight or noon
-        if date.hour in [0, 12] and date.minute == 0 and date.second == 0:
-            d = str(date).split(" ")[0]
-        else:
-            d = str(date)
+        d = (
+            str(date).split(" ")[0]
+            if date.hour in [0, 12] and date.minute == 0 and date.second == 0
+            else str(date)
+        )
     else:
         d = str(date)
 
     return shorten(d, width=22, placeholder="")
 
 
 def filter_metrics(
-    metrics, ignore_stat_endswith: List[str], show_stats: Optional[List[str]] = None
+    metrics, ignore_stat_endswith: list[str], show_stats: list[str] | None = None
 ):
     """
     Filter metrics by excluding based on suffix and/or including when matching a pattern
     """
     metrics = [
         m for m in metrics if not any(m.endswith(s) for s in ignore_stat_endswith)
     ]
```

### Comparing `popmon-1.4.0/popmon/visualization/alert_section_generator.py` & `popmon-1.4.3/popmon/visualization/alert_section_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,23 +13,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-
-from typing import Optional
+from __future__ import annotations
 
 import pandas as pd
 from tqdm import tqdm
 
-from ..base import Module
-from ..config import Report
-from ..utils import filter_metrics, short_date
+from popmon.base import Module
+from popmon.config import Report
+from popmon.utils import filter_metrics, short_date
+
 from .traffic_light_section_generator import _plot_metrics
 
 
 class AlertSectionGenerator(Module):
     """This module takes the time-series data of already computed statistics, plots the data and
     combines all the plots into a list which is stored together with the section name in a dictionary
     which later will be used for the report generation.
@@ -44,15 +44,15 @@
         store_key,
         settings: Report,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
         prefix="traffic_light_",
-        suffices=["_red_high", "_yellow_high", "_yellow_low", "_red_low"],
+        suffices=None,
         ignore_stat_endswith=None,
     ):
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
@@ -68,15 +68,20 @@
         self.store_key = store_key
         self.dynamic_bounds = dynamic_bounds
         self.static_bounds = static_bounds
 
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.prefix = prefix
-        self.suffices = suffices
+        self.suffices = suffices or [
+            "_red_high",
+            "_yellow_high",
+            "_yellow_low",
+            "_red_low",
+        ]
         self.ignore_stat_endswith = ignore_stat_endswith or []
 
         self.last_n = settings.last_n
         self.skip_first_n = settings.skip_first_n
         self.skip_last_n = settings.skip_last_n
         self.show_stats = settings.show_stats if not settings.extended_report else None
 
@@ -87,17 +92,17 @@
 
     def get_description(self):
         return self.section_name
 
     def transform(
         self,
         data_obj: dict,
-        static_bounds: Optional[dict] = None,
-        dynamic_bounds: Optional[dict] = None,
-        sections: Optional[list] = None,
+        static_bounds: dict | None = None,
+        dynamic_bounds: dict | None = None,
+        sections: list | None = None,
     ):
         assert isinstance(data_obj, dict)
         if static_bounds is None:
             static_bounds = {}
         assert isinstance(static_bounds, dict)
         if dynamic_bounds is None:
             dynamic_bounds = {}
@@ -114,17 +119,16 @@
         for feature in tqdm(features, ncols=100):
             df = data_obj.get(feature, pd.DataFrame())
             fdbounds = dynamic_bounds.get(feature, pd.DataFrame(index=df.index))
 
             assert all(df.index == fdbounds.index)
 
             # prepare date labels
-            df.drop(
+            df = df.drop(
                 columns=["histogram", "reference_histogram"],
-                inplace=True,
                 errors="ignore",
             )
             dates = [short_date(date) for date in df.index.tolist()]
 
             metrics = filter_metrics(
                 df.columns, self.ignore_stat_endswith, self.show_stats
             )
```

### Comparing `popmon-1.4.0/popmon/visualization/histogram_section.py` & `popmon-1.4.3/popmon/visualization/histogram_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,32 +12,30 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-from typing import Optional
+from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 from histogrammar.util import get_hist_props
 from tqdm import tqdm
 
-from ..analysis.hist_numpy import (
+from popmon.analysis.hist_numpy import (
     assert_similar_hists,
     get_consistent_numpy_1dhists,
     get_consistent_numpy_entries,
 )
-from ..base import Module
-from ..config import HistogramSectionModel
-from ..utils import parallel, short_date
-from ..visualization.utils import (
+from popmon.base import Module
+from popmon.config import HistogramSectionModel
+from popmon.utils import parallel, short_date
+from popmon.visualization.utils import (
     histogram_basic_checks,
     plot_heatmap,
     plot_histogram_overlay,
 )
 
 
 class HistogramSection(Module):
@@ -86,15 +84,15 @@
         self.top_n = settings.top_n
         self.n_choices = settings.inspector_histogram_choices
         self.cmap = settings.cmap
 
     def get_description(self):
         return self.section_name
 
-    def transform(self, data_obj: dict, sections: Optional[list] = None):
+    def transform(self, data_obj: dict, sections: list | None = None):
         if sections is None:
             sections = []
 
         features = self.get_features(list(data_obj.keys()))
         features_w_metrics = []
 
         # Treat these as static
@@ -187,17 +185,16 @@
                 histogram = [histogram]
             else:
                 histogram = []
 
             # filter out potential empty heatmap plots, then prepend them to the sorted histograms
             hplots = []
             for h in heatmaps:
-                if isinstance(h, dict):
-                    if len(h["plot"]):
-                        hplots.append(h)
+                if isinstance(h, dict) and len(h["plot"]):
+                    hplots.append(h)
 
             if len(hplots) > 0:
                 plot_type_layouts["heatmap"] = hplots[0]["layout"]
 
             plots = hplots + histogram
 
             features_w_metrics.append(
@@ -270,16 +267,16 @@
         # normalize histograms for plotting (comparison!) in case there is more than one.
         if len(hc_list) >= 2:
             entries_list = [
                 el / hc.entries if hc.entries > 0 else el
                 for el, hc in zip(entries_list, hc_list)
             ]
         # if categorical
+        # get top_n categories for histogram
         if not is_num:
-            # get top_n categories for histogram
             if len(bins) > top_n:
                 entries_list = np.stack(entries_list, axis=1)
                 entries_list, bins = get_top_categories(entries_list, bins, top_n)
                 entries_list = np.stack(entries_list, axis=1)
                 entries_list = np.reshape(entries_list.ravel(), (-1, len(bins)))
 
         hists = [(el, bins) for el in entries_list]
@@ -426,7 +423,8 @@
     return top_rows, bins
 
 
 def hist_lookup(plot, hist_name):
     for pl in plot:
         if pl["name"] == hist_name:
             return pl
+    return None
```

### Comparing `popmon-1.4.0/popmon/visualization/overview_section.py` & `popmon-1.4.3/popmon/visualization/overview_section.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,28 +13,28 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 from datetime import datetime
-from typing import Optional
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
-from ..base import Module
-from ..config import Report
-from ..resources import templates_env
-from ..utils import filter_metrics
-from ..version import version as __version__
-from ..visualization.utils import _prune, get_reproduction_table, get_summary_table
+from popmon.base import Module
+from popmon.config import Report
+from popmon.resources import templates_env
+from popmon.utils import filter_metrics
+from popmon.version import version as __version__
+from popmon.visualization.utils import _prune, get_reproduction_table, get_summary_table
 
 
 class OverviewSectionGenerator(Module):
     """This module takes the time-series data of already computed statistics, plots the data and
     combines all the plots into a list which is stored together with the section name in a dictionary
     which later will be used for the report generation.
     """
@@ -51,15 +51,15 @@
         time_axis,
         bin_specs,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
         prefix="traffic_light_",
-        suffices=["_red_high", "_yellow_high", "_yellow_low", "_red_low"],
+        suffices=None,
         ignore_stat_endswith=None,
     ):
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
@@ -77,15 +77,20 @@
         self.end_time = "end_time"
         self.dynamic_bounds = dynamic_bounds
         self.static_bounds = static_bounds
 
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.prefix = prefix
-        self.suffices = suffices
+        self.suffices = suffices or [
+            "_red_high",
+            "_yellow_high",
+            "_yellow_low",
+            "_red_low",
+        ]
         self.ignore_stat_endswith = ignore_stat_endswith or []
         self.reference_type = reference_type
         self.time_axis = time_axis
         self.bin_specs = bin_specs
 
         self.last_n = settings.last_n
         self.skip_first_n = settings.skip_first_n
@@ -96,18 +101,18 @@
 
     def get_description(self):
         return self.section_name
 
     def transform(
         self,
         data_obj: dict,
-        dynamic_bounds: Optional[dict] = None,
-        sections: Optional[list] = None,
-        start_time: Optional[datetime] = None,
-        end_time: Optional[datetime] = None,
+        dynamic_bounds: dict | None = None,
+        sections: list | None = None,
+        start_time: datetime | None = None,
+        end_time: datetime | None = None,
     ):
         assert isinstance(data_obj, dict)
         if dynamic_bounds is None:
             dynamic_bounds = {}
         assert isinstance(dynamic_bounds, dict)
         if sections is None:
             sections = []
@@ -126,17 +131,16 @@
             offset = df.index.min()
             max_timestamp = df.index.max()
 
             fdbounds = dynamic_bounds.get(feature, pd.DataFrame(index=df.index))
             assert all(df.index == fdbounds.index)
 
             # prepare date labels
-            df.drop(
+            df = df.drop(
                 columns=["histogram", "reference_histogram"],
-                inplace=True,
                 errors="ignore",
             )
 
             metrics = filter_metrics(
                 df.columns, self.ignore_stat_endswith, self.show_stats
             )
 
@@ -148,20 +152,20 @@
                 self.skip_last_n,
             )
 
         # Dataset summary table and Analysis Details  table
         tables = []
         bin_width = (
             self.bin_specs[self.time_axis]["bin_width"]
-            if self.time_axis in self.bin_specs.keys()
+            if self.time_axis in self.bin_specs
             else 0
         )
 
         if (
-            self.time_axis in self.bin_specs.keys()
+            self.time_axis in self.bin_specs
             and self.bin_specs[self.time_axis]["bin_offset"] > 0
         ):
             offset = datetime.utcfromtimestamp(
                 self.bin_specs[self.time_axis]["bin_offset"] // 1e9
             )
         tables.append(
             get_summary_table(
@@ -195,26 +199,25 @@
         return sections
 
 
 def _plot_metrics(
     values,
 ):
     # sort features by n_red, n_yellow, n_green
-    values = {
-        k: v
-        for k, v in sorted(
+    values = dict(
+        sorted(
             values.items(),
             key=lambda x: (
                 x[1][2] / x[1]["total"] if x[1]["total"] > 0 else 0,
                 x[1][1] / x[1]["total"] if x[1]["total"] > 0 else 0,
                 x[1][0] / x[1]["total"] if x[1]["total"] > 0 else 0,
             ),
             reverse=True,
         )
-    }
+    )
 
     plot = templates_env(
         "aggregated-overview.html",
         values=values,
     )
 
     return {
```

### Comparing `popmon-1.4.0/popmon/visualization/report_generator.py` & `popmon-1.4.3/popmon/visualization/report_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -16,18 +16,18 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import htmlmin
 
-from ..base import Module
-from ..config import Report
-from ..resources import templates_env
-from ..version import version
+from popmon.base import Module
+from popmon.config import Report
+from popmon.resources import templates_env
+from popmon.version import version
 
 
 class ReportGenerator(Module):
     """This module takes already prepared section data, renders HTML section template with the data and
     glues sections together into one compressed report which is created based on the provided template.
     """
```

### Comparing `popmon-1.4.0/popmon/visualization/section_generator.py` & `popmon-1.4.3/popmon/visualization/section_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,28 +12,28 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+from __future__ import annotations
+
 from collections import defaultdict
-from typing import Optional
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from popmon.analysis.comparison import Comparisons
 from popmon.analysis.profiling import Profiles
-
-from ..base import Module
-from ..config import Report
-from ..utils import filter_metrics, parallel, short_date
-from ..visualization.utils import _prune, plot_bars
+from popmon.base import Module
+from popmon.config import Report
+from popmon.utils import filter_metrics, parallel, short_date
+from popmon.visualization.utils import _prune, plot_bars
 
 profiles = Profiles.get_descriptions()
 
 comparisons = Comparisons.get_descriptions()
 
 
 group_titles = {
@@ -95,15 +95,15 @@
         section_name,
         settings: Report,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
         prefix="traffic_light_",
-        suffices=["_red_high", "_yellow_high", "_yellow_low", "_red_low"],
+        suffices=None,
         ignore_stat_endswith=None,
         description="",
     ):
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
@@ -126,30 +126,35 @@
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.section_name = section_name
         self.last_n = settings.last_n
         self.skip_first_n = settings.skip_first_n
         self.skip_last_n = settings.skip_last_n
         self.prefix = prefix
-        self.suffices = suffices
+        self.suffices = suffices or [
+            "_red_high",
+            "_yellow_high",
+            "_yellow_low",
+            "_red_low",
+        ]
         self.ignore_stat_endswith = ignore_stat_endswith or []
         self.description = description
         self.show_stats = settings.show_stats if not settings.extended_report else None
         self.primary_color = settings.primary_color
         self.tl_colors = settings.tl_colors
 
     def get_description(self):
         return self.section_name
 
     def transform(
         self,
         data_obj: dict,
-        static_bounds: Optional[dict] = None,
-        dynamic_bounds: Optional[dict] = None,
-        sections: Optional[list] = None,
+        static_bounds: dict | None = None,
+        dynamic_bounds: dict | None = None,
+        sections: list | None = None,
     ):
         if static_bounds is None:
             static_bounds = {}
         if dynamic_bounds is None:
             dynamic_bounds = {}
         if sections is None:
             sections = []
@@ -162,17 +167,16 @@
         for feature in tqdm(features, ncols=100):
             df = data_obj.get(feature, pd.DataFrame())
             fdbounds = dynamic_bounds.get(feature, pd.DataFrame(index=df.index))
 
             assert all(df.index == fdbounds.index)
 
             # prepare date labels
-            df.drop(
+            df = df.drop(
                 columns=["histogram", "reference_histogram"],
-                inplace=True,
                 errors="ignore",
             )
             dates = np.array([short_date(date) for date in df.index.tolist()])
 
             metrics = filter_metrics(
                 df.columns, self.ignore_stat_endswith, self.show_stats
             )
@@ -300,14 +304,14 @@
 
     return {
         "name": metric,
         "type": "barplot",
         "description": get_stat_description(metric),
         "plot": plot["data"],
         "shapes": plot["layout"]["shapes"] if "shapes" in plot["layout"] else "",
-        "yaxis_range": [
-            "null" if r is None else r for r in plot["layout"]["yaxis"]["range"]
-        ]
-        if "range" in plot["layout"]["yaxis"]
-        else "",
+        "yaxis_range": (
+            ["null" if r is None else r for r in plot["layout"]["yaxis"]["range"]]
+            if "range" in plot["layout"]["yaxis"]
+            else ""
+        ),
         "layout": plot["layout"],
     }
```

### Comparing `popmon-1.4.0/popmon/visualization/templates/aggregated-overview.html` & `popmon-1.4.3/popmon/visualization/templates/aggregated-overview.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/css/bootstrap.min.css` & `popmon-1.4.3/popmon/visualization/templates/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/css/custom-style.css` & `popmon-1.4.3/popmon/visualization/templates/assets/css/custom-style.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js` & `popmon-1.4.3/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/js/custom-script.js` & `popmon-1.4.3/popmon/visualization/templates/assets/js/custom-script.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/js/jquery.easing.min.js` & `popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.easing.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/js/jquery.min.js` & `popmon-1.4.3/popmon/visualization/templates/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/js/plotly.js` & `popmon-1.4.3/popmon/visualization/templates/assets/js/plotly.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/assets/js/scrolling-nav.js` & `popmon-1.4.3/popmon/visualization/templates/assets/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/card.html` & `popmon-1.4.3/popmon/visualization/templates/card.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/core.html` & `popmon-1.4.3/popmon/visualization/templates/core.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/footer.html` & `popmon-1.4.3/popmon/visualization/templates/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <footer class="py-5 bg-dark">
     <div class="container">
-        <p class="m-0 text-center text-white">Copyright &copy; ING WBAA 2022</p>
+        <p class="m-0 text-center text-white">Copyright &copy; INGA WB 2023</p>
     </div>
 </footer>
 
 {%- if online_report -%}
     <script src="https://cdn.plot.ly/plotly-2.12.1.min.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/jquery@3.4.1/dist/jquery.min.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/js/bootstrap.bundle.min.js"></script>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
-Copyright © ING WBAA 2022
+Copyright © INGA WB 2023
  {%- if online_report -%}
  {%- endif -%}
```

### Comparing `popmon-1.4.0/popmon/visualization/templates/header.html` & `popmon-1.4.3/popmon/visualization/templates/header.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/modal-popup.html` & `popmon-1.4.3/popmon/visualization/templates/modal-popup.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/section.html` & `popmon-1.4.3/popmon/visualization/templates/section.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/templates/table.html` & `popmon-1.4.3/popmon/visualization/templates/table.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.0/popmon/visualization/traffic_light_section_generator.py` & `popmon-1.4.3/popmon/visualization/traffic_light_section_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -12,26 +12,24 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-from typing import Optional
+from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
-from ..base import Module
-from ..config import Report
-from ..utils import filter_metrics, short_date
-from ..visualization.utils import (
+from popmon.base import Module
+from popmon.config import Report
+from popmon.utils import filter_metrics, short_date
+from popmon.visualization.utils import (
     _prune,
     plot_traffic_lights_alerts_aggregate,
     plot_traffic_lights_overview,
 )
 
 
 class TrafficLightSectionGenerator(Module):
@@ -49,15 +47,15 @@
         store_key,
         settings: Report,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
         prefix="traffic_light_",
-        suffices=["_red_high", "_yellow_high", "_yellow_low", "_red_low"],
+        suffices=None,
         ignore_stat_endswith=None,
     ):
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
@@ -76,30 +74,35 @@
 
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.last_n = settings.last_n
         self.skip_first_n = settings.skip_first_n
         self.skip_last_n = settings.skip_last_n
         self.prefix = prefix
-        self.suffices = suffices
+        self.suffices = suffices or [
+            "_red_high",
+            "_yellow_high",
+            "_yellow_low",
+            "_red_low",
+        ]
         self.ignore_stat_endswith = ignore_stat_endswith or []
         self.show_stats = settings.show_stats if not settings.extended_report else None
 
         self.section_name = settings.section.traffic_lights.name
         self.description = settings.section.traffic_lights.description
         self.tl_colors = settings.tl_colors
 
     def get_description(self):
         return self.section_name
 
     def transform(
         self,
         data_obj: dict,
-        dynamic_bounds: Optional[dict] = None,
-        sections: Optional[list] = None,
+        dynamic_bounds: dict | None = None,
+        sections: list | None = None,
     ):
         assert isinstance(data_obj, dict)
         if dynamic_bounds is None:
             dynamic_bounds = {}
         assert isinstance(dynamic_bounds, dict)
         if sections is None:
             sections = []
@@ -113,17 +116,16 @@
         for feature in tqdm(features, ncols=100):
             df = data_obj.get(feature, pd.DataFrame())
             fdbounds = dynamic_bounds.get(feature, pd.DataFrame(index=df.index))
 
             assert all(df.index == fdbounds.index)
 
             # prepare date labels
-            df.drop(
+            df = df.drop(
                 columns=["histogram", "reference_histogram"],
-                inplace=True,
                 errors="ignore",
             )
             dates = [short_date(date) for date in df.index.tolist()]
 
             metrics = sorted(
                 filter_metrics(df.columns, self.ignore_stat_endswith, self.show_stats)
             )
```

### Comparing `popmon-1.4.0/popmon/visualization/utils.py` & `popmon-1.4.3/popmon/visualization/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 ING Wholesale Banking Advanced Analytics
+# Copyright (c) 2023 ING Analytics Wholesale Banking
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy of
 # this software and associated documentation files (the "Software"), to deal in
 # the Software without restriction, including without limitation the rights to
 # use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 # the Software, and to permit persons to whom the Software is furnished to do so,
 # subject to the following conditions:
@@ -13,22 +13,22 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 import datetime
 import json
 import logging
 import math
 import warnings
 from collections import defaultdict
-from typing import Dict, List, Union
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 
 from popmon.resources import templates_env
@@ -43,15 +43,15 @@
     """Get x-tick."""
     lab = str(lab)
     if len(lab) > top:
         lab = lab[: top - 3] + "..."
     return lab
 
 
-def convert_time_delta(td: Union[datetime.timedelta, float, int]) -> str:
+def convert_time_delta(td: datetime.timedelta | float | int) -> str:
     """
     It converts a time delta in nanoseconds to a string
 
     :param td: Timedelta or the time difference in nanoseconds
     :rtype: str
     """
     if not isinstance(td, datetime.timedelta):
@@ -202,19 +202,19 @@
         "plot": plot.get("data", ""),
         "layout": plot.get("layout", ""),
     }
 
 
 def plot_bars(
     data,
-    labels: List[str],
+    labels: list[str],
     bounds: tuple,
     ylim: bool,
     primary_color: str,
-    tl_colors: Dict[str, str],
+    tl_colors: dict[str, str],
     metric: str,
 ) -> str:
     """Plotting histogram data.
 
     :param numpy.ndarray data: bin values of a histogram
     :param labels: common bin labels for all histograms. default is None.
     :param bounds: traffic light bounds (y-coordinates). default is None.
@@ -319,15 +319,15 @@
     except Exception:
         logger.debug("unable to plot boundaries")
 
     plot = json.loads(fig.to_json())
     return plot
 
 
-def plot_traffic_lights_overview(feature, data, metrics: List[str], labels: List[str]):
+def plot_traffic_lights_overview(feature, data, metrics: list[str], labels: list[str]):
     colors = defaultdict(dict)
     color_map = ["g", "y", "r"]
     for c1, metric in enumerate(metrics):
         for c2, label in enumerate(labels):
             colors[metric][label] = [color_map[data[c1][c2]]]
 
     return templates_env(
@@ -342,15 +342,15 @@
 
 def hex_to_rgb(h):
     """Takes a hex rgb string and returns an RGB tuple."""
     return tuple(int(h[i : i + 2], 16) for i in (1, 3, 5))
 
 
 def plot_traffic_lights_alerts_aggregate(
-    feature, data, metrics: List[str], labels: List[str], tl_colors: Dict[str, str]
+    feature, data, metrics: list[str], labels: list[str], tl_colors: dict[str, str]
 ):
     assert data.shape[0] == 3
 
     # Reorder metrics if needed
     pos_green = metrics.index("n_green")
     pos_yellow = metrics.index("n_yellow")
     pos_red = metrics.index("n_red")
@@ -387,26 +387,25 @@
         labels=labels,
         data=colors,
         links=False,
     )
 
 
 # basic checks for histograms
-def histogram_basic_checks(plots={}):
-    if len(plots) == 0:
+def histogram_basic_checks(plots=None):
+    if plots is None or len(plots) == 0:
         return
 
     for plot in plots:
         if len(plot["hist_names"]) == 0:
             plot["hist_names"] = [f"hist{i}" for i in range(len(plot["hists"]))]
-        if plot["hist_names"]:
-            if len(plot["hists"]) != len(plot["hist_names"]):
-                raise ValueError("length of hist and hist_names are different")
+        if plot["hist_names"] and len(plot["hists"]) != len(plot["hist_names"]):
+            raise ValueError("length of hist and hist_names are different")
 
-        for i, hist in enumerate(plot["hists"]):
+        for hist in plot["hists"]:
             try:
                 hist_values, hist_bins = hist
             except BaseException as e:
                 raise ValueError(
                     "Cannot extract binning and values from input histogram"
                 ) from e
 
@@ -433,57 +432,58 @@
                 values = hist_values
                 assert len(labels) == len(
                     values
                 ), f'labels and values have different array lengths: {len(labels):d} vs {len(values):d}. {plot["feature"]}'
 
 
 def plot_histogram_overlay(
-    plots=[],
+    plots=None,
     is_num=True,
     is_ts=False,
     is_static_reference=True,
     top=20,
     n_choices=2,
 ):
     """Create and plot (overlapping/grouped) histogram(s) of column values.
 
     Copyright Eskapade:
     Kindly taken from Eskapade package and then modified. Reference link:
     https://github.com/KaveIO/Eskapade/blob/master/python/eskapade/visualization/vis_utils.py#L397
     License: https://github.com/KaveIO/Eskapade-Core/blob/master/LICENSE
-    Modifications copyright ING WBAA.
+    Modifications copyright INGA WB.
 
     :param list plots: list of dicts containing histograms for all timestamps
         :param bool is_num: True if observable to plot is numeric. default is True.
         :param bool is_ts: True if observable to plot is a timestamp. default is False.
     :param bool is_static_reference: True if the reference is static. default is True
     :param int top: only print the top 20 characters of x-labels and y-labels. default is 20.
     :param int n_choices: number of plots to compare at once
     :return: JSON encoded plot image
     :rtype: str
     """
 
+    if plots is None:
+        plots = []
     fig = go.Figure()
 
     alpha = 0.4
 
-    # check number of plots
+    # check the number of plots
     if len(plots) < 2:
         warnings.warn("insufficient plots for histogram inspection")
-        return
+        return None
 
     base_plot = plots[0]
 
     # basic attribute check: time stamps treated as numeric.
     if is_ts:
         is_num = True
 
     # plot numeric and time stamps
     if is_num:
-
         # plot histogram
         for index in range(n_choices):
             bin_edges = plots[index]["hists"][0][1]
             bin_values = plots[index]["hists"][0][0]
             fig.add_trace(
                 go.Bar(
                     x=bin_edges[1:],
@@ -509,31 +509,34 @@
             )
             fig.add_trace(
                 go.Bar(
                     x=bin_edges[1:],
                     y=bin_values,
                     opacity=alpha,
                     showlegend=True,
-                    name="no_ref"
-                    if len(plots[index]["hists"]) < 2
-                    else "Reference"
-                    if is_static_reference
-                    else (plots[index]["date"] + "-")
-                    + plots[index]["hist_names"][1].split("_")[-1],
+                    name=(
+                        "no_ref"
+                        if len(plots[index]["hists"]) < 2
+                        else (
+                            "Reference"
+                            if is_static_reference
+                            else (plots[index]["date"] + "-")
+                            + plots[index]["hist_names"][1].split("_")[-1]
+                        )
+                    ),
                     meta=index + 2,
                 )
             )
 
         # set x-axis properties
         xlim = [min(bin_edges), max(bin_edges)]
         fig.update_xaxes(range=xlim)
 
     # plot categories
     else:
-
         # plot histogram for first 'n_choices' timestamps
         for index in range(n_choices):
             labels = plots[index]["hists"][0][1]
             values = plots[index]["hists"][0][0]
             fig.add_trace(
                 go.Bar(
                     x=[xtick(lab, top) for lab in labels],
@@ -559,21 +562,25 @@
             )
             fig.add_trace(
                 go.Bar(
                     x=[xtick(lab, top) for lab in labels],
                     y=values,
                     opacity=alpha,
                     showlegend=True,
-                    name="no_ref"
-                    if len(plots[index]["hists"]) < 2
-                    else "Reference"
-                    if is_static_reference
-                    else plots[index]["date"]
-                    + " "
-                    + plots[index]["hist_names"][1].split("_")[-1],
+                    name=(
+                        "no_ref"
+                        if len(plots[index]["hists"]) < 2
+                        else (
+                            "Reference"
+                            if is_static_reference
+                            else plots[index]["date"]
+                            + " "
+                            + plots[index]["hist_names"][1].split("_")[-1]
+                        )
+                    ),
                     meta=index + n_choices,
                 )
             )
 
     # set common histogram layout properties
     y_label = (
         str(base_plot["y_label"]) if base_plot["y_label"] is not None else "Bin count"
@@ -615,27 +622,33 @@
                         {
                             "label": f'{plot["date"]}',
                             "method": "restyle",
                             "args": [
                                 {
                                     "y": [
                                         plot["hists"][0][0],
-                                        [0 for _ in range(len(plot["hists"][0][0]))]
-                                        if len(plot["hists"]) < 2
-                                        else plot["hists"][1][0],
+                                        (
+                                            [0 for _ in range(len(plot["hists"][0][0]))]
+                                            if len(plot["hists"]) < 2
+                                            else plot["hists"][1][0]
+                                        ),
                                     ],
                                     "name": [
                                         plot["date"],
-                                        "no_ref"
-                                        if len(plot["hist_names"]) < 2
-                                        else "Reference"
-                                        if is_static_reference
-                                        else plots[index]["date"]
-                                        + " "
-                                        + plot["hist_names"][1].split("_")[-1],
+                                        (
+                                            "no_ref"
+                                            if len(plot["hist_names"]) < 2
+                                            else (
+                                                "Reference"
+                                                if is_static_reference
+                                                else plots[index]["date"]
+                                                + " "
+                                                + plot["hist_names"][1].split("_")[-1]
+                                            )
+                                        ),
                                     ],
                                 },
                                 [b, b + 2],
                             ],
                         }
                         for plot in plots
                     ],
@@ -701,32 +714,31 @@
 ):
     """Create and plot heatmap of column values.
 
     Copyright Eskapade:
     Kindly taken from Eskapade package and then modified. Reference link:
     https://github.com/KaveIO/Eskapade/blob/master/python/eskapade/visualization/vis_utils.py#L397
     License: https://github.com/KaveIO/Eskapade-Core/blob/master/LICENSE
-    Modifications copyright ING WBAA.
+    Modifications copyright INGA WB.
 
     :param list hist_values: values of heatmap in a 2d numpy array =
     :param list hist_bins: bin labels/edges on y-axis
     :param list date: dates for x/time axis of heatmap
     :param str x_label: Label for heatmap x-axis
     :param list hist_names: list of histogram names. default is [].
     :param str y_label: Label for histogram y-axis. default is None.
     :param bool is_num: True if observable to plot is numeric. default is True.
     :param bool is_ts: True if observable to plot is a timestamp. default is False.
     :param int top: only print the top 20 characters of x-labels and y-labels. default is 20.
     :param cmap: the colormap for heatmap. default is ylorrd.
     :return: base64 encoded plot image
     :rtype: str
     """
-    if hist_name:
-        if len(hist_name) == 0:
-            raise ValueError("length of heatmap names is zero")
+    if hist_name and len(hist_name) == 0:
+        raise ValueError("length of heatmap names is zero")
 
     assert hist_values is not None and len(
         hist_values
     ), "Heatmap bin values have not been set."
     assert hist_bins is not None and len(hist_bins), "Heatmap binning has not been set."
 
     # basic attribute check: time stamps treated as numeric.
```

### Comparing `popmon-1.4.0/popmon.egg-info/PKG-INFO` & `popmon-1.4.3/popmon.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.0
+Version: 1.4.3
 Summary: Monitor the stability of a pandas or spark dataset
-Home-page: https://github.com/ing-bank/popmon
-Author: ING Wholesale Banking Advanced Analytics
-License: MIT
-Keywords: pandas spark data-science data-analysis monitoring statistics python jupyter ipython
-Platform: UNKNOWN
+Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
+License: Copyright 2023 ING Analytics Wholesale Banking
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+        documentation files (the "Software"), to deal in the Software without restriction, including without limitation
+        the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
+        to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions
+        of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+        TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+        THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+        CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+        DEALINGS IN THE SOFTWARE.
+        
+Project-URL: repository, https://github.com/ing-bank/popmon
+Keywords: pandas,spark,data-science,data-analysis,monitoring,statistics,python,jupyter,ipython
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: diptest
 License-File: LICENSE
 License-File: NOTICE
 
 ===========================
 Population Shift Monitoring
 ===========================
 
-|build| |docs| |release| |release_date| |downloads|
+|build| |docs| |release| |release_date| |downloads| |ruff|
 
 |logo|
 
 `popmon` is a package that allows one to check the stability of a dataset.
 `popmon` works with both **pandas** and **spark datasets**.
 
 `popmon` creates histograms of features binned in time-slices,
@@ -205,15 +220,15 @@
 +----------------+---------------+
 | Grafana        | Kibana        |
 +----------------+---------------+
 
 Resources on how to integrate popmon are available in the `examples directory <https://github.com/ing-bank/popmon/tree/master/examples/integrations>`_.
 Contributions of additional or improved integrations are welcome!
 
-.. |grafana_logo| image:: https://upload.wikimedia.org/wikipedia/en/a/a1/Grafana_logo.svg
+.. |grafana_logo| image:: https://upload.wikimedia.org/wikipedia/commons/a/a1/Grafana_logo.svg
     :alt: Grafana logo
     :height: 120
     :target: https://github.com/grafana/grafana
 
 .. |kibana_logo| image:: https://miro.medium.com/max/1400/1*HW_x9ZvIbUkyaqHstsB1ig.png
     :alt: Kibana logo
     :height: 120
@@ -262,34 +277,37 @@
 
 Articles
 --------
 
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | Title                                                                                                                                                                                             | Date             | Author                                      |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
+|`POPMON v1.0.0: The Dataset-Shift Pokémon <https://medium.com/wbaa/popmon-v1-0-0-the-dataset-shift-pok%C3%A9mon-7dea9cb49a71>`_                                                                    | Aug 3, 2022      | Pradyot Patil                               |
++---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`Monitoring Model Drift with Python <https://medium.com/broadhorizon-cmotions/monitoring-model-drift-with-python-b9e15ca16b18>`_                                                                   | April 16, 2022   | Jeanine Schoonemann                         |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`The Statistics Underlying the Popmon Hood <https://www.theanalyticslab.nl/the-statistics-underlying-the-popmon-hood/>`_                                                                           | April 15, 2022   | Jurriaan Nagelkerke and Jeanine Schoonemann |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 |`popmon: code breakfast session <https://simonbrugman.nl/2021/11/09/popmon-code-breakfast.html>`_                                                                                                  | November 9, 2022 | Simon Brugman                               |       
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | `Population Shift Analysis: Monitoring Data Quality with Popmon <https://www.codemotion.com/magazine/dev-hub/big-data-analyst/popmon-data-quality-monitoring/>`_                                  | May 21, 2021     | Vito Gentile                                |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 | `Popmon Open Source Package — Population Shift Monitoring Made Easy <https://medium.com/wbaa/population-monitoring-open-source-1ce3139d8c3a>`_                                                    | May 20, 2020     | Nicole Mpozika                              |
 +---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------------------------+
 
+
 Software
 --------
 
 - `Kedro-popmon <https://github.com/stephanecollot/kedro-popmon>`_ is a plugin to integrate popmon reporting with kedro. This plugin allows you to automate the process of popmon feature and output stability monitoring. Package created by `Marian Dabrowski <https://www.linkedin.com/in/marian-dabrowski/>`_ and `Stephane Collot <https://github.com/stephanecollot/>`_.
 
 Project contributors
 ====================
 
-This package was authored by ING Wholesale Banking Advanced Analytics.
+This package was authored by ING Analytics Wholesale Banking (INGA WB).
 Special thanks to the following people who have contributed to the development of this package: `Ahmet Erdem <https://github.com/aerdem4>`_, `Fabian Jansen <https://github.com/faab5>`_, `Nanne Aben <https://github.com/nanne-aben>`_, Mathieu Grimal.
 
 
 Citing popmon
 =============
 If ``popmon`` has been relevant in your work, and you would like to acknowledge the project in your publication, we suggest citing the following paper:
 
@@ -311,32 +329,35 @@
 
 
 Contact and support
 ===================
 
 * Issues & Ideas & Support: https://github.com/ing-bank/popmon/issues
 
-Please note that ING WBAA provides support only on a best-effort basis.
+Please note that INGA WB provides support only on a best-effort basis.
 
 License
 =======
-Copyright ING WBAA. `popmon` is completely free, open-source and licensed under the `MIT license <https://en.wikipedia.org/wiki/MIT_License>`_.
+Copyright INGA WB. `popmon` is completely free, open-source and licensed under the `MIT license <https://en.wikipedia.org/wiki/MIT_License>`_.
 
 .. |logo| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/popmon-logo.png
     :alt: POPMON logo
     :target: https://github.com/ing-bank/popmon
 .. |example| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/report_overview.png
     :alt: Traffic Light Overview
 .. |histograms| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/histogram_inspector.png
     :alt: Histogram inspector
 .. |pipeline| image:: https://raw.githubusercontent.com/ing-bank/popmon/master/docs/source/assets/pipeline.png
     :alt: Pipeline Visualization
     :target: https://github.com/ing-bank/popmon/files/7417124/pipeline_amazingpipeline_subgraphs_unversioned.pdf
 .. |build| image:: https://github.com/ing-bank/popmon/workflows/build/badge.svg
     :alt: Build status
+.. |ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+    :alt: Ruff
+    :target: https://github.com/charliermarsh/ruff
 .. |docs| image:: https://readthedocs.org/projects/popmon/badge/?version=latest
     :alt: Package docs status
     :target: https://popmon.readthedocs.io
 .. |release| image:: https://img.shields.io/github/v/release/ing-bank/popmon
     :alt: Latest GitHub release
     :target: https://github.com/ing-bank/popmon/releases
 .. |release_date| image:: https://img.shields.io/github/release-date/ing-bank/popmon
@@ -357,9 +378,7 @@
     :target: https://colab.research.google.com/github/ing-bank/popmon/blob/master/popmon/notebooks/popmon_tutorial_reports.ipynb
 .. |downloads| image:: https://pepy.tech/badge/popmon
     :alt: PyPi downloads
     :target: https://pepy.tech/project/popmon
 
 .. _profiles: https://popmon.readthedocs.io/en/latest/profiles.html
 .. _comparisons: https://popmon.readthedocs.io/en/latest/comparisons.html
-
-
```

### Comparing `popmon-1.4.0/popmon.egg-info/SOURCES.txt` & `popmon-1.4.3/popmon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 NOTICE
 README.rst
 extras.json
 pyproject.toml
 requirements.txt
-setup.py
 popmon/__init__.py
 popmon/config.py
 popmon/resources.py
 popmon/utils.py
 popmon/version.py
 popmon.egg-info/PKG-INFO
 popmon.egg-info/SOURCES.txt
@@ -38,15 +37,14 @@
 popmon/base/registry.py
 popmon/decorators/__init__.py
 popmon/decorators/pandas.py
 popmon/decorators/spark.py
 popmon/extensions/__init__.py
 popmon/extensions/extension.py
 popmon/extensions/profile_diptest.py
-popmon/extensions/utils.py
 popmon/hist/__init__.py
 popmon/hist/hist_splitter.py
 popmon/hist/hist_utils.py
 popmon/hist/filling/__init__.py
 popmon/io/__init__.py
 popmon/io/file_reader.py
 popmon/io/file_writer.py
```

