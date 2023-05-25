# Comparing `tmp/cellpy-1.0.0a8.tar.gz` & `tmp/cellpy-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.0a8.tar", last modified: Sun May 14 17:53:18 2023, max compression
+gzip compressed data, was "cellpy-1.0.0a9.tar", last modified: Thu May 25 17:56:35 2023, max compression
```

## Comparing `cellpy-1.0.0a8.tar` & `cellpy-1.0.0a9.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.397303 cellpy-1.0.0a8/
--rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     6518 2023-05-14 17:53:18.397303 cellpy-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.117245 cellpy-1.0.0a8/cellpy/
--rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2023-05-14 17:52:59.000000 cellpy-1.0.0a8/cellpy/_version.py
--rw-rw-rw-   0        0        0    53597 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.129456 cellpy-1.0.0a8/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.139109 cellpy-1.0.0a8/cellpy/parameters/
--rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a8/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    23452 2023-05-14 17:34:31.000000 cellpy-1.0.0a8/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.142108 cellpy-1.0.0a8/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a8/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a8/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.151689 cellpy-1.0.0a8/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   230654 2023-05-14 17:41:37.000000 cellpy-1.0.0a8/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    39537 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.179208 cellpy-1.0.0a8/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    49052 2023-05-12 17:21:48.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27324 2023-05-09 19:57:46.000000 cellpy-1.0.0a8/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.190716 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.193716 cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.199716 cellpy-1.0.0a8/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.223716 cellpy-1.0.0a8/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a8/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.242716 cellpy-1.0.0a8/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    41058 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/collectors_old.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.244716 cellpy-1.0.0a8/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3700143 2023-05-14 17:50:44.000000 cellpy-1.0.0a8/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.249716 cellpy-1.0.0a8/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a8/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a8/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a8/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.127456 cellpy-1.0.0a8/cellpy.egg-info/
--rw-rw-rw-   0        0        0     6518 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7846 2023-05-14 17:53:18.000000 cellpy-1.0.0a8/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 17:53:16.000000 cellpy-1.0.0a8/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      337 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-14 17:53:17.000000 cellpy-1.0.0a8/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.259228 cellpy-1.0.0a8/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a8/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.089754 cellpy-1.0.0a8/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.088754 cellpy-1.0.0a8/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.266226 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.295735 cellpy-1.0.0a8/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
--rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
--rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
--rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
--rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
--rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
--rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
--rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
--rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
--rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a8/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
--rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a8/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.300268 cellpy-1.0.0a8/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a8/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a8/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a8/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/adapted_readme.rst
--rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.313794 cellpy-1.0.0a8/docs/developers_guide/
--rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_packaging_pypi.rst
--rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_setup.rst
--rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_conda_package.rst
--rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_docs.rst
--rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_loaders_and_instruments.rst
--rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/dev_various.rst
--rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/developers_guide/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.322793 cellpy-1.0.0a8/docs/examples_and_tutorials/
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.334793 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/
--rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
--rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
--rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
--rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
--rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
--rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
--rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/basics.rst
--rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/examples.rst
--rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.343793 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/
--rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/01_arbin.rst
--rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/02_maccor.rst
--rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/03_PEC.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/04_Neware.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/05_biologics.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders/06_custom.rst
--rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/loaders.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.091754 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.347793 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/
--rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
--rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks.rst
--rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.358792 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/
--rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/batch.rst
--rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/collectors.rst
--rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.362793 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/
--rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/ica.rst
--rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/plotting.rst
--rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/templates.rst
--rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/examples_and_tutorials/utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.366794 cellpy-1.0.0a8/docs/figures/
--rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/figures/cellpy-icon-bw.png
--rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/figures/cellpy-logo-v1.png
--rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.376793 cellpy-1.0.0a8/docs/main_description/
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/authors.rst
--rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/contributing.rst
--rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/formats.rst
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/history.rst
--rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/index.rst
--rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/installation.rst
--rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/main_description/usage.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a8/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-14 17:53:18.396303 cellpy-1.0.0a8/docs/source/
--rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.internals.rst
--rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.parameters.legacy.rst
--rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.configurations.rst
--rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
--rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.processors.rst
--rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a8/docs/source/modules.rst
--rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 17:53:18.398304 cellpy-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     2922 2023-05-12 17:21:47.000000 cellpy-1.0.0a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.181958 cellpy-1.0.0a9/
+-rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     4001 2023-05-25 17:55:44.000000 cellpy-1.0.0a9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6767 2023-05-25 17:56:35.180958 cellpy-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.911380 cellpy-1.0.0a9/cellpy/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-05-25 17:56:19.000000 cellpy-1.0.0a9/cellpy/_version.py
+-rw-rw-rw-   0        0        0    52893 2023-05-23 14:55:13.000000 cellpy-1.0.0a9/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.924379 cellpy-1.0.0a9/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.931380 cellpy-1.0.0a9/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a9/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    23452 2023-05-14 17:34:31.000000 cellpy-1.0.0a9/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.934380 cellpy-1.0.0a9/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    12261 2023-05-23 14:50:48.000000 cellpy-1.0.0a9/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a9/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.943380 cellpy-1.0.0a9/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   235011 2023-05-25 17:44:20.000000 cellpy-1.0.0a9/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    38338 2023-05-25 16:54:28.000000 cellpy-1.0.0a9/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.966380 cellpy-1.0.0a9/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    49052 2023-05-12 17:21:48.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    27324 2023-05-09 19:57:46.000000 cellpy-1.0.0a9/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.976379 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.979380 cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.984379 cellpy-1.0.0a9/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.007380 cellpy-1.0.0a9/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a9/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.027387 cellpy-1.0.0a9/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    40056 2023-05-16 14:17:12.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/collectors_old.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.029379 cellpy-1.0.0a9/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3700143 2023-05-25 17:51:11.000000 cellpy-1.0.0a9/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.033380 cellpy-1.0.0a9/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a9/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a9/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a9/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    31653 2023-05-19 21:09:17.000000 cellpy-1.0.0a9/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.921380 cellpy-1.0.0a9/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     6767 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7846 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 17:56:33.000000 cellpy-1.0.0a9/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      337 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 17:56:34.000000 cellpy-1.0.0a9/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.042889 cellpy-1.0.0a9/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a9/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.886380 cellpy-1.0.0a9/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.886380 cellpy-1.0.0a9/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.049889 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.079958 cellpy-1.0.0a9/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
+-rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
+-rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
+-rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
+-rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
+-rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
+-rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
+-rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
+-rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
+-rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a9/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
+-rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a9/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.084957 cellpy-1.0.0a9/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a9/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a9/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a9/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/adapted_readme.rst
+-rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.097958 cellpy-1.0.0a9/docs/developers_guide/
+-rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_packaging_pypi.rst
+-rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_setup.rst
+-rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_conda_package.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_docs.rst
+-rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_loaders_and_instruments.rst
+-rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/dev_various.rst
+-rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/developers_guide/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.106958 cellpy-1.0.0a9/docs/examples_and_tutorials/
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.117958 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/
+-rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
+-rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
+-rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
+-rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
+-rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
+-rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
+-rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/basics.rst
+-rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/examples.rst
+-rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.126958 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/
+-rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/01_arbin.rst
+-rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/02_maccor.rst
+-rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/03_PEC.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/04_Neware.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/05_biologics.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders/06_custom.rst
+-rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/loaders.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:34.888380 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.129958 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/
+-rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
+-rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks.rst
+-rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.140958 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/
+-rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/batch.rst
+-rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/collectors.rst
+-rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.145957 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/ica.rst
+-rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/plotting.rst
+-rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/templates.rst
+-rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/examples_and_tutorials/utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.148958 cellpy-1.0.0a9/docs/figures/
+-rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/figures/cellpy-icon-bw.png
+-rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/figures/cellpy-logo-v1.png
+-rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.160958 cellpy-1.0.0a9/docs/main_description/
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/authors.rst
+-rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/contributing.rst
+-rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/formats.rst
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/history.rst
+-rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/index.rst
+-rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/installation.rst
+-rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/main_description/usage.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-25 17:56:35.179958 cellpy-1.0.0a9/docs/source/
+-rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.internals.rst
+-rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.parameters.legacy.rst
+-rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.configurations.rst
+-rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
+-rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.processors.rst
+-rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a9/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:56:35.181958 cellpy-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     2922 2023-05-12 17:21:47.000000 cellpy-1.0.0a9/setup.py
```

### Comparing `cellpy-1.0.0a8/CONTRIBUTING.rst` & `cellpy-1.0.0a9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/LICENSE` & `cellpy-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/MANIFEST.in` & `cellpy-1.0.0a9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/PKG-INFO` & `cellpy-1.0.0a9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,26 +93,32 @@
 History
 =======
 
 
 1.0.0 (2023) [under development]
 ================================
 
+* Unit handling: new unit handling (using pint)
 * Unit handling: renaming summary headers
 * Unit handling: new cellpy-file-format version
 * Unit handling: tool for converting old to new format
+* Unit handling: parsing input parameters for units
 * Templates: using one repository with sub-folders
 * Templates: adding more documentation
 * File handling: allow for external raw files (ssh)
 * Readers: neware.txt (one version/model)
 * Readers: arbin_sql7 (experimental, @jtgibson91)
 * Batch plotting: collectors for both data collection, plotting and saving
+* OCV-rlx: improvements of the OCV-rlx tools
 * Internals: rename main classes (CellpyData -> CellpyCell, Cell -> Data)
 * Internals: rename .cell property to .data
 * Internals: allow for only one Data-object pr CellpyCell object
+* CLI: general improvements and bug fixes
+* CLI: move editing of db-file to the edit sub-command
+
 
 
 0.4.3 (2023)
 ============
 
 * Neware txt loader (supports one specific format only, other formats will have to wait for v.1.0)
```

### Comparing `cellpy-1.0.0a8/README.rst` & `cellpy-1.0.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/__init__.py` & `cellpy-1.0.0a9/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/cli.py` & `cellpy-1.0.0a9/cellpy/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1686 +1,1736 @@
-import base64
-import getpass
-import logging
-import os
-import pathlib
-from pprint import pprint
-import re
-import subprocess
-import sys
-from typing import Union
-import urllib
-from pathlib import Path
-
-import click
-import pkg_resources
-from github import Github
-
-import cellpy._version
-from cellpy.exceptions import ConfigFileNotWritten
-from cellpy.parameters import prmreader
-from cellpy.parameters.internal_settings import OTHERPATHS
-from cellpy.internals.core import OtherPath
-
-VERSION = cellpy._version.__version__
-REPO = "jepegit/cellpy"
-USER = "jepegit"
-GITHUB_PWD_VAR_NAME = "GD_PWD"
-
-
-def save_prm_file(prm_filename):
-    """saves (writes) the prms to file"""
-    prmreader._write_prm_file(prm_filename)
-
-
-def get_package_prm_dir():
-    """gets the folder where the cellpy package lives"""
-    prm_dir = pkg_resources.resource_filename("cellpy", "parameters")
-    return pathlib.Path(prm_dir)
-
-
-def get_default_config_file_path(init_filename=None):
-    """gets the path to the default config-file"""
-    prm_dir = get_package_prm_dir()
-    if not init_filename:
-        init_filename = prmreader.DEFAULT_FILENAME
-    src = prm_dir / init_filename
-    return src
-
-
-def get_dst_file(user_dir, init_filename):
-    user_dir = pathlib.Path(user_dir)
-    dst_file = user_dir / init_filename
-    return dst_file
-
-
-def check_if_needed_modules_exists():
-    pass
-
-
-def modify_config_file():
-    pass
-
-
-def create_cellpy_folders():
-    pass
-
-
-@click.group("cellpy")
-def cli():
-    pass
-
-
-# ----------------------- setup --------------------------------------
-@click.command()
-@click.option(
-    "--interactive",
-    "-i",
-    is_flag=True,
-    default=False,
-    help="Allows you to specify div. folders and setting.",
-)
-@click.option(
-    "--not-relative",
-    "-nr",
-    is_flag=True,
-    default=False,
-    help="If root-dir is given, put it directly in the root (/) folder"
-    " i.e. don't put it in your home directory. Defaults to False. Remark"
-    " that if you specifically write a path name instead of selecting the"
-    " suggested default, the path you write will be used as is.",
-)
-@click.option(
-    "--dry-run",
-    "-dr",
-    is_flag=True,
-    default=False,
-    help="Run setup in dry mode (only print - do not execute). This is"
-    " typically used when developing and testing cellpy. Defaults to"
-    " False.",
-)
-@click.option(
-    "--reset",
-    "-r",
-    is_flag=True,
-    default=False,
-    help="Do not suggest path defaults based on your current configuration-file",
-)
-@click.option(
-    "--root-dir",
-    "-d",
-    default=None,
-    type=click.Path(),
-    help="Use custom root dir. If not given, your home directory"
-    " will be used as the top level where cellpy-folders"
-    " will be put. The folder path must follow"
-    " directly after this option (if used). Example:\n"
-    " $ cellpy setup -d 'MyDir'",
-)
-@click.option(
-    "--folder-name",
-    "-n",
-    default=None,
-    type=click.Path(),
-    help="",
-)
-@click.option(
-    "--test_user", "-t", default=None, help="Fake name for fake user (for testing)"
-)
-def setup(interactive, not_relative, dry_run, reset, root_dir, folder_name, test_user):
-    """This will help you to set up cellpy."""
-
-    click.echo("[cellpy] (setup)")
-    click.echo(f"[cellpy] root-dir: {root_dir}")
-
-    # generate variables
-    init_filename = prmreader.create_custom_init_filename()
-    user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
-
-    if dry_run:
-        click.echo("Create custom init filename and get user_dir and destination")
-        click.echo(f"Got the following parameters:")
-        click.echo(f" - init_filename: {init_filename}")
-        click.echo(f" - user_dir: {user_dir}")
-        click.echo(f" - dst_file: {dst_file}")
-        click.echo(f" - not_relative: {not_relative}")
-
-    if root_dir and not interactive:
-        click.echo("[cellpy] custom root-dir can only be used in interactive mode")
-        click.echo("[cellpy] -> setting interactive mode")
-        interactive = True
-
-    if not root_dir:
-        root_dir = user_dir
-        # root_dir = pathlib.Path(os.getcwd())
-    root_dir = pathlib.Path(root_dir)
-
-    if dry_run:
-        click.echo(f" - root_dir: {root_dir}")
-
-    if test_user:
-        click.echo(f"[cellpy] (setup) DEV-MODE test_user: {test_user}")
-        init_filename = prmreader.create_custom_init_filename(test_user)
-        user_dir = root_dir
-        dst_file = get_dst_file(user_dir, init_filename)
-        click.echo(f"[cellpy] (setup) DEV-MODE user_dir: {user_dir}")
-        click.echo(f"[cellpy] (setup) DEV-MODE dst_file: {dst_file}")
-
-    if not pathlib.Path(dst_file).is_file():
-        click.echo(f"[cellpy] {dst_file} not found -> I will make one for you!")
-        reset = True
-
-    if interactive:
-        click.echo(" interactive mode ".center(80, "-"))
-        _update_paths(
-            custom_dir=root_dir,
-            relative_home=not not_relative,
-            default_dir=folder_name,
-            dry_run=dry_run,
-            reset=reset,
-        )
-        _write_config_file(user_dir, dst_file, init_filename, dry_run)
-        _check(dry_run=dry_run)
-
-    else:
-        if reset:
-            _update_paths(
-                user_dir,
-                False,
-                default_dir=folder_name,
-                dry_run=dry_run,
-                reset=True,
-                silent=True,
-            )
-        _write_config_file(user_dir, dst_file, init_filename, dry_run)
-        _check(dry_run=dry_run)
-
-
-def _update_paths(
-    custom_dir=None,
-    relative_home=True,
-    reset=False,
-    dry_run=False,
-    default_dir=None,
-    silent=False,
-):
-    # please, refactor me :-(
-
-    h = prmreader.get_user_dir()
-
-    if default_dir is None:
-        default_dir = "cellpy_data"
-
-    if dry_run:
-        click.echo(f" - default_dir: {default_dir}")
-        click.echo(f" - custom_dir: {custom_dir}")
-        click.echo(f" - retalive_home: {relative_home}")
-
-    if custom_dir:
-        reset = True
-        if relative_home:
-            h = h / custom_dir
-        if not custom_dir.parts[-1] == default_dir:
-            h = h / default_dir
-
-    if not reset:
-        outdatadir = pathlib.Path(prmreader.prms.Paths.outdatadir)
-        rawdatadir = OtherPath(prmreader.prms.Paths.rawdatadir)
-        cellpydatadir = OtherPath(prmreader.prms.Paths.cellpydatadir)
-        filelogdir = pathlib.Path(prmreader.prms.Paths.filelogdir)
-        examplesdir = pathlib.Path(prmreader.prms.Paths.examplesdir)
-        db_path = pathlib.Path(prmreader.prms.Paths.db_path)
-        db_filename = prmreader.prms.Paths.db_filename
-        notebookdir = pathlib.Path(prmreader.prms.Paths.notebookdir)
-        batchfiledir = pathlib.Path(prmreader.prms.Paths.batchfiledir)
-        templatedir = pathlib.Path(prmreader.prms.Paths.templatedir)
-        instrumentdir = pathlib.Path(prmreader.prms.Paths.instrumentsdir)
-    else:
-        outdatadir = "out"
-        rawdatadir = "raw"
-        cellpydatadir = "cellpyfiles"
-        filelogdir = "logs"
-        examplesdir = "examples"
-        db_path = "db"
-        db_filename = "cellpy_db.xlsx"
-        notebookdir = "notebooks"
-        batchfiledir = "batchfiles"
-        templatedir = "templates"
-        instrumentdir = "instruments"
-
-    outdatadir = h / outdatadir
-    rawdatadir = h / rawdatadir
-    cellpydatadir = h / cellpydatadir
-    filelogdir = h / filelogdir
-    examplesdir = h / examplesdir
-    db_path = h / db_path
-    notebookdir = h / notebookdir
-    batchfiledir = h / batchfiledir
-    templatedir = h / templatedir
-    instrumentdir = h / instrumentdir
-
-    if dry_run:
-        click.echo(f" - base (h): {h}")
-
-    if not silent:
-        outdatadir = _ask_about_path(
-            "where to output processed data and results", outdatadir
-        )
-        rawdatadir = _ask_about_otherpath("where your raw data are located", rawdatadir)
-        cellpydatadir = _ask_about_otherpath("where to put cellpy-files", cellpydatadir)
-        filelogdir = _ask_about_path("where to dump the log-files", filelogdir)
-        examplesdir = _ask_about_path(
-            "where to download cellpy examples and tests", examplesdir
-        )
-        db_path = _ask_about_path("what folder your db file lives in", db_path)
-        db_filename = _ask_about_name("the name of your db-file", db_filename)
-        notebookdir = _ask_about_path(
-            "where to put your jupyter notebooks", notebookdir
-        )
-        batchfiledir = _ask_about_path("where to put your batch files", batchfiledir)
-        templatedir = _ask_about_path("where to put your batch files", templatedir)
-        instrumentdir = _ask_about_path("where to put your batch files", instrumentdir)
-
-    # update folders based on suggestions
-    for d in [
-        outdatadir,
-        rawdatadir,
-        cellpydatadir,
-        filelogdir,
-        examplesdir,
-        notebookdir,
-        db_path,
-        batchfiledir,
-        templatedir,
-        instrumentdir,
-    ]:
-        if not dry_run:
-            _create_dir(d)
-        else:
-            click.echo(f"dry run (so I did not create {d})")
-
-    # update config-file based on suggestions
-    prmreader.prms.Paths.outdatadir = str(outdatadir)
-    prmreader.prms.Paths.rawdatadir = str(rawdatadir)
-    prmreader.prms.Paths.cellpydatadir = str(cellpydatadir)
-    prmreader.prms.Paths.filelogdir = str(filelogdir)
-    prmreader.prms.Paths.examplesdir = str(examplesdir)
-    prmreader.prms.Paths.db_path = str(db_path)
-    prmreader.prms.Paths.db_filename = str(db_filename)
-    prmreader.prms.Paths.notebookdir = str(notebookdir)
-    prmreader.prms.Paths.batchfiledir = str(batchfiledir)
-    prmreader.prms.Paths.templatedir = str(templatedir)
-    prmreader.prms.Paths.instrumentdir = str(instrumentdir)
-
-
-def _ask_about_path(q, p):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {p}")
-    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_path:
-        new_path = p
-    return pathlib.Path(new_path)
-
-
-def _ask_about_otherpath(q, p):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {p}")
-    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_path:
-        new_path = p
-    return OtherPath(new_path)
-
-
-def _ask_about_name(q, n):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {n}")
-    new_name = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_name:
-        new_name = n
-    return new_name
-
-
-def _create_dir(path, confirm=True, parents=True, exist_ok=True):
-    if isinstance(path, OtherPath):
-        if path.is_external:
-            return path
-    o = path.resolve()
-    if not o.is_dir():
-        o_parent = o.parent
-        create_dir = True
-        if confirm:
-            if not o_parent.is_dir():
-                create_dir = input(
-                    f"\n[cellpy] (setup) {o_parent} does not exist. Create it [y]/n ?"
-                )
-                if not create_dir:
-                    create_dir = True
-                elif create_dir in ["y", "Y"]:
-                    create_dir = True
-                else:
-                    create_dir = False
-
-        if create_dir:
-            try:
-                o.mkdir(parents=parents, exist_ok=exist_ok)
-                click.echo(f"[cellpy] (setup) Created {o}")
-            except FileExistsError:
-                click.echo(f"[cellpy] (setup) {o} already exists.")
-            except FileNotFoundError:
-                click.echo(f"[cellpy] (setup) {o} not available.")
-            except Exception as e:
-                click.echo(f"[cellpy] (setup) WARNING! Could not create {o}.")
-                logging.debug(e)
-                click.echo(f"[cellpy] (setup) ...continuing anyway.")
-        else:
-            click.echo(f"[cellpy] (setup) Could not create {o}")
-    return o
-
-
-def _check_import_cellpy():
-    try:
-        import cellpy
-        from cellpy import log
-        from cellpy.readers import cellreader
-
-        return True
-    except:
-        return False
-
-
-def _check_import_pyodbc():
-    import platform
-
-    from cellpy.parameters import prms
-
-    ODBC = prms._odbc
-    SEARCH_FOR_ODBC_DRIVERS = prms._search_for_odbc_driver
-
-    use_subprocess = prms.Instruments.Arbin.use_subprocess
-    detect_subprocess_need = prms.Instruments.Arbin.detect_subprocess_need
-    click.echo(f" reading prms")
-    click.echo(f" - ODBC: {ODBC}")
-    click.echo(f" - SEARCH_FOR_ODBC_DRIVERS: {SEARCH_FOR_ODBC_DRIVERS}")
-    click.echo(f" - use_subprocess: {use_subprocess}")
-    click.echo(f" - detect_subprocess_need: {detect_subprocess_need}")
-    click.echo(f" - stated office version: {prms.Instruments.Arbin.office_version}")
-
-    click.echo(" checking system")
-    is_posix = False
-    is_macos = False
-    if os.name == "posix":
-        is_posix = True
-        click.echo(f" - running on posix")
-    current_platform = platform.system()
-    if current_platform == "Darwin":
-        is_macos = True
-        click.echo(f" - running on a mac")
-
-    python_version, os_version = platform.architecture()
-    click.echo(f" - python version: {python_version}")
-    click.echo(f" - os version: {os_version}")
-
-    if not is_posix:
-        if not prms.Instruments.Arbin.sub_process_path:
-            sub_process_path = str(prms._sub_process_path)
-        else:
-            sub_process_path = str(prms.Instruments.Arbin.sub_process_path)
-        click.echo(f" stated path to sub-process: {sub_process_path}")
-        if not os.path.isfile(sub_process_path):
-            click.echo(f" - OBS! missing")
-
-    if is_posix:
-        click.echo(" checking existence of mdb-export")
-        sub_process_path = "mdb-export"
-        from subprocess import PIPE, run
-
-        command = ["command", "-v", sub_process_path]
-
-        try:
-            result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-            if result.returncode == 0:
-                click.echo(f" - found it: {result.stdout}")
-            else:
-                click.echo(f" - failed finding it")
-
-            if is_macos:
-                driver = "/usr/local/lib/libmdbodbc.dylib"
-                click.echo(f" looks like you are on a mac (driver set to\n {driver})")
-                if not os.path.isfile(driver):
-                    click.echo(" - but cannot find it!")
-                    return False
-            return True
-
-        except AssertionError:
-            click.echo(" - not found")
-            return False
-
-    # not posix - checking for odbc drivers
-    # 1) checking if you have defined one
-    try:
-        driver = prms.Instruments.Arbin.odbc_driver
-        if not driver:
-            raise AttributeError
-        click.echo("You have defined an odbc driver in your conifg file")
-        click.echo(f"driver: {driver}")
-    except AttributeError:
-        click.echo("FYI: you have not defined any odbc_driver(s)")
-        click.echo(
-            "(The name of the driver from the configuration file is "
-            "used as a backup when cellpy cannot locate a driver by itself)"
-        )
-
-    use_ado = False
-
-    if ODBC == "ado":
-        use_ado = True
-        click.echo(" you stated that you prefer the ado loader")
-        click.echo(" checking if adodbapi is installed")
-        try:
-            import adodbapi as dbloader
-        except ImportError:
-            use_ado = False
-            click.echo(" Failed! Try setting pyodbc as your loader or install")
-            click.echo(" adodbapi (http://adodbapi.sourceforge.net/)")
-
-    if not use_ado:
-        if ODBC == "pyodbc":
-            click.echo(" you stated that you prefer the pyodbc loader")
-            try:
-                import pyodbc as dbloader
-            except ImportError:
-                click.echo(" Failed! Could not import it.")
-                click.echo(" Try 'pip install pyodbc'")
-                dbloader = None
-
-        elif ODBC == "pypyodbc":
-            click.echo(" you stated that you prefer the pypyodbc loader")
-            try:
-                import pypyodbc as dbloader
-            except ImportError:
-                click.echo(" Failed! Could not import it.")
-                click.echo(" try 'pip install pypyodbc'")
-                click.echo(" or set pyodbc as your loader in your prm file")
-                click.echo(" (and install it)")
-                dbloader = None
-
-    click.echo(" searching for odbc drivers")
-    try:
-        drivers = [
-            driver
-            for driver in dbloader.drivers()
-            if "Microsoft Access Driver" in driver
-        ]
-        click.echo(f"Found these: {drivers}")
-        driver = drivers[0]
-        click.echo(f"odbc driver: {driver}")
-        return True
-
-    except IndexError as e:
-        logging.debug("Unfortunately, it seems the list of drivers is emtpy.")
-        click.echo(
-            "\nCould not find any odbc-drivers suitable for .res-type files. "
-            "Check out the homepage of pydobc for info on installing drivers"
-        )
-        click.echo(
-            "One solution that might work is downloading "
-            "the Microsoft Access database engine "
-            "(in correct bytes (32 or 64)) "
-            "from:\n"
-            "https://www.microsoft.com/en-us/download/details.aspx?id=13255"
-        )
-        click.echo("Or install mdbtools and set it up (check the cellpy docs for help)")
-        click.echo("\n")
-        return False
-
-
-def _check_config_file():
-    prm_file_name = _configloc()
-    prm_dict = prmreader._read_prm_file_without_updating(prm_file_name)
-    try:
-        prm_paths = prm_dict["Paths"]
-        required_dirs = [
-            "cellpydatadir",
-            "examplesdir",
-            "filelogdir",
-            "notebookdir",
-            "outdatadir",
-            "rawdatadir",
-            "batchfiledir",
-            "templatedir",
-            "db_path",
-        ]
-        missing = 0
-        for k in required_dirs:
-            value = prm_paths.get(k, None)
-            click.echo(f"{k}: {value}")
-            # splitting this into two if-statements to make it easier to debug if OtherPath changes
-            if k in OTHERPATHS:
-                print(f"skipping check for external {k} (for now)")
-                # if not OtherPath(
-                #     value
-                # ).is_dir():  # Assuming OtherPath returns True if it is external.
-                #     missing += 1
-                #     click.echo("COULD NOT CONNECT!")
-                #     click.echo(f"({value} is not a directory)")
-            elif value and not pathlib.Path(value).is_dir():
-                missing += 1
-                click.echo("COULD NOT CONNECT!")
-                click.echo(f"({value} is not a directory)")
-            if not value:
-                missing += 1
-                click.echo("MISSING")
-
-        value = prm_paths.get("db_filename", None)
-        click.echo(f"db_filename: {value}")
-        if not value:
-            missing += 1
-            click.echo("MISSING")
-
-        if missing:
-            return False
-        else:
-            return True
-
-    except Exception as e:
-        click.echo("Following error occurred:")
-        click.echo(e)
-        return False
-
-
-def _check(dry_run=False):
-    click.echo(" checking ".center(80, "="))
-    if dry_run:
-        click.echo("*** dry-run: skipping the test")
-        return
-    failed_checks = 0
-    number_of_checks = 0
-
-    def sub_check(check_type, check_func):
-        failed = 0
-        click.echo(f"[cellpy] * - Checking {check_type}")
-        if check_func():
-            click.echo(f"[cellpy] -> succeeded!")
-        else:
-            click.echo("f[cellpy] -> failed!!!!")
-            failed = 1
-        click.echo(80 * "-")
-        return failed
-
-    check_types = ["cellpy imports", "importing pyodbc", "configuration (prm) file"]
-    check_funcs = [_check_import_cellpy, _check_import_pyodbc, _check_config_file]
-
-    for ct, cf in zip(check_types, check_funcs):
-        try:
-            failed_checks += sub_check(ct, cf)
-        except Exception as e:
-            click.echo(f"[cellpy] check raised an exception ({e})")
-        number_of_checks += 1
-    succeeded_checks = number_of_checks - failed_checks
-    if failed_checks > 0:
-        click.echo(f"[cellpy] OH NO!!! You (or I) failed!")
-        click.echo(f"[cellpy] Failed {failed_checks} out of {number_of_checks} checks.")
-    else:
-        click.echo(
-            f"[cellpy] Succeeded {succeeded_checks} out of {number_of_checks} checks."
-        )
-    click.echo(80 * "=")
-
-
-def _write_config_file(user_dir, dst_file, init_filename, dry_run):
-    click.echo(" update configuration ".center(80, "-"))
-    click.echo("[cellpy] (setup) Writing configurations to user directory:")
-    click.echo(f"\n         {user_dir}\n")
-
-    if os.path.isfile(dst_file):
-        click.echo("[cellpy] (setup) File already exists!")
-        click.echo("[cellpy] (setup) Keeping most of the old configuration parameters")
-    try:
-        if dry_run:
-            click.echo(
-                f"*** dry-run: skipping actual saving of {dst_file} ***", color="red"
-            )
-        else:
-            click.echo(f"[cellpy] (setup) Saving file ({dst_file})")
-            save_prm_file(dst_file)
-
-    except ConfigFileNotWritten:
-        click.echo("[cellpy] (setup) Something went wrong! Could not write the file")
-        click.echo(
-            "[cellpy] (setup) Trying to write a file"
-            + f"called {prmreader.DEFAULT_FILENAME} instead"
-        )
-
-        try:
-            user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
-            if dry_run:
-                click.echo(
-                    f"*** dry-run: skipping actual saving of {dst_file} ***",
-                    color="red",
-                )
-            else:
-                save_prm_file(dst_file)
-
-        except ConfigFileNotWritten:
-            _txt = "[cellpy] (setup) No, that did not work either.\n"
-            _txt += "[cellpy] (setup) Well, guess you have to talk to the developers."
-            click.echo(_txt)
-    else:
-        click.echo(f"[cellpy] (setup) Configuration file written!")
-        click.echo(
-            f"[cellpy] (setup) OK! Now you can edit it. For example by "
-            f"issuing \n\n         [your-favourite-editor] {init_filename}\n"
-        )
-
-
-# ----------------------- edit ---------------------------------------
-@click.command()
-@click.option(
-    "--default-editor",
-    "-e",
-    default=None,
-    type=str,
-    help="try to use this editor instead (e.g. notepad.exe)",
-)
-def edit(default_editor):
-    """Edit your cellpy config file."""
-
-    config_file = _configloc()
-    if config_file:
-        config_file_str = str(config_file.resolve())
-
-        if default_editor is not None:
-            args = [default_editor, config_file_str]
-            click.echo(f"[cellpy] (edit) Calling '{default_editor}'")
-            try:
-                subprocess.call(args)
-            except:
-                click.echo(f"[cellpy] (edit) Failed!")
-                click.echo(
-                    "[cellpy] (edit) Try 'cellpy edit -e notepad.exe' if you are on Windows"
-                )
-
-        if default_editor is None:
-            try:
-                import editor
-
-                editor.edit(filename=config_file_str)
-            except ImportError:
-                click.echo(f"[cellpy] (edit) Failed!")
-                click.echo(
-                    f"[cellpy] (edit) Searching for editors uses the python-editor package"
-                )
-                click.echo(f"[cellpy] (edit) Possible fixes:")
-                click.echo(
-                    f"[cellpy] (edit) - provide a default editor "
-                    f"using the -e option (e.g. cellpy edit -e notepad.exe)"
-                )
-                click.echo(
-                    f"[cellpy] (edit) - install teh python-editor package "
-                    f"(pip install python-editor)"
-                )
-
-
-# ----------------------- info ---------------------------------------
-@click.command()
-@click.option("--version", "-v", is_flag=True, help="Print version information.")
-@click.option(
-    "--configloc", "-l", is_flag=True, help="Print full path to the config file."
-)
-@click.option("--params", "-p", is_flag=True, help="Dump all parameters to screen.")
-@click.option(
-    "--check",
-    "-c",
-    is_flag=True,
-    help="Do a sanity check to see if things" " works as they should.",
-)
-def info(version, configloc, params, check):
-    """This will give you some valuable information about your cellpy."""
-    complete_info = True
-
-    if check:
-        complete_info = False
-        _check()
-
-    if version:
-        complete_info = False
-        _version()
-
-    if configloc:
-        complete_info = False
-        _configloc()
-
-    if params:
-        complete_info = False
-        _dump_params()
-
-    if complete_info:
-        _version()
-        _configloc()
-
-
-# ----------------------- run ----------------------------------------
-@click.command()
-@click.option(
-    "--journal",
-    "-j",
-    is_flag=True,
-    help="Run a batch job defined in the given journal-file",
-)
-@click.option("--key", "-k", is_flag=True, help="Run a batch job defined by batch-name")
-@click.option(
-    "--folder",
-    "-f",
-    is_flag=True,
-    help="Run all batch jobs iteratively in a given folder",
-)
-@click.option(
-    "--cellpy-project",
-    "-p",
-    is_flag=True,
-    help="Use PaperMill to run the notebook(s) within the given project folder "
-    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'). "
-    "Warning! since we are using `click` - the NAME will be 'converted' when it is loaded "
-    "(same as print(name) does) - "
-    "so you can't use backslash ('\\') as normal in windows (use either '/' or '\\\\' instead).",
-)
-@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
-@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
-@click.option("--raw", is_flag=True, help="Force loading raw-file(s).")
-@click.option("--cellpyfile", is_flag=True, help="Force cellpy-file(s).")
-@click.option("--minimal", is_flag=True, help="Minimal processing.")
-@click.option(
-    "--nom-cap",
-    default=None,
-    type=float,
-    help="nominal capacity (used in calculating rates etc)",
-)
-@click.option(
-    "--batch_col",
-    default=None,
-    type=str,
-    help="batch column (if selecting running from db)",
-)
-@click.option(
-    "--project",
-    default=None,
-    type=str,
-    help="name of the project (if selecting running from db)",
-)
-@click.option("--list", "-l", "list_", is_flag=True, help="List batch-files.")
-@click.argument("name", default="NONE")
-def run(
-    journal,
-    key,
-    folder,
-    cellpy_project,
-    debug,
-    silent,
-    raw,
-    cellpyfile,
-    minimal,
-    nom_cap,
-    batch_col,
-    project,
-    list_,
-    name,
-):
-    """Run a cellpy process (batch-job, edit db, ...).
-
-    You can use this to launch specific applications.
-
-    Examples:
-
-        edit your cellpy database
-
-           cellpy run db
-
-        run a batch job described in a journal file
-
-           cellpy run -j my_experiment.json
-
-    """
-    if list_:
-        _run_list(name)
-        return
-
-    if name == "NONE":
-        click.echo(
-            "Usage: cellpy run [OPTIONS] NAME\n"
-            "Try 'cellpy run --help' for help.\n\n"
-            "Error: Missing argument 'NAME'."
-        )
-        sys.exit(-1)
-
-    if debug:
-        click.echo("[cellpy] (run) debug mode on")
-
-    if silent:
-        click.echo("[cellpy] (run) silent mode on")
-
-    click.echo("[cellpy]\n")
-
-    if cellpy_project:
-        _run_project(name)
-
-    elif journal:
-        _run_journal(name, debug, silent, raw, cellpyfile, minimal, nom_cap)
-
-    elif folder:
-        _run_journals(name, debug, silent, raw, cellpyfile, minimal)
-
-    elif key:
-        _run_from_db(
-            name,
-            debug,
-            silent,
-            raw,
-            cellpyfile,
-            minimal,
-            nom_cap,
-            batch_col,
-            project,
-        )
-
-    elif name.lower() == "db":
-        _run_db(debug, silent)
-
-    else:
-        _run(name, debug, silent)
-
-
-def _run_from_db(
-    name,
-    debug,
-    silent,
-    raw,
-    cellpyfile,
-    minimal,
-    nom_cap,
-    batch_col,
-    project,
-):
-    click.echo(
-        f"running from db \nkey={name}, batch_col={batch_col}, project={project}"
-    )
-
-    kwargs = dict()
-    kwargs["name"] = name
-
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    if batch_col is not None:
-        kwargs["batch_col"] = batch_col
-    if project is None:
-        kwargs["project"] = "various"
-    else:
-        kwargs["project"] = project
-
-    click.echo("Warming up ...")
-
-    from cellpy.utils import batch
-
-    click.echo("  - starting batch processing")
-    b = batch.process_batch(
-        force_raw_file=raw,
-        force_cellpy=cellpyfile,
-        nom_cap=nom_cap,
-        backend="matplotlib",
-        **kwargs,
-    )
-
-    if b is not None and not silent:
-        print(b)
-    click.echo("---")
-
-
-def _run_journal(file_name, debug, silent, raw, cellpyfile, minimal, nom_cap):
-    click.echo(f"running journal {file_name}")
-    # click.echo(f" --debug [{debug}]")
-    # click.echo(f" --silent [{silent}]")
-    # click.echo(f" --raw [{raw}]")
-    # click.echo(f" --cellpyfile [{cellpyfile}]")
-    # click.echo(f" --minimal [{minimal}]")
-    # click.echo(f" --nom_cap [{nom_cap}] {type(nom_cap)}")
-
-    kwargs = dict()
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    from cellpy import prms
-    from cellpy.utils import batch
-
-    batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
-    file = pathlib.Path(file_name)
-    if not file.is_file():
-        click.echo(f"file_name={file_name} not found - looking into batchfiledir")
-        if not batchfiledir.is_dir():
-            click.echo("batchfiledir not found - aborting")
-            return
-        file = batchfiledir / file.name
-
-    if not file.is_file():
-        click.echo(f"{file} not found - aborting")
-        return
-
-    b = batch.process_batch(
-        file,
-        force_raw_file=raw,
-        force_cellpy=cellpyfile,
-        nom_cap=nom_cap,
-        backend="matplotlib",
-        **kwargs,
-    )
-    if b is not None and not silent:
-        print(b)
-    click.echo("---")
-
-
-def _run_list(batchfiledir):
-    from cellpy import prms
-
-    if batchfiledir == "NONE" or batchfiledir is None:
-        batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
-    else:
-        batchfiledir = pathlib.Path(batchfiledir).resolve()
-
-    if batchfiledir.is_dir():
-        click.echo(f"Content of '{batchfiledir}':\n")
-        i = 0
-        for i, f in enumerate(batchfiledir.glob("cellpy*.json")):
-            click.echo(f"{f.name}")
-        if i:
-            print(f"\nnumber of batch-files located: {i}")
-        else:
-            print("No batch-files found in this directory.")
-    else:
-        click.echo(f"{batchfiledir} not found.")
-
-
-def _run_journals(folder_name, debug, silent, raw, cellpyfile, minimal):
-    click.echo(f"running journals in {folder_name}")
-    # click.echo(f" --debug [{debug}]")
-    # click.echo(f" --silent [{silent}]")
-    # click.echo(f" --raw [{raw}]")
-    # click.echo(f" --cellpyfile [{cellpyfile}]")
-    # click.echo(f" --minimal [{minimal}]")
-
-    kwargs = dict()
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    from cellpy.utils import batch
-
-    folder_name = pathlib.Path(folder_name).resolve()
-
-    if not folder_name.is_dir():
-        click.echo(f"{folder_name} not found - aborting")
-        return
-
-    batch.iterate_batches(
-        folder_name, force_raw_file=raw, force_cellpy=cellpyfile, silent=True, **kwargs
-    )
-    click.echo("---")
-
-
-def _run_project(our_new_project, **kwargs):
-    try:
-        import papermill as pm
-    except ImportError:
-        click.echo(
-            "[cellpy]: You need to install papermill for automatically execute the notebooks."
-        )
-        click.echo("[cellpy]: You can install it using pip like this:")
-        click.echo(" >> pip install papermill")
-        return
-    our_new_project = pathlib.Path(our_new_project)
-    click.echo(f"[cellpy]: trying to run notebooks in {our_new_project}")
-    notebooks = sorted(list(our_new_project.glob("*.ipynb")))
-    for notebook in notebooks:
-        click.echo(f"[cellpy - papermill] running {notebook.name}")
-        pm.execute_notebook(notebook, notebook, parameters=kwargs)
-
-
-def _run(name, debug, silent):
-    click.echo(f"running {name}")
-    click.echo(f" --debug [{debug}]")
-    click.echo(f" --silent [{silent}]")
-
-
-def _run_db(debug, silent):
-    import platform
-
-    from cellpy import prms
-
-    if not silent:
-        click.echo(f"running database editor")
-    if debug:
-        click.echo("running in debug-mode, but nothing to tell")
-
-    db_path = Path(prms.Paths.db_path) / prms.Paths.db_filename
-
-    if platform.system() == "Windows":
-        try:
-            os.system(f'start excel "{str(db_path)}"')
-        except Exception as e:
-            click.echo("Something went wrong trying to open")
-            click.echo(db_path)
-            print()
-            print(e)
-
-    elif platform.system() == "Linux":
-        click.echo("RUNNING LINUX")
-        # not tested
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-    elif platform.system() == "Darwin":
-        click.echo(f" - running on a mac")
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-    else:
-        print("RUNNING SOMETHING ELSE")
-        print(platform.system())
-        # not tested
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-
-# ----------------------- pull ---------------------------------------
-@click.command()
-@click.option("--tests", "-t", is_flag=True, help="Download test-files from repo.")
-@click.option(
-    "--examples", "-e", is_flag=True, help="Download example-files from repo."
-)
-@click.option("--clone", "-c", is_flag=True, help="Clone the full repo.")
-@click.option("--directory", "-d", default=None, help="Save into custom directory DIR")
-@click.option("--password", "-p", default=None, help="Password option for the repo")
-def pull(tests, examples, clone, directory, password):
-    """Download examples or tests from the big internet (needs git)."""
-    if directory is not None:
-        click.echo(f"[cellpy] (pull) custom directory: {directory}")
-    else:
-        directory = pathlib.Path(prmreader.prms.Paths.examplesdir)
-
-    if password is not None:
-        click.echo("DEV MODE: password provided")
-    if clone:
-        _clone_repo(directory, password)
-    else:
-        if tests:
-            _pull_tests(directory, password)
-        if examples:
-            _pull_examples(directory, password)
-        else:
-            click.echo(
-                f"[cellpy] (pull) Nothing selected for pulling. "
-                f"Please select an option (--tests,--examples, -clone, ...) "
-            )
-
-
-def _clone_repo(directory, password):
-    directory = pathlib.Path(directory)
-    txt = "[cellpy] The plan is that this "
-    txt += "[cellpy] cmd will pull (clone) the cellpy repo.\n"
-    txt += "[cellpy] For now it only prints the link to the git-hub\n"
-    txt += "[cellpy] repository:\n"
-    txt += "[cellpy]\n"
-    txt += "[cellpy] https://github.com/jepegit/cellpy.git\n"
-    txt += "[cellpy]\n"
-    click.echo(txt)
-
-
-def _pull_tests(directory, pw=None):
-    txt = (
-        "[cellpy] (pull) Pulling tests from",
-        " https://github.com/jepegit/cellpy.git",
-    )
-    click.echo(txt)
-    _pull(gdirpath="tests", rootpath=directory, pw=pw)
-    _pull(gdirpath="testdata", rootpath=directory, pw=pw)
-
-
-def _pull_examples(directory, pw):
-    txt = (
-        "[cellpy] (pull) Pulling examples from",
-        " https://github.com/jepegit/cellpy.git",
-    )
-    click.echo(txt)
-    _pull(gdirpath="examples", rootpath=directory, pw=pw)
-
-
-def _version():
-    txt = "[cellpy] version: " + str(VERSION)
-    click.echo(txt)
-
-
-def _configloc():
-    _, config_file_name = prmreader.get_user_dir_and_dst()
-    click.echo("[cellpy] ->%s" % config_file_name)
-    if not os.path.isfile(config_file_name):
-        click.echo("[cellpy] File does not exist!")
-    else:
-        return config_file_name
-
-
-def _dump_params():
-    click.echo("[cellpy] Dumping parameters to screen:\n")
-    prmreader.info()
-
-
-def _download_g_blob(name, local_path):
-    import urllib.request
-
-    dirs = local_path.parent
-    if not dirs.is_dir():
-        click.echo(f"[cellpy] (pull) creating dir: {dirs}")
-        dirs.mkdir(parents=True)
-
-    filename, headers = urllib.request.urlretrieve(
-        name.download_url, filename=local_path
-    )
-    click.echo(f"[cellpy] (pull) downloaded blob: {filename}")
-
-
-def _parse_g_dir(repo, gdirpath):
-    """parses a repo directory two-levels deep"""
-    for f in repo.get_contents(gdirpath):
-        if f.type == "dir":
-            for sf in repo.get_contents(f.path):
-                yield sf
-        else:
-            yield f
-
-
-def _get_user_name():
-    return "jepegit"
-
-
-def _get_pw(method):
-    if method == "ask":
-        return getpass.getpass()
-    elif method == "env":
-        return os.environ.get(GITHUB_PWD_VAR_NAME, None)
-
-    else:
-        return None
-
-
-def _pull(gdirpath="examples", rootpath=None, u=None, pw=None):
-    if rootpath is None:
-        rootpath = prmreader.prms.Paths.examplesdir
-
-    rootpath = pathlib.Path(rootpath)
-
-    ndirpath = rootpath / gdirpath
-
-    if pw is not None:
-        click.echo(" DEV MODE ".center(80, "-"))
-        u = _get_user_name()
-        if pw == "ask":
-            click.echo("   - ask for password")
-            pw = _get_pw(pw)
-        elif pw == "env":
-            click.echo("   - check environ for password ")
-            pw = _get_pw(pw)
-            click.echo("   - got something")
-            if pw is None:
-                click.echo("   - only None")
-                u = None
-
-    g = Github(u, pw)
-    repo = g.get_repo(REPO)
-
-    click.echo(f"[cellpy] (pull) pulling {gdirpath}")
-    click.echo(f"[cellpy] (pull) -> {ndirpath}")
-
-    if not ndirpath.is_dir():
-        click.echo(f"[cellpy] (pull) creating dir: {ndirpath}")
-        ndirpath.mkdir(parents=True)
-
-    for gfile in _parse_g_dir(repo, gdirpath):
-        gfilename = pathlib.Path(gfile.path)
-        nfilename = rootpath / gfilename
-
-        _download_g_blob(gfile, nfilename)
-
-
-def _get_default_template():
-    template = "standard"
-    try:
-        template = prmreader.prms.Batch.template
-    except:
-        logging.debug("You dont have any default template defined in you .conf file")
-    return template
-
-
-def _read_local_templates(local_templates_path=None):
-    if local_templates_path is None:
-        local_templates_path = pathlib.Path(prmreader.prms.Paths.templatedir)
-    templates = {}
-    for p in list(local_templates_path.rglob("cellpy_cookie*.zip")):
-        label = p.stem.strip()[len("cellpy_cookie_") :]
-        templates[label] = (str(p), None)
-    logging.debug(f"Found the following templates: {templates}")
-    return templates
-
-
-# ----------------------- new ----------------------------------------
-@click.command()
-@click.option("--template", "-t", help="Provide template name.")
-@click.option("--directory", "-d", default=None, help="Create in custom directory.")
-@click.option(
-    "--project",
-    "-p",
-    default=None,
-    help="Provide project name (i.e. sub-directory name).",
-)
-@click.option(
-    "--experiment",
-    "-e",
-    default=None,
-    help="Provide experiment name (i.e. lookup-value).",
-)
-@click.option(
-    "--local-user-template",
-    "-u",
-    is_flag=True,
-    default=False,
-    help="Use local template from the templates directory.",
-)
-@click.option("--serve", "-s", "serve_", is_flag=True, help="Run Jupyter.")
-@click.option(
-    "--run",
-    "-r",
-    "run_",
-    is_flag=True,
-    help="Use PaperMill to run the notebook(s) from the template "
-    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'.",
-)
-@click.option(
-    "--lab",
-    "-j",
-    is_flag=True,
-    help="Use Jupyter Lab instead of Notebook when serving.",
-)
-@click.option(
-    "--list", "-l", "list_", is_flag=True, help="List available templates and exit."
-)
-def new(
-    template,
-    directory,
-    project,
-    experiment,
-    local_user_template,
-    serve_,
-    run_,
-    lab,
-    list_,
-):
-    """Set up a batch experiment (might need git installed)."""
-    _new(
-        template,
-        directory=directory,
-        project_dir=project,
-        session_id=experiment,
-        local_user_template=local_user_template,
-        serve_=serve_,
-        run_=run_,
-        lab=lab,
-        list_=list_,
-    )
-
-
-def _new(
-    template: str,
-    directory: Union[Path, str, None] = None,
-    project_dir: Union[str, None] = None,
-    local_user_template: bool = False,
-    serve_: bool = False,
-    run_: bool = False,
-    lab: bool = False,
-    list_: bool = False,
-    session_id: str = "experiment_001",
-    no_input: bool = False,
-    cookie_directory: str = "",
-):
-    """Set up a batch experiment (might need git installed).
-
-    Args:
-        template: short-name of template.
-        directory: the directory for your cellpy projects.
-        local_user_template: use local template if True.
-        serve_: serve the notebook after creation if True.
-        run_: run the notebooks using papermill if True.
-        lab: use jupyter-lab instead of jupyter notebook if True.
-        list_: list all available templates and return if True.
-        project_dir: your project directory.
-        session_id: the lookup value.
-        no_input: accept defaults if True (only valid when providing project_dir and session_id)
-        cookie_directory: name of the directory for your cookie (inside the repository or zip file).
-    Returns:
-        None
-    """
-
-    from cellpy.parameters import prms
-
-    if list_:
-        click.echo(f"\n[cellpy] batch templates")
-
-        default_template = _get_default_template()
-        local_templates = _read_local_templates()
-        local_templates_path = prmreader.prms.Paths.templatedir
-        registered_templates = prms._registered_templates
-        click.echo(f"[cellpy] - default: {default_template}")
-        click.echo("[cellpy] - registered templates (on github):")
-        for label, link in registered_templates.items():
-            click.echo(f"\t\t{label:18s} {link}")
-
-        if local_templates:
-            click.echo(f"[cellpy] - local templates ({local_templates_path}):")
-            for label, link in local_templates.items():
-                click.echo(f"\t\t{label:18s} {link}")
-        else:
-            click.echo(f"[cellpy] - local templates ({local_templates_path}): none")
-
-        return
-
-    if project_dir is None or session_id is None:
-        no_input = False
-
-    if not template:
-        template = _get_default_template()
-
-    if lab:
-        server = "lab"
-    else:
-        server = "notebook"
-
-    try:
-        import cookiecutter.exceptions
-        import cookiecutter.main
-        import cookiecutter.prompt
-
-    except ModuleNotFoundError:
-        click.echo("Could not import cookiecutter.")
-        click.echo("Try installing it, for example by writing:")
-        click.echo("\npip install cookiecutter\n")
-
-    click.echo(f"Template: {template}")
-    if local_user_template:
-        # forcing using local template
-        templates = _read_local_templates()
-
-        if not templates:
-            click.echo(
-                "You asked me to use a local template, but you have none. Aborting."
-            )
-            return
-    else:
-        templates = prms._registered_templates
-        if local_templates := _read_local_templates():
-            templates.update(local_templates)
-
-    if not template.lower() in templates.keys():
-        click.echo("This template does not exist. Aborting.")
-        return
-
-    if directory is None:
-        logging.debug("no dir given")
-        directory = prms.Paths.notebookdir
-
-    if not os.path.isdir(directory):
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(f" - {directory} does not exist")
-        return
-
-    directory = Path(directory)
-    selected_project_dir = None
-
-    if project_dir:
-        selected_project_dir = directory / project_dir
-        if not selected_project_dir.is_dir():
-            if cookiecutter.prompt.read_user_yes_no(
-                f"{project_dir} does not exist. Create?", "yes"
-            ):
-                os.mkdir(selected_project_dir)
-                click.echo(f"Created {selected_project_dir}")
-
-            else:
-                selected_project_dir = None
-                click.echo(f"Select another directory instead")
-
-    if not selected_project_dir:
-        project_dirs = [
-            d.name
-            for d in directory.iterdir()
-            if d.is_dir() and not d.name.startswith(".")
-        ]
-        project_dirs.insert(0, "[create new dir]")
-
-        project_dir = cookiecutter.prompt.read_user_choice(
-            "project folder", project_dirs
-        )
-
-        if project_dir == "[create new dir]":
-            default_name = "cellpy_project"
-            temp_default_name = default_name
-            for j in range(999):
-                if temp_default_name in project_dirs:
-                    temp_default_name = default_name + str(j + 1).zfill(3)
-                else:
-                    default_name = temp_default_name
-                    break
-
-            project_dir = cookiecutter.prompt.read_user_variable(
-                "New name", default_name
-            )
-            try:
-                os.mkdir(directory / project_dir)
-                click.echo(f"created {project_dir}")
-            except FileExistsError:
-                click.echo("OK - but this directory already exists!")
-        selected_project_dir = directory / project_dir
-
-    # get a list of all folders
-    existing_projects = os.listdir(selected_project_dir)
-
-    os.chdir(selected_project_dir)
-    cellpy_version = cellpy.__version__
-
-    try:
-        selected_template, cookie_dir = templates[template.lower()]
-
-        if cookie_directory:
-            cookie_dir = cookie_directory
-        if not cookie_dir:
-            cookie_dir = template.lower()
-
-        cookiecutter.main.cookiecutter(
-            selected_template,
-            extra_context={
-                "author_name": os.getlogin(),
-                "project_name": project_dir,
-                "cellpy_version": cellpy_version,
-                "session_id": session_id,
-            },
-            no_input=no_input,
-            directory=cookie_dir,
-        )
-    except cookiecutter.exceptions.OutputDirExistsException as e:
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(" - cookiecutter refused to create the project")
-        click.echo(e)
-
-    if serve_:
-        os.chdir(directory)
-        _serve(server)
-
-    if run_:
-        try:
-            import papermill as pm
-        except ImportError:
-            click.echo(
-                "[cellpy]: You need to install papermill for automatically execute the notebooks."
-            )
-            click.echo("[cellpy]: You can install it using pip like this:")
-            click.echo(" >> pip install papermill")
-            return
-        new_existing_projects = os.listdir(selected_project_dir)
-        our_new_projects = list(set(new_existing_projects) - set(existing_projects))
-
-        if not len(our_new_projects):
-            click.echo(
-                "[cellpy]: Sorry, could not deiced what is the new project "
-                "- so I don't dare to try to execute automatically."
-            )
-            return
-        our_new_project = selected_project_dir / our_new_projects[0]
-
-        _run_project(our_new_project)
-
-
-def _serve(server):
-    click.echo(f"serving with jupyter {server}")
-    subprocess.run(["jupyter", server], check=True)
-    click.echo("Finished serving.")
-
-
-# ----------------------- serve ---------------------------------------
-@click.command()
-@click.option("--lab", "-l", is_flag=True, help="Use Jupyter Lab instead of Notebook")
-@click.option("--directory", "-d", default=None, help="Start in custom directory DIR")
-def serve(lab, directory):
-    """Start a Jupyter server."""
-
-    from cellpy.parameters import prms
-
-    if directory is None:
-        directory = prms.Paths.notebookdir
-    elif directory == "home":
-        directory = Path().home()
-    elif directory == "here":
-        directory = Path(os.getcwd())
-
-    if not os.path.isdir(directory):
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(f" - {directory} does not exist")
-        return
-
-    if lab:
-        server = "lab"
-    else:
-        server = "notebook"
-
-    os.chdir(directory)
-    _serve(server)
-
-
-cli.add_command(setup)
-cli.add_command(info)
-cli.add_command(edit)
-cli.add_command(pull)
-cli.add_command(run)
-cli.add_command(new)
-cli.add_command(serve)
-
-
-# tests etc
-def _main_pull():
-    if sys.platform == "win32":
-        rootpath = pathlib.Path(r"C:\Temp\cellpy_user")
-    else:
-        rootpath = pathlib.Path("/Users/jepe/scripting/tmp/cellpy_test_user")
-    _pull_examples(rootpath, pw="env")
-    _pull_tests(rootpath, pw="env")
-    # _pull(gdirpath="examples", rootpath=rootpath, u="ask", pw="ask")
-    # _pull(gdirpath="tests", rootpath=rootpath, u="ask", pw="ask")
-    # _pull(gdirpath="testdata", rootpath=rootpath, u="ask", pw="ask")
-
-
-def _main():
-    file_name = prmreader.create_custom_init_filename()
-    click.echo(file_name)
-    user_directory, destination_file_name = prmreader.get_user_dir_and_dst(file_name)
-    click.echo(user_directory)
-    click.echo(destination_file_name)
-    click.echo("trying to save it")
-    save_prm_file(destination_file_name + "_dummy")
-
-    click.echo(" Testing setup ".center(80, "="))
-    setup(["--interactive", "--reset"])
-
-
-def _cli_setup_interactive():
-    from click.testing import CliRunner
-
-    if sys.platform == "win32":
-        root_dir = r"C:\Temp\cellpy_user"
-    else:
-        root_dir = "/Users/jepe/scripting/tmp/cellpy_test_user"
-    testuser = "tester"
-    init_filename = prmreader.create_custom_init_filename(testuser)
-    dst_file = get_dst_file(root_dir, init_filename)
-    init_file = pathlib.Path(dst_file)
-    opts = list()
-    opts.append("setup")
-    opts.append("-i")
-    # opts.append("-nr")
-    opts.append("-r")
-    opts.extend(["-d", root_dir])
-    opts.extend(["-t", testuser])
-
-    input_str = "\n"  # out
-    input_str += "\n"  # rawdatadir
-    input_str += "\n"  # cellpyfiles
-    input_str += "\n"  # log
-    input_str += "\n"  # examples
-    input_str += "\n"  # dbfolder
-    input_str += "\n"  # dbfile
-    runner = CliRunner()
-    result = runner.invoke(cli, opts, input=input_str)
-
-    click.echo(" out ".center(80, "."))
-    click.echo(result.output)
-    from pprint import pprint
-
-    pprint(prmreader.prms.Paths)
-    click.echo(" conf-file ".center(80, "."))
-    click.echo(init_file)
-    click.echo()
-    with init_file.open() as f:
-        for line in f.readlines():
-            click.echo(line.strip())
-
-
-def check_it(var=None):
-    import pathlib
-    import sys
-
-    p_env = pathlib.Path(sys.prefix)
-    print(p_env.name)
-    new(list_=True)
-
-
-if __name__ == "__main__":
-    u1 = os.getlogin()
-    u2 = os.path.expanduser("~")
-    u3 = os.environ.get("USERNAME")
-
-    print(u1)
-    print(u2)
-    print(u3)
-    # check_it()
-    # click.echo("\n\n", " RUNNING MAIN PULL ".center(80, "*"), "\n")
-    # _main_pull()
-    # click.echo("ok")
+import base64
+import getpass
+import logging
+import os
+import pathlib
+import platform
+from pprint import pprint
+import re
+import subprocess
+import sys
+from typing import Union
+import urllib
+from pathlib import Path
+
+import click
+import pkg_resources
+from github import Github
+
+import cellpy._version
+from cellpy.exceptions import ConfigFileNotWritten
+from cellpy.parameters import prmreader
+from cellpy.parameters.internal_settings import OTHERPATHS
+from cellpy.internals.core import OtherPath
+
+VERSION = cellpy._version.__version__
+REPO = "jepegit/cellpy"
+USER = "jepegit"
+GITHUB_PWD_VAR_NAME = "GD_PWD"
+DEFAULT_EDITOR = 'vim'
+EDITORS = {'Windows': 'notepad'}
+
+
+def save_prm_file(prm_filename):
+    """saves (writes) the prms to file"""
+    prmreader._write_prm_file(prm_filename)
+
+
+def get_package_prm_dir():
+    """gets the folder where the cellpy package lives"""
+    prm_dir = pkg_resources.resource_filename("cellpy", "parameters")
+    return pathlib.Path(prm_dir)
+
+
+def get_default_config_file_path(init_filename=None):
+    """gets the path to the default config-file"""
+    prm_dir = get_package_prm_dir()
+    if not init_filename:
+        init_filename = prmreader.DEFAULT_FILENAME
+    src = prm_dir / init_filename
+    return src
+
+
+def get_dst_file(user_dir, init_filename):
+    user_dir = pathlib.Path(user_dir)
+    dst_file = user_dir / init_filename
+    return dst_file
+
+
+def check_if_needed_modules_exists():
+    pass
+
+
+def modify_config_file():
+    pass
+
+
+def create_cellpy_folders():
+    pass
+
+
+@click.group("cellpy")
+def cli():
+    pass
+
+
+# ----------------------- setup --------------------------------------
+@click.command()
+@click.option(
+    "--interactive",
+    "-i",
+    is_flag=True,
+    default=False,
+    help="Allows you to specify div. folders and setting.",
+)
+@click.option(
+    "--not-relative",
+    "-nr",
+    is_flag=True,
+    default=False,
+    help="If root-dir is given, put it directly in the root (/) folder"
+    " i.e. don't put it in your home directory. Defaults to False. Remark"
+    " that if you specifically write a path name instead of selecting the"
+    " suggested default, the path you write will be used as is.",
+)
+@click.option(
+    "--dry-run",
+    "-dr",
+    is_flag=True,
+    default=False,
+    help="Run setup in dry mode (only print - do not execute). This is"
+    " typically used when developing and testing cellpy. Defaults to"
+    " False.",
+)
+@click.option(
+    "--reset",
+    "-r",
+    is_flag=True,
+    default=False,
+    help="Do not suggest path defaults based on your current configuration-file",
+)
+@click.option(
+    "--root-dir",
+    "-d",
+    default=None,
+    type=click.Path(),
+    help="Use custom root dir. If not given, your home directory"
+    " will be used as the top level where cellpy-folders"
+    " will be put. The folder path must follow"
+    " directly after this option (if used). Example:\n"
+    " $ cellpy setup -d 'MyDir'",
+)
+@click.option(
+    "--folder-name",
+    "-n",
+    default=None,
+    type=click.Path(),
+    help="",
+)
+@click.option(
+    "--test_user", "-t", default=None, help="Fake name for fake user (for testing)"
+)
+def setup(interactive, not_relative, dry_run, reset, root_dir, folder_name, test_user):
+    """This will help you to set up cellpy."""
+
+    click.echo("[cellpy] (setup)")
+    click.echo(f"[cellpy] root-dir: {root_dir}")
+
+    # generate variables
+    init_filename = prmreader.create_custom_init_filename()
+    user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
+
+    if dry_run:
+        click.echo("Create custom init filename and get user_dir and destination")
+        click.echo(f"Got the following parameters:")
+        click.echo(f" - init_filename: {init_filename}")
+        click.echo(f" - user_dir: {user_dir}")
+        click.echo(f" - dst_file: {dst_file}")
+        click.echo(f" - not_relative: {not_relative}")
+
+    if root_dir and not interactive:
+        click.echo("[cellpy] custom root-dir can only be used in interactive mode")
+        click.echo("[cellpy] -> setting interactive mode")
+        interactive = True
+
+    if not root_dir:
+        root_dir = user_dir
+        # root_dir = pathlib.Path(os.getcwd())
+    root_dir = pathlib.Path(root_dir)
+
+    if dry_run:
+        click.echo(f" - root_dir: {root_dir}")
+
+    if test_user:
+        click.echo(f"[cellpy] (setup) DEV-MODE test_user: {test_user}")
+        init_filename = prmreader.create_custom_init_filename(test_user)
+        user_dir = root_dir
+        dst_file = get_dst_file(user_dir, init_filename)
+        click.echo(f"[cellpy] (setup) DEV-MODE user_dir: {user_dir}")
+        click.echo(f"[cellpy] (setup) DEV-MODE dst_file: {dst_file}")
+
+    if not pathlib.Path(dst_file).is_file():
+        click.echo(f"[cellpy] {dst_file} not found -> I will make one for you!")
+        reset = True
+
+    if interactive:
+        click.echo(" interactive mode ".center(80, "-"))
+        _update_paths(
+            custom_dir=root_dir,
+            relative_home=not not_relative,
+            default_dir=folder_name,
+            dry_run=dry_run,
+            reset=reset,
+        )
+        _write_config_file(user_dir, dst_file, init_filename, dry_run)
+        _check(dry_run=dry_run)
+
+    else:
+        if reset:
+            _update_paths(
+                user_dir,
+                False,
+                default_dir=folder_name,
+                dry_run=dry_run,
+                reset=True,
+                silent=True,
+            )
+        _write_config_file(user_dir, dst_file, init_filename, dry_run)
+        _check(dry_run=dry_run)
+
+
+def _update_paths(
+    custom_dir=None,
+    relative_home=True,
+    reset=False,
+    dry_run=False,
+    default_dir=None,
+    silent=False,
+):
+    # please, refactor me :-(
+
+    h = prmreader.get_user_dir()
+
+    if default_dir is None:
+        default_dir = "cellpy_data"
+
+    if dry_run:
+        click.echo(f" - default_dir: {default_dir}")
+        click.echo(f" - custom_dir: {custom_dir}")
+        click.echo(f" - retalive_home: {relative_home}")
+
+    if custom_dir:
+        reset = True
+        if relative_home:
+            h = h / custom_dir
+        if not custom_dir.parts[-1] == default_dir:
+            h = h / default_dir
+
+    if not reset:
+        outdatadir = pathlib.Path(prmreader.prms.Paths.outdatadir)
+        rawdatadir = OtherPath(prmreader.prms.Paths.rawdatadir)
+        cellpydatadir = OtherPath(prmreader.prms.Paths.cellpydatadir)
+        filelogdir = pathlib.Path(prmreader.prms.Paths.filelogdir)
+        examplesdir = pathlib.Path(prmreader.prms.Paths.examplesdir)
+        db_path = pathlib.Path(prmreader.prms.Paths.db_path)
+        db_filename = prmreader.prms.Paths.db_filename
+        notebookdir = pathlib.Path(prmreader.prms.Paths.notebookdir)
+        batchfiledir = pathlib.Path(prmreader.prms.Paths.batchfiledir)
+        templatedir = pathlib.Path(prmreader.prms.Paths.templatedir)
+        instrumentdir = pathlib.Path(prmreader.prms.Paths.instrumentsdir)
+    else:
+        outdatadir = "out"
+        rawdatadir = "raw"
+        cellpydatadir = "cellpyfiles"
+        filelogdir = "logs"
+        examplesdir = "examples"
+        db_path = "db"
+        db_filename = "cellpy_db.xlsx"
+        notebookdir = "notebooks"
+        batchfiledir = "batchfiles"
+        templatedir = "templates"
+        instrumentdir = "instruments"
+
+    outdatadir = h / outdatadir
+    rawdatadir = h / rawdatadir
+    cellpydatadir = h / cellpydatadir
+    filelogdir = h / filelogdir
+    examplesdir = h / examplesdir
+    db_path = h / db_path
+    notebookdir = h / notebookdir
+    batchfiledir = h / batchfiledir
+    templatedir = h / templatedir
+    instrumentdir = h / instrumentdir
+
+    if dry_run:
+        click.echo(f" - base (h): {h}")
+
+    if not silent:
+        outdatadir = _ask_about_path(
+            "where to output processed data and results", outdatadir
+        )
+        rawdatadir = _ask_about_otherpath("where your raw data are located", rawdatadir)
+        cellpydatadir = _ask_about_otherpath("where to put cellpy-files", cellpydatadir)
+        filelogdir = _ask_about_path("where to dump the log-files", filelogdir)
+        examplesdir = _ask_about_path(
+            "where to download cellpy examples and tests", examplesdir
+        )
+        db_path = _ask_about_path("what folder your db file lives in", db_path)
+        db_filename = _ask_about_name("the name of your db-file", db_filename)
+        notebookdir = _ask_about_path(
+            "where to put your jupyter notebooks", notebookdir
+        )
+        batchfiledir = _ask_about_path("where to put your batch files", batchfiledir)
+        templatedir = _ask_about_path("where to put your batch files", templatedir)
+        instrumentdir = _ask_about_path("where to put your batch files", instrumentdir)
+
+    # update folders based on suggestions
+    for d in [
+        outdatadir,
+        rawdatadir,
+        cellpydatadir,
+        filelogdir,
+        examplesdir,
+        notebookdir,
+        db_path,
+        batchfiledir,
+        templatedir,
+        instrumentdir,
+    ]:
+        if not dry_run:
+            _create_dir(d)
+        else:
+            click.echo(f"dry run (so I did not create {d})")
+
+    # update config-file based on suggestions
+    prmreader.prms.Paths.outdatadir = str(outdatadir)
+    prmreader.prms.Paths.rawdatadir = str(rawdatadir)
+    prmreader.prms.Paths.cellpydatadir = str(cellpydatadir)
+    prmreader.prms.Paths.filelogdir = str(filelogdir)
+    prmreader.prms.Paths.examplesdir = str(examplesdir)
+    prmreader.prms.Paths.db_path = str(db_path)
+    prmreader.prms.Paths.db_filename = str(db_filename)
+    prmreader.prms.Paths.notebookdir = str(notebookdir)
+    prmreader.prms.Paths.batchfiledir = str(batchfiledir)
+    prmreader.prms.Paths.templatedir = str(templatedir)
+    prmreader.prms.Paths.instrumentdir = str(instrumentdir)
+
+
+def _ask_about_path(q, p):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {p}")
+    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_path:
+        new_path = p
+    return pathlib.Path(new_path)
+
+
+def _ask_about_otherpath(q, p):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {p}")
+    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_path:
+        new_path = p
+    return OtherPath(new_path)
+
+
+def _ask_about_name(q, n):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {n}")
+    new_name = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_name:
+        new_name = n
+    return new_name
+
+
+def _create_dir(path, confirm=True, parents=True, exist_ok=True):
+    if isinstance(path, OtherPath):
+        if path.is_external:
+            return path
+    o = path.resolve()
+    if not o.is_dir():
+        o_parent = o.parent
+        create_dir = True
+        if confirm:
+            if not o_parent.is_dir():
+                create_dir = input(
+                    f"\n[cellpy] (setup) {o_parent} does not exist. Create it [y]/n ?"
+                )
+                if not create_dir:
+                    create_dir = True
+                elif create_dir in ["y", "Y"]:
+                    create_dir = True
+                else:
+                    create_dir = False
+
+        if create_dir:
+            try:
+                o.mkdir(parents=parents, exist_ok=exist_ok)
+                click.echo(f"[cellpy] (setup) Created {o}")
+            except FileExistsError:
+                click.echo(f"[cellpy] (setup) {o} already exists.")
+            except FileNotFoundError:
+                click.echo(f"[cellpy] (setup) {o} not available.")
+            except Exception as e:
+                click.echo(f"[cellpy] (setup) WARNING! Could not create {o}.")
+                logging.debug(e)
+                click.echo(f"[cellpy] (setup) ...continuing anyway.")
+        else:
+            click.echo(f"[cellpy] (setup) Could not create {o}")
+    return o
+
+
+def _check_import_cellpy():
+    try:
+        import cellpy
+        from cellpy import log
+        from cellpy.readers import cellreader
+
+        return True
+    except:
+        return False
+
+
+def _check_import_pyodbc():
+    import platform
+
+    from cellpy.parameters import prms
+
+    ODBC = prms._odbc
+    SEARCH_FOR_ODBC_DRIVERS = prms._search_for_odbc_driver
+
+    use_subprocess = prms.Instruments.Arbin.use_subprocess
+    detect_subprocess_need = prms.Instruments.Arbin.detect_subprocess_need
+    click.echo(f" reading prms")
+    click.echo(f" - ODBC: {ODBC}")
+    click.echo(f" - SEARCH_FOR_ODBC_DRIVERS: {SEARCH_FOR_ODBC_DRIVERS}")
+    click.echo(f" - use_subprocess: {use_subprocess}")
+    click.echo(f" - detect_subprocess_need: {detect_subprocess_need}")
+    click.echo(f" - stated office version: {prms.Instruments.Arbin.office_version}")
+
+    click.echo(" checking system")
+    is_posix = False
+    is_macos = False
+    if os.name == "posix":
+        is_posix = True
+        click.echo(f" - running on posix")
+    current_platform = platform.system()
+    if current_platform == "Darwin":
+        is_macos = True
+        click.echo(f" - running on a mac")
+
+    python_version, os_version = platform.architecture()
+    click.echo(f" - python version: {python_version}")
+    click.echo(f" - os version: {os_version}")
+
+    if not is_posix:
+        if not prms.Instruments.Arbin.sub_process_path:
+            sub_process_path = str(prms._sub_process_path)
+        else:
+            sub_process_path = str(prms.Instruments.Arbin.sub_process_path)
+        click.echo(f" stated path to sub-process: {sub_process_path}")
+        if not os.path.isfile(sub_process_path):
+            click.echo(f" - OBS! missing")
+
+    if is_posix:
+        click.echo(" checking existence of mdb-export")
+        sub_process_path = "mdb-export"
+        from subprocess import PIPE, run
+
+        command = ["command", "-v", sub_process_path]
+
+        try:
+            result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+            if result.returncode == 0:
+                click.echo(f" - found it: {result.stdout}")
+            else:
+                click.echo(f" - failed finding it")
+
+            if is_macos:
+                driver = "/usr/local/lib/libmdbodbc.dylib"
+                click.echo(f" looks like you are on a mac (driver set to\n {driver})")
+                if not os.path.isfile(driver):
+                    click.echo(" - but cannot find it!")
+                    return False
+            return True
+
+        except AssertionError:
+            click.echo(" - not found")
+            return False
+
+    # not posix - checking for odbc drivers
+    # 1) checking if you have defined one
+    try:
+        driver = prms.Instruments.Arbin.odbc_driver
+        if not driver:
+            raise AttributeError
+        click.echo("You have defined an odbc driver in your conifg file")
+        click.echo(f"driver: {driver}")
+    except AttributeError:
+        click.echo("FYI: you have not defined any odbc_driver(s)")
+        click.echo(
+            "(The name of the driver from the configuration file is "
+            "used as a backup when cellpy cannot locate a driver by itself)"
+        )
+
+    use_ado = False
+
+    if ODBC == "ado":
+        use_ado = True
+        click.echo(" you stated that you prefer the ado loader")
+        click.echo(" checking if adodbapi is installed")
+        try:
+            import adodbapi as dbloader
+        except ImportError:
+            use_ado = False
+            click.echo(" Failed! Try setting pyodbc as your loader or install")
+            click.echo(" adodbapi (http://adodbapi.sourceforge.net/)")
+
+    if not use_ado:
+        if ODBC == "pyodbc":
+            click.echo(" you stated that you prefer the pyodbc loader")
+            try:
+                import pyodbc as dbloader
+            except ImportError:
+                click.echo(" Failed! Could not import it.")
+                click.echo(" Try 'pip install pyodbc'")
+                dbloader = None
+
+        elif ODBC == "pypyodbc":
+            click.echo(" you stated that you prefer the pypyodbc loader")
+            try:
+                import pypyodbc as dbloader
+            except ImportError:
+                click.echo(" Failed! Could not import it.")
+                click.echo(" try 'pip install pypyodbc'")
+                click.echo(" or set pyodbc as your loader in your prm file")
+                click.echo(" (and install it)")
+                dbloader = None
+
+    click.echo(" searching for odbc drivers")
+    try:
+        drivers = [
+            driver
+            for driver in dbloader.drivers()
+            if "Microsoft Access Driver" in driver
+        ]
+        click.echo(f"Found these: {drivers}")
+        driver = drivers[0]
+        click.echo(f"odbc driver: {driver}")
+        return True
+
+    except IndexError as e:
+        logging.debug("Unfortunately, it seems the list of drivers is emtpy.")
+        click.echo(
+            "\nCould not find any odbc-drivers suitable for .res-type files. "
+            "Check out the homepage of pydobc for info on installing drivers"
+        )
+        click.echo(
+            "One solution that might work is downloading "
+            "the Microsoft Access database engine "
+            "(in correct bytes (32 or 64)) "
+            "from:\n"
+            "https://www.microsoft.com/en-us/download/details.aspx?id=13255"
+        )
+        click.echo("Or install mdbtools and set it up (check the cellpy docs for help)")
+        click.echo("\n")
+        return False
+
+
+def _check_config_file():
+    prm_file_name = _configloc()
+    prm_dict = prmreader._read_prm_file_without_updating(prm_file_name)
+    try:
+        prm_paths = prm_dict["Paths"]
+        required_dirs = [
+            "cellpydatadir",
+            "examplesdir",
+            "filelogdir",
+            "notebookdir",
+            "outdatadir",
+            "rawdatadir",
+            "batchfiledir",
+            "templatedir",
+            "db_path",
+        ]
+        missing = 0
+        for k in required_dirs:
+            value = prm_paths.get(k, None)
+            click.echo(f"{k}: {value}")
+            # splitting this into two if-statements to make it easier to debug if OtherPath changes
+            if k in OTHERPATHS:
+                print(f"skipping check for external {k} (for now)")
+                # if not OtherPath(
+                #     value
+                # ).is_dir():  # Assuming OtherPath returns True if it is external.
+                #     missing += 1
+                #     click.echo("COULD NOT CONNECT!")
+                #     click.echo(f"({value} is not a directory)")
+            elif value and not pathlib.Path(value).is_dir():
+                missing += 1
+                click.echo("COULD NOT CONNECT!")
+                click.echo(f"({value} is not a directory)")
+            if not value:
+                missing += 1
+                click.echo("MISSING")
+
+        value = prm_paths.get("db_filename", None)
+        click.echo(f"db_filename: {value}")
+        if not value:
+            missing += 1
+            click.echo("MISSING")
+
+        if missing:
+            return False
+        else:
+            return True
+
+    except Exception as e:
+        click.echo("Following error occurred:")
+        click.echo(e)
+        return False
+
+
+def _check(dry_run=False):
+    click.echo(" checking ".center(80, "="))
+    if dry_run:
+        click.echo("*** dry-run: skipping the test")
+        return
+    failed_checks = 0
+    number_of_checks = 0
+
+    def sub_check(check_type, check_func):
+        failed = 0
+        click.echo(f"[cellpy] * - Checking {check_type}")
+        if check_func():
+            click.echo(f"[cellpy] -> succeeded!")
+        else:
+            click.echo("f[cellpy] -> failed!!!!")
+            failed = 1
+        click.echo(80 * "-")
+        return failed
+
+    check_types = ["cellpy imports", "importing pyodbc", "configuration (prm) file"]
+    check_funcs = [_check_import_cellpy, _check_import_pyodbc, _check_config_file]
+
+    for ct, cf in zip(check_types, check_funcs):
+        try:
+            failed_checks += sub_check(ct, cf)
+        except Exception as e:
+            click.echo(f"[cellpy] check raised an exception ({e})")
+        number_of_checks += 1
+    succeeded_checks = number_of_checks - failed_checks
+    if failed_checks > 0:
+        click.echo(f"[cellpy] OH NO!!! You (or I) failed!")
+        click.echo(f"[cellpy] Failed {failed_checks} out of {number_of_checks} checks.")
+    else:
+        click.echo(
+            f"[cellpy] Succeeded {succeeded_checks} out of {number_of_checks} checks."
+        )
+    click.echo(80 * "=")
+
+
+def _write_config_file(user_dir, dst_file, init_filename, dry_run):
+    click.echo(" update configuration ".center(80, "-"))
+    click.echo("[cellpy] (setup) Writing configurations to user directory:")
+    click.echo(f"\n         {user_dir}\n")
+
+    if os.path.isfile(dst_file):
+        click.echo("[cellpy] (setup) File already exists!")
+        click.echo("[cellpy] (setup) Keeping most of the old configuration parameters")
+    try:
+        if dry_run:
+            click.echo(
+                f"*** dry-run: skipping actual saving of {dst_file} ***", color="red"
+            )
+        else:
+            click.echo(f"[cellpy] (setup) Saving file ({dst_file})")
+            save_prm_file(dst_file)
+
+    except ConfigFileNotWritten:
+        click.echo("[cellpy] (setup) Something went wrong! Could not write the file")
+        click.echo(
+            "[cellpy] (setup) Trying to write a file"
+            + f"called {prmreader.DEFAULT_FILENAME} instead"
+        )
+
+        try:
+            user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
+            if dry_run:
+                click.echo(
+                    f"*** dry-run: skipping actual saving of {dst_file} ***",
+                    color="red",
+                )
+            else:
+                save_prm_file(dst_file)
+
+        except ConfigFileNotWritten:
+            _txt = "[cellpy] (setup) No, that did not work either.\n"
+            _txt += "[cellpy] (setup) Well, guess you have to talk to the developers."
+            click.echo(_txt)
+    else:
+        click.echo(f"[cellpy] (setup) Configuration file written!")
+        click.echo(
+            f"[cellpy] (setup) OK! Now you can edit it. For example by "
+            f"issuing \n\n         [your-favourite-editor] {init_filename}\n"
+        )
+
+
+def _get_default_editor():
+    """
+    Return the default text editor.
+
+    This code is based on the `editor` library by @rec.
+    """
+
+    return os.environ.get('VISUAL') or (
+        os.environ.get('EDITOR')
+        or EDITORS.get(platform.system(), DEFAULT_EDITOR)
+    )
+
+
+# ----------------------- edit ---------------------------------------
+@click.command()
+@click.option(
+    "--default-editor",
+    "-e",
+    default=None,
+    type=str,
+    help="try to use this editor instead",
+)
+@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
+@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
+@click.argument(
+    "name",
+    type=str,
+    default=None,
+    required=False,
+)
+def edit(name, default_editor, debug, silent):
+    """Edit your cellpy config or database files.
+
+    You can use this to edit the configuration file, the database file, or the
+    environment file. If you do not specify which file to edit, the configuration
+    file will be opened.
+
+    Examples:
+
+        edit your cellpy configuration file
+
+            cellpy edit config
+
+        or just
+
+            cellpy edit
+
+        edit your cellpy database file
+
+            cellpy edit db
+
+        edit your cellpy environment file using notepad.exe (on Windows)
+
+            cellpy edit env -e notepad.exe
+
+    """
+
+    if name.lower() == "db":
+        _run_db(debug, silent)
+        return
+
+    elif name.lower() not in ["env", "config"] and name is not None:
+        click.echo("unknown file")
+        return
+
+    if name is None or name.lower() == "config":
+        config_file = _configloc()
+        filename = str(config_file.resolve())
+        if config_file is None:
+            print("could not find the config file")
+            return
+    elif name.lower() == "env":
+        filename = _envloc()
+        if filename is None:
+            print("could not find the env file")
+            return
+    else:
+        filename = name
+
+    if default_editor is None:
+        default_editor = _get_default_editor()
+
+    args = [default_editor, filename]
+    click.echo(f"[cellpy] (edit) Calling '{default_editor}'")
+    try:
+        subprocess.call(args)
+    except:
+        click.echo(f"[cellpy] (edit) Failed!")
+        click.echo(
+            "[cellpy] (edit) Try 'cellpy edit -e notepad.exe' if you are on Windows"
+        )
+
+
+# ----------------------- info ---------------------------------------
+@click.command()
+@click.option("--version", "-v", is_flag=True, help="Print version information.")
+@click.option(
+    "--configloc", "-l", is_flag=True, help="Print full path to the config file."
+)
+@click.option("--params", "-p", is_flag=True, help="Dump all parameters to screen.")
+@click.option(
+    "--check",
+    "-c",
+    is_flag=True,
+    help="Do a sanity check to see if things" " works as they should.",
+)
+def info(version, configloc, params, check):
+    """This will give you some valuable information about your cellpy."""
+    complete_info = True
+
+    if check:
+        complete_info = False
+        _check()
+
+    if version:
+        complete_info = False
+        _version()
+
+    if configloc:
+        complete_info = False
+        _configloc()
+
+    if params:
+        complete_info = False
+        _dump_params()
+
+    if complete_info:
+        _version()
+        _configloc()
+
+
+# ----------------------- run ----------------------------------------
+@click.command()
+@click.option(
+    "--journal",
+    "-j",
+    is_flag=True,
+    help="Run a batch job defined in the given journal-file",
+)
+@click.option("--key", "-k", is_flag=True, help="Run a batch job defined by batch-name")
+@click.option(
+    "--folder",
+    "-f",
+    is_flag=True,
+    help="Run all batch jobs iteratively in a given folder",
+)
+@click.option(
+    "--cellpy-project",
+    "-p",
+    is_flag=True,
+    help="Use PaperMill to run the notebook(s) within the given project folder "
+    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'). "
+    "Warning! since we are using `click` - the NAME will be 'converted' when it is loaded "
+    "(same as print(name) does) - "
+    "so you can't use backslash ('\\') as normal in windows (use either '/' or '\\\\' instead).",
+)
+@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
+@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
+@click.option("--raw", is_flag=True, help="Force loading raw-file(s).")
+@click.option("--cellpyfile", is_flag=True, help="Force cellpy-file(s).")
+@click.option("--minimal", is_flag=True, help="Minimal processing.")
+@click.option(
+    "--nom-cap",
+    default=None,
+    type=float,
+    help="nominal capacity (used in calculating rates etc)",
+)
+@click.option(
+    "--batch_col",
+    default=None,
+    type=str,
+    help="batch column (if selecting running from db)",
+)
+@click.option(
+    "--project",
+    default=None,
+    type=str,
+    help="name of the project (if selecting running from db)",
+)
+@click.option("--list", "-l", "list_", is_flag=True, help="List batch-files.")
+@click.argument("name", default="NONE")
+def run(
+    journal,
+    key,
+    folder,
+    cellpy_project,
+    debug,
+    silent,
+    raw,
+    cellpyfile,
+    minimal,
+    nom_cap,
+    batch_col,
+    project,
+    list_,
+    name,
+):
+    """Run a cellpy process (e.g. a batch-job).
+
+    You can use this to launch specific applications.
+
+    Examples:
+
+        run a batch job described in a journal file
+
+           cellpy run -j my_experiment.json
+
+    """
+    if list_:
+        _run_list(name)
+        return
+
+    if name == "NONE":
+        click.echo(
+            "Usage: cellpy run [OPTIONS] NAME\n"
+            "Try 'cellpy run --help' for help.\n\n"
+            "Error: Missing argument 'NAME'."
+        )
+        sys.exit(-1)
+
+    if debug:
+        click.echo("[cellpy] (run) debug mode on")
+
+    if silent:
+        click.echo("[cellpy] (run) silent mode on")
+
+    click.echo("[cellpy]\n")
+
+    if cellpy_project:
+        _run_project(name)
+
+    elif journal:
+        _run_journal(name, debug, silent, raw, cellpyfile, minimal, nom_cap)
+
+    elif folder:
+        _run_journals(name, debug, silent, raw, cellpyfile, minimal)
+
+    elif key:
+        _run_from_db(
+            name,
+            debug,
+            silent,
+            raw,
+            cellpyfile,
+            minimal,
+            nom_cap,
+            batch_col,
+            project,
+        )
+
+    else:
+        _run(name, debug, silent)
+
+
+def _run_from_db(
+    name,
+    debug,
+    silent,
+    raw,
+    cellpyfile,
+    minimal,
+    nom_cap,
+    batch_col,
+    project,
+):
+    click.echo(
+        f"running from db \nkey={name}, batch_col={batch_col}, project={project}"
+    )
+
+    kwargs = dict()
+    kwargs["name"] = name
+
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    if batch_col is not None:
+        kwargs["batch_col"] = batch_col
+    if project is None:
+        kwargs["project"] = "various"
+    else:
+        kwargs["project"] = project
+
+    click.echo("Warming up ...")
+
+    from cellpy.utils import batch
+
+    click.echo("  - starting batch processing")
+    b = batch.process_batch(
+        force_raw_file=raw,
+        force_cellpy=cellpyfile,
+        nom_cap=nom_cap,
+        backend="matplotlib",
+        **kwargs,
+    )
+
+    if b is not None and not silent:
+        print(b)
+    click.echo("---")
+
+
+def _run_journal(file_name, debug, silent, raw, cellpyfile, minimal, nom_cap):
+    click.echo(f"running journal {file_name}")
+    # click.echo(f" --debug [{debug}]")
+    # click.echo(f" --silent [{silent}]")
+    # click.echo(f" --raw [{raw}]")
+    # click.echo(f" --cellpyfile [{cellpyfile}]")
+    # click.echo(f" --minimal [{minimal}]")
+    # click.echo(f" --nom_cap [{nom_cap}] {type(nom_cap)}")
+
+    kwargs = dict()
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    from cellpy import prms
+    from cellpy.utils import batch
+
+    batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
+    file = pathlib.Path(file_name)
+    if not file.is_file():
+        click.echo(f"file_name={file_name} not found - looking into batchfiledir")
+        if not batchfiledir.is_dir():
+            click.echo("batchfiledir not found - aborting")
+            return
+        file = batchfiledir / file.name
+
+    if not file.is_file():
+        click.echo(f"{file} not found - aborting")
+        return
+
+    b = batch.process_batch(
+        file,
+        force_raw_file=raw,
+        force_cellpy=cellpyfile,
+        nom_cap=nom_cap,
+        backend="matplotlib",
+        **kwargs,
+    )
+    if b is not None and not silent:
+        print(b)
+    click.echo("---")
+
+
+def _run_list(batchfiledir):
+    from cellpy import prms
+
+    if batchfiledir == "NONE" or batchfiledir is None:
+        batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
+    else:
+        batchfiledir = pathlib.Path(batchfiledir).resolve()
+
+    if batchfiledir.is_dir():
+        click.echo(f"Content of '{batchfiledir}':\n")
+        i = 0
+        for i, f in enumerate(batchfiledir.glob("cellpy*.json")):
+            click.echo(f"{f.name}")
+        if i:
+            print(f"\nnumber of batch-files located: {i}")
+        else:
+            print("No batch-files found in this directory.")
+    else:
+        click.echo(f"{batchfiledir} not found.")
+
+
+def _run_journals(folder_name, debug, silent, raw, cellpyfile, minimal):
+    click.echo(f"running journals in {folder_name}")
+    # click.echo(f" --debug [{debug}]")
+    # click.echo(f" --silent [{silent}]")
+    # click.echo(f" --raw [{raw}]")
+    # click.echo(f" --cellpyfile [{cellpyfile}]")
+    # click.echo(f" --minimal [{minimal}]")
+
+    kwargs = dict()
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    from cellpy.utils import batch
+
+    folder_name = pathlib.Path(folder_name).resolve()
+
+    if not folder_name.is_dir():
+        click.echo(f"{folder_name} not found - aborting")
+        return
+
+    batch.iterate_batches(
+        folder_name, force_raw_file=raw, force_cellpy=cellpyfile, silent=True, **kwargs
+    )
+    click.echo("---")
+
+
+def _run_project(our_new_project, **kwargs):
+    try:
+        import papermill as pm
+    except ImportError:
+        click.echo(
+            "[cellpy]: You need to install papermill for automatically execute the notebooks."
+        )
+        click.echo("[cellpy]: You can install it using pip like this:")
+        click.echo(" >> pip install papermill")
+        return
+    our_new_project = pathlib.Path(our_new_project)
+    click.echo(f"[cellpy]: trying to run notebooks in {our_new_project}")
+    notebooks = sorted(list(our_new_project.glob("*.ipynb")))
+    for notebook in notebooks:
+        click.echo(f"[cellpy - papermill] running {notebook.name}")
+        pm.execute_notebook(notebook, notebook, parameters=kwargs)
+
+
+def _run(name, debug, silent):
+    click.echo(f"running {name}")
+    click.echo(f" --debug [{debug}]")
+    click.echo(f" --silent [{silent}]")
+    click.echo("[cellpy]: sorry, I am not allowed to run this on my own")
+
+
+def _run_db(debug, silent):
+    import platform
+
+    from cellpy import prms
+
+    if not silent:
+        click.echo(f"running database editor")
+    if debug:
+        click.echo("running in debug-mode, but nothing to tell")
+
+    db_path = Path(prms.Paths.db_path) / prms.Paths.db_filename
+
+    if platform.system() == "Windows":
+        try:
+            os.system(f'start excel "{str(db_path)}"')
+        except Exception as e:
+            click.echo("Something went wrong trying to open")
+            click.echo(db_path)
+            print()
+            print(e)
+
+    elif platform.system() == "Linux":
+        click.echo("RUNNING LINUX")
+        # not tested
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+    elif platform.system() == "Darwin":
+        click.echo(f" - running on a mac")
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+    else:
+        print("RUNNING SOMETHING ELSE")
+        print(platform.system())
+        # not tested
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+
+# ----------------------- pull ---------------------------------------
+@click.command()
+@click.option("--tests", "-t", is_flag=True, help="Download test-files from repo.")
+@click.option(
+    "--examples", "-e", is_flag=True, help="Download example-files from repo."
+)
+@click.option("--clone", "-c", is_flag=True, help="Clone the full repo.")
+@click.option("--directory", "-d", default=None, help="Save into custom directory DIR")
+@click.option("--password", "-p", default=None, help="Password option for the repo")
+def pull(tests, examples, clone, directory, password):
+    """Download examples or tests from the big internet (needs git)."""
+    if directory is not None:
+        click.echo(f"[cellpy] (pull) custom directory: {directory}")
+    else:
+        directory = pathlib.Path(prmreader.prms.Paths.examplesdir)
+
+    if password is not None:
+        click.echo("DEV MODE: password provided")
+    if clone:
+        _clone_repo(directory, password)
+    else:
+        if tests:
+            _pull_tests(directory, password)
+        if examples:
+            _pull_examples(directory, password)
+        else:
+            click.echo(
+                f"[cellpy] (pull) Nothing selected for pulling. "
+                f"Please select an option (--tests,--examples, -clone, ...) "
+            )
+
+
+def _clone_repo(directory, password):
+    directory = pathlib.Path(directory)
+    txt = "[cellpy] The plan is that this "
+    txt += "[cellpy] cmd will pull (clone) the cellpy repo.\n"
+    txt += "[cellpy] For now it only prints the link to the git-hub\n"
+    txt += "[cellpy] repository:\n"
+    txt += "[cellpy]\n"
+    txt += "[cellpy] https://github.com/jepegit/cellpy.git\n"
+    txt += "[cellpy]\n"
+    click.echo(txt)
+
+
+def _pull_tests(directory, pw=None):
+    txt = (
+        "[cellpy] (pull) Pulling tests from",
+        " https://github.com/jepegit/cellpy.git",
+    )
+    click.echo(txt)
+    _pull(gdirpath="tests", rootpath=directory, pw=pw)
+    _pull(gdirpath="testdata", rootpath=directory, pw=pw)
+
+
+def _pull_examples(directory, pw):
+    txt = (
+        "[cellpy] (pull) Pulling examples from",
+        " https://github.com/jepegit/cellpy.git",
+    )
+    click.echo(txt)
+    _pull(gdirpath="examples", rootpath=directory, pw=pw)
+
+
+def _version():
+    txt = "[cellpy] version: " + str(VERSION)
+    click.echo(txt)
+
+
+def _configloc():
+    _, config_file_name = prmreader.get_user_dir_and_dst()
+    click.echo("[cellpy] ->%s" % config_file_name)
+    if not os.path.isfile(config_file_name):
+        click.echo("[cellpy] File does not exist!")
+    else:
+        return config_file_name
+
+
+def _envloc():
+    click.echo(f"[cellpy] ->{prmreader.get_env_file_name()}")
+    if not os.path.isfile(prmreader.get_env_file_name()):
+        click.echo("[cellpy] File does not exist!")
+    else:
+        return prmreader.get_env_file_name()
+
+
+def _dump_params():
+    click.echo("[cellpy] Dumping parameters to screen:\n")
+    prmreader.info()
+
+
+def _download_g_blob(name, local_path):
+    import urllib.request
+
+    dirs = local_path.parent
+    if not dirs.is_dir():
+        click.echo(f"[cellpy] (pull) creating dir: {dirs}")
+        dirs.mkdir(parents=True)
+
+    filename, headers = urllib.request.urlretrieve(
+        name.download_url, filename=local_path
+    )
+    click.echo(f"[cellpy] (pull) downloaded blob: {filename}")
+
+
+def _parse_g_dir(repo, gdirpath):
+    """parses a repo directory two-levels deep"""
+    for f in repo.get_contents(gdirpath):
+        if f.type == "dir":
+            for sf in repo.get_contents(f.path):
+                yield sf
+        else:
+            yield f
+
+
+def _get_user_name():
+    return "jepegit"
+
+
+def _get_pw(method):
+    if method == "ask":
+        return getpass.getpass()
+    elif method == "env":
+        return os.environ.get(GITHUB_PWD_VAR_NAME, None)
+
+    else:
+        return None
+
+
+def _pull(gdirpath="examples", rootpath=None, u=None, pw=None):
+    if rootpath is None:
+        rootpath = prmreader.prms.Paths.examplesdir
+
+    rootpath = pathlib.Path(rootpath)
+
+    ndirpath = rootpath / gdirpath
+
+    if pw is not None:
+        click.echo(" DEV MODE ".center(80, "-"))
+        u = _get_user_name()
+        if pw == "ask":
+            click.echo("   - ask for password")
+            pw = _get_pw(pw)
+        elif pw == "env":
+            click.echo("   - check environ for password ")
+            pw = _get_pw(pw)
+            click.echo("   - got something")
+            if pw is None:
+                click.echo("   - only None")
+                u = None
+
+    g = Github(u, pw)
+    repo = g.get_repo(REPO)
+
+    click.echo(f"[cellpy] (pull) pulling {gdirpath}")
+    click.echo(f"[cellpy] (pull) -> {ndirpath}")
+
+    if not ndirpath.is_dir():
+        click.echo(f"[cellpy] (pull) creating dir: {ndirpath}")
+        ndirpath.mkdir(parents=True)
+
+    for gfile in _parse_g_dir(repo, gdirpath):
+        gfilename = pathlib.Path(gfile.path)
+        nfilename = rootpath / gfilename
+
+        _download_g_blob(gfile, nfilename)
+
+
+def _get_default_template():
+    template = "standard"
+    try:
+        template = prmreader.prms.Batch.template
+    except:
+        logging.debug("You dont have any default template defined in you .conf file")
+    return template
+
+
+def _read_local_templates(local_templates_path=None):
+    if local_templates_path is None:
+        local_templates_path = pathlib.Path(prmreader.prms.Paths.templatedir)
+    templates = {}
+    for p in list(local_templates_path.rglob("cellpy_cookie*.zip")):
+        label = p.stem.strip()[len("cellpy_cookie_") :]
+        templates[label] = (str(p), None)
+    logging.debug(f"Found the following templates: {templates}")
+    return templates
+
+
+# ----------------------- new ----------------------------------------
+@click.command()
+@click.option("--template", "-t", help="Provide template name.")
+@click.option("--directory", "-d", default=None, help="Create in custom directory.")
+@click.option(
+    "--project",
+    "-p",
+    default=None,
+    help="Provide project name (i.e. sub-directory name).",
+)
+@click.option(
+    "--experiment",
+    "-e",
+    default=None,
+    help="Provide experiment name (i.e. lookup-value).",
+)
+@click.option(
+    "--local-user-template",
+    "-u",
+    is_flag=True,
+    default=False,
+    help="Use local template from the templates directory.",
+)
+@click.option("--serve", "-s", "serve_", is_flag=True, help="Run Jupyter.")
+@click.option(
+    "--run",
+    "-r",
+    "run_",
+    is_flag=True,
+    help="Use PaperMill to run the notebook(s) from the template "
+    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'.",
+)
+@click.option(
+    "--lab",
+    "-j",
+    is_flag=True,
+    help="Use Jupyter Lab instead of Notebook when serving.",
+)
+@click.option(
+    "--list", "-l", "list_", is_flag=True, help="List available templates and exit."
+)
+def new(
+    template,
+    directory,
+    project,
+    experiment,
+    local_user_template,
+    serve_,
+    run_,
+    lab,
+    list_,
+):
+    """Set up a batch experiment (might need git installed)."""
+    _new(
+        template,
+        directory=directory,
+        project_dir=project,
+        session_id=experiment,
+        local_user_template=local_user_template,
+        serve_=serve_,
+        run_=run_,
+        lab=lab,
+        list_=list_,
+    )
+
+
+def _new(
+    template: str,
+    directory: Union[Path, str, None] = None,
+    project_dir: Union[str, None] = None,
+    local_user_template: bool = False,
+    serve_: bool = False,
+    run_: bool = False,
+    lab: bool = False,
+    list_: bool = False,
+    session_id: str = "experiment_001",
+    no_input: bool = False,
+    cookie_directory: str = "",
+):
+    """Set up a batch experiment (might need git installed).
+
+    Args:
+        template: short-name of template.
+        directory: the directory for your cellpy projects.
+        local_user_template: use local template if True.
+        serve_: serve the notebook after creation if True.
+        run_: run the notebooks using papermill if True.
+        lab: use jupyter-lab instead of jupyter notebook if True.
+        list_: list all available templates and return if True.
+        project_dir: your project directory.
+        session_id: the lookup value.
+        no_input: accept defaults if True (only valid when providing project_dir and session_id)
+        cookie_directory: name of the directory for your cookie (inside the repository or zip file).
+    Returns:
+        None
+    """
+
+    from cellpy.parameters import prms
+
+    if list_:
+        click.echo(f"\n[cellpy] batch templates")
+
+        default_template = _get_default_template()
+        local_templates = _read_local_templates()
+        local_templates_path = prmreader.prms.Paths.templatedir
+        registered_templates = prms._registered_templates
+        click.echo(f"[cellpy] - default: {default_template}")
+        click.echo("[cellpy] - registered templates (on github):")
+        for label, link in registered_templates.items():
+            click.echo(f"\t\t{label:18s} {link}")
+
+        if local_templates:
+            click.echo(f"[cellpy] - local templates ({local_templates_path}):")
+            for label, link in local_templates.items():
+                click.echo(f"\t\t{label:18s} {link}")
+        else:
+            click.echo(f"[cellpy] - local templates ({local_templates_path}): none")
+
+        return
+
+    if project_dir is None or session_id is None:
+        no_input = False
+
+    if not template:
+        template = _get_default_template()
+
+    if lab:
+        server = "lab"
+    else:
+        server = "notebook"
+
+    try:
+        import cookiecutter.exceptions
+        import cookiecutter.main
+        import cookiecutter.prompt
+
+    except ModuleNotFoundError:
+        click.echo("Could not import cookiecutter.")
+        click.echo("Try installing it, for example by writing:")
+        click.echo("\npip install cookiecutter\n")
+
+    click.echo(f"Template: {template}")
+    if local_user_template:
+        # forcing using local template
+        templates = _read_local_templates()
+
+        if not templates:
+            click.echo(
+                "You asked me to use a local template, but you have none. Aborting."
+            )
+            return
+    else:
+        templates = prms._registered_templates
+        if local_templates := _read_local_templates():
+            templates.update(local_templates)
+
+    if not template.lower() in templates.keys():
+        click.echo("This template does not exist. Aborting.")
+        return
+
+    if directory is None:
+        logging.debug("no dir given")
+        directory = prms.Paths.notebookdir
+
+    if not os.path.isdir(directory):
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(f" - {directory} does not exist")
+        return
+
+    directory = Path(directory)
+    selected_project_dir = None
+
+    if project_dir:
+        selected_project_dir = directory / project_dir
+        if not selected_project_dir.is_dir():
+            if cookiecutter.prompt.read_user_yes_no(
+                f"{project_dir} does not exist. Create?", "yes"
+            ):
+                os.mkdir(selected_project_dir)
+                click.echo(f"Created {selected_project_dir}")
+
+            else:
+                selected_project_dir = None
+                click.echo(f"Select another directory instead")
+
+    if not selected_project_dir:
+        project_dirs = [
+            d.name
+            for d in directory.iterdir()
+            if d.is_dir() and not d.name.startswith(".")
+        ]
+        project_dirs.insert(0, "[create new dir]")
+
+        project_dir = cookiecutter.prompt.read_user_choice(
+            "project folder", project_dirs
+        )
+
+        if project_dir == "[create new dir]":
+            default_name = "cellpy_project"
+            temp_default_name = default_name
+            for j in range(999):
+                if temp_default_name in project_dirs:
+                    temp_default_name = default_name + str(j + 1).zfill(3)
+                else:
+                    default_name = temp_default_name
+                    break
+
+            project_dir = cookiecutter.prompt.read_user_variable(
+                "New name", default_name
+            )
+            try:
+                os.mkdir(directory / project_dir)
+                click.echo(f"created {project_dir}")
+            except FileExistsError:
+                click.echo("OK - but this directory already exists!")
+        selected_project_dir = directory / project_dir
+
+    # get a list of all folders
+    existing_projects = os.listdir(selected_project_dir)
+
+    os.chdir(selected_project_dir)
+    cellpy_version = cellpy.__version__
+
+    try:
+        selected_template, cookie_dir = templates[template.lower()]
+
+        if cookie_directory:
+            cookie_dir = cookie_directory
+        if not cookie_dir:
+            cookie_dir = template.lower()
+
+        cookiecutter.main.cookiecutter(
+            selected_template,
+            extra_context={
+                "author_name": os.getlogin(),
+                "project_name": project_dir,
+                "cellpy_version": cellpy_version,
+                "session_id": session_id,
+            },
+            no_input=no_input,
+            directory=cookie_dir,
+        )
+    except cookiecutter.exceptions.OutputDirExistsException as e:
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(" - cookiecutter refused to create the project")
+        click.echo(e)
+
+    if serve_:
+        os.chdir(directory)
+        _serve(server)
+
+    if run_:
+        try:
+            import papermill as pm
+        except ImportError:
+            click.echo(
+                "[cellpy]: You need to install papermill for automatically execute the notebooks."
+            )
+            click.echo("[cellpy]: You can install it using pip like this:")
+            click.echo(" >> pip install papermill")
+            return
+        new_existing_projects = os.listdir(selected_project_dir)
+        our_new_projects = list(set(new_existing_projects) - set(existing_projects))
+
+        if not len(our_new_projects):
+            click.echo(
+                "[cellpy]: Sorry, could not deiced what is the new project "
+                "- so I don't dare to try to execute automatically."
+            )
+            return
+        our_new_project = selected_project_dir / our_new_projects[0]
+
+        _run_project(our_new_project)
+
+
+def _serve(server):
+    click.echo(f"serving with jupyter {server}")
+    subprocess.run(["jupyter", server], check=True)
+    click.echo("Finished serving.")
+
+
+# ----------------------- serve ---------------------------------------
+@click.command()
+@click.option("--lab", "-l", is_flag=True, help="Use Jupyter Lab instead of Notebook")
+@click.option("--directory", "-d", default=None, help="Start in custom directory DIR")
+def serve(lab, directory):
+    """Start a Jupyter server."""
+
+    from cellpy.parameters import prms
+
+    if directory is None:
+        directory = prms.Paths.notebookdir
+    elif directory == "home":
+        directory = Path().home()
+    elif directory == "here":
+        directory = Path(os.getcwd())
+
+    if not os.path.isdir(directory):
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(f" - {directory} does not exist")
+        return
+
+    if lab:
+        server = "lab"
+    else:
+        server = "notebook"
+
+    os.chdir(directory)
+    _serve(server)
+
+
+cli.add_command(setup)
+cli.add_command(info)
+cli.add_command(edit)
+cli.add_command(pull)
+cli.add_command(run)
+cli.add_command(new)
+cli.add_command(serve)
+
+
+# tests etc
+def _main_pull():
+    if sys.platform == "win32":
+        rootpath = pathlib.Path(r"C:\Temp\cellpy_user")
+    else:
+        rootpath = pathlib.Path("/Users/jepe/scripting/tmp/cellpy_test_user")
+    _pull_examples(rootpath, pw="env")
+    _pull_tests(rootpath, pw="env")
+    # _pull(gdirpath="examples", rootpath=rootpath, u="ask", pw="ask")
+    # _pull(gdirpath="tests", rootpath=rootpath, u="ask", pw="ask")
+    # _pull(gdirpath="testdata", rootpath=rootpath, u="ask", pw="ask")
+
+
+def _main():
+    file_name = prmreader.create_custom_init_filename()
+    click.echo(file_name)
+    user_directory, destination_file_name = prmreader.get_user_dir_and_dst(file_name)
+    click.echo(user_directory)
+    click.echo(destination_file_name)
+    click.echo("trying to save it")
+    save_prm_file(destination_file_name + "_dummy")
+
+    click.echo(" Testing setup ".center(80, "="))
+    setup(["--interactive", "--reset"])
+
+
+def _cli_setup_interactive():
+    from click.testing import CliRunner
+
+    if sys.platform == "win32":
+        root_dir = r"C:\Temp\cellpy_user"
+    else:
+        root_dir = "/Users/jepe/scripting/tmp/cellpy_test_user"
+    testuser = "tester"
+    init_filename = prmreader.create_custom_init_filename(testuser)
+    dst_file = get_dst_file(root_dir, init_filename)
+    init_file = pathlib.Path(dst_file)
+    opts = list()
+    opts.append("setup")
+    opts.append("-i")
+    # opts.append("-nr")
+    opts.append("-r")
+    opts.extend(["-d", root_dir])
+    opts.extend(["-t", testuser])
+
+    input_str = "\n"  # out
+    input_str += "\n"  # rawdatadir
+    input_str += "\n"  # cellpyfiles
+    input_str += "\n"  # log
+    input_str += "\n"  # examples
+    input_str += "\n"  # dbfolder
+    input_str += "\n"  # dbfile
+    runner = CliRunner()
+    result = runner.invoke(cli, opts, input=input_str)
+
+    click.echo(" out ".center(80, "."))
+    click.echo(result.output)
+    from pprint import pprint
+
+    pprint(prmreader.prms.Paths)
+    click.echo(" conf-file ".center(80, "."))
+    click.echo(init_file)
+    click.echo()
+    with init_file.open() as f:
+        for line in f.readlines():
+            click.echo(line.strip())
+
+
+def check_it(var=None):
+    import pathlib
+    import sys
+
+    p_env = pathlib.Path(sys.prefix)
+    print(p_env.name)
+    new(list_=True)
+
+
+if __name__ == "__main__":
+    u1 = os.getlogin()
+    u2 = os.path.expanduser("~")
+    u3 = os.environ.get("USERNAME")
+
+    print(u1)
+    print(u2)
+    print(u3)
+    # check_it()
+    # click.echo("\n\n", " RUNNING MAIN PULL ".center(80, "*"), "\n")
+    # _main_pull()
+    # click.echo("ok")
```

### Comparing `cellpy-1.0.0a8/cellpy/exceptions.py` & `cellpy-1.0.0a9/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/internals/core.py` & `cellpy-1.0.0a9/cellpy/internals/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/log.py` & `cellpy-1.0.0a9/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/logging.json` & `cellpy-1.0.0a9/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.0a9/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/parameters/internal_settings.py` & `cellpy-1.0.0a9/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.0a9/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/parameters/prmreader.py` & `cellpy-1.0.0a9/cellpy/parameters/prmreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,19 @@
 
 def _save_current_prms_to_user_dir():
     # This should be put into the cellpy setup script
     file_name = os.path.join(prms.user_dir, prms._prm_default_name)  # NOQA
     _write_prm_file(file_name)
 
 
+def get_env_file_name():
+    """returns the location of the env-file"""
+    return pathlib.Path(prms.Paths.env_file)
+
+
 def info():
     """this function will show only the 'box'-type
     attributes and their content in the cellpy.prms module"""
     print("Convenience function for listing prms")
     print(prms.__name__)
     print(f"prm file (for current user): {_get_prm_file()}")
     print()
```

### Comparing `cellpy-1.0.0a8/cellpy/parameters/prms.py` & `cellpy-1.0.0a9/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/cellreader.py` & `cellpy-1.0.0a9/cellpy/readers/cellreader.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,38 +194,41 @@
         selected_scans=None,
         profile=False,
         filestatuschecker=None,  # "modified"
         tester=None,
         initialize=False,
         cellpy_units=None,
         output_units=None,
+        debug=False,
     ):
         """CellpyCell object
 
         Args:
             filenames: list of files to load.
             selected_scans:
             profile: experimental feature.
             filestatuschecker: property to compare cellpy and raw-files;
                default read from prms-file.
             tester: instrument used (e.g. "arbin_res") (checks prms-file as
                default).
             initialize: create a dummy (empty) dataset; defaults to False.
             cellpy_units (dict): sent to cellpy.parameters.internal_settings.get_cellpy_units
             output_units (dict): sent to cellpy.parameters.internal_settings.get_default_output_units
+            debug (bool): set to True if you want to see debug messages.
         """
 
         # TODO v 1.1: move to data (allow for multiple testers for same cell)
         if tester is None:
             self.tester = prms.Instruments.tester
             logging.debug(f"reading instrument from prms: {prms.Instruments}")
         else:
             self.tester = tester
 
         self.loader = None  # this will be set in the function set_instrument
+        self.debug = debug
         logging.debug("created CellpyCell instance")
 
         self._session_name = None
         self.profile = profile
 
         self.minimum_selection = {}
         self.filestatuschecker = filestatuschecker or prms.Reader.filestatuschecker
@@ -261,14 +264,15 @@
             "not_known",
         ]
         # - options
         self.force_step_table_creation = prms.Reader.force_step_table_creation
         self.force_all = prms.Reader.force_all
         self.sep = prms.Reader.sep
         self._cycle_mode = None
+        self._nom_cap_specifics = prms.Materials.default_nom_cap_specifics
         self.select_minimal = prms.Reader.select_minimal
         self.limit_loaded_cycles = prms.Reader.limit_loaded_cycles
         self.limit_data_points = None
         self.ensure_step_table = prms.Reader.ensure_step_table
         self.ensure_summary_table = prms.Reader.ensure_summary_table
         self.raw_datadir = OtherPath(prms.Paths.rawdatadir)
         self.cellpy_datadir = OtherPath(prms.Paths.cellpydatadir)
@@ -323,14 +327,77 @@
             return
         if self.session_name and not override:
             return
         path = Path(filename)
         self.session_name = path.with_suffix("").name
 
     @property
+    def mass(self):
+        """returns the mass"""
+        return self.data.mass
+
+    @mass.setter
+    def mass(self, m):
+        self.data.mass = self._dump_cellpy_unit(m, "mass")
+
+    @property
+    def active_electrode_area(self):
+        """returns the area"""
+        return self.data.active_electrode_area
+
+    @active_electrode_area.setter
+    def active_electrode_area(self, a):
+        self.data.active_electrode_area = self._dump_cellpy_unit(a, "area")
+
+    @property
+    def nom_cap(self):
+        """returns the nominal capacity"""
+        return self.data.nom_cap
+
+    @nom_cap.setter
+    def nom_cap(self, c):
+        self.data.nom_cap = self._dump_cellpy_unit(c, "nominal_capacity")
+
+    def _dump_cellpy_unit(self, value, parameter):
+        """Parse for unit, update cellpy_units class, and return magnitude."""
+        if isinstance(value, numbers.Number):
+            return value
+        logging.debug(f"Parsing {parameter} ({value})")
+        try:
+            c = Q(value)
+            c_unit = c.units
+            self.cellpy_units[parameter] = f"{c_unit}"
+            c = c.magnitude
+        except ValueError:
+            logging.debug(f"Could not parse {value}")
+            return
+        return c
+
+    @property
+    def nom_cap_specifics(self):
+        """returns the nominal capacity specific"""
+        return self._nom_cap_specifics
+
+    # NEXT: update make_summary and make_step_table to use this. And update get() to use this.
+
+    @nom_cap_specifics.setter
+    def nom_cap_specifics(self, c):
+        if c.lower() == "areal":
+            self.cellpy_units.nominal_capacity = f"{self.cellpy_units.charge}/{self.cellpy_units.specific_areal}"
+        elif c.lower() == "gravimetric":
+            self.cellpy_units.nominal_capacity = f"{self.cellpy_units.charge}/{self.cellpy_units.specific_gravimetric}"
+        elif c.lower() == "volumetric":
+            self.cellpy_units.nominal_capacity = f"{self.cellpy_units.charge}/{self.cellpy_units.specific_volumetric}"
+        else:
+            logging.warning(f"Unknown nominal capacity specific: {c}")
+            return
+
+        self._nom_cap_specifics = c
+
+    @property
     def raw_units(self):
         """returns the raw_units dictionary"""
 
         return self.data.raw_units
 
     @property
     def data(self):
@@ -2550,15 +2617,15 @@
         """
         # TODO: @jepe - include option for omitting steps
         # TODO: @jepe  - make it is possible to update only new data
 
         time_00 = time.time()
 
         if nom_cap_specifics is None:
-            nom_cap_specifics = prms.Materials.default_nom_cap_specifics
+            nom_cap_specifics = self.nom_cap_specifics
 
         if profiling:
             print("PROFILING MAKE_STEP_TABLE".center(80, "="))
 
         def first(x):
             return x.iloc[0]
 
@@ -4518,26 +4585,36 @@
     def nominal_capacity_as_absolute(
         self,
         value=None,
         specific=None,
         nom_cap_specifics=None,
         convert_charge_units=False,
     ):
+        """Get the nominal capacity as absolute value."""
+
         # TODO: implement handling of edge-cases (i.e. the raw capacity is not in absolute values)
+        if self.debug:
+            print("nominal_capacity_as_absolute".center(80, "="))
+            print(f"{value=}")
+            print(f"{specific=}")
+            print(f"{nom_cap_specifics=}")
+            print(f"{convert_charge_units=}")
+            print(80 * "-")
         if nom_cap_specifics is None:
             nom_cap_specifics = "gravimetric"
 
         if specific is None:
             if nom_cap_specifics == "gravimetric":
                 specific = self.data.mass
             elif nom_cap_specifics == "areal":
                 specific = self.data.active_electrode_area
 
         if value is None:
             value = self.data.nom_cap
+
         value = Q(value, self.cellpy_units["nominal_capacity"])
 
         if nom_cap_specifics == "gravimetric":
             specific = Q(specific, self.cellpy_units["mass"])
         elif nom_cap_specifics == "areal":
             specific = Q(specific, self.cellpy_units["area"])
 
@@ -4547,14 +4624,21 @@
             )
         else:
             conversion_factor_charge = 1.0
 
         absolute_value = (
             (value * conversion_factor_charge * specific).to_reduced_units().to("Ah")
         )
+        if self.debug:
+            print(f"{self.mass=}")
+            print(f"{self.active_electrode_area=}")
+            print(f"{self.nom_cap=}")
+            print(f"{self.cellpy_units=}")
+            print(f"nominal capacity: {value} [{self.cellpy_units.nominal_capacity}] -> {absolute_value:.3f} [Ah]")
+            print(80 * "=")
         return absolute_value.m
 
     def with_cellpy_unit(self, parameter, as_str=False):
         """Return quantity as `pint.Quantity` object."""
         _look_up = {
             "nom_cap": "nominal_capacity",
             "active_electrode_area": "area",
@@ -4906,15 +4990,15 @@
         find_end_voltage=True,
         use_cellpy_stat_file=None,
         # all_tests=True,
         ensure_step_table=True,
         # add_c_rate=True,
         normalization_cycles=None,
         nom_cap=None,
-        nom_cap_specifics="gravimetric",
+        nom_cap_specifics=None,
         # from_cycle=None,
     ):
         """Convenience function that makes a summary of the cycling data."""
         # TODO: @jepe - include option for omitting steps
         # TODO: @jepe  - make it is possible to update only new data by implementing
         #  from_cycle (only calculate summary from a given cycle number).
         #  Probably best to keep the old summary and make
@@ -5024,14 +5108,16 @@
         # RIC_disconnect = charge_cap[n-1] - charge_cap[n] / charge_cap[n-1]
 
         # --------- notes --------------------------------------------------------
         # @jepe 2022.09.11: trying to use .assign from now on
         #   as it is recommended (but this will likely increase memory usage)
 
         # TODO: add this to arguments and possible prms:
+        if nom_cap_specifics is None:
+            nom_cap_specifics = self.nom_cap_specifics
         specifics = ["gravimetric", "areal"]
         cycle_index_as_index = True
         time_00 = time.time()
         logging.debug("start making summary")
 
         cell = self.data
         if not mass:
@@ -5726,28 +5812,30 @@
 
 def get(
     filename=None,
     instrument=None,
     instrument_file=None,
     cellpy_file=None,
     cycle_mode=None,
-    mass=None,
-    nominal_capacity=None,
+    mass: Union[str, numbers.Number] = None,
+    nominal_capacity: Union[str, numbers.Number] = None,
+    nom_cap_specifics=None,
     loading=None,
-    area=None,
+    area: Union[str, numbers.Number] = None,
     estimate_area=True,
     logging_mode=None,
     auto_pick_cellpy_format=True,
     auto_summary=True,
     units=None,
     step_kwargs=None,
     summary_kwargs=None,
     selector=None,
     testing=False,
     refuse_copying=False,
+    debug=False,
     **kwargs,
 ):
     """Create a CellpyCell object
 
     Args:
         filename (str, os.PathLike, OtherPath, or list of raw-file names): path to file(s) to load
         instrument (str): instrument to use (defaults to the one in your cellpy config file)
@@ -5756,25 +5844,27 @@
             is provided, cellpy will try to check if the raw-file is has been updated since the
             creation of the cellpy-file and select this instead of the raw file if cellpy thinks
             they are similar (use with care!).
         logging_mode (str): "INFO" or "DEBUG"
         cycle_mode (str): the cycle mode (e.g. "anode" or "full_cell")
         mass (float): mass of active material (mg) (defaults to mass given in cellpy-file or 1.0)
         nominal_capacity (float): nominal capacity for the cell (e.g. used for finding C-rates)
+        nom_cap_specifics (str): either "gravimetric" (pr mass), "areal" (per area), or "volumetric" (per volume)
         loading (float): loading in units [mass] / [area]
         area (float): active electrode area (e.g. used for finding the areal capacity)
         estimate_area (bool): calculate area from loading if given (defaults to True)
         auto_pick_cellpy_format (bool): decide if it is a cellpy-file based on suffix.
         auto_summary (bool): (re-) create summary.
         units (dict): update cellpy units (used after the file is loaded, e.g. when creating summary).
         step_kwargs (dict): sent to make_steps
         summary_kwargs (dict): sent to make_summary
         selector (dict): passed to load (when loading cellpy-files).
         testing (bool): set to True if testing (will for example prevent making .log files)
         refuse_copying (bool): set to True if you do not want to copy the raw-file before loading.
+        debug (bool): set to True if you want to debug the loader.
         **kwargs: sent to the loader
 
     Returns:
         CellpyCell object (if successful, None if not)
 
     Examples:
         >>> # read an arbin .res file and create a cellpy object with
@@ -5809,29 +5899,30 @@
 
     step_kwargs = step_kwargs or {}
     summary_kwargs = summary_kwargs or {}
     load_cellpy_file = False
     logging_mode = "DEBUG" if testing else logging_mode
     log.setup_logging(default_level=logging_mode, testing=testing)
     logging.debug("-------running-get--------")
-    cellpy_instance = CellpyCell()
+    cellpy_instance = CellpyCell(debug=debug)
     logging.debug(f"created CellpyCell instance")
 
     logging.debug(f"{cellpy_file=}")
     logging.debug(f"{filename=}")
 
     if filename is None:
         if cellpy_file is None:
             logging.info("Running cellpy.get without a filename")
             logging.info("Returning an empty CellpyCell object.")
             cellpy_instance = _update_meta(
                 cellpy_instance,
                 cycle_mode=cycle_mode,
                 mass=mass,
                 nominal_capacity=nominal_capacity,
+                nom_cap_specifics=nom_cap_specifics,
                 area=area,
                 loading=loading,
                 estimate_area=estimate_area,
                 units=units,
             )
             return cellpy_instance
 
@@ -5896,19 +5987,25 @@
     )
 
     if not cellpy_instance:
         print("Could not load file: check log!")
         print("Returning None")
         return
 
+    # fix for allowing for setting nom_cap_specifics the "old" way:
+    nom_cap_specifics = summary_kwargs.pop("nom_cap_specifics", None)
+    if nom_cap_specifics is None:
+        nom_cap_specifics = step_kwargs.pop("nom_cap_specifics", None)
+
     cellpy_instance = _update_meta(
         cellpy_instance,
         cycle_mode=cycle_mode,
         mass=mass,
         nominal_capacity=nominal_capacity,
+        nom_cap_specifics=nom_cap_specifics,
         area=area,
         loading=loading,
         estimate_area=estimate_area,
         units=units,
     )
 
     if auto_summary:
@@ -5922,35 +6019,42 @@
 
 
 def _update_meta(
     cellpy_instance,
     cycle_mode=None,
     mass=None,
     nominal_capacity=None,
+    nom_cap_specifics=None,
     area=None,
     loading=None,
     estimate_area=None,
     units=None,
 ):
     # TODO: make this a method on CellpyCell
     if cycle_mode is not None:
         logging.debug("Setting cycle mode")
         cellpy_instance.cycle_mode = cycle_mode
 
+    if nom_cap_specifics is not None:
+        logging.debug("Setting nom_cap_specifics as given")
+        cellpy_instance.nom_cap_specifics = nom_cap_specifics
+
     if units is not None:
         logging.debug(f"Updating units: {units}")
         cellpy_instance.cellpy_units.update(units)
 
     if mass is not None:
         logging.info(f"Setting mass: {mass}")
-        cellpy_instance.data.mass = mass
+        cellpy_instance.mass = mass
 
     if nominal_capacity is not None:
         logging.info(f"Setting nominal capacity: {nominal_capacity}")
-        cellpy_instance.data.nom_cap = nominal_capacity
+        if nom_cap_specifics is not None and not isinstance(nominal_capacity, numbers.Number):
+            logging.info("Providing nominal capacity as string might override the given nom_cap_specifics")
+        cellpy_instance.nom_cap = nominal_capacity
 
     if area is not None:
         logging.debug(f"got area: {area}")
         cellpy_instance.data.meta_common.active_electrode_area = area
 
     elif loading and estimate_area:
         logging.debug("-------------AREA-CALC----------------")
@@ -6080,15 +6184,17 @@
 
     print(" loading cellpy file and saving to excel ".center(80, "="))
 
     raw_file = Path("../../testdata/data/20160805_test001_45_cc_01.res")
     cellpy_file = Path("../../tmp/20160805_test001_45_cc.h5")
     excel_file = Path("../../tmp/20160805_test001_45_cc.xlsx")
 
-    c = get(raw_file, mass=1.0, nominal_capacity=3579)
+    c = get(raw_file, area=1.55, nominal_capacity=2000, summary_kwargs={"nom_cap_specifics": "areal"}, debug=True)
+    c = get(raw_file, mass=1.55, nominal_capacity="3579 mAh/g", debug=True)
+    c = get(raw_file, area=1.55, nominal_capacity=2000, nom_cap_specifics="areal", debug=True)
     print("loaded ...")
     c.to_excel(excel_file)
     print("saved ...")
     #
     # c.save(cellpy_file)
     # c2 = get(cellpy_file)
     # print("loaded again ...")
```

### Comparing `cellpy-1.0.0a8/cellpy/readers/core.py` & `cellpy-1.0.0a9/cellpy/utils/plotutils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1226 +1,1427 @@
-""" This module contains several of the most important classes used in cellpy.
-
-It also contains functions that are used by readers and utils.
-And it has the file version definitions.
+# -*- coding: utf-8 -*-
+"""
+Utilities for helping to plot cellpy-data.
 """
-import abc
-import datetime
+
+import collections
 import importlib
+import itertools
 import logging
 import os
-import pathlib
-import pickle
 import sys
-import time
 import warnings
-from typing import Any, Tuple, Dict, List, Union, TypeVar
+from io import StringIO
+from pathlib import Path
 
-import numpy as np
-import pandas as pd
-import pint
-from scipy import interpolate
-
-from cellpy.exceptions import NullData
-from cellpy.internals.core import OtherPath
 from cellpy.parameters.internal_settings import (
+    get_headers_journal,
     get_headers_normal,
     get_headers_step_table,
     get_headers_summary,
-    get_default_raw_units,
-    get_default_raw_limits,
-    CellpyMetaCommon,
-    CellpyMetaIndividualTest,
 )
+from cellpy.utils import helpers
+
+try:
+    import matplotlib.pyplot as plt
 
-HEADERS_NORMAL = get_headers_normal()  # TODO @jepe refactor this (not needed)
-HEADERS_SUMMARY = get_headers_summary()  # TODO @jepe refactor this (not needed)
-HEADERS_STEP_TABLE = get_headers_step_table()  # TODO @jepe refactor this (not needed)
+    plt_available = True
+except ImportError:
+    plt_available = False
+
+try:
+    import holoviews as hv
+    from holoviews import opts
+    from holoviews.plotting.links import RangeToolLink
+
+    hv_available = True
+except ImportError:
+    hv_available = False
+
+bokeh_available = importlib.util.find_spec("bokeh") is not None
+
+# logger = logging.getLogger(__name__)
+logging.captureWarnings(True)
+
+SYMBOL_DICT = {
+    "all": [
+        "s",
+        "o",
+        "v",
+        "^",
+        "<",
+        ">",
+        "D",
+        "p",
+        "*",
+        "1",
+        "2",
+        ".",
+        ",",
+        "3",
+        "4",
+        "8",
+        "p",
+        "d",
+        "h",
+        "H",
+        "+",
+        "x",
+        "X",
+        "|",
+        "_",
+    ],
+    "simple": ["s", "o", "v", "^", "<", ">", "*", "d"],
+}
+
+COLOR_DICT = {
+    "classic": ["b", "g", "r", "c", "m", "y", "k"],
+    "grayscale": ["0.00", "0.40", "0.60", "0.70"],
+    "bmh": [
+        "#348ABD",
+        "#A60628",
+        "#7A68A6",
+        "#467821",
+        "#D55E00",
+        "#CC79A7",
+        "#56B4E9",
+        "#009E73",
+        "#F0E442",
+        "#0072B2",
+    ],
+    "dark_background": [
+        "#8dd3c7",
+        "#feffb3",
+        "#bfbbd9",
+        "#fa8174",
+        "#81b1d2",
+        "#fdb462",
+        "#b3de69",
+        "#bc82bd",
+        "#ccebc4",
+        "#ffed6f",
+    ],
+    "ggplot": [
+        "#E24A33",
+        "#348ABD",
+        "#988ED5",
+        "#777777",
+        "#FBC15E",
+        "#8EBA42",
+        "#FFB5B8",
+    ],
+    "fivethirtyeight": ["#30a2da", "#fc4f30", "#e5ae38", "#6d904f", "#8b8b8b"],
+    "seaborn-colorblind": [
+        "#0072B2",
+        "#009E73",
+        "#D55E00",
+        "#CC79A7",
+        "#F0E442",
+        "#56B4E9",
+    ],
+    "seaborn-deep": ["#4C72B0", "#55A868", "#C44E52", "#8172B2", "#CCB974", "#64B5CD"],
+    "seaborn-bright": [
+        "#003FFF",
+        "#03ED3A",
+        "#E8000B",
+        "#8A2BE2",
+        "#FFC400",
+        "#00D7FF",
+    ],
+    "seaborn-muted": ["#4878CF", "#6ACC65", "#D65F5F", "#B47CC7", "#C4AD66", "#77BEDB"],
+    "seaborn-pastel": [
+        "#92C6FF",
+        "#97F0AA",
+        "#FF9F9A",
+        "#D0BBFF",
+        "#FFFEA3",
+        "#B0E0E6",
+    ],
+    "seaborn-dark-palette": [
+        "#001C7F",
+        "#017517",
+        "#8C0900",
+        "#7600A1",
+        "#B8860B",
+        "#006374",
+    ],
+}
+
+hdr_summary = get_headers_summary()
+hdr_raw = get_headers_normal()
+hdr_steps = get_headers_step_table()
+hdr_journal = get_headers_journal()
+
+
+def _hv_bokeh_available():
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
+    if not hv_available:
+        print("You need holoviews. But I cannot load it. Aborting...")
+        return False
+    if not bokeh_available:
+        print("You need Bokeh. But I cannot find it. Aborting...")
+        return False
+    return True
 
 
-# pint (https://pint.readthedocs.io/en/stable/)
-ureg = pint.UnitRegistry()
-Q = ureg.Quantity
+def find_column(columns, label=None, end="cycle_index"):
+    """find columns based on how the column-name ends.
 
+    Args:
+        columns: pandas columns
+        label: if not provided, generate, if provided, return as is
+        end: the string to use for searching
 
-# TODO: in future versions (maybe 1.1.0) we should "copy-paste" the whole pathlib module
-#  from CPython and add the functionality we need to it. This will make
-#  it easier to keep up with changes in the pathlib module.
+    Returns:
+        column header, label
+    """
 
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
+    # TODO @jepe: refactor and use col names directly from HeadersNormal instead
+    hdr = None
+    lab = None
+    for col in columns:
+        if col.endswith(end):
+            hdr = col
+            if label is None:
+                lab = col.replace("_", " ")
+            else:
+                lab = label
+            break
+    return hdr, lab
 
-# https://stackoverflow.com/questions/60067953/
-# 'is-it-possible-to-specify-the-pickle-protocol-when-writing-pandas-to-hdf5
-class PickleProtocol:
-    """Context for using a specific pickle protocol."""
 
-    def __init__(self, level):
-        self.previous = pickle.HIGHEST_PROTOCOL
-        self.level = level
+def plot_concatenated(
+    dataframe,
+    title="",
+    x=None,
+    y=None,
+    err=None,
+    xlabel=None,
+    ylabel=None,
+    points=True,
+    line=True,
+    errors=True,
+    hover=True,
+    width=800,
+    height=300,
+    journal=None,
+    file_id_level=0,
+    hdr_level=None,
+    axis=1,
+    mean_end="_mean",
+    std_end="_std",
+    cycle_end="cycle_index",
+    legend_title="cell-type",
+    marker_size=None,
+    cmap="default_colors",
+    spread=False,
+    extension="bokeh",
+    edges=False,
+    keys=None,
+    simple=False,
+    **kwargs,
+):
+    """Create a holoviews plot of the concatenated summary.
 
-    def __enter__(self):
-        importlib.reload(pickle)
-        pickle.HIGHEST_PROTOCOL = self.level
+    This function is still under development. Feel free to contribute.
 
-    def __exit__(self, *exc):
-        importlib.reload(pickle)
-        pickle.HIGHEST_PROTOCOL = self.previous
+    Args:
+        dataframe: the concatenated summary
+        title (str): title of the plot (defaults to empty)
+        x: colum-name for the x variable (not implemented yet)
+        y: colum-name for the y variable (not implemented yet)
+        err: colum-name for the std variable (not implemented yet)
+        xlabel: label for x-axis
+        ylabel: label for y-axis
+        points (bool): plot points if True
+        line (bool): plot line if True
+        errors (bool): plot errors if True
+        hover (bool): add hover tool if True
+        width: width of plot
+        height: height of plot
+        journal: `batch.journal` object
+        file_id_level: the level (multiindex-level) where the cell-names are.
+        hdr_level:  the level (multiindex-level) where the parameter names are.
+        axis: what axis to use when looking in the data-frame (row-based or col-based).
+        mean_end: used for searching for y-column names
+        std_end: used for searching for e-column names
+        cycle_end: used for searching for x-column name
+        legend_title: title to put over the legend
+        marker_size: size of the markers used
+        cmap: color-map to use
+        spread (bool): plot error-bands instead of error-bars if True
+        extension (str): "matplotlib" or "bokeh". Note, this uses `hv.extension`) and will affect the
+            state of your notebook
+        edges (bool): show all axes
+        keys (dict): columns to plot (not working yet)
+        simple (bool): making a simple hv.Overlay instead of an hv.NdOverlay if True
+        **kwargs: key-word arguments sent to hv.NdOverlay
+
+    Example:
+        >>> my_mpl_plot = plot_concatenated(
+        >>>     cap_cycle_norm_fast_1000, journal=b.experiment.journal,
+        >>>     height=500, marker_size=5,
+        >>>     extension="matplotlib",
+        >>>     edges=True,
+        >>> )
+
+        >>> my_bokeh_plot = plot_concatenated(
+        >>>     cap_cycle_norm_fast_1000, journal=b.experiment.journal,
+        >>>     height=500, marker_size=5,
+        >>>     edges=True,
+        >>> )
+
+
+    Example:
+        >>> # Simple conversion from bokeh to matplotlib
+        >>> # NB! make sure you have only used matplotlib-bokeh convertable key-words (not marker_size)
+
+        >>> hv.extension("matplotlib")
+        >>> my_plot.opts(aspect="auto", fig_inches=(12,7), fig_size=90, legend_position="top_right",
+        >>>              legend_cols = 2,
+        >>>              show_frame=True)
 
+    """
+    # TODO: add option for using labels from journal in the legend
+    # TODO @jepe: refactor and use col names directly from HeadersNormal instead
 
-def pickle_protocol(level):
-    return PickleProtocol(level)
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
 
+    if keys is None:
+        keys = dict()
 
-class BaseDbReader(metaclass=abc.ABCMeta):
-    """Base class for database readers."""
+    if not hv_available:
+        print(
+            "This function uses holoviews. But could not import it."
+            "So I am aborting..."
+        )
+        return
 
-    @abc.abstractmethod
-    def select_batch(self, batch: str) -> List[int]:
-        pass
+    if extension == "matplotlib":
+        hover = False
+    elif extension == "plotly":
+        print("The plotly backend might not work properly yet.")
+        print("Fingers crossed.")
+        print(
+            "(at least, make sure you are using the most "
+            "recent versions of jupyter, holoviews and plotly)"
+        )
 
-    @abc.abstractmethod
-    def get_mass(self, pk: int) -> float:
-        pass
+    try:
+        current_extension = hv.Store.current_backend
+        if extension != current_extension:
+            hv.extension(extension, logo=False)
+    except Exception as e:
+        hv.extension(extension, logo=False)
+
+    if hdr_level is None:
+        hdr_level = 0 if file_id_level == 1 else 1
+
+    averaged = True
+    columns = list(set(dataframe.columns.get_level_values(hdr_level)))
+    hdr_x, lab_x = find_column(columns, label=xlabel, end=cycle_end)
+    hdr_y, lab_y = find_column(columns, label=ylabel, end=mean_end)
+
+    if hdr_y is None:
+        averaged = False
+        errors = False
+        if hdr_x is not None:
+            columns.remove(hdr_x)
+        hdr_y = columns[0]
+        if ylabel is None:
+            lab_y = hdr_y.replace("_", " ")
+        else:
+            lab_y = ylabel
+    if errors:
+        hdr_e, _ = find_column(columns, end=std_end)
+
+    grouped = dataframe.groupby(axis=axis, level=file_id_level)
+    curve_dict = dict()
+
+    if not averaged and journal is not None:
+        journal_pages = journal.pages[
+            [hdr_journal["group"], hdr_journal["sub_group"]]
+        ].copy()
+        journal_pages["g"] = 0
+        journal_pages["sg"] = 0
+        markers = itertools.cycle(["s", "o", "<", "*", "+", "x"])
+        colors = itertools.cycle(hv.Cycle(cmap).values)
+
+        j = journal_pages.groupby(hdr_journal["group"])
+        for i, (jn, jg) in enumerate(j):
+            journal_pages.loc[journal_pages["group"] == jn, "g"] = i
+            journal_pages.loc[journal_pages["group"] == jn, "sg"] = list(range(len(jg)))
+
+        markers = [next(markers) for _ in range(journal_pages["sg"].max() + 1)]
+        colors = [next(colors) for _ in range(journal_pages["g"].max() + 1)]
+        journal_pages = journal_pages[["g", "sg"]]
+
+    for i, (name, group) in enumerate(grouped):
+        if name in keys:
+            label = keys[name]
+        else:
+            label = name
+            keys[name] = name
 
-    @abc.abstractmethod
-    def get_area(self, pk: int) -> float:
-        pass
+        group.columns = group.columns.droplevel(file_id_level)
+        if hdr_x is None:
+            group = group.reset_index()
+            hdr_x = group.columns[0]
+
+        if lab_x is None:
+            lab_x = hdr_x.replace("_", " ")
+
+        if not averaged and journal is not None:
+            g = journal_pages.loc[name, "g"]
+            sg = journal_pages.loc[name, "sg"]
+            color = colors[g]
+            marker = markers[sg]
+            curve = hv.Curve(group, (hdr_x, lab_x), (hdr_y, lab_y), label=label).opts(
+                color=color
+            )
 
-    @abc.abstractmethod
-    def get_loading(self, pk: int) -> float:
-        pass
+        else:
+            curve = hv.Curve(group, (hdr_x, lab_x), (hdr_y, lab_y), label=label)
 
-    @abc.abstractmethod
-    def get_nom_cap(self, pk: int) -> float:
-        pass
+        if points:
+            if not averaged and journal is not None:
+                scatter = hv.Scatter(curve).opts(color=color, marker=marker)
 
-    @abc.abstractmethod
-    def get_total_mass(self, pk: int) -> float:
-        pass
+                if edges and extension == "matplotlib":
+                    scatter = scatter.opts(edgecolor="k")
 
-    @abc.abstractmethod
-    def get_cell_name(self, pk: int) -> str:
-        pass
+                if edges and extension == "bokeh":
+                    scatter = scatter.opts(line_color="k", line_width=1)
 
-    @abc.abstractmethod
-    def get_cell_type(self, pk: int) -> str:
-        pass
+                if marker_size is not None and extension == "bokeh":
+                    scatter = scatter.opts(size=marker_size)
+            else:
+                scatter = hv.Scatter(curve)
 
-    @abc.abstractmethod
-    def get_label(self, pk: int) -> str:
-        pass
+                if marker_size is not None and extension == "bokeh":
+                    scatter = scatter.opts(size=marker_size)
 
-    @abc.abstractmethod
-    def get_comment(self, pk: int) -> str:
-        pass
+        if points and line:
+            curve *= scatter
 
-    @abc.abstractmethod
-    def get_group(self, pk: int) -> str:
-        pass
+        elif points:
+            curve = scatter
 
-    @abc.abstractmethod
-    def get_args(self, pk: int) -> dict:
-        pass
+        if errors:
+            if spread:
+                curve *= hv.Spread(group, hdr_x, [hdr_y, hdr_e])
+            else:
+                curve *= hv.ErrorBars(
+                    group, hdr_x, [hdr_y, hdr_e]
+                )  # should get the color from curve and set it here
+        curve_dict[label] = curve
+
+    if extension == "matplotlib":
+        overlay_opts = {
+            "aspect": "auto",
+            "fig_inches": (width * 0.016, height * 0.012),
+            "show_frame": True,
+        }
+    else:
+        overlay_opts = {"width": width, "height": height}
 
-    @abc.abstractmethod
-    def get_experiment_type(self, pk: int) -> str:
-        pass
+    if simple:
+        if len(keys) == len(curve_dict):
+            new_curve_dict = {}
+            for k in keys:
+                new_curve_dict[k] = curve_dict[keys[k]]
+            curve_dict = new_curve_dict
+
+        final_plot = hv.Overlay(
+            [*curve_dict.values()], vdims=[*curve_dict.keys()]
+        ).opts(**overlay_opts, **kwargs)
+    else:
+        overlay_opts["title"] = title
+        logging.info(f"overlay_opts: {overlay_opts}")
+        logging.info(f"additional_kwargs_overlay_opts: {kwargs}")
+        final_plot = hv.NdOverlay(curve_dict, kdims=legend_title).opts(
+            **overlay_opts, **kwargs
+        )
 
-    @abc.abstractmethod
-    def get_instrument(self, pk: int) -> str:
-        pass
+    if hover and not extension == "plotly":
+        if points:
+            final_plot.opts(opts.Scatter(tools=["hover"]))
+        else:
+            final_plot.opts(opts.Curve(tools=["hover"]))
+    return final_plot
 
-    @abc.abstractmethod
-    def inspect_hd5f_fixed(self, pk: int) -> int:
-        pass
 
-    @abc.abstractmethod
-    def get_by_column_label(self, pk: int, name: str) -> Any:
-        pass
+def create_colormarkerlist_for_journal(
+    journal, symbol_label="all", color_style_label="seaborn-colorblind"
+):
+    """Fetch lists with color names and marker types of correct length for a journal.
 
-    @abc.abstractmethod
-    def from_batch(
-        self,
-        batch_name: str,
-        include_key: bool = False,
-        include_individual_arguments: bool = False,
-    ) -> dict:
-        pass
+    Args:
+        journal: cellpy journal
+        symbol_label: sub-set of markers to use
+        color_style_label: cmap to use for colors
 
+    Returns:
+        colors (list), markers (list)
+    """
+    logging.debug("symbol_label: " + symbol_label)
+    logging.debug("color_style_label: " + color_style_label)
+    groups = journal.pages[hdr_journal.group].unique()
+    sub_groups = journal.pages[hdr_journal.subgroup].unique()
+    return create_colormarkerlist(groups, sub_groups, symbol_label, color_style_label)
 
-class FileID:
-    """class for storing information about the raw-data files.
 
-    This class is used for storing and handling raw-data file information.
-    It is important to keep track of when the data was extracted from the
-    raw-data files so that it is easy to know if the hdf5-files used for
-    @storing "treated" data is up-to-date.
+def create_colormarkerlist(
+    groups, sub_groups, symbol_label="all", color_style_label="seaborn-colorblind"
+):
+    """Fetch lists with color names and marker types of correct length.
 
-    Attributes:
-        name (str): Filename of the raw-data file.
-        full_name (str): Filename including path of the raw-data file.
-        size (float): Size of the raw-data file.
-        last_modified (datetime): Last time of modification of the raw-data
-            file.
-        last_accessed (datetime): last time of access of the raw-data file.
-        last_info_changed (datetime): st_ctime of the raw-data file.
-        location (str): Location of the raw-data file.
+    Args:
+        groups: list of group numbers (used to generate the list of colors)
+        sub_groups: list of sub-group numbers (used to generate the list of markers).
+        symbol_label: sub-set of markers to use
+        color_style_label: cmap to use for colors
 
+    Returns:
+        colors (list), markers (list)
     """
+    symbol_list = SYMBOL_DICT[symbol_label]
+    color_list = COLOR_DICT[color_style_label]
 
-    def __init__(self, filename: Union[str, OtherPath] = None, is_db: bool = False):
-        """Initialize the FileID class."""
+    # checking that we have enough colors and symbols (if not, then use cycler (e.g. reset))
+    color_cycler = itertools.cycle(color_list)
+    symbol_cycler = itertools.cycle(symbol_list)
+    _color_list = []
+    _symbol_list = []
+    for i in groups:
+        _color_list.append(next(color_cycler))
+    for i in sub_groups:
+        _symbol_list.append(next(symbol_cycler))
+    return _color_list, _symbol_list
+
+
+def _raw_plot(raw_curve, title="Voltage versus time", **kwargs):
+    tgt = raw_curve.relabel(title).opts(
+        width=800,
+        height=300,
+        labelled=["y"],
+        # tools=["pan","box_zoom", "reset"],
+        active_tools=["pan"],
+    )
+    src = raw_curve.opts(width=800, height=100, yaxis=None, default_tools=[])
 
-        self.is_db: bool = is_db
-        self._last_data_point: Optional[int] = None
-        self.name: Optional[str] = None
-        self.full_name: Optional[str] = None
-        self.size: Optional[int] = None
-        self.last_modified: Optional[int] = None
-        self.last_accessed: Optional[int] = None
-        self.last_info_changed: Optional[int] = None
-        self.location: Optional[int] = None
+    RangeToolLink(src, tgt)
 
-        if self.is_db:
-            self._from_db(filename)
-            return
+    layout = (tgt + src).cols(1)
+    layout.opts(opts.Layout(shared_axes=False, merge_tools=False))
+    return layout
 
-        make_defaults = True
-        if filename is not None:
-            if not isinstance(filename, OtherPath):
-                logging.debug("filename is not an OtherPath object")
-                filename = OtherPath(filename)
-
-            if filename.is_file():
-                self.populate(filename)
-                make_defaults = False
-
-        if make_defaults:
-            self.name = None
-            self.full_name = None
-            self.size = 0
-            self.last_modified = None
-            self.last_accessed = None
-            self.last_info_changed = None
-            self.location = None
-            self._last_data_point = 0  # to be used later when updating is implemented
 
-    def __str__(self):
-        """Return a string representation of the FileID object."""
-        try:
-            if self.is_db:
-                txt = "\n<fileID><is_db>\n"
-            else:
-                txt = "\n<fileID><is_file>\n"
-        except AttributeError:
-            txt = "\n<fileID><is_file>\n"
-
-        txt += f"full name: {self.full_name}\n"
-        txt += f"name: {self.name}\n"
-        txt += f"location: {self.location}\n"
+def raw_plot(cell, y=("voltage", "Voltage (V vs Li/Li+)"), title=None, **kwargs):
+    # TODO: missing doc-string
 
-        if self.last_modified is not None:
-            txt += f"modified: {self.last_modified}\n"
-        else:
-            txt += "modified: NAN\n"
+    warnings.warn(
+        "This utility function will be replaced shortly", category=DeprecationWarning
+    )
 
-        if self.size is not None:
-            txt += f"size: {self.size}\n"
+    if title is None:
+        if isinstance(y, (list, tuple)):
+            pre_title = str(y[0])
         else:
-            txt += "size: NAN\n"
+            pre_title = str(y)
+        title = " ".join([pre_title, "versus", "time"])
 
-        txt += f"last data point: {self.last_data_point}\n"
+    if not _hv_bokeh_available():
+        return
 
-        return txt
+    hv.extension("bokeh", logo=False)
 
-    def _from_db(self, filename):
-        self.name = filename
-        self.full_name = filename
-        self.size = 0
-        self.last_modified = None
-        self.last_accessed = None
-        self.last_info_changed = None
-        self.location = None
-        self._last_data_point = 0
-
-    @property
-    def last_data_point(self):
-        # TODO: consider including a method here to find the last data point (raw data)
-        # ideally, this value should be set when loading the raw data before
-        # merging files (if it consists of several files)
-        return self._last_data_point
-
-    @last_data_point.setter
-    def last_data_point(self, value):
-        self._last_data_point = value
-
-    def populate(self, filename: Union[str, OtherPath]):
-        """Finds the file-stats and populates the class with stat values.
-
-        Args:
-            filename (str, OtherPath): name of the file.
-        """
-        if not isinstance(filename, OtherPath):
-            logging.debug("filename is not an OtherPath object")
-            filename = OtherPath(filename)
-
-        if filename.is_file():
-            fid_st = filename.stat()
-            self.name = filename.name
-            self.full_name = filename.full_path
-            self.size = fid_st.st_size
-            self.last_modified = fid_st.st_mtime
-            self.last_accessed = fid_st.st_atime
-            self.last_info_changed = fid_st.st_ctime
-            self.location = str(filename.parent)
-
-    def get_raw(self):
-        """Get a list with information about the file.
-
-        The returned list contains name, size, last_modified and location.
-        """
-        return [self.name, self.size, self.last_modified, self.location]
-
-    def get_name(self):
-        """Get the filename."""
-        return self.name
-
-    def get_size(self):
-        """Get the size of the file."""
-        return self.size
-
-    def get_last(self):
-        """Get last modification time of the file."""
-        return self.last_modified
-
-
-class Data:
-    """Object to store data for a cell-test.
-
-    This class is used for storing all the relevant data for a cell-test, i.e. all
-    the data collected by the tester as stored in the raw-files, and user-provided
-    metadata about the cell-test.
-    """
+    raw = cell.data.raw
+    raw["test_time_hrs"] = raw[hdr_raw["test_time_txt"]] / 3600
+    x = ("test_time_hrs", "Time (hours)")
+    raw_curve = hv.Curve(raw, x, y)
+    layout = _raw_plot(raw_curve, title=title, **kwargs)
+    return layout
 
-    def _repr_html_(self):
-        txt = f"<h2>Data-object</h2> id={hex(id(self))}"
-        txt += "<p>"
-        for p in dir(self):
-            if not p.startswith("_"):
-                if p not in ["raw", "summary", "steps", "logger"]:
-                    value = self.__getattribute__(p)
-                    txt += f"<b>{p}</b>: {value}<br>"
-        txt += "</p>"
-        try:
-            raw_txt = f"<p><b>raw data-frame (summary)</b><br>{self.raw.describe()._repr_html_()}</p>"  # noqa
-            raw_txt += f"<p><b>raw data-frame (head)</b><br>{self.raw.head()._repr_html_()}</p>"  # noqa
-        except AttributeError:
-            raw_txt = "<p><b>raw data-frame </b><br> not found!</p>"
-        except ValueError:
-            raw_txt = "<p><b>raw data-frame </b><br> does not contain any columns!</p>"
 
-        try:
-            summary_txt = f"<p><b>summary data-frame (summary)</b><br>{self.summary.describe()._repr_html_()}</p>"  # noqa
-            summary_txt += f"<p><b>summary data-frame (head)</b><br>{self.summary.head()._repr_html_()}</p>"  # noqa
-        except AttributeError:
-            summary_txt = "<p><b>summary data-frame </b><br> not found!</p>"
-        except ValueError:
-            summary_txt = (
-                "<p><b>summary data-frame </b><br> does not contain any columns!</p>"
-            )
+def cycle_info_plot(
+    cell,
+    cycle=None,
+    step=None,
+    title=None,
+    points=False,
+    x=None,
+    y=None,
+    info_level=1,
+    h_cycle=None,
+    h_step=None,
+    show_it=True,
+    label_cycles=True,
+    label_steps=False,
+    get_axes=False,
+    use_bokeh=True,
+    **kwargs,
+):
+    """Show raw data together with step and cycle information.
 
-        try:
-            steps_txt = f"<p><b>steps data-frame (summary)</b><br>{self.steps.describe()._repr_html_()}</p>"  # noqa
-            steps_txt += f"<p><b>steps data-frame (head)</b><br>{self.steps.head()._repr_html_()}</p>"  # noqa
-        except AttributeError:
-            steps_txt = "<p><b>steps data-frame </b><br> not found!</p>"
-        except ValueError:
-            steps_txt = (
-                "<p><b>steps data-frame </b><br> does not contain any columns!</p>"
-            )
+    Args:
+        cell: cellpy object
+        cycle: cycles to select (optional, default is all)
+        step: steps to select (optional, defaults is all)
+        title: a title to give the plot
+        points: overlay a scatter plot
+        x (str): column header for the x-value (defaults to "Test_Time")
+        y (str): column header for the y-value (defaults to "Voltage")
+        info_level (int): how much information to display (defaults to 1)
+            (0 - almost nothing
+            1 - pretty much
+            2 - something else
+            3 - not implemented yet).
+        h_cycle: column header for the cycle number (defaults to "Cycle_Index")
+        h_step: column header for the step number (defaults to "Step_Index")
+        show_it (bool): show the figure (defaults to True). If not, return the figure.
+        label_cycles (bool): add labels with cycle numbers.
+        label_steps (bool): add labels with step numbers
+        get_axes (bool): return axes (for matplotlib)
+        use_bokeh (bool): use bokeh to plot (defaults to True). If not, use matplotlib.
+        **kwargs: parameters specific to either matplotlib or bokeh.
 
-        return txt + summary_txt + steps_txt + raw_txt
+    Returns:
+        ``matplotlib.axes`` or None
+    """
+    # TODO: missing doc-string
 
-    def __init__(self, **kwargs):
-        self.logger = logging.getLogger(__name__)
-        self.logger.debug("created DataSet instance")
-
-        self.raw_data_files = []
-        self.raw_data_files_length = []
-        self.loaded_from = None
-        self._raw_id = None
-        self.raw_units = get_default_raw_units()
-        self.raw_limits = get_default_raw_limits()
-
-        self.raw = pd.DataFrame()
-        self.summary = pd.DataFrame()
-        self.steps = pd.DataFrame()
-
-        self.meta_common = CellpyMetaCommon()
-        self.meta_test_dependent = CellpyMetaIndividualTest()
-
-        # custom meta-data
-        for k in kwargs:
-            if hasattr(self, k):
-                setattr(self, k, kwargs[k])
-
-    # ---------------- left-over-properties v7 -> v8 -----------------
-    # these now belong to the CellpyMeta attributes
-    #   however, since they are extensively used in the instrument
-    #   loaders and cellreader, they are also accessible here as properties
-
-    @property
-    def raw_id(self):
-        return self.meta_common.raw_id
-
-    @property
-    def start_datetime(self):
-        return self.meta_common.start_datetime
-
-    @start_datetime.setter
-    def start_datetime(self, n):
-        self.meta_common.start_datetime = n
-
-    @property
-    def material(self):
-        return self.meta_common.material
-
-    @material.setter
-    def material(self, n):
-        self.meta_common.material = n
-
-    @property
-    def mass(self):
-        return self.meta_common.mass
-
-    @mass.setter
-    def mass(self, n):
-        self.meta_common.mass = n
-
-    @property
-    def tot_mass(self):
-        return self.meta_common.tot_mass
-
-    @tot_mass.setter
-    def tot_mass(self, n):
-        self.meta_common.tot_mass = n
-
-    @property
-    def active_electrode_area(self):
-        return self.meta_common.active_electrode_area
-
-    @active_electrode_area.setter
-    def active_electrode_area(self, area):
-        self.meta_common.active_electrode_area = area
-
-    @property
-    def cell_name(self):
-        return self.meta_common.cell_name
-
-    @cell_name.setter
-    def cell_name(self, cell_name):
-        self.meta_common.cell_name = cell_name
-
-    @property
-    def nom_cap(self):
-        return self.meta_common.nom_cap
-
-    @nom_cap.setter
-    def nom_cap(self, value):
-        if value < 1.0:
-            warnings.warn(
-                f"POSSIBLE BUG: NOMINAL CAPACITY LESS THAN 1.0 ({value}).",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        self.meta_common.nom_cap = value  # nominal capacity
+    warnings.warn(
+        "This utility function will be replaced shortly", category=DeprecationWarning
+    )
 
-    @staticmethod
-    def _header_str(hdr):
-        txt = "\n"
-        txt += 80 * "-" + "\n"
-        txt += f" {hdr} ".center(80) + "\n"
-        txt += 80 * "-" + "\n"
-        return txt
-
-    def __str__(self):
-        txt = "<Data>\n"
-        txt += "loaded from file(s)\n"
-        if isinstance(self.loaded_from, (list, tuple)):
-            for f in self.loaded_from:
-                txt += str(f)
-                txt += "\n"
+    if use_bokeh and not bokeh_available:
+        print("OBS! bokeh is not available - using matplotlib instead")
+        use_bokeh = False
+
+    if use_bokeh:
+        axes = _cycle_info_plot_bokeh(
+            cell,
+            cycle=cycle,
+            step=step,
+            title=title,
+            points=points,
+            x=x,
+            y=y,
+            info_level=info_level,
+            h_cycle=h_cycle,
+            h_step=h_step,
+            show_it=show_it,
+            label_cycles=label_cycles,
+            label_steps=label_steps,
+            **kwargs,
+        )
+    else:
+        if isinstance(cycle, (list, tuple)):
+            if len(cycle) > 1:
+                print("OBS! The matplotlib-plotter only accepts single cycles.")
+                print(f"Selecting first cycle ({cycle[0]})")
+            cycle = cycle[0]
+        axes = _cycle_info_plot_matplotlib(cell, cycle, get_axes)
+    if get_axes:
+        return axes
+
+
+def _plot_step(ax, x, y, color):
+    ax.plot(x, y, color=color, linewidth=3)
+
+
+def _get_info(table, cycle, step):
+    # obs! hard-coded col-names. Please fix me.
+    m_table = (table.cycle == cycle) & (table.step == step)
+    p1, p2 = table.loc[m_table, ["point_min", "point_max"]].values[0]
+    c1, c2 = table.loc[m_table, ["current_min", "current_max"]].abs().values[0]
+    d_voltage, d_current = table.loc[
+        m_table, ["voltage_delta", "current_delta"]
+    ].values[0]
+    d_discharge, d_charge = table.loc[
+        m_table, ["discharge_delta", "charge_delta"]
+    ].values[0]
+    current_max = (c1 + c2) / 2
+    rate = table.loc[m_table, "rate_avr"].values[0]
+    step_type = table.loc[m_table, "type"].values[0]
+    return [step_type, rate, current_max, d_voltage, d_current, d_discharge, d_charge]
+
+
+def _add_step_info_cols(df, table, cycles=None, steps=None, h_cycle=None, h_step=None):
+    if h_cycle is None:
+        h_cycle = "cycle_index"  # edit
+    if h_step is None:
+        h_step = "step_index"  # edit
+
+    col_name_mapper = {"cycle": h_cycle, "step": h_step}
+
+    df = df.merge(
+        table.rename(columns=col_name_mapper),
+        on=("cycle_index", "step_index"),
+        how="left",
+    )
 
-        else:
-            txt += str(self.loaded_from)
-            txt += "\n"
-        txt += "\n* GLOBAL\n"
-        txt += f"material:            {self.meta_common.material}\n"
-        txt += f"mass (active):       {self.meta_common.mass}\n"
-        txt += f"mass (total):        {self.meta_common.tot_mass}\n"
-        txt += f"nominal capacity:    {self.meta_common.nom_cap}\n"
-        txt += f"test ID:             {self.meta_test_dependent.test_ID}\n"
-        txt += f"channel index:       {self.meta_test_dependent.channel_index}\n"
-        txt += f"creator:             {self.meta_test_dependent.creator}\n"
-        txt += f"schedule file name:  {self.meta_test_dependent.schedule_file_name}\n"
+    return df
 
-        try:
-            if self.start_datetime:
-                start_datetime_str = xldate_as_datetime(self.start_datetime)
-            else:
-                start_datetime_str = "Not given"
-        except AttributeError:
-            start_datetime_str = "NOT READABLE YET"
 
-        txt += f"start-date:         {start_datetime_str}\n"
+def _cycle_info_plot_bokeh(
+    cell,
+    cycle=None,
+    step=None,
+    title=None,
+    points=False,
+    x=None,
+    y=None,
+    info_level=0,
+    h_cycle=None,
+    h_step=None,
+    show_it=False,
+    label_cycles=True,
+    label_steps=False,
+    **kwargs,
+):
+    """Plot raw data with annotations.
 
-        txt += self._header_str("DATA")
-        try:
-            txt += str(self.raw.describe())
-        except (AttributeError, ValueError):
-            txt += "EMPTY (Not processed yet)\n"
+    This function uses Bokeh for plotting and is intended for use in
+    Jupyter Notebooks.
+    """
+    # TODO: check that correct new column-names are used
+    # TODO: fix bokeh import (use e.g. import bokeh.io)
 
-        txt += self._header_str("SUMMARY")
-        try:
-            txt += str(self.summary.describe())
-        except (AttributeError, ValueError):
-            txt += "EMPTY (Not processed yet)\n"
+    try:
+        from bokeh.io import output_notebook, show
+        from bokeh.layouts import column, row
+        from bokeh.models import ColumnDataSource, HoverTool, LabelSet
+        from bokeh.models.annotations import Span
+        from bokeh.models.widgets import Slider, TextInput
+        from bokeh.plotting import figure
 
-        txt += self._header_str("STEP TABLE")
-        try:
-            txt += str(self.steps.describe())
-            txt += str(self.steps.head())
-        except (AttributeError, ValueError):
-            txt += "EMPTY (Not processed yet)\n"
+    except ImportError:
+        warnings.warn("Could not import bokeh")
+        return
 
-        txt += self._header_str("RAW UNITS")
-        try:
-            txt += str(self.raw.describe())
-            txt += str(self.raw.head())
-        except (AttributeError, ValueError):
-            txt += "EMPTY (Not processed yet)\n"
-        return txt
-
-    def populate_defaults(self):
-        # modify this method upon need
-        logging.debug("checking and populating defaults for the cell")
-
-        if not self.active_electrode_area:
-            self.active_electrode_area = 1.0
-            logging.debug(
-                f"active_electrode_area not set -> setting to: {self.active_electrode_area}"
-            )
+    try:
+        output_notebook(hide_banner=True)
+    finally:
+        sys.stdout = sys.__stdout__
+
+    if points:
+        if cycle is None or (len(cycle) > 1):
+            print("Plotting points only allowed when plotting one single cycle.")
+            print("Turning points off.")
+            points = False
+
+    if h_cycle is None:
+        h_cycle = "cycle_index"  # edit
+    if h_step is None:
+        h_step = "step_index"  # edit
 
-        if not self.mass:
-            self.mass = 1.0
-            logging.debug(f"mass not set -> setting to: {self.mass}")
-
-        if not self.tot_mass:
-            self.tot_mass = self.mass
-            logging.debug(
-                f"total mass not set -> setting to same as mass: {self.tot_mass}"
-            )
+    if x is None:
+        x = "test_time"  # edit
+    if y is None:
+        y = "voltage"  # edit
 
-        return True
+    if isinstance(x, tuple):
+        x, x_label = x
+    else:
+        x_label = x
 
-    @property
-    def empty(self):
-        if self.has_data:
-            return False
-        return True
-
-    @property
-    def has_summary(self):
-        """check if the summary table exists"""
-        try:
-            empty = self.summary.empty
-            # TODO: check if the summary has the expected columns
-            #  (since it can be unprocessed directly from the raw data)
-        except AttributeError:
-            empty = True
-        return not empty
-
-    @property
-    def has_steps(self):
-        """check if the step table exists"""
-        try:
-            empty = self.steps.empty
-        except AttributeError:
-            empty = True
-        return not empty
+    if isinstance(y, tuple):
+        y, y_label = y
+    else:
+        y_label = y
 
-    @property
-    def has_data(self):
-        try:
-            empty = self.raw.empty
-        except AttributeError:
-            empty = True
-        return not empty
+    t_x = x  # used in generating title - replace with a selector
+    t_y = y  # used in generating title - replace with a selector
 
+    if title is None:
+        title = f"{t_y} vs. {t_x}"
 
-class InstrumentFactory:
-    def __init__(self):
-        self._builders = {}
-        self._kwargs = {}
+    cols = [x, y]
+    cols.extend([h_cycle, h_step])
 
-    def register_builder(self, key: str, builder: Tuple[str, Any], **kwargs) -> None:
-        """register an instrument loader module.
+    df = cell.data.raw.loc[:, cols]
 
-        Args:
-            key: instrument id
-            builder: (module_name, module_path)
-            **kwargs: stored in the factory (will be used in the future for allowing to set
-               defaults to the builders to allow for using .query).
-        """
+    if cycle is not None:
+        if not isinstance(cycle, (list, tuple)):
+            cycle = [cycle]
 
-        logging.debug(f"Registering instrument {key}")
-        self._builders[key] = builder
-        self._kwargs[key] = kwargs
+        _df = df.loc[df[h_cycle].isin(cycle), :]
+        if len(cycle) < 5:
+            title += f" [c:{cycle}]"
+        else:
+            title += f" [c:{cycle[0]}..{cycle[-1]}]"
+        if _df.empty:
+            print(f"EMPTY (available cycles: {df[h_step].unique()})")
+            return
+        else:
+            df = _df
 
-    def create(self, key: Union[str, None], **kwargs):
-        """Create the instrument loader module and initialize the loader class.
+    cycle = df[h_cycle].unique()
 
-        Args:
-            key: instrument id
-            **kwargs: sent to the initializer of the loader class.
+    if step is not None:
+        if not isinstance(step, (list, tuple)):
+            step = [step]
 
-        Returns:
-            instance of loader class.
-        """
+        _df = df.loc[df[h_step].isin(step), :]
+        if len(step) < 5:
+            title += f" (s:{step})"
+        else:
+            title += f" [s:{step[0]}..{step[-1]}]"
+        if _df.empty:
+            print(f"EMPTY (available steps: {df[h_step].unique()})")
+            return
+        else:
+            df = _df
 
-        module_name, module_path = self._builders.get(key, (None, None))
+    x_min, x_max = df[x].min(), df[x].max()
+    y_min, y_max = df[y].min(), df[y].max()
 
-        # constant:
-        instrument_class = "DataLoader"
+    if info_level > 0:
+        table = cell.data.steps
+        df = _add_step_info_cols(df, table, cycle, step)
+
+    source = ColumnDataSource(df)
+
+    plot = figure(
+        title=title,
+        tools="pan,reset,save,wheel_zoom,box_zoom,undo,redo",
+        x_range=[x_min, x_max],
+        y_range=[y_min, y_max],
+        **kwargs,
+    )
 
-        if not module_name:
-            raise ValueError(key)
+    plot.line(x, y, source=source, line_width=3, line_alpha=0.6)
 
-        spec = importlib.util.spec_from_file_location(module_name, module_path)
-        loader_module = importlib.util.module_from_spec(spec)
-        sys.modules[module_name] = loader_module  # noqa
-        spec.loader.exec_module(loader_module)
-        cls = getattr(loader_module, instrument_class)
+    # labelling cycles
+    if label_cycles:
+        cycle_line_positions = [df.loc[df[h_cycle] == c, x].min() for c in cycle]
+        cycle_line_positions.append(df.loc[df[h_cycle] == cycle[-1], x].max())
+        for m in cycle_line_positions:
+            _s = Span(
+                location=m,
+                dimension="height",
+                line_color="red",
+                line_width=3,
+                line_alpha=0.5,
+            )
+            plot.add_layout(_s)
 
-        # TODO: get stored kwargs from self.__kwargs and merge them with the supplied kwargs
-        #  (supplied should have preference)
+        s_y_pos = y_min + 0.9 * (y_max - y_min)
+        s_x = []
+        s_y = []
+        s_l = []
+
+        for s in cycle:
+            s_x_min = df.loc[df[h_cycle] == s, x].min()
+            s_x_max = df.loc[df[h_cycle] == s, x].max()
+            s_x_pos = (s_x_min + s_x_max) / 2
+            s_x.append(s_x_pos)
+            s_y.append(s_y_pos)
+            s_l.append(f"c{s}")
+
+        c_labels = ColumnDataSource(data={x: s_x, y: s_y, "names": s_l})
+
+        c_labels = LabelSet(
+            x=x,
+            y=y,
+            text="names",
+            level="glyph",
+            source=c_labels,
+            render_mode="canvas",
+            text_color="red",
+            text_alpha=0.7,
+        )
 
-        return cls(**kwargs)
+        plot.add_layout(c_labels)
 
-    def query(self, key: str, variable: str) -> Any:
-        """performs a get_params lookup for the instrument loader.
+        # labelling steps
+    if label_steps:
+        for c in cycle:
+            step = df.loc[df[h_cycle] == c, h_step].unique()
+            step_line_positions = [
+                df.loc[(df[h_step] == s) & (df[h_cycle] == c), x].min()
+                for s in step[0:]
+            ]
+            for m in step_line_positions:
+                _s = Span(
+                    location=m,
+                    dimension="height",
+                    line_color="olive",
+                    line_width=3,
+                    line_alpha=0.1,
+                )
+                plot.add_layout(_s)
 
-        Args:
-            key: instrument id.
-            variable: the variable you want to lookup.
+            # s_y_pos = y_min + 0.8 * (y_max - y_min)
+            s_x = []
+            s_y = []
+            s_l = []
+
+            for s in step:
+                s_x_min = df.loc[(df[h_step] == s) & (df[h_cycle] == c), x].min()
+                s_x_max = df.loc[(df[h_step] == s) & (df[h_cycle] == c), x].max()
+                s_x_pos = s_x_min
+
+                s_y_min = df.loc[(df[h_step] == s) & (df[h_cycle] == c), y].min()
+                s_y_max = df.loc[(df[h_step] == s) & (df[h_cycle] == c), y].max()
+                s_y_pos = (s_y_max + s_y_min) / 2
+
+                s_x.append(s_x_pos)
+                s_y.append(s_y_pos)
+                s_l.append(f"s{s}")
+
+            s_labels = ColumnDataSource(data={x: s_x, y: s_y, "names": s_l})
+
+            s_labels = LabelSet(
+                x=x,
+                y=y,
+                text="names",
+                level="glyph",
+                source=s_labels,
+                render_mode="canvas",
+                text_color="olive",
+                text_alpha=0.3,
+            )
 
-        Returns:
-            The value of the variable if the loaders get_params method supports it.
-        """
-        loader = self.create(key)
-        try:
-            value = loader.get_params(variable)
-            logging.debug(f"GOT {variable}={value} for {key}")
-            return value
+            plot.add_layout(s_labels)
 
-        except (AttributeError, NotImplementedError, KeyError):
-            logging.debug(f"COULD NOT RETRIEVE {variable} for {key}")
+    hover = HoverTool()
+    if info_level == 0:
+        hover.tooltips = [
+            (x, "$x{0.2f}"),
+            (y, "$y"),
+            ("cycle", f"@{h_cycle}"),
+            ("step", f"@{h_step}"),
+        ]
+    elif info_level == 1:
+        # insert C-rates etc here
+        hover.tooltips = [
+            (f"(x,y)", "($x{0.2f} $y"),
+            ("cycle", f"@{h_cycle}"),
+            ("step", f"@{h_step}"),
+            ("step_type", "@type"),
+            ("rate", "@rate_avr{0.2f}"),
+        ]
+
+    elif info_level == 2:
+        hover.tooltips = [
+            (x, "$x{0.2f}"),
+            (y, "$y"),
+            ("cycle", f"@{h_cycle}"),
+            ("step", f"@{h_step}"),
+            ("step_type", "@type"),
+            ("rate (C)", "@rate_avr{0.2f}"),
+            ("dv (%)", "@voltage_delta{0.2f}"),
+            ("I-max (A)", "@current_max"),
+            ("I-min (A)", "@current_min"),
+            ("dCharge (%)", "@charge_delta{0.2f}"),
+            ("dDischarge (%)", "@discharge_delta{0.2f}"),
+        ]
+
+    hover.mode = "vline"
+    plot.add_tools(hover)
+
+    plot.xaxis.axis_label = x_label
+    plot.yaxis.axis_label = y_label
+
+    if points:
+        plot.scatter(x, y, source=source, alpha=0.3)
+
+    if show_it:
+        show(plot)
+
+    return plot
+
+
+def _cycle_info_plot_matplotlib(cell, cycle, get_axes=False):
+    # obs! hard-coded col-names. Please fix me.
+    if not plt_available:
+        print(
+            "This function uses matplotlib. But I could not import it. "
+            "So I decided to abort..."
+        )
         return
 
+    data = cell.data.raw
+    table = cell.data.steps
 
-def generate_default_factory():
-    """This function searches for all available instrument readers
-    and registers them in an InstrumentFactory instance.
+    span_colors = ["#4682B4", "#FFA07A"]
 
-    Returns:
-        InstrumentFactory
-    """
-    instrument_factory = InstrumentFactory()
-    instruments = find_all_instruments()
-    for instrument_id, instrument in instruments.items():
-        instrument_factory.register_builder(instrument_id, instrument)
-    return instrument_factory
-
-
-def find_all_instruments() -> Dict[str, Tuple[str, pathlib.Path]]:
-    """finds all the supported instruments"""
-
-    import cellpy.readers.instruments as hard_coded_instruments_site
-
-    instruments_found = {}
-    logging.debug("Searching for modules in base instrument folder:")
-
-    hard_coded_instruments_site = pathlib.Path(
-        hard_coded_instruments_site.__file__
-    ).parent
-    modules_in_hard_coded_instruments_site = [
-        s
-        for s in hard_coded_instruments_site.glob("*.py")
-        if not (
-            str(s.name).startswith("_")
-            or str(s.name).startswith("dev_")
-            or str(s.name).startswith("base")
-            or str(s.name).startswith("backup")
-            or str(s.name).startswith("registered_loaders")
-        )
-    ]
+    voltage_color = "#008B8B"
+    current_color = "#CD5C5C"
 
-    for module_path in modules_in_hard_coded_instruments_site:
-        module_name = module_path.name.rstrip(".py")
-        logging.debug(module_name)
-        instruments_found[module_name] = (
-            module_name,
-            module_path,
+    m_cycle_data = data.cycle_index == cycle
+    all_steps = data[m_cycle_data]["step_index"].unique()
+
+    color = itertools.cycle(span_colors)
+
+    fig = plt.figure(figsize=(20, 8))
+    fig.suptitle(f"Cycle: {cycle}")
+
+    ax3 = plt.subplot2grid((8, 3), (0, 0), colspan=3, rowspan=1, fig=fig)  # steps
+    ax4 = plt.subplot2grid((8, 3), (1, 0), colspan=3, rowspan=2, fig=fig)  # rate
+    ax1 = plt.subplot2grid((8, 3), (3, 0), colspan=3, rowspan=5, fig=fig)  # data
+
+    ax2 = ax1.twinx()
+    ax1.set_xlabel("time (minutes)")
+    ax1.set_ylabel("voltage (V vs. Li/Li+)", color=voltage_color)
+    ax2.set_ylabel("current (mA)", color=current_color)
+
+    annotations_1 = []  # step number (IR)
+    annotations_2 = []  # step number
+    annotations_4 = []  # rate
+
+    for i, s in enumerate(all_steps):
+        m = m_cycle_data & (data.step_index == s)
+        c = data.loc[m, "current"] * 1000
+        v = data.loc[m, "voltage"]
+        t = data.loc[m, "test_time"] / 60
+        step_type, rate, current_max, dv, dc, d_discharge, d_charge = _get_info(
+            table, cycle, s
         )
-        logging.debug(" -> added")
+        if len(t) > 1:
+            fcolor = next(color)
 
-    logging.debug("Searching for module configurations in user instrument folder:")
-    # These are only yaml-files and should ideally import the appropriate
-    #    custom loader class
-    # Might not be needed.
-    logging.debug("- Not implemented yet")
-
-    logging.debug("Searching for modules through plug-ins:")
-    # Not sure how to do this yet. Probably also some importlib trick.
-    logging.debug("- Not implemented yet")
-    return instruments_found
-
-
-def identify_last_data_point(data):
-    """Find the last data point and store it in the fid instance"""
+            info_txt = (
+                f"{step_type}\nc-rate = {rate}\ni = |{1000 * current_max:0.2f}| mA\n"
+            )
+            info_txt += f"delta V = {dv:0.2f} %\ndelta i = {dc:0.2f} %\n"
+            info_txt += f"delta C = {d_charge:0.2} %\ndelta DC = {d_discharge:0.2} %\n"
 
-    logging.debug("searching for last data point")
-    hdr_data_point = HEADERS_NORMAL.data_point_txt
-    try:
-        if hdr_data_point in data.raw.columns:
-            last_data_point = data.raw[hdr_data_point].max()
-        else:
-            last_data_point = data.raw.index.max()
-    except AttributeError:
-        logging.debug("AttributeError - setting last data point to 0")
-        last_data_point = 0
-    if not last_data_point > 0:
-        last_data_point = 0
-    data.raw_data_files[0].last_data_point = last_data_point
-    logging.debug(f"last data point: {last_data_point}")
-    return data
-
-
-# TODO: move this to internals/core
-def check64bit(current_system="python"):
-    """checks if you are on a 64-bit platform"""
-    if current_system == "python":
-        return sys.maxsize > 2147483647
-    elif current_system == "os":
-        import platform
-
-        pm = platform.machine()
-        if pm != ".." and pm.endswith("64"):  # recent Python (not Iron)
-            return True
+            for ax in [ax2, ax3, ax4]:
+                ax.axvspan(t.iloc[0], t.iloc[-1], facecolor=fcolor, alpha=0.2)
+            _plot_step(ax1, t, v, voltage_color)
+            _plot_step(ax2, t, c, current_color)
+            annotations_1.append([f"{s}", t.mean()])
+            annotations_4.append([info_txt, t.mean()])
         else:
-            if "PROCESSOR_ARCHITEW6432" in os.environ:
-                return True  # 32 bit program running on 64-bit Windows
-            try:
-                # 64-bit Windows 64 bit program
-                return os.environ["PROCESSOR_ARCHITECTURE"].endswith("64")
-            except IndexError:
-                pass  # not Windows
-            try:
-                # this often works in Linux
-                return "64" in platform.architecture()[0]
-            except Exception:  # noqa
-                # is an older version of Python, assume also an older os@
-                # (best we can guess)
-                return False
-
-
-# TODO: move this to internals/core
-def humanize_bytes(b, precision=1):
-    """Return a humanized string representation of a number of b."""
-
-    abbrevs = (
-        (1 << 50, "PB"),
-        (1 << 40, "TB"),
-        (1 << 30, "GB"),
-        (1 << 20, "MB"),
-        (1 << 10, "kB"),
-        (1, "b"),
-    )
-    if b == 1:
-        return "1 byte"
-    for factor, suffix in abbrevs:
-        if b >= factor:
-            break
-    # return '%.*f %s' % (precision, old_div(b, factor), suffix)
-    return "%.*f %s" % (precision, b // factor, suffix)  # noqa
-
-
-# TODO: move this to internals/core
-def xldate_as_datetime(xldate, datemode=0, option="to_datetime"):
-    """Converts a xls date stamp to a more sensible format.
-
-    Args:
-        xldate (str, int): date stamp in Excel format.
-        datemode (int): 0 for 1900-based, 1 for 1904-based.
-        option (str): option in ("to_datetime", "to_float", "to_string"),
-            return value
+            info_txt = f"{s}({step_type})"
+            annotations_2.append([info_txt, t.mean()])
+    ax3.set_ylim(0, 1)
+    for s in annotations_1:
+        ax3.annotate(f"{s[0]}", (s[1], 0.2), ha="center")
 
-    Returns:
-        datetime (datetime object, float, or string).
+    for s in annotations_2:
+        ax3.annotate(f"{s[0]}", (s[1], 0.6), ha="center")
 
-    """
+    for s in annotations_4:
+        ax4.annotate(f"{s[0]}", (s[1], 0.0), ha="center")
 
-    # This does not work for numpy-arrays
+    for ax in [ax3, ax4]:
+        ax.axes.get_yaxis().set_visible(False)
+        ax.axes.get_xaxis().set_visible(False)
 
-    if option == "to_float":
-        d = (xldate - 25589) * 86400.0
-    else:
-        try:
-            d = datetime.datetime(1899, 12, 30) + datetime.timedelta(
-                days=xldate + 1462 * datemode
-            )
-            # date_format = "%Y-%m-%d %H:%M:%S:%f" # with microseconds,
-            # Excel cannot cope with this!
-            if option == "to_string":
-                date_format = "%Y-%m-%d %H:%M:%S"  # without microseconds
-                d = d.strftime(date_format)
-        except TypeError:
-            logging.info(f"The date is not of correct type [{xldate}]")
-            d = xldate
-    return d
+    if get_axes:
+        return ax1, ax2, ax2, ax4
 
 
-def collect_capacity_curves(
-    cell,
-    direction="charge",
-    trim_taper_steps=None,
-    steps_to_skip=None,
-    steptable=None,
-    max_cycle_number=None,
-    **kwargs,
-):
-    """Create a list of pandas.DataFrames, one for each charge step.
+def save_fig(figure, file_name=None, wide=False, size=None, dpi=300, **kwargs):
+    """Save a figure, either a holoviews plot or a matplotlib figure.
 
-    The DataFrames are named by its cycle number.
+    This function should mainly be used when using the standard cellpy notebook
+    template (generated by '> cellpy new')
 
     Args:
-        cell (``CellpyCell``):  object
-        direction (str):
-        trim_taper_steps (integer): number of taper steps to skip (counted
-            from the end, i.e. 1 means skip last step in each cycle).
-        steps_to_skip (list): step numbers that should not be included.
-        steptable (``pandas.DataFrame``): optional steptable.
-        max_cycle_number (int): only select cycles up to this value.
-
-    Returns:
-        list of pandas.DataFrames,
-        list of cycle numbers,
-        minimum voltage value,
-        maximum voltage value
-
+        figure (obj): the figure or plot object
+        file_name (str): the file name
+        wide (bool): release the equal aspect lock (default on for holoviews)
+        size (int or tuple of ints): figure size in inches
+        dpi (int): resolution
+        **kwargs: sent to cellpy.utils.plotutils.hv_bokeh_to_mpl
     """
 
-    # TODO: should allow for giving cycle numbers as input (e.g. cycle=[1, 2, 10]
-    #  or cycle=2), not only max_cycle_number. Intermediate solution:
-    #  The cycle keyword will not break the method but raise a warning:
-    for arg in kwargs:
-        if arg in ["cycle", "cycles"]:
-            logging.warning(
-                f"{arg} is not implemented yet, but might exist in newer versions of cellpy."
-            )
-        else:
-            logging.warning(
-                f"collect_capacity_curve received unknown key-word argument: {arg=}"
-            )
-
-    minimum_v_value = np.Inf
-    maximum_v_value = -np.Inf
-    charge_list = []
-    cycles = kwargs.pop("cycle", None)
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
 
-    if cycles is None:
-        cycles = cell.get_cycle_numbers()
+    out_path = Path("out/")
+    extension = "png"
 
-    if max_cycle_number is None:
-        max_cycle_number = max(cycles)
+    if size is None:
+        size = (6, 6)
 
-    for cycle in cycles:
-        if cycle > max_cycle_number:
-            break
-        try:
-            if direction == "charge":
-                q, v = cell.get_ccap(
-                    cycle,
-                    trim_taper_steps=trim_taper_steps,
-                    steps_to_skip=steps_to_skip,
-                    steptable=steptable,
-                    return_dataframe=False,
-                )
+    # create file name:
+    if file_name is None:
+        counter = 1
+        while True:
+            _file_name = f"cellpy-plot-{str(counter).zfill(3)}.{extension}"
+            _file_name = out_path / _file_name
+            if not os.path.isfile(_file_name):
+                break
+            counter += 1
+        file_name = _file_name
+
+    type_str = str(type(figure))
+
+    is_hv = type_str.find("holoviews") >= 0
+    is_mpl = type_str.find("matplotlib") >= 0
+
+    if is_mpl:
+        is_mpl_figure = type_str.find("figure.Figure") >= 0
+        is_mpl_axes = type_str.find(".axes.") >= 0
+        if not is_mpl_figure:
+            if is_mpl_axes:
+                figure = figure.get_figure()
             else:
-                q, v = cell.get_dcap(
-                    cycle,
-                    trim_taper_steps=trim_taper_steps,
-                    steps_to_skip=steps_to_skip,
-                    steptable=steptable,
-                    return_dataframe=False,
-                )
+                print("this matplotlib object is not supported")
+                print(type_str)
+                return
+
+        figure.savefig(file_name, dpi=dpi)
+    elif is_hv:
+        is_hv_nd_overlay = isinstance(figure, hv.core.overlay.NdOverlay)
+        is_hv_overlay = isinstance(figure, hv.core.overlay.Overlay)
+        is_hv_layout = isinstance(figure, hv.core.layout.Layout)
 
-        except NullData as e:
-            logging.warning(e)
-            d = pd.DataFrame()
-            d.name = cycle
-            charge_list.append(d)
-        else:
-            d = pd.DataFrame({"q": q, "v": v})
-            # d.name = f"{cycle}"
-            d.name = cycle
-            charge_list.append(d)
-            v_min = v.min()
-            v_max = v.max()
-            if v_min < minimum_v_value:
-                minimum_v_value = v_min
-            if v_max > maximum_v_value:
-                maximum_v_value = v_max
-    return charge_list, cycles, minimum_v_value, maximum_v_value
+        figure = hv_bokeh_to_mpl(figure, wide=wide, size=size, **kwargs)
+        figure.savefig(file_name, dpi=dpi)
 
+    else:
+        print("this figure object is not supported")
+        print(type_str)
+        return
+    print(f"saved to {file_name}")
 
-def interpolate_y_on_x(
-    df,
-    x=None,
-    y=None,
-    new_x=None,
-    dx=10.0,
-    number_of_points=None,
-    direction=1,
+
+def hv_bokeh_to_mpl(figure, wide=False, size=(6, 4), **kwargs):
+    # I think this needs to be tackled differently. For example by setting hv.extension("matplotlib") and
+    # re-making the figure. Or making a custom renderer.
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
+    figure = hv.render(figure, backend="matplotlib")
+    axes = figure.axes
+    number_of_axes = len(axes)
+    if number_of_axes > 1:
+        for j, ax in enumerate(axes):
+            if j < number_of_axes - 1:
+                ax.set_xlabel("")
+            if j < number_of_axes - 1:
+                ax.get_legend().remove()
+            else:
+                handles, labels = ax.get_legend_handles_labels()
+                # This does not work:
+                # ax.legend(handles, labels, bbox_to_anchor=(1.05, 1), loc="upper_right")
+                # TODO: create new legend based on the ax data
+
+    if wide:
+        for axis in axes:
+            axis.set_aspect("auto")
+
+    figure.tight_layout()
+    figure.set_size_inches(size)
+
+    return figure
+
+
+def oplot(
+    b,
+    cap_ylim=None,
+    ce_ylim=None,
+    ir_ylim=None,
+    simple=False,
+    group_it=False,
+    spread=True,
+    capacity_unit="gravimetric",
+    capacity_unit_label=None,
+    internal_resistance_unit="Ohm",
     **kwargs,
 ):
-    """Interpolate a column based on another column.
+    """create a holoviews-plot containing Coulombic Efficiency, Capacity, and IR.
 
     Args:
-        df: DataFrame with the (cycle) data.
-        x: Column name for the x-value (defaults to the step-time column).
-        y: Column name for the y-value (defaults to the voltage column).
-        new_x (numpy array or None): Interpolate using these new x-values
-            instead of generating x-values based on dx or number_of_points.
-        dx: step-value (defaults to 10.0)
-        number_of_points: number of points for interpolated values (use
-            instead of dx and overrides dx if given).
-        direction (-1,1): if direction is negative, then invert the
-            x-values before interpolating.
-        **kwargs: arguments passed to ``scipy.interpolate.interp1d``
+        b (cellpy.batch object): the batch with the cells.
+        cap_ylim (tuple of two floats): scaling of y-axis for capacity plots.
+        ce_ylim (tuple of two floats): scaling of y-axis for c.e. plots.
+        ir_ylim (tuple of two floats): scaling of y-axis for i.r. plots.
+        simple (bool): if True, use hv.Overlay instead of hv.NdOverlay.
+        group_it (bool): if True, average pr group.
+        spread (bool): if True, show spread instead of error-bars.
+        capacity_unit (str): select "gravimetric", or "areal".
+        capacity_unit_label (str): shown in the plot title for the capacity plot
+            (defaults to mAh/g(a.m.) for gravimetric and mAh/cm2 for areal).
+        internal_resistance_unit (str): shown in the plot title for the ir plots (defaults to Ohm).
 
-    Returns: DataFrame with interpolated y-values based on given or
-        generated x-values.
+    **kwargs:
+        Sent to plotutils.bplot.
 
+    Returns:
+        ``hv.Overlay`` or ``hv.NdOverlay``
     """
 
-    # TODO: allow for giving a fixed interpolation range (x-values).
-    #  Remember to treat extrapolation properly (e.g. replace with NaN?).
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
 
-    if x is None:
-        x = df.columns[0]
-    if y is None:
-        y = df.columns[1]
+    extension = kwargs.pop("extension", "bokeh")
 
-    xs = df[x].values
-    ys = df[y].values
+    cap_colum_dict = {
+        "gravimetric": {
+            "discharge": "discharge_capacity_gravimetric",
+            "charge": "charge_capacity_gravimetric",
+            "unit": capacity_unit_label or "mAh/g(a.m.)",
+            "ylim": (0, 5000),
+        },
+        "areal": {
+            "discharge": "discharge_capacity_areal",
+            "charge": "charge_capacity_areal",
+            "unit": capacity_unit_label or "mAh/cm2",
+            "ylim": (0, 3),
+        },
+    }
 
-    if direction > 0:
-        x_min = xs.min()
-        x_max = xs.max()
-    else:
-        x_max = xs.min()
-        x_min = xs.max()
-        dx = -dx
-
-    bounds_error = kwargs.pop("bounds_error", False)
-    f = interpolate.interp1d(xs, ys, bounds_error=bounds_error, **kwargs)
-    if new_x is None:
-        if number_of_points:
-            new_x = np.linspace(x_min, x_max, number_of_points)
-        else:
-            new_x = np.arange(x_min, x_max, dx)
+    if cap_ylim is not None:
+        cap_colum_dict[capacity_unit]["ylim"] = cap_ylim
 
-    new_y = f(new_x)
+    if ce_ylim is None:
+        ce_ylim = (80, 120)
 
-    new_df = pd.DataFrame({x: new_x, y: new_y})
+    if ir_ylim is None:
+        ir_ylim = (0, 200)
 
-    return new_df
+    overlay_sensitive_opts = {"ce": {}, "dcap": {}, "ccap": {}, "ird": {}, "irc": {}}
+
+    layout_sensitive_opts = {"ce": {}, "dcap": {}, "ccap": {}, "ird": {}, "irc": {}}
+
+    if extension == "bokeh":
+        overlay_sensitive_opts["ce"] = {"height": 150}
+        overlay_sensitive_opts["dcap"] = {"height": 400}
+        overlay_sensitive_opts["ccap"] = {"height": 150}
+        overlay_sensitive_opts["ird"] = {"height": 150}
+        overlay_sensitive_opts["irc"] = {"height": 150}
+
+    elif extension == "matplotlib":
+        simple = True
+        overlay_sensitive_opts["ce"] = {"aspect": 2}
+        overlay_sensitive_opts["dcap"] = {"aspect": 2}
+        overlay_sensitive_opts["ccap"] = {"aspect": 2}
+        overlay_sensitive_opts["ird"] = {"aspect": 2}
+        overlay_sensitive_opts["irc"] = {"aspect": 2}
+
+        hspace = 2
+        layout_sensitive_opts["ce"] = {"hspace": hspace}
+        layout_sensitive_opts["dcap"] = {"hspace": hspace}
+        layout_sensitive_opts["ccap"] = {"hspace": hspace}
+        layout_sensitive_opts["ird"] = {"hspace": hspace}
+        layout_sensitive_opts["irc"] = {"hspace": hspace}
+
+    bplot_shared_opts = {
+        "group_it": group_it,
+        "simple": simple,
+        "spread": spread,
+        "extension": extension,
+    }
 
+    if simple:
+        overlay_opts = hv.opts.Overlay
+        layout_opts = hv.opts.Layout
+    else:
+        overlay_opts = hv.opts.NdOverlay
+        layout_opts = hv.opts.NdLayout
 
-def group_by_interpolate(
-    df,
-    x=None,
-    y=None,
-    group_by=None,
-    number_of_points=100,
-    tidy=False,
-    individual_x_cols=False,
-    header_name="Unit",
-    dx=10.0,
-    generate_new_x=True,
-):
-    """Do a pandas.DataFrame.group_by and perform interpolation for all groups.
+    # print("creating interactive plots")
+    oplot_ce = bplot(
+        b, columns=["coulombic_efficiency"], **bplot_shared_opts, **kwargs
+    ).opts(
+        hv.opts.Curve(ylim=ce_ylim),
+        overlay_opts(
+            title="",
+            show_legend=False,
+            xlabel="",
+            ylabel="C.E.",
+            **overlay_sensitive_opts["ce"],
+        ),
+        layout_opts(title="Coulombic efficiency (%)", **layout_sensitive_opts["ce"]),
+    )
+    # print(" - created oplot_ce")
 
-    This function is a wrapper around an internal interpolation function in
-    cellpy (that uses scipy.interpolate.interp1d) that combines doing a group-by
-    operation and interpolation.
+    oplot_dcap = bplot(
+        b,
+        columns=[cap_colum_dict[capacity_unit]["discharge"]],
+        **bplot_shared_opts,
+        **kwargs,
+    ).opts(
+        hv.opts.Curve(ylim=cap_colum_dict[capacity_unit]["ylim"]),
+        overlay_opts(
+            title="",
+            show_legend=True,
+            xlabel="",
+            ylabel="discharge",
+            **overlay_sensitive_opts["dcap"],
+        ),
+        layout_opts(
+            title=f"Capacity ({cap_colum_dict[capacity_unit]['unit']})",
+            **layout_sensitive_opts["dcap"],
+        ),
+    )
+    # print(" - created oplot_dcap")
 
-    Args:
-        df (pandas.DataFrame): the dataframe to morph.
-        x (str): the header for the x-value
-            (defaults to normal header step_time_txt) (remark that the default
-            group_by column is the cycle column, and each cycle normally
-            consist of several steps (so you risk interpolating / merging
-            several curves on top of each other (not good)).
-        y (str): the header for the y-value
-            (defaults to normal header voltage_txt).
-        group_by (str): the header to group by
-            (defaults to normal header cycle_index_txt)
-        number_of_points (int): if generating new x-column, how many values it
-            should contain.
-        tidy (bool): return the result in tidy (i.e. long) format.
-        individual_x_cols (bool): return as xy xy xy ... data.
-        header_name (str): name for the second level of the columns (only
-            applies for xy xy xy ... data) (defaults to "Unit").
-        dx (float): if generating new x-column and number_of_points is None or
-            zero, distance between the generated values.
-        generate_new_x (bool): create a new x-column by
-            using the x-min and x-max values from the original dataframe where
-            the method is set by the number_of_points key-word:
-
-            1)  if number_of_points is not None (default is 100):
-
-                ```
-                new_x = np.linspace(x_max, x_min, number_of_points)
-                ```
-            2)  else:
-                ```
-                new_x = np.arange(x_max, x_min, dx)
-                ```
+    oplot_ccap = bplot(
+        b,
+        columns=[cap_colum_dict[capacity_unit]["charge"]],
+        **bplot_shared_opts,
+        **kwargs,
+    ).opts(
+        hv.opts.Curve(ylim=cap_colum_dict[capacity_unit]["ylim"]),
+        overlay_opts(
+            title="",
+            show_legend=False,
+            xlabel="",
+            ylabel="charge",
+            **overlay_sensitive_opts["ccap"],
+        ),
+        layout_opts(title="", **layout_sensitive_opts["ccap"]),
+    )
+    # print(" - created oplot_ccap")
 
+    oplot_ird = bplot(b, columns=["ir_discharge"], **bplot_shared_opts, **kwargs).opts(
+        hv.opts.Curve(ylim=ir_ylim),
+        overlay_opts(
+            title="",
+            show_legend=False,
+            xlabel="",
+            ylabel="discharge",
+            **overlay_sensitive_opts["ird"],
+        ),
+        layout_opts(
+            title=f"Internal Resistance ({internal_resistance_unit})",
+            **layout_sensitive_opts["ird"],
+        ),
+    )
 
-    Returns: pandas.DataFrame with interpolated x- and y-values. The returned
-        dataframe is in tidy (long) format for tidy=True.
+    oplot_irc = bplot(b, columns=["ir_charge"], **bplot_shared_opts, **kwargs).opts(
+        hv.opts.Curve(ylim=ir_ylim),
+        overlay_opts(
+            title="",
+            show_legend=False,
+            ylabel="charge",
+            **overlay_sensitive_opts["irc"],
+        ),
+        layout_opts(title="", **layout_sensitive_opts["irc"]),
+    )
 
-    """
-    # TODO: @jepe - create more tests
-    time_00 = time.time()
-    if x is None:
-        x = HEADERS_NORMAL.step_time_txt
-    if y is None:
-        y = HEADERS_NORMAL.voltage_txt
-    if group_by is None:
-        group_by = [HEADERS_NORMAL.cycle_index_txt]
-
-    if not isinstance(group_by, (list, tuple)):
-        group_by = [group_by]
-
-    if not generate_new_x:
-        # check if it makes sense
-        if (not tidy) and (not individual_x_cols):
-            logging.warning("Unlogical condition")
-            generate_new_x = True
-
-    new_x = None
-
-    if generate_new_x:
-        x_max = df[x].max()
-        x_min = df[x].min()
-        if number_of_points:
-            new_x = np.linspace(x_max, x_min, number_of_points)
-        else:
-            new_x = np.arange(x_max, x_min, dx)
+    return (oplot_ce + oplot_dcap + oplot_ccap + oplot_ird + oplot_irc).cols(1)
 
-    new_dfs = []
-    keys = []
 
-    for name, group in df.groupby(group_by):
-        keys.append(name)
-        if not isinstance(name, (list, tuple)):
-            name = [name]
+def bplot(b, individual=False, cols=1, **kwargs):
+    """plot batch summaries.
 
-        new_group = interpolate_y_on_x(
-            group, x=x, y=y, new_x=new_x, number_of_points=number_of_points, dx=dx
-        )
+    This is wrapper around the two functions concatenate_summaries and plot_concatenated.
 
-        if tidy or (not tidy and not individual_x_cols):
-            for i, j in zip(group_by, name):
-                new_group[i] = j
-        new_dfs.append(new_group)
+    >>> p1 = bplot(b, columns=["charge_capacity_gravimetric"], journal=b.experiment.journal, group_it=True)
 
-    if tidy:
-        new_df = pd.concat(new_dfs)
-    else:
-        if individual_x_cols:
-            new_df = pd.concat(new_dfs, axis=1, keys=keys)
-            group_by.append(header_name)
-            new_df.columns.names = group_by
-        else:
-            new_df = pd.concat(new_dfs)
-            new_df = new_df.pivot(index=x, columns=group_by[0], values=y)
+    is equivalent to:
 
-    time_01 = time.time() - time_00
-    logging.debug(f"duration: {time_01} seconds")
-    return new_df
-
-
-def convert_from_simple_unit_label_to_string_unit_label(k, v):
-    old_raw_units = {
-        "current": 1.0,
-        "charge": 1.0,
-        "voltage": 1.0,
-        "time": 1.0,
-        "resistance": 1.0,
-        "power": 1.0,
-        "energy": 1.0,
-        "frequency": 1.0,
-        "mass": 0.001,
-        "nominal_capacity": 1.0,
-        "specific_gravimetric": 1.0,
-        "specific_areal": 1.0,
-        "specific_volumetric": 1.0,
-        "length": 1.0,
-        "area": 1.0,
-        "volume": 1.0,
-        "temperature": 1.0,
-        "pressure": 1.0,
-    }
-    old_unit = old_raw_units[k]
-    value = v / old_unit
-    default_units = get_default_raw_units()
-
-    new_unit = default_units[k]
-    value = Q(value, new_unit)
-    str_value = str(value)
-    return str_value
-
-
-# ---------------- LOCAL DEV TESTS ----------------
-
-
-def check_convert_from_simple_unit_label_to_string_unit_label():
-    k = "resistance"
-    v = 1.0
-    n = convert_from_simple_unit_label_to_string_unit_label(k, v)
-    print(n)
-
-
-def check_path_things():
-    p = "//jepe@mymachine.my.no/./path/file.txt"
-    p2 = pathlib.Path(p)
-    print(f"{p2=}")
-    print(f"{p2.resolve()=}")
-    print(f"{p2.drive=}")
-    print(f"{p2.as_uri()=}")
-    print(f"{p2.root=}")
-    print(f"{p2.anchor=}")
-    print(f"{p2.parent=}")
-    print(f"{p2.name=}")
-    print(f"{p2.stem=}")
-    print(f"{p2.suffix=}")
-    print(f"{p2.suffixes=}")
-    print(f"{p2.parts=}")
-    print(f"{p2.is_absolute()=}")
-    print(f"{p2.is_reserved()=}")
-    print(f"{p2.is_dir()=}")
-    print(f"{p2.is_file()=}")
+    >>> cs = helpers.concatenate_summaries(b, columns=["charge_capacity_gravimetric"], group_it=True)
+    >>> p1 = plot_concatenated(cs, journal=journal)
 
-    try:
-        print(f"{p2.is_socket()=}")
-    except NotImplementedError as e:
-        print(f"{e}")
-    try:
-        print(f"{p2.is_mount()=}")
-    except NotImplementedError as e:
-        print(f"{e}")
-    try:
-        print(f"{p2.is_symlink()=}")
-    except NotImplementedError as e:
-        print(f"{e}")
+    Args:
+        b (cellpy.batch object): the batch with the cells.
+        individual (bool): in case of multiple columns, return a list of plots instaed of a hv.Layout
+        cols (int): number of columns.
+
+    Key-word arguments sent further to the concatenator:
+
+    Keyword Args:
+        rate (float): filter on rate (C-rate)
+        on (str or list of str): only select cycles if based on the rate of this step-type (e.g. on="charge").
+        columns (list): selected column(s) (using cellpy attribute name) [defaults to "charge_capacity_gravimetric"]
+        column_names (list): selected column(s) (using exact column name)
+        normalize_capacity_on (list): list of cycle numbers that will be used for setting the basis of the normalization
+            (typically the first few cycles after formation)
+        scale_by (float or str): scale the normalized data with nominal capacity if "nom_cap", or given value (defaults to one).
+        nom_cap (float): nominal capacity of the cell
+        normalize_cycles (bool): perform a normalisation of the cycle numbers (also called equivalent cycle index)
+        add_areal (bool):  add areal capacity to the summary
+        group_it (bool): if True, average pr group.
+        rate_std (float): allow for this inaccuracy when selecting cycles based on rate
+        rate_column (str): name of the column containing the C-rates.
+        inverse (bool): select steps that do not have the given C-rate.
+        inverted (bool): select cycles that do not have the steps filtered by given C-rate.
+        journal (batch.journal object): the journal (will use the journal in b if not given).
+
+    Key-word arguments sent further to the plotter:
+
+    Keyword Args:
+        width (int): width of plot.
+        spread (bool): use error-spread instead of error-bars.
+        simple (bool): use ``hv.Overlay`` instead of ``hv.NdOverlay``.
+        extension (str): plotting backend.
 
-    try:
-        print(f"{p2.owner()=}")
-    except NotImplementedError as e:
-        print(f"{e}")
+    Returns:
+        ``holoviews`` plot
+    """
+    warnings.warn(
+        "This utility function will be removed shortly", category=DeprecationWarning
+    )
 
-    try:
-        print(f"{p2.group()=}")
-    except NotImplementedError as e:
-        print(f"{e}")
-
-    print(f"{p2.exists()=}")
-
-
-def check_another_path_things():
-    p01 = r"C:\scripting\cellpy\testdata\data\20160805_test001_45_cc_01.res"
-    p02 = r"ssh://jepe@server.no/home/jepe/cellpy/testdata/data/20160805_test001_45_cc_01.res"
-    p03 = r"scripting\cellpy\testdata\data\20160805_test001_45_cc_01.res"
-    p04 = r"..\data\20160805_test001_45_cc_01.res"
-    p05 = pathlib.Path(p01)
-    p06 = pathlib.Path(p02)
-    for p in [p01, p02, p03, p04, p05, p06]:
-        print(f"{p}".center(110, "-"))
-        p2 = OtherPath(p)
-        print(f"{p2=}")
-        print(p2)
-        print(f"{p2.resolve()=}")
-        print(f"{p2.drive=}")
-        print(f"{p2.exists()=}")
-        print(f"{p2._is_external=}")  # noqa
-        print(f"{p2._location=}")  # noqa
-        print(f"{p2._uri_prefix=}")  # noqa
-        print(f"{p2.resolve()=}")
-        if p2.is_absolute():
-            print(f"{p2.as_uri()=}")
-        print(f"{p2.is_external=}")
-        print(f"{p2.location=}")
-        print(f"{p2.uri_prefix=}")
-        print(f"{p2.root=}")
-        print(f"{p2.anchor=}")
-        print(f"{p2.parent=}")
-        print(f"{p2.name=}")
-        print(f"{p2.stem=}")
-        print(f"{p2.suffix=}")
-        print(f"{p2.suffixes=}")
-        print(f"{p2.parts=}")
-        print(f"{type(p2)}")
-        print(f"{isinstance(p2, pathlib.Path)=}")
-        print(f"{isinstance(p2, OtherPath)=}")
-        print()
-
-
-def check_how_other_path_works():
-    p01 = r"C:\scripting\cellpy\testdata\data\20160805_test001_45_cc_01.res"
-    p02 = r"ssh://jepe@somewhere.else.no/home/jepe/cellpy/testdata/data/20160805_test001_45_cc_01.res"
-    p03 = None
-    p03b = OtherPath(p03)
-    p05 = pathlib.Path(p01)
-    p06 = pathlib.Path(p02)
-    p07 = OtherPath(p01)
-    p08 = OtherPath(p02)
-    print(80 * "=")
-    for p in [p01, p02, p03, p03b, p05, p06, p07, p08]:
-        print(f"{p}".center(110, "-"))
-        print(f"{type(p)}".center(110, "*"))
-        p2 = OtherPath(p)
-        print(f"{p2=}")
-        print(p2)
-        print(f"{p2.raw_path=}")
-        print(f"{p2.is_external=}")
-        print(f"{p2.location=}")
-        print(f"{p2.uri_prefix=}")
-        print(f"{p2._original=}")  # noqa
-        print(f"{p2.full_path=}")
-        print(f"{p2.parts=}")
-
-
-def check_copy_external_file():
-    from cellpy import prms
-
-    prms.Paths.env_file = r"C:\scripting\cellpy\local\.env_cellpy"
-    dst = r"C:\scripting\cellpy\tmp\20210629_moz_cat_02_cc_01.res"
-    src = "ssh://jepe@not.in.no/home/jepe@ad.ife.no/Temp/20210629_moz_cat_02_cc_01.res"
-    copy_external_file(src, dst)
+    width = kwargs.pop("width", 800)
+    journal = kwargs.pop("journal", b.experiment.journal)
+    spread = kwargs.pop("spread", True)
+    simple = kwargs.pop("simple", False)
+    columns = kwargs.pop("columns", ["charge_capacity_gravimetric"])
+    extension = kwargs.pop("extension", "bokeh")
+    if extension != "bokeh":
+        logging.critical(
+            f"Setting extension to {extension}. Remark that this will globally change the hv settings."
+        )
+    p = collections.OrderedDict()
+    i_width = width // cols
+    for i, col in enumerate(columns):
+        try:
+            cs = helpers.concatenate_summaries(b, columns=[col], **kwargs)
+            _p = plot_concatenated(
+                cs,
+                journal=journal,
+                spread=spread,
+                width=i_width,
+                extension=extension,
+                title=col,
+                simple=simple,
+            )
+
+            if i < len(columns) - 1:
+                _p.opts(show_legend=False)
+                if cols == 1:
+                    _p.opts(xlabel="")
+            else:
+                _p.opts(show_legend=True, legend_position="right")
+            # if (len(columns) > 1) and cols > 1:
+            #     _p.opts(frame_width=width)
+            if extension == "bokeh":
+                _p.opts(frame_width=width)
+            p[col] = _p
+
+        except KeyError as e:
+            print(f"Sorry - missing key: {col}")
+            logging.debug(e)
+
+    w = width / 180 * cols
+    h = 5 * len(p) / cols
+
+    if len(p) >= 1:
+        if not individual:
+            if simple:
+                out = hv.Layout(list(p.values())).cols(cols)
+            else:
+                out = hv.NdLayout(p, sort=False).cols(cols)
+            if extension == "matplotlib":
+                out.opts(fig_inches=(w, h))
+        else:
+            if extension == "matplotlib":
+                out = [o.opts(fig_inches=(w, h)) for o in p.values()]
+            else:
+                out = [p.values()]
+        return out
 
 
 if __name__ == "__main__":
-    check_how_other_path_works()
+    pass
```

### Comparing `cellpy-1.0.0a8/cellpy/readers/dbreader.py` & `cellpy-1.0.0a9/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/filefinder.py` & `cellpy-1.0.0a9/cellpy/readers/filefinder.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/base.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/custom.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.0a9/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.0a9/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch.py` & `cellpy-1.0.0a9/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_experiments.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,1002 +1,1002 @@
-import ast
-import logging
-import os
-import pathlib
-import sys
-import warnings
-
-import pandas as pd
-from tqdm.auto import tqdm
-
-import cellpy
-from cellpy import prms
-from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
-from cellpy.readers import cellreader
-from cellpy.internals.core import OtherPath
-from cellpy.utils.batch_tools import batch_helpers as helper
-from cellpy.utils.batch_tools.batch_core import BaseExperiment
-from cellpy.utils.batch_tools.batch_journals import LabJournal
-
-hdr_journal = get_headers_journal()
-hdr_summary = get_headers_summary()
-
-
-class CyclingExperiment(BaseExperiment):
-    """Load experimental data into memory.
-
-    This is a re-implementation of the old batch behaviour where
-    all the data-files are processed sequentially (and optionally exported)
-    while the summary tables are kept and processed. This implementation
-    also saves the step tables (for later use when using look-up
-    functionality).
-
-
-    Attributes:
-        journal (:obj: LabJournal): information about the experiment.
-        force_cellpy (bool): tries only to load the cellpy-file if True.
-        force_raw (bool): loads raw-file(s) even though appropriate cellpy-file
-           exists if True.
-        save_cellpy (bool): saves a cellpy-file for each cell if True.
-        accept_errors (bool): in case of error, dont raise an exception, but
-           continue to the next file if True.
-        all_in_memory (bool): store the cellpydata-objects in memory if True.
-        export_cycles (bool): export voltage-capacity curves if True.
-        shifted_cycles (bool): set this to True if you want to export the
-           voltage-capacity curves using the shifted-cycles option (only valid
-           if you set export_cycles to True).
-        export_raw (bool): export the raw-data if True.
-        export_ica (bool): export dq-dv curves if True.
-        last_cycle (int): sets the last cycle (i.e. the highest cycle number)
-           that you would like to process dq-dv on). Use all if None (the
-           default value).
-        selected_summaries (list): a list of summary labels defining what
-           summary columns to make joint summaries from (optional).
-        errors (dict): contains a dictionary listing all the errors encountered.
-
-    Args:
-        db_reader (str or object): custom db_reader (see doc on db_reader).
-
-    Example:
-
-
-    """
-
-    def __init__(self, *args, **kwargs):
-        db_reader = kwargs.pop("db_reader", "default")
-        super().__init__(*args)
-        self.journal = LabJournal(db_reader=db_reader)
-        self.errors = dict()
-        self.log = dict()
-
-        self.force_cellpy = False
-        self.force_raw = False
-        self.force_recalc = False
-        self.save_cellpy = True
-        self.accept_errors = False
-        self.all_in_memory = False
-
-        self.export_cycles = False
-        self.shifted_cycles = False
-        self.export_raw = True
-        self.export_ica = False
-        self.last_cycle = None
-        self.nom_cap = None
-        self.instrument = None
-        self.custom_data_folder = None
-
-        self.selected_summaries = None
-
-    def _repr_html_(self):
-        txt = f"<h2>CyclingExperiment-object</h2> id={hex(id(self))}"
-        txt += "<h3>Main attributes</h3>"
-        txt += f"""
-        <table>
-            <thead>
-                <tr>
-                    <th>Attribute</th>
-                    <th>Value</th>
-                </tr>
-            </thead>
-            <tbody>
-                <tr><td><b>force_cellpy</b></td><td>{self.force_cellpy}</td></tr>
-                <tr><td><b>force_raw</b></td><td>{self.force_raw}</td></tr>
-                <tr><td><b>force_recalc</b></td><td>{self.force_recalc}</td></tr>
-                <tr><td><b>save_cellpy</b></td><td>{self.save_cellpy}</td></tr>
-                <tr><td><b>accept_errors</b></td><td>{self.accept_errors}</td></tr>
-                <tr><td><b>all_in_memory</b></td><td>{self.all_in_memory}</td></tr>
-                <tr><td><b>export_cycles</b></td><td>{self.export_cycles}</td></tr>
-                <tr><td><b>shifted_cycles</b></td><td>{self.shifted_cycles}</td></tr>
-                <tr><td><b>export_raw</b></td><td>{self.export_raw}</td></tr>
-                <tr><td><b>export_ica</b></td><td>{self.export_ica}</td></tr>
-                <tr><td><b>last_cycle</b></td><td>{self.last_cycle}</td></tr>
-                <tr><td><b>nom_cap</b></td><td>{self.nom_cap}</td></tr>
-                <tr><td><b>instrument</b></td><td>{self.instrument}</td></tr>
-                <tr><td><b>custom_data_folder</b></td><td>{self.custom_data_folder}</td></tr>
-                <tr><td><b>selected_summaries</b></td><td>{self.selected_summaries}</td></tr>
-            </tbody>
-        </table>
-        """
-        txt += "<h3>Cells</h3>"
-        txt += f"<p><b>data</b>: contains {len(self)} cells.</p>"
-        return txt
-
-    @staticmethod
-    def _get_cell_spec_from_page(indx: int, row: pd.Series) -> dict:
-        # Edit this if we decide to make "argument families", e.g. loader_split or merger_recalc.
-
-        PRM_SPLITTER = ";"
-        EQUAL_SIGN = "="
-
-        def _arg_parser(text: str) -> None:
-            individual_specs = text.split(PRM_SPLITTER)
-            for p in individual_specs:
-                p, a = p.split(EQUAL_SIGN)
-
-        logging.debug(f"getting cell_spec from journal pages ({indx})")
-        try:
-            cell_spec = row[hdr_journal.argument]
-            logging.debug(cell_spec)
-            if not isinstance(cell_spec, dict):
-                raise TypeError("the cell spec argument is not a dictionary")
-        except Exception as e:
-            logging.warning(f"could not get cell spec for {indx}")
-            logging.warning(f"error message: {e}")
-            return {}
-
-        # converting from str if needed
-        for spec in cell_spec:
-            if isinstance(cell_spec[spec], str):
-                if cell_spec[spec].lower() == "true":
-                    cell_spec[spec] = True
-                elif cell_spec[spec].lower() == "false":
-                    cell_spec[spec] = False
-                elif cell_spec[spec].lower() == "none":
-                    cell_spec[spec] = None
-                else:
-                    try:
-                        logging.debug(
-                            f"Using ast.literal_eval to convert cell-spec value from str '{cell_spec[spec]}'"
-                        )
-                        cell_spec[spec] = ast.literal_eval(cell_spec[spec])
-                    except ValueError as e:
-                        logging.warning(
-                            f"ERROR! Could not convert from str to python object!"
-                        )
-                        logging.debug(e)
-        return cell_spec
-
-    def update(
-        self,
-        all_in_memory=None,
-        cell_specs=None,
-        logging_mode=None,
-        accept_errors=None,
-        **kwargs,
-    ):
-        """Updates the selected datasets.
-
-        Args:
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-            logging_mode (str): sets the logging mode for the loader(s).
-            accept_errors (bool): if True, the loader will continue even if it encounters errors.
-
-            kwargs:
-                transferred all the way to the instrument loader, if not
-                picked up earlier. Remark that you can obtain the same pr. cell by
-                providing a `cellspecs` dictionary. The kwargs have precedence over the
-                parameters given in the journal pages, but will be overridden by parameters
-                given by `cellspecs`.
-
-                Merging:
-                    recalc (Bool): set to False if you don't want automatic "recalc" of
-                        cycle numbers etc. when merging several data-sets.
-                Loading:
-                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                    loading from raw is not necessary (or turned off).
-
-                Debugging:
-                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
-
-        Debug-mode:
-                 - runs only for the first item in your journal
-
-        Examples:
-            >>> # Don't perform recalculation of cycle numbers etc. when merging
-            >>> # All cells:
-            >>> b.update(recalc=False)
-            >>> # For specific cell(s):
-            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
-            >>> b.update(cell_specs=cell_specs_cell_01)
-
-        """
-
-        # TODO: implement experiment.last_cycle
-        accept_errors = accept_errors or self.accept_errors
-
-        debugging = kwargs.pop("debug", False)
-        testing = kwargs.pop("testing", False)
-
-        # --- cleaning up attributes / arguments etc ---
-        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
-        force_raw = kwargs.pop("force_raw", self.force_raw)
-
-        logging.info("[update experiment]")
-        if all_in_memory is not None:
-            self.all_in_memory = all_in_memory
-
-        logging.info(f"Additional keyword arguments: {kwargs}")
-        selector = kwargs.get("selector", None)
-
-        pages = self.journal.pages
-        if self.nom_cap:
-            warnings.warn(
-                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
-                "the journal pages."
-            )
-            pages[hdr_journal.nom_cap] = self.nom_cap
-
-        if self.instrument:
-            warnings.warn(
-                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
-            )
-            pages[hdr_journal.instrument] = self.instrument
-
-        if x := kwargs.pop("instrument", None):
-            warnings.warn(
-                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
-                "Future version will require instrument in the journal pages."
-            )
-            pages[hdr_journal.instrument] = x
-
-        if pages.empty:
-            raise Exception("your journal is empty")
-
-        # --- init ---
-        summary_frames = dict()
-        cell_data_frames = dict()
-        number_of_runs = len(pages)
-        logging.debug(f"You have {number_of_runs} cells in your journal")
-        counter = 0
-        errors = []
-
-        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
-
-        if debugging:
-            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
-
-        # --- iterating ---
-        # TODO: create a multiprocessing pool and get one statusbar pr cell
-        for index, row in pbar:
-            counter += 1
-            h_txt = f"{index}"
-            n_txt = f"loading {counter}"
-            l_txt = f"starting to process file # {counter} ({index})"
-            pbar.set_description(n_txt, refresh=True)
-            cell_spec_page = self._get_cell_spec_from_page(index, row)
-
-            if cell_specs is not None:
-                cell_spec = cell_specs.get(index, dict())
-            else:
-                cell_spec = dict()
-
-            cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
-            l_txt += f" cell_spec: {cell_spec}"
-            logging.debug(l_txt)
-
-            # --- UPDATING ARGUMENTS ---
-            filename = None
-            instrument = None
-            cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
-            _cellpy_file = None
-            if not force_raw and cellpy_file.is_file():
-                _cellpy_file = cellpy_file
-                logging.debug(f"Got cellpy file: {_cellpy_file}")
-            if not force_cellpy:
-                filename = row[hdr_journal.raw_file_names]
-                instrument = row[hdr_journal.instrument]
-
-            cycle_mode = row[hdr_journal.cell_type]
-            mass = row[hdr_journal.mass]
-            nom_cap = row[hdr_journal.nom_cap]
-
-            loading = None
-            area = None
-            if hdr_journal.loading in row:
-                loading = row[hdr_journal.loading]
-            if hdr_journal.area in row:
-                area = row[hdr_journal.area]
-
-            summary_kwargs = {
-                "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
-            }
-
-            step_kwargs = {}
-            if not filename and not force_cellpy:
-                logging.info(
-                    f"Raw file(s) not given in the journal.pages for index={index}"
-                )
-                errors.append(index)
-                continue
-
-            elif not cellpy_file and force_cellpy:
-                logging.info(
-                    f"Cellpy file not given in the journal.pages for index={index}"
-                )
-                errors.append(index)
-                continue
-
-            else:
-                logging.info(f"Processing {index}")
-
-            logging.info("loading cell")
-            try:
-                logging.debug("inside try: running cellpy.get")
-                cell_data = cellpy.get(
-                    filename=filename,
-                    instrument=instrument,
-                    cellpy_file=_cellpy_file,
-                    cycle_mode=cycle_mode,
-                    mass=mass,
-                    nom_cap=nom_cap,
-                    loading=loading,
-                    area=area,
-                    step_kwargs=step_kwargs,
-                    summary_kwargs=summary_kwargs,
-                    selector=selector,
-                    logging_mode=logging_mode,
-                    testing=testing,
-                    **cell_spec,
-                )
-                logging.info("loaded cell")
-
-            except Exception as e:
-                logging.info("Failed to load: " + str(e))
-                errors.append("update:" + str(index))
-                h_txt += " [-]"
-                pbar.set_postfix_str(s=h_txt, refresh=True)
-                if not accept_errors:
-                    raise e
-                continue
-
-            if cell_data.empty:
-                logging.info("...not loaded...")
-                logging.debug("Data is empty. Could not load cell!")
-                errors.append("check:" + str(index))
-                h_txt += " [-]"
-                pbar.set_postfix_str(s=h_txt, refresh=True)
-                continue
-
-            logging.info("...loaded successfully...")
-            h_txt += " [OK]"
-            pbar.set_postfix_str(s=h_txt, refresh=True)
-            summary_tmp = cell_data.data.summary
-            logging.info("Trying to get summary_data")
-
-            if cell_data.data.steps is None or self.force_recalc:
-                logging.info("Running make_step_table")
-                n_txt = f"steps {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.make_step_table()
-
-            if summary_tmp is None or self.force_recalc:
-                logging.info("Running make_summary")
-                n_txt = f"summary {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.make_summary(find_end_voltage=True, find_ir=True)
-
-            # some clean-ups (might not be needed anymore):
-            if not summary_tmp.index.name == hdr_summary.cycle_index:
-                logging.debug("Setting index to Cycle_Index")
-                # check if it is a byte-string
-                if b"Cycle_Index" in summary_tmp.columns:
-                    logging.debug("Seems to be a byte-string in the column-headers")
-                    summary_tmp.rename(
-                        columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
-                    )
-                try:
-                    summary_tmp.set_index("cycle_index", inplace=True)
-                except KeyError:
-                    logging.debug("cycle_index already an index")
-
-            summary_frames[index] = summary_tmp
-
-            if self.all_in_memory:
-                cell_data_frames[index] = cell_data
-            else:
-                cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
-                cell_data_frames[index].data.steps = cell_data.data.steps
-
-            if self.save_cellpy:
-                logging.info("saving to cellpy-format")
-                n_txt = f"saving {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                if self.custom_data_folder is not None:
-                    print("Save to custom data-folder not implemented yet")
-                    print(f"Saving to {row.cellpy_file_name} instead")
-                if not row.fixed:
-                    logging.info("saving cell to %s" % row.cellpy_file_name)
-                    cell_data.ensure_step_table = True
-                    try:
-                        cell_data.save(row.cellpy_file_name)
-                    except Exception as e:
-                        logging.error("saving file failed")
-                        logging.error(e)
-
-                else:
-                    logging.debug("saving cell skipped (set to 'fixed' in info_df)")
-            else:
-                logging.info("You opted to not save to cellpy-format")
-                logging.info("It is usually recommended to save to cellpy-format:")
-                logging.info(" >>> b.experiment.save_cellpy = True")
-                logging.info(
-                    "Without the cellpy-files, you cannot select specific cells"
-                )
-                logging.info("if you did not opt to store all in memory")
-
-            if self.export_raw or self.export_cycles:
-                export_text = "exporting"
-                if self.export_raw:
-                    export_text += " [raw]"
-                if self.export_cycles:
-                    export_text += " [cycles]"
-                logging.info(export_text)
-                n_txt = f"{export_text} {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.to_csv(
-                    self.journal.raw_dir,
-                    sep=prms.Reader.sep,
-                    cycles=self.export_cycles,
-                    shifted=self.shifted_cycles,
-                    raw=self.export_raw,
-                    last_cycle=self.last_cycle,
-                )
-
-            if self.export_ica:
-                logging.info("exporting [ica]")
-                try:
-                    helper.export_dqdv(
-                        cell_data,
-                        savedir=self.journal.raw_dir,
-                        sep=prms.Reader.sep,
-                        last_cycle=self.last_cycle,
-                    )
-                except Exception as e:
-                    logging.error("Could not make/export dq/dv data")
-                    logging.debug(
-                        "Failed to make/export " "dq/dv data (%s): %s" % (index, str(e))
-                    )
-                    errors.append("ica:" + str(index))
-
-        self.errors["update"] = errors
-        self.summary_frames = summary_frames
-        self.cell_data_frames = cell_data_frames
-
-    def parallel_update(
-        self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs
-    ):
-        """Updates the selected datasets in parallel.
-
-        Args:
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-            logging_mode (str): sets the logging mode for the loader(s).
-
-            kwargs:
-                transferred all the way to the instrument loader, if not
-                picked up earlier. Remark that you can obtain the same pr. cell by
-                providing a `cellspecs` dictionary. The kwargs have precedence over the
-                parameters given in the journal pages, but will be overridden by parameters
-                given by `cellspecs`.
-
-                Merging:
-                    recalc (Bool): set to False if you don't want automatic "recalc" of
-                        cycle numbers etc. when merging several data-sets.
-                Loading:
-                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                    loading from raw is not necessary (or turned off).
-
-                Debugging:
-                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
-
-        Debug-mode:
-                 - runs only for the first item in your journal
-
-        Examples:
-            >>> # Don't perform recalculation of cycle numbers etc. when merging
-            >>> # All cells:
-            >>> b.update(recalc=False)
-            >>> # For specific cell(s):
-            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
-            >>> b.update(cell_specs=cell_specs_cell_01)
-
-        """
-        status = "PROD"  # set this to DEV when developing this
-        async_mode = "threading"
-        logging.debug("PARALLEL UPDATE")
-        # TODO: implement experiment.last_cycle
-        if status != "DEV":
-            print("SORRY - MULTIPROCESSING IS NOT IMPLEMENTED PROPERLY YET")
-            return self.update(
-                all_in_memory=all_in_memory,
-                cell_specs=cell_specs,
-                logging_mode=logging_mode,
-                **kwargs,
-            )
-
-        import concurrent.futures
-        import multiprocessing
-
-        max_number_processes = multiprocessing.cpu_count()
-
-        if async_mode == "threading":
-            pool_executor = concurrent.futures.ThreadPoolExecutor
-        else:
-            pool_executor = concurrent.futures.ProcessPoolExecutor
-
-        debugging = kwargs.pop("debug", False)
-
-        # --- cleaning up attributes / arguments etc ---
-        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
-        force_raw = kwargs.pop("force_raw", self.force_raw)
-
-        logging.info("[update experiment]")
-        if all_in_memory is not None:
-            self.all_in_memory = all_in_memory
-
-        logging.info(f"Additional keyword arguments: {kwargs}")
-        selector = kwargs.get("selector", None)
-
-        pages = self.journal.pages
-        if self.nom_cap:
-            warnings.warn(
-                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
-                "the journal pages."
-            )
-            pages[hdr_journal.nom_cap] = self.nom_cap
-
-        if self.instrument:
-            warnings.warn(
-                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
-            )
-            pages[hdr_journal.instrument] = self.instrument
-
-        if x := kwargs.pop("instrument", None):
-            warnings.warn(
-                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
-                "Future version will require instrument in the journal pages."
-            )
-            pages[hdr_journal.instrument] = x
-
-        if pages.empty:
-            raise Exception("your journal is empty")
-
-        # --- init ---
-        summary_frames = dict()
-        cell_data_frames = dict()
-        number_of_runs = len(pages)
-        logging.debug(f"You have {number_of_runs} cells in your journal")
-        counter = 0
-        errors = []
-
-        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
-
-        if debugging:
-            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
-
-        # --- iterating ---
-        # TODO: create a multiprocessing pool and get one statusbar pr cell
-        params = []
-        with pool_executor(max_number_processes) as executor:
-            for index, row in pages.iterrows():
-                counter += 1
-                cell_spec_page = self._get_cell_spec_from_page(index, row)
-
-                if cell_specs is not None:
-                    cell_spec = cell_specs.get(index, dict())
-                else:
-                    cell_spec = dict()
-
-                cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
-
-                # --- UPDATING ARGUMENTS ---
-                filename = None
-                instrument = None
-                cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
-                _cellpy_file = None
-                if not force_raw and cellpy_file.is_file():
-                    _cellpy_file = cellpy_file
-                    logging.debug(f"Got cellpy file: {_cellpy_file}")
-                if not force_cellpy:
-                    filename = row[hdr_journal.raw_file_names]
-                    instrument = row[hdr_journal.instrument]
-
-                cycle_mode = row[hdr_journal.cell_type]
-                mass = row[hdr_journal.mass]
-                nom_cap = row[hdr_journal.nom_cap]
-
-                loading = None
-                area = None
-                if hdr_journal.loading in row:
-                    loading = row[hdr_journal.loading]
-                if hdr_journal.area in row:
-                    area = row[hdr_journal.area]
-
-                summary_kwargs = {
-                    "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
-                }
-
-                step_kwargs = {}
-                if not filename and not force_cellpy:
-                    logging.info(
-                        f"Raw file(s) not given in the journal.pages for index={index}"
-                    )
-                    errors.append(index)
-                    continue
-
-                elif not cellpy_file and force_cellpy:
-                    logging.info(
-                        f"Cellpy file not given in the journal.pages for index={index}"
-                    )
-                    errors.append(index)
-                    continue
-
-                else:
-                    logging.info(f"Processing {index}")
-
-                logging.info("loading cell")
-                params.append(
-                    dict(
-                        filename=filename,
-                        instrument=instrument,
-                        cellpy_file=_cellpy_file,
-                        cycle_mode=cycle_mode,
-                        mass=mass,
-                        nom_cap=nom_cap,
-                        loading=loading,
-                        area=area,
-                        step_kwargs=step_kwargs,
-                        summary_kwargs=summary_kwargs,
-                        selector=selector,
-                        logging_mode=logging_mode,
-                        testing=False,
-                        **cell_spec,
-                    )
-                )
-
-            pool = [executor.submit(cellpy.get, **param) for param in params]
-            for i in concurrent.futures.as_completed(pool):
-                cell_data = i.result()
-                if cell_data.empty:
-                    logging.info("...not loaded...")
-                    logging.debug("Data is empty. Could not load cell!")
-                    errors.append("check:" + str(index))
-
-                logging.info("...loaded successfully...")
-                summary_tmp = cell_data.data.summary
-                logging.info("Trying to get summary_data")
-
-                if cell_data.data.steps is None or self.force_recalc:
-                    logging.info("Running make_step_table")
-                    cell_data.make_step_table()
-
-                if summary_tmp is None or self.force_recalc:
-                    logging.info("Running make_summary")
-                    cell_data.make_summary(find_end_voltage=True, find_ir=True)
-
-                # some clean-ups (might not be needed anymore):
-                if not summary_tmp.index.name == hdr_summary.cycle_index:
-                    logging.debug("Setting index to Cycle_Index")
-                    # check if it is a byte-string
-                    if b"Cycle_Index" in summary_tmp.columns:
-                        logging.debug("Seems to be a byte-string in the column-headers")
-                        summary_tmp.rename(
-                            columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
-                        )
-                    try:
-                        summary_tmp.set_index("cycle_index", inplace=True)
-                    except KeyError:
-                        logging.debug("cycle_index already an index")
-
-                summary_frames[index] = summary_tmp
-
-                if self.all_in_memory:
-                    cell_data_frames[index] = cell_data
-                else:
-                    cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
-                    cell_data_frames[index].data.steps = cell_data.data.steps
-
-                if self.save_cellpy:
-                    logging.info("saving to cellpy-format")
-                    n_txt = f"saving {counter}"
-                    pbar.set_description(n_txt, refresh=True)
-                    if self.custom_data_folder is not None:
-                        print("Save to custom data-folder not implemented yet")
-                        print(f"Saving to {row.cellpy_file_name} instead")
-                    if not row.fixed:
-                        logging.info("saving cell to %s" % row.cellpy_file_name)
-                        cell_data.ensure_step_table = True
-                        try:
-                            cell_data.save(row.cellpy_file_name)
-                        except Exception as e:
-                            logging.error("saving file failed")
-                            logging.error(e)
-
-                    else:
-                        logging.debug("saving cell skipped (set to 'fixed' in info_df)")
-                else:
-                    logging.info("You opted to not save to cellpy-format")
-                    logging.info("It is usually recommended to save to cellpy-format:")
-                    logging.info(" >>> b.experiment.save_cellpy = True")
-                    logging.info(
-                        "Without the cellpy-files, you cannot select specific cells"
-                    )
-                    logging.info("if you did not opt to store all in memory")
-
-                if self.export_raw or self.export_cycles:
-                    export_text = "exporting"
-                    if self.export_raw:
-                        export_text += " [raw]"
-                    if self.export_cycles:
-                        export_text += " [cycles]"
-                    logging.info(export_text)
-                    n_txt = f"{export_text} {counter}"
-                    pbar.set_description(n_txt, refresh=True)
-                    cell_data.to_csv(
-                        self.journal.raw_dir,
-                        sep=prms.Reader.sep,
-                        cycles=self.export_cycles,
-                        shifted=self.shifted_cycles,
-                        raw=self.export_raw,
-                        last_cycle=self.last_cycle,
-                    )
-
-                if self.export_ica:
-                    logging.info("exporting [ica]")
-                    try:
-                        helper.export_dqdv(
-                            cell_data,
-                            savedir=self.journal.raw_dir,
-                            sep=prms.Reader.sep,
-                            last_cycle=self.last_cycle,
-                        )
-                    except Exception as e:
-                        logging.error("Could not make/export dq/dv data")
-                        logging.debug(
-                            "Failed to make/export "
-                            "dq/dv data (%s): %s" % (index, str(e))
-                        )
-                        errors.append("ica:" + str(index))
-
-        self.errors["update"] = errors
-        self.summary_frames = summary_frames
-        self.cell_data_frames = cell_data_frames
-
-    def export_cellpy_files(self, path=None, **kwargs):
-        """Export all cellpy-files to a given path.
-
-        Remarks:
-            This method can only export to local folders
-            (OtherPath objects are not formally supported, but
-            might still work if the path is local).
-
-        Args:
-            path (str, pathlib.Path): path to export to (default: current working directory)
-        """
-        if path is None:
-            path = "."
-        errors = []
-        path = pathlib.Path(path)
-        cell_names = self.cell_names
-        for cell_name in cell_names:
-            cellpy_file_name = self.journal.pages.loc[
-                cell_name, hdr_journal.cellpy_file_name
-            ]
-            cellpy_file_name = path / pathlib.Path(cellpy_file_name).name
-            print(f"Exporting {cell_name} to {cellpy_file_name}")
-            try:
-                c = self.data[cell_name]
-            except TypeError as e:
-                errors.append(f"could not extract data for {cell_name} - linking")
-                self._link_cellpy_file(cell_name)
-
-            c.save(cellpy_file_name, **kwargs)
-        self.errors["export_cellpy_files"] = errors
-
-    @property
-    def cell_names(self):
-        """Returns a list of cell-names (strings)"""
-        try:
-            return [key for key in self.cell_data_frames]
-        except TypeError:
-            return None
-
-    def status(self):
-        print("\n")
-        print(" STATUS ".center(80, "="))
-        print(self)
-        print(" summary frames ".center(80, "-"))
-        if self.summary_frames is not None:
-            for key in self.summary_frames:
-                print(f" {{{key}}}")
-        print(" memory dumped ".center(80, "-"))
-        if self.memory_dumped is not None:
-            for key in self.memory_dumped:
-                print(f"{key}: {type(self.memory_dumped[key])}")
-        print(80 * "=")
-
-    def link(self, **kwargs):
-        """Ensure that an appropriate link to the cellpy-files exists for
-        each cell.
-
-        The experiment will then contain a CellpyCell object for each cell
-        (in the cell_data_frames attribute) with only the step-table stored.
-
-        Remark that running update persists the summary frames instead (or
-        everything in case you specify all_in_memory=True).
-        This might be considered "a strange and unexpected behaviour". Sorry
-        for that (but the authors of this package is also a bit strange...).
-
-        (OK, I will change it. Soon.)
-
-        **kwargs: passed to _link_cellpy_file
-            max_cycle (int): maximum cycle number to link/load (remark that the
-                cellpy objects will get the property overwrite_able set to False
-                if you give a max_cycle to prevent accidentally saving a "truncated"
-                file (use c.save(filename, overwrite=True) to force overwrite))
-
-
-        """
-        logging.info("[establishing links]")
-        logging.debug("checking and establishing link to data")
-
-        errors = []
-
-        for cell_label in self.journal.pages.index:
-            logging.debug(f"trying to link {cell_label}")
-            try:
-                self._link_cellpy_file(cell_label, **kwargs)
-            except IOError as e:
-                logging.warning(e)
-                e_txt = f"{cell_label}: links not established - try update instead"
-                logging.warning(e_txt)
-                errors.append(e_txt)
-
-        self.errors["link"] = errors
-
-    def recalc(
-        self,
-        save=True,
-        step_opts=None,
-        summary_opts=None,
-        indexes=None,
-        calc_steps=True,
-        testing=False,
-    ):
-        """Run make_step_table and make_summary on all cells.
-
-        Args:
-            save (bool): Save updated cellpy-files if True.
-            step_opts (dict): parameters to inject to make_steps.
-            summary_opts (dict): parameters to inject to make_summary.
-            indexes (list): Only recalculate for given indexes (i.e. list of cell-names).
-            calc_steps (bool): Run make_steps before making the summary.
-            testing (bool): Only for testing purposes.
-
-        Returns:
-            None
-        """
-
-        # TODO: option (default) to only recalc if the values (mass, nom_cap,...) have changed
-        errors = []
-        log = []
-        if testing:
-            pbar = tqdm(
-                list(self.journal.pages.iloc[0:2, :].iterrows()),
-                file=sys.stdout,
-                leave=False,
-            )
-        elif indexes is not None:
-            pbar = tqdm(
-                list(self.journal.pages.loc[indexes, :].iterrows()),
-                file=sys.stdout,
-                leave=False,
-            )
-        else:
-            pbar = tqdm(
-                list(self.journal.pages.iterrows()), file=sys.stdout, leave=False
-            )
-        for indx, row in pbar:
-            nom_cap = row[hdr_journal.nom_cap]
-            mass = row[hdr_journal.mass]
-            pbar.set_description(indx)
-            try:
-                c = self.data[indx]
-            except TypeError as e:
-                e_txt = (
-                    f"could not extract data for {indx} - have you forgotten to link?"
-                )
-                errors.append(e_txt)
-                warnings.warn(e_txt)
-
-            else:
-                if nom_cap:
-                    c.set_nom_cap(nom_cap)
-                if mass:
-                    c.set_mass(mass)
-                try:
-                    if calc_steps:
-                        pbar.set_postfix_str(s="steps", refresh=True)
-                        if step_opts is not None:
-                            c.make_step_table(**step_opts)
-                        else:
-                            c.make_step_table()
-
-                    pbar.set_postfix_str(s="summary", refresh=True)
-                    if summary_opts is not None:
-                        c.make_summary(**summary_opts)
-                    else:
-                        c.make_summary(find_end_voltage=True, find_ir=True)
-
-                except Exception as e:
-                    e_txt = f"recalculating for {indx} failed!"
-                    errors.append(e_txt)
-                    warnings.warn(e_txt)
-                else:
-                    if save:
-                        # remark! got a win error when trying to save (hdf5-file in use) (must fix this)
-                        pbar.set_postfix_str(s="save", refresh=True)
-                        try:
-                            c.save(row.cellpy_file_name)
-                            log.append(f"saved {indx} to {row.cellpy_file_name}")
-                        except Exception as e:
-                            e_txt = f"saving {indx} to {row.cellpy_file_name} failed!"
-                            errors.append(e_txt)
-                            warnings.warn(e_txt)
-        self.errors["recalc"] = errors
-        self.log["recalc"] = log
-
-
-class ImpedanceExperiment(BaseExperiment):
-    def __init__(self):
-        super().__init__()
-
-
-class LifeTimeExperiment(BaseExperiment):
-    def __init__(self):
-        super().__init__()
-
-
-if __name__ == "__main__":
-    from pathlib import Path
-    import os
-    import pandas as pd
-    import numpy as np
-    import seaborn as sns
-    import plotly.express as px
-
-    import cellpy
-    from cellpy.utils import batch, helpers, plotutils
-
-    project_dir = Path("../../../testdata/batch_project")
-    print(f"{project_dir.resolve()=}")
-    journal = project_dir / "test_project.json"
-    journal = journal.resolve()
-    print(f"{journal=}")
-    assert project_dir.is_dir()
-    assert journal.is_file()
-    os.chdir(project_dir)
-
-    print(f"cellpy version: {cellpy.__version__}")
-    cellpy.log.setup_logging("INFO")
-
-    b = batch.from_journal(journal)
-    b.update()
-
-    print("Ended OK")
+import ast
+import logging
+import os
+import pathlib
+import sys
+import warnings
+
+import pandas as pd
+from tqdm.auto import tqdm
+
+import cellpy
+from cellpy import prms
+from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
+from cellpy.readers import cellreader
+from cellpy.internals.core import OtherPath
+from cellpy.utils.batch_tools import batch_helpers as helper
+from cellpy.utils.batch_tools.batch_core import BaseExperiment
+from cellpy.utils.batch_tools.batch_journals import LabJournal
+
+hdr_journal = get_headers_journal()
+hdr_summary = get_headers_summary()
+
+
+class CyclingExperiment(BaseExperiment):
+    """Load experimental data into memory.
+
+    This is a re-implementation of the old batch behaviour where
+    all the data-files are processed sequentially (and optionally exported)
+    while the summary tables are kept and processed. This implementation
+    also saves the step tables (for later use when using look-up
+    functionality).
+
+
+    Attributes:
+        journal (:obj: LabJournal): information about the experiment.
+        force_cellpy (bool): tries only to load the cellpy-file if True.
+        force_raw (bool): loads raw-file(s) even though appropriate cellpy-file
+           exists if True.
+        save_cellpy (bool): saves a cellpy-file for each cell if True.
+        accept_errors (bool): in case of error, dont raise an exception, but
+           continue to the next file if True.
+        all_in_memory (bool): store the cellpydata-objects in memory if True.
+        export_cycles (bool): export voltage-capacity curves if True.
+        shifted_cycles (bool): set this to True if you want to export the
+           voltage-capacity curves using the shifted-cycles option (only valid
+           if you set export_cycles to True).
+        export_raw (bool): export the raw-data if True.
+        export_ica (bool): export dq-dv curves if True.
+        last_cycle (int): sets the last cycle (i.e. the highest cycle number)
+           that you would like to process dq-dv on). Use all if None (the
+           default value).
+        selected_summaries (list): a list of summary labels defining what
+           summary columns to make joint summaries from (optional).
+        errors (dict): contains a dictionary listing all the errors encountered.
+
+    Args:
+        db_reader (str or object): custom db_reader (see doc on db_reader).
+
+    Example:
+
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        db_reader = kwargs.pop("db_reader", "default")
+        super().__init__(*args)
+        self.journal = LabJournal(db_reader=db_reader)
+        self.errors = dict()
+        self.log = dict()
+
+        self.force_cellpy = False
+        self.force_raw = False
+        self.force_recalc = False
+        self.save_cellpy = True
+        self.accept_errors = False
+        self.all_in_memory = False
+
+        self.export_cycles = False
+        self.shifted_cycles = False
+        self.export_raw = True
+        self.export_ica = False
+        self.last_cycle = None
+        self.nom_cap = None
+        self.instrument = None
+        self.custom_data_folder = None
+
+        self.selected_summaries = None
+
+    def _repr_html_(self):
+        txt = f"<h2>CyclingExperiment-object</h2> id={hex(id(self))}"
+        txt += "<h3>Main attributes</h3>"
+        txt += f"""
+        <table>
+            <thead>
+                <tr>
+                    <th>Attribute</th>
+                    <th>Value</th>
+                </tr>
+            </thead>
+            <tbody>
+                <tr><td><b>force_cellpy</b></td><td>{self.force_cellpy}</td></tr>
+                <tr><td><b>force_raw</b></td><td>{self.force_raw}</td></tr>
+                <tr><td><b>force_recalc</b></td><td>{self.force_recalc}</td></tr>
+                <tr><td><b>save_cellpy</b></td><td>{self.save_cellpy}</td></tr>
+                <tr><td><b>accept_errors</b></td><td>{self.accept_errors}</td></tr>
+                <tr><td><b>all_in_memory</b></td><td>{self.all_in_memory}</td></tr>
+                <tr><td><b>export_cycles</b></td><td>{self.export_cycles}</td></tr>
+                <tr><td><b>shifted_cycles</b></td><td>{self.shifted_cycles}</td></tr>
+                <tr><td><b>export_raw</b></td><td>{self.export_raw}</td></tr>
+                <tr><td><b>export_ica</b></td><td>{self.export_ica}</td></tr>
+                <tr><td><b>last_cycle</b></td><td>{self.last_cycle}</td></tr>
+                <tr><td><b>nom_cap</b></td><td>{self.nom_cap}</td></tr>
+                <tr><td><b>instrument</b></td><td>{self.instrument}</td></tr>
+                <tr><td><b>custom_data_folder</b></td><td>{self.custom_data_folder}</td></tr>
+                <tr><td><b>selected_summaries</b></td><td>{self.selected_summaries}</td></tr>
+            </tbody>
+        </table>
+        """
+        txt += "<h3>Cells</h3>"
+        txt += f"<p><b>data</b>: contains {len(self)} cells.</p>"
+        return txt
+
+    @staticmethod
+    def _get_cell_spec_from_page(indx: int, row: pd.Series) -> dict:
+        # Edit this if we decide to make "argument families", e.g. loader_split or merger_recalc.
+
+        PRM_SPLITTER = ";"
+        EQUAL_SIGN = "="
+
+        def _arg_parser(text: str) -> None:
+            individual_specs = text.split(PRM_SPLITTER)
+            for p in individual_specs:
+                p, a = p.split(EQUAL_SIGN)
+
+        logging.debug(f"getting cell_spec from journal pages ({indx})")
+        try:
+            cell_spec = row[hdr_journal.argument]
+            logging.debug(cell_spec)
+            if not isinstance(cell_spec, dict):
+                raise TypeError("the cell spec argument is not a dictionary")
+        except Exception as e:
+            logging.warning(f"could not get cell spec for {indx}")
+            logging.warning(f"error message: {e}")
+            return {}
+
+        # converting from str if needed
+        for spec in cell_spec:
+            if isinstance(cell_spec[spec], str):
+                if cell_spec[spec].lower() == "true":
+                    cell_spec[spec] = True
+                elif cell_spec[spec].lower() == "false":
+                    cell_spec[spec] = False
+                elif cell_spec[spec].lower() == "none":
+                    cell_spec[spec] = None
+                else:
+                    try:
+                        logging.debug(
+                            f"Using ast.literal_eval to convert cell-spec value from str '{cell_spec[spec]}'"
+                        )
+                        cell_spec[spec] = ast.literal_eval(cell_spec[spec])
+                    except ValueError as e:
+                        logging.warning(
+                            f"ERROR! Could not convert from str to python object!"
+                        )
+                        logging.debug(e)
+        return cell_spec
+
+    def update(
+        self,
+        all_in_memory=None,
+        cell_specs=None,
+        logging_mode=None,
+        accept_errors=None,
+        **kwargs,
+    ):
+        """Updates the selected datasets.
+
+        Args:
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+            accept_errors (bool): if True, the loader will continue even if it encounters errors.
+
+            kwargs:
+                transferred all the way to the instrument loader, if not
+                picked up earlier. Remark that you can obtain the same pr. cell by
+                providing a `cellspecs` dictionary. The kwargs have precedence over the
+                parameters given in the journal pages, but will be overridden by parameters
+                given by `cellspecs`.
+
+                Merging:
+                    recalc (Bool): set to False if you don't want automatic "recalc" of
+                        cycle numbers etc. when merging several data-sets.
+                Loading:
+                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                    loading from raw is not necessary (or turned off).
+
+                Debugging:
+                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
+
+        Debug-mode:
+                 - runs only for the first item in your journal
+
+        Examples:
+            >>> # Don't perform recalculation of cycle numbers etc. when merging
+            >>> # All cells:
+            >>> b.update(recalc=False)
+            >>> # For specific cell(s):
+            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
+            >>> b.update(cell_specs=cell_specs_cell_01)
+
+        """
+
+        # TODO: implement experiment.last_cycle
+        accept_errors = accept_errors or self.accept_errors
+
+        debugging = kwargs.pop("debug", False)
+        testing = kwargs.pop("testing", False)
+
+        # --- cleaning up attributes / arguments etc ---
+        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
+        force_raw = kwargs.pop("force_raw", self.force_raw)
+
+        logging.info("[update experiment]")
+        if all_in_memory is not None:
+            self.all_in_memory = all_in_memory
+
+        logging.info(f"Additional keyword arguments: {kwargs}")
+        selector = kwargs.get("selector", None)
+
+        pages = self.journal.pages
+        if self.nom_cap:
+            warnings.warn(
+                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
+                "the journal pages."
+            )
+            pages[hdr_journal.nom_cap] = self.nom_cap
+
+        if self.instrument:
+            warnings.warn(
+                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
+            )
+            pages[hdr_journal.instrument] = self.instrument
+
+        if x := kwargs.pop("instrument", None):
+            warnings.warn(
+                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
+                "Future version will require instrument in the journal pages."
+            )
+            pages[hdr_journal.instrument] = x
+
+        if pages.empty:
+            raise Exception("your journal is empty")
+
+        # --- init ---
+        summary_frames = dict()
+        cell_data_frames = dict()
+        number_of_runs = len(pages)
+        logging.debug(f"You have {number_of_runs} cells in your journal")
+        counter = 0
+        errors = []
+
+        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
+
+        if debugging:
+            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
+
+        # --- iterating ---
+        # TODO: create a multiprocessing pool and get one statusbar pr cell
+        for index, row in pbar:
+            counter += 1
+            h_txt = f"{index}"
+            n_txt = f"loading {counter}"
+            l_txt = f"starting to process file # {counter} ({index})"
+            pbar.set_description(n_txt, refresh=True)
+            cell_spec_page = self._get_cell_spec_from_page(index, row)
+
+            if cell_specs is not None:
+                cell_spec = cell_specs.get(index, dict())
+            else:
+                cell_spec = dict()
+
+            cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
+            l_txt += f" cell_spec: {cell_spec}"
+            logging.debug(l_txt)
+
+            # --- UPDATING ARGUMENTS ---
+            filename = None
+            instrument = None
+            cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+            _cellpy_file = None
+            if not force_raw and cellpy_file.is_file():
+                _cellpy_file = cellpy_file
+                logging.debug(f"Got cellpy file: {_cellpy_file}")
+            if not force_cellpy:
+                filename = row[hdr_journal.raw_file_names]
+                instrument = row[hdr_journal.instrument]
+
+            cycle_mode = row[hdr_journal.cell_type]
+            mass = row[hdr_journal.mass]
+            nom_cap = row[hdr_journal.nom_cap]
+
+            loading = None
+            area = None
+            if hdr_journal.loading in row:
+                loading = row[hdr_journal.loading]
+            if hdr_journal.area in row:
+                area = row[hdr_journal.area]
+
+            summary_kwargs = {
+                "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
+            }
+
+            step_kwargs = {}
+            if not filename and not force_cellpy:
+                logging.info(
+                    f"Raw file(s) not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
+
+            elif not cellpy_file and force_cellpy:
+                logging.info(
+                    f"Cellpy file not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
+
+            else:
+                logging.info(f"Processing {index}")
+
+            logging.info("loading cell")
+            try:
+                logging.debug("inside try: running cellpy.get")
+                cell_data = cellpy.get(
+                    filename=filename,
+                    instrument=instrument,
+                    cellpy_file=_cellpy_file,
+                    cycle_mode=cycle_mode,
+                    mass=mass,
+                    nom_cap=nom_cap,
+                    loading=loading,
+                    area=area,
+                    step_kwargs=step_kwargs,
+                    summary_kwargs=summary_kwargs,
+                    selector=selector,
+                    logging_mode=logging_mode,
+                    testing=testing,
+                    **cell_spec,
+                )
+                logging.info("loaded cell")
+
+            except Exception as e:
+                logging.info("Failed to load: " + str(e))
+                errors.append("update:" + str(index))
+                h_txt += " [-]"
+                pbar.set_postfix_str(s=h_txt, refresh=True)
+                if not accept_errors:
+                    raise e
+                continue
+
+            if cell_data.empty:
+                logging.info("...not loaded...")
+                logging.debug("Data is empty. Could not load cell!")
+                errors.append("check:" + str(index))
+                h_txt += " [-]"
+                pbar.set_postfix_str(s=h_txt, refresh=True)
+                continue
+
+            logging.info("...loaded successfully...")
+            h_txt += " [OK]"
+            pbar.set_postfix_str(s=h_txt, refresh=True)
+            summary_tmp = cell_data.data.summary
+            logging.info("Trying to get summary_data")
+
+            if cell_data.data.steps is None or self.force_recalc:
+                logging.info("Running make_step_table")
+                n_txt = f"steps {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.make_step_table()
+
+            if summary_tmp is None or self.force_recalc:
+                logging.info("Running make_summary")
+                n_txt = f"summary {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.make_summary(find_end_voltage=True, find_ir=True)
+
+            # some clean-ups (might not be needed anymore):
+            if not summary_tmp.index.name == hdr_summary.cycle_index:
+                logging.debug("Setting index to Cycle_Index")
+                # check if it is a byte-string
+                if b"Cycle_Index" in summary_tmp.columns:
+                    logging.debug("Seems to be a byte-string in the column-headers")
+                    summary_tmp.rename(
+                        columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
+                    )
+                try:
+                    summary_tmp.set_index("cycle_index", inplace=True)
+                except KeyError:
+                    logging.debug("cycle_index already an index")
+
+            summary_frames[index] = summary_tmp
+
+            if self.all_in_memory:
+                cell_data_frames[index] = cell_data
+            else:
+                cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
+                cell_data_frames[index].data.steps = cell_data.data.steps
+
+            if self.save_cellpy:
+                logging.info("saving to cellpy-format")
+                n_txt = f"saving {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                if self.custom_data_folder is not None:
+                    print("Save to custom data-folder not implemented yet")
+                    print(f"Saving to {row.cellpy_file_name} instead")
+                if not row.fixed:
+                    logging.info("saving cell to %s" % row.cellpy_file_name)
+                    cell_data.ensure_step_table = True
+                    try:
+                        cell_data.save(row.cellpy_file_name)
+                    except Exception as e:
+                        logging.error("saving file failed")
+                        logging.error(e)
+
+                else:
+                    logging.debug("saving cell skipped (set to 'fixed' in info_df)")
+            else:
+                logging.info("You opted to not save to cellpy-format")
+                logging.info("It is usually recommended to save to cellpy-format:")
+                logging.info(" >>> b.experiment.save_cellpy = True")
+                logging.info(
+                    "Without the cellpy-files, you cannot select specific cells"
+                )
+                logging.info("if you did not opt to store all in memory")
+
+            if self.export_raw or self.export_cycles:
+                export_text = "exporting"
+                if self.export_raw:
+                    export_text += " [raw]"
+                if self.export_cycles:
+                    export_text += " [cycles]"
+                logging.info(export_text)
+                n_txt = f"{export_text} {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.to_csv(
+                    self.journal.raw_dir,
+                    sep=prms.Reader.sep,
+                    cycles=self.export_cycles,
+                    shifted=self.shifted_cycles,
+                    raw=self.export_raw,
+                    last_cycle=self.last_cycle,
+                )
+
+            if self.export_ica:
+                logging.info("exporting [ica]")
+                try:
+                    helper.export_dqdv(
+                        cell_data,
+                        savedir=self.journal.raw_dir,
+                        sep=prms.Reader.sep,
+                        last_cycle=self.last_cycle,
+                    )
+                except Exception as e:
+                    logging.error("Could not make/export dq/dv data")
+                    logging.debug(
+                        "Failed to make/export " "dq/dv data (%s): %s" % (index, str(e))
+                    )
+                    errors.append("ica:" + str(index))
+
+        self.errors["update"] = errors
+        self.summary_frames = summary_frames
+        self.cell_data_frames = cell_data_frames
+
+    def parallel_update(
+        self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs
+    ):
+        """Updates the selected datasets in parallel.
+
+        Args:
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+
+            kwargs:
+                transferred all the way to the instrument loader, if not
+                picked up earlier. Remark that you can obtain the same pr. cell by
+                providing a `cellspecs` dictionary. The kwargs have precedence over the
+                parameters given in the journal pages, but will be overridden by parameters
+                given by `cellspecs`.
+
+                Merging:
+                    recalc (Bool): set to False if you don't want automatic "recalc" of
+                        cycle numbers etc. when merging several data-sets.
+                Loading:
+                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                    loading from raw is not necessary (or turned off).
+
+                Debugging:
+                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
+
+        Debug-mode:
+                 - runs only for the first item in your journal
+
+        Examples:
+            >>> # Don't perform recalculation of cycle numbers etc. when merging
+            >>> # All cells:
+            >>> b.update(recalc=False)
+            >>> # For specific cell(s):
+            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
+            >>> b.update(cell_specs=cell_specs_cell_01)
+
+        """
+        status = "PROD"  # set this to DEV when developing this
+        async_mode = "threading"
+        logging.debug("PARALLEL UPDATE")
+        # TODO: implement experiment.last_cycle
+        if status != "DEV":
+            print("SORRY - MULTIPROCESSING IS NOT IMPLEMENTED PROPERLY YET")
+            return self.update(
+                all_in_memory=all_in_memory,
+                cell_specs=cell_specs,
+                logging_mode=logging_mode,
+                **kwargs,
+            )
+
+        import concurrent.futures
+        import multiprocessing
+
+        max_number_processes = multiprocessing.cpu_count()
+
+        if async_mode == "threading":
+            pool_executor = concurrent.futures.ThreadPoolExecutor
+        else:
+            pool_executor = concurrent.futures.ProcessPoolExecutor
+
+        debugging = kwargs.pop("debug", False)
+
+        # --- cleaning up attributes / arguments etc ---
+        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
+        force_raw = kwargs.pop("force_raw", self.force_raw)
+
+        logging.info("[update experiment]")
+        if all_in_memory is not None:
+            self.all_in_memory = all_in_memory
+
+        logging.info(f"Additional keyword arguments: {kwargs}")
+        selector = kwargs.get("selector", None)
+
+        pages = self.journal.pages
+        if self.nom_cap:
+            warnings.warn(
+                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
+                "the journal pages."
+            )
+            pages[hdr_journal.nom_cap] = self.nom_cap
+
+        if self.instrument:
+            warnings.warn(
+                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
+            )
+            pages[hdr_journal.instrument] = self.instrument
+
+        if x := kwargs.pop("instrument", None):
+            warnings.warn(
+                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
+                "Future version will require instrument in the journal pages."
+            )
+            pages[hdr_journal.instrument] = x
+
+        if pages.empty:
+            raise Exception("your journal is empty")
+
+        # --- init ---
+        summary_frames = dict()
+        cell_data_frames = dict()
+        number_of_runs = len(pages)
+        logging.debug(f"You have {number_of_runs} cells in your journal")
+        counter = 0
+        errors = []
+
+        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
+
+        if debugging:
+            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
+
+        # --- iterating ---
+        # TODO: create a multiprocessing pool and get one statusbar pr cell
+        params = []
+        with pool_executor(max_number_processes) as executor:
+            for index, row in pages.iterrows():
+                counter += 1
+                cell_spec_page = self._get_cell_spec_from_page(index, row)
+
+                if cell_specs is not None:
+                    cell_spec = cell_specs.get(index, dict())
+                else:
+                    cell_spec = dict()
+
+                cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
+
+                # --- UPDATING ARGUMENTS ---
+                filename = None
+                instrument = None
+                cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+                _cellpy_file = None
+                if not force_raw and cellpy_file.is_file():
+                    _cellpy_file = cellpy_file
+                    logging.debug(f"Got cellpy file: {_cellpy_file}")
+                if not force_cellpy:
+                    filename = row[hdr_journal.raw_file_names]
+                    instrument = row[hdr_journal.instrument]
+
+                cycle_mode = row[hdr_journal.cell_type]
+                mass = row[hdr_journal.mass]
+                nom_cap = row[hdr_journal.nom_cap]
+
+                loading = None
+                area = None
+                if hdr_journal.loading in row:
+                    loading = row[hdr_journal.loading]
+                if hdr_journal.area in row:
+                    area = row[hdr_journal.area]
+
+                summary_kwargs = {
+                    "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
+                }
+
+                step_kwargs = {}
+                if not filename and not force_cellpy:
+                    logging.info(
+                        f"Raw file(s) not given in the journal.pages for index={index}"
+                    )
+                    errors.append(index)
+                    continue
+
+                elif not cellpy_file and force_cellpy:
+                    logging.info(
+                        f"Cellpy file not given in the journal.pages for index={index}"
+                    )
+                    errors.append(index)
+                    continue
+
+                else:
+                    logging.info(f"Processing {index}")
+
+                logging.info("loading cell")
+                params.append(
+                    dict(
+                        filename=filename,
+                        instrument=instrument,
+                        cellpy_file=_cellpy_file,
+                        cycle_mode=cycle_mode,
+                        mass=mass,
+                        nom_cap=nom_cap,
+                        loading=loading,
+                        area=area,
+                        step_kwargs=step_kwargs,
+                        summary_kwargs=summary_kwargs,
+                        selector=selector,
+                        logging_mode=logging_mode,
+                        testing=False,
+                        **cell_spec,
+                    )
+                )
+
+            pool = [executor.submit(cellpy.get, **param) for param in params]
+            for i in concurrent.futures.as_completed(pool):
+                cell_data = i.result()
+                if cell_data.empty:
+                    logging.info("...not loaded...")
+                    logging.debug("Data is empty. Could not load cell!")
+                    errors.append("check:" + str(index))
+
+                logging.info("...loaded successfully...")
+                summary_tmp = cell_data.data.summary
+                logging.info("Trying to get summary_data")
+
+                if cell_data.data.steps is None or self.force_recalc:
+                    logging.info("Running make_step_table")
+                    cell_data.make_step_table()
+
+                if summary_tmp is None or self.force_recalc:
+                    logging.info("Running make_summary")
+                    cell_data.make_summary(find_end_voltage=True, find_ir=True)
+
+                # some clean-ups (might not be needed anymore):
+                if not summary_tmp.index.name == hdr_summary.cycle_index:
+                    logging.debug("Setting index to Cycle_Index")
+                    # check if it is a byte-string
+                    if b"Cycle_Index" in summary_tmp.columns:
+                        logging.debug("Seems to be a byte-string in the column-headers")
+                        summary_tmp.rename(
+                            columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
+                        )
+                    try:
+                        summary_tmp.set_index("cycle_index", inplace=True)
+                    except KeyError:
+                        logging.debug("cycle_index already an index")
+
+                summary_frames[index] = summary_tmp
+
+                if self.all_in_memory:
+                    cell_data_frames[index] = cell_data
+                else:
+                    cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
+                    cell_data_frames[index].data.steps = cell_data.data.steps
+
+                if self.save_cellpy:
+                    logging.info("saving to cellpy-format")
+                    n_txt = f"saving {counter}"
+                    pbar.set_description(n_txt, refresh=True)
+                    if self.custom_data_folder is not None:
+                        print("Save to custom data-folder not implemented yet")
+                        print(f"Saving to {row.cellpy_file_name} instead")
+                    if not row.fixed:
+                        logging.info("saving cell to %s" % row.cellpy_file_name)
+                        cell_data.ensure_step_table = True
+                        try:
+                            cell_data.save(row.cellpy_file_name)
+                        except Exception as e:
+                            logging.error("saving file failed")
+                            logging.error(e)
+
+                    else:
+                        logging.debug("saving cell skipped (set to 'fixed' in info_df)")
+                else:
+                    logging.info("You opted to not save to cellpy-format")
+                    logging.info("It is usually recommended to save to cellpy-format:")
+                    logging.info(" >>> b.experiment.save_cellpy = True")
+                    logging.info(
+                        "Without the cellpy-files, you cannot select specific cells"
+                    )
+                    logging.info("if you did not opt to store all in memory")
+
+                if self.export_raw or self.export_cycles:
+                    export_text = "exporting"
+                    if self.export_raw:
+                        export_text += " [raw]"
+                    if self.export_cycles:
+                        export_text += " [cycles]"
+                    logging.info(export_text)
+                    n_txt = f"{export_text} {counter}"
+                    pbar.set_description(n_txt, refresh=True)
+                    cell_data.to_csv(
+                        self.journal.raw_dir,
+                        sep=prms.Reader.sep,
+                        cycles=self.export_cycles,
+                        shifted=self.shifted_cycles,
+                        raw=self.export_raw,
+                        last_cycle=self.last_cycle,
+                    )
+
+                if self.export_ica:
+                    logging.info("exporting [ica]")
+                    try:
+                        helper.export_dqdv(
+                            cell_data,
+                            savedir=self.journal.raw_dir,
+                            sep=prms.Reader.sep,
+                            last_cycle=self.last_cycle,
+                        )
+                    except Exception as e:
+                        logging.error("Could not make/export dq/dv data")
+                        logging.debug(
+                            "Failed to make/export "
+                            "dq/dv data (%s): %s" % (index, str(e))
+                        )
+                        errors.append("ica:" + str(index))
+
+        self.errors["update"] = errors
+        self.summary_frames = summary_frames
+        self.cell_data_frames = cell_data_frames
+
+    def export_cellpy_files(self, path=None, **kwargs):
+        """Export all cellpy-files to a given path.
+
+        Remarks:
+            This method can only export to local folders
+            (OtherPath objects are not formally supported, but
+            might still work if the path is local).
+
+        Args:
+            path (str, pathlib.Path): path to export to (default: current working directory)
+        """
+        if path is None:
+            path = "."
+        errors = []
+        path = pathlib.Path(path)
+        cell_names = self.cell_names
+        for cell_name in cell_names:
+            cellpy_file_name = self.journal.pages.loc[
+                cell_name, hdr_journal.cellpy_file_name
+            ]
+            cellpy_file_name = path / pathlib.Path(cellpy_file_name).name
+            print(f"Exporting {cell_name} to {cellpy_file_name}")
+            try:
+                c = self.data[cell_name]
+            except TypeError as e:
+                errors.append(f"could not extract data for {cell_name} - linking")
+                self._link_cellpy_file(cell_name)
+
+            c.save(cellpy_file_name, **kwargs)
+        self.errors["export_cellpy_files"] = errors
+
+    @property
+    def cell_names(self):
+        """Returns a list of cell-names (strings)"""
+        try:
+            return [key for key in self.cell_data_frames]
+        except TypeError:
+            return None
+
+    def status(self):
+        print("\n")
+        print(" STATUS ".center(80, "="))
+        print(self)
+        print(" summary frames ".center(80, "-"))
+        if self.summary_frames is not None:
+            for key in self.summary_frames:
+                print(f" {{{key}}}")
+        print(" memory dumped ".center(80, "-"))
+        if self.memory_dumped is not None:
+            for key in self.memory_dumped:
+                print(f"{key}: {type(self.memory_dumped[key])}")
+        print(80 * "=")
+
+    def link(self, **kwargs):
+        """Ensure that an appropriate link to the cellpy-files exists for
+        each cell.
+
+        The experiment will then contain a CellpyCell object for each cell
+        (in the cell_data_frames attribute) with only the step-table stored.
+
+        Remark that running update persists the summary frames instead (or
+        everything in case you specify all_in_memory=True).
+        This might be considered "a strange and unexpected behaviour". Sorry
+        for that (but the authors of this package is also a bit strange...).
+
+        (OK, I will change it. Soon.)
+
+        **kwargs: passed to _link_cellpy_file
+            max_cycle (int): maximum cycle number to link/load (remark that the
+                cellpy objects will get the property overwrite_able set to False
+                if you give a max_cycle to prevent accidentally saving a "truncated"
+                file (use c.save(filename, overwrite=True) to force overwrite))
+
+
+        """
+        logging.info("[establishing links]")
+        logging.debug("checking and establishing link to data")
+
+        errors = []
+
+        for cell_label in self.journal.pages.index:
+            logging.debug(f"trying to link {cell_label}")
+            try:
+                self._link_cellpy_file(cell_label, **kwargs)
+            except IOError as e:
+                logging.warning(e)
+                e_txt = f"{cell_label}: links not established - try update instead"
+                logging.warning(e_txt)
+                errors.append(e_txt)
+
+        self.errors["link"] = errors
+
+    def recalc(
+        self,
+        save=True,
+        step_opts=None,
+        summary_opts=None,
+        indexes=None,
+        calc_steps=True,
+        testing=False,
+    ):
+        """Run make_step_table and make_summary on all cells.
+
+        Args:
+            save (bool): Save updated cellpy-files if True.
+            step_opts (dict): parameters to inject to make_steps.
+            summary_opts (dict): parameters to inject to make_summary.
+            indexes (list): Only recalculate for given indexes (i.e. list of cell-names).
+            calc_steps (bool): Run make_steps before making the summary.
+            testing (bool): Only for testing purposes.
+
+        Returns:
+            None
+        """
+
+        # TODO: option (default) to only recalc if the values (mass, nom_cap,...) have changed
+        errors = []
+        log = []
+        if testing:
+            pbar = tqdm(
+                list(self.journal.pages.iloc[0:2, :].iterrows()),
+                file=sys.stdout,
+                leave=False,
+            )
+        elif indexes is not None:
+            pbar = tqdm(
+                list(self.journal.pages.loc[indexes, :].iterrows()),
+                file=sys.stdout,
+                leave=False,
+            )
+        else:
+            pbar = tqdm(
+                list(self.journal.pages.iterrows()), file=sys.stdout, leave=False
+            )
+        for indx, row in pbar:
+            nom_cap = row[hdr_journal.nom_cap]
+            mass = row[hdr_journal.mass]
+            pbar.set_description(indx)
+            try:
+                c = self.data[indx]
+            except TypeError as e:
+                e_txt = (
+                    f"could not extract data for {indx} - have you forgotten to link?"
+                )
+                errors.append(e_txt)
+                warnings.warn(e_txt)
+
+            else:
+                if nom_cap:
+                    c.set_nom_cap(nom_cap)
+                if mass:
+                    c.set_mass(mass)
+                try:
+                    if calc_steps:
+                        pbar.set_postfix_str(s="steps", refresh=True)
+                        if step_opts is not None:
+                            c.make_step_table(**step_opts)
+                        else:
+                            c.make_step_table()
+
+                    pbar.set_postfix_str(s="summary", refresh=True)
+                    if summary_opts is not None:
+                        c.make_summary(**summary_opts)
+                    else:
+                        c.make_summary(find_end_voltage=True, find_ir=True)
+
+                except Exception as e:
+                    e_txt = f"recalculating for {indx} failed!"
+                    errors.append(e_txt)
+                    warnings.warn(e_txt)
+                else:
+                    if save:
+                        # remark! got a win error when trying to save (hdf5-file in use) (must fix this)
+                        pbar.set_postfix_str(s="save", refresh=True)
+                        try:
+                            c.save(row.cellpy_file_name)
+                            log.append(f"saved {indx} to {row.cellpy_file_name}")
+                        except Exception as e:
+                            e_txt = f"saving {indx} to {row.cellpy_file_name} failed!"
+                            errors.append(e_txt)
+                            warnings.warn(e_txt)
+        self.errors["recalc"] = errors
+        self.log["recalc"] = log
+
+
+class ImpedanceExperiment(BaseExperiment):
+    def __init__(self):
+        super().__init__()
+
+
+class LifeTimeExperiment(BaseExperiment):
+    def __init__(self):
+        super().__init__()
+
+
+if __name__ == "__main__":
+    from pathlib import Path
+    import os
+    import pandas as pd
+    import numpy as np
+    import seaborn as sns
+    import plotly.express as px
+
+    import cellpy
+    from cellpy.utils import batch, helpers, plotutils
+
+    project_dir = Path("../../../testdata/batch_project")
+    print(f"{project_dir.resolve()=}")
+    journal = project_dir / "test_project.json"
+    journal = journal.resolve()
+    print(f"{journal=}")
+    assert project_dir.is_dir()
+    assert journal.is_file()
+    os.chdir(project_dir)
+
+    print(f"cellpy version: {cellpy.__version__}")
+    cellpy.log.setup_logging("INFO")
+
+    b = batch.from_journal(journal)
+    b.update()
+
+    print("Ended OK")
```

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.0a9/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/collectors.py` & `cellpy-1.0.0a9/cellpy/utils/collectors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/collectors_old.py` & `cellpy-1.0.0a9/cellpy/utils/collectors_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-1.0.0a9/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-1.0.0a9/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/easyplot.py` & `cellpy-1.0.0a9/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/example_data.py` & `cellpy-1.0.0a9/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/helpers.py` & `cellpy-1.0.0a9/cellpy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/ica.py` & `cellpy-1.0.0a9/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy/utils/processor.py` & `cellpy-1.0.0a9/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.0a9/cellpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,26 +93,32 @@
 History
 =======
 
 
 1.0.0 (2023) [under development]
 ================================
 
+* Unit handling: new unit handling (using pint)
 * Unit handling: renaming summary headers
 * Unit handling: new cellpy-file-format version
 * Unit handling: tool for converting old to new format
+* Unit handling: parsing input parameters for units
 * Templates: using one repository with sub-folders
 * Templates: adding more documentation
 * File handling: allow for external raw files (ssh)
 * Readers: neware.txt (one version/model)
 * Readers: arbin_sql7 (experimental, @jtgibson91)
 * Batch plotting: collectors for both data collection, plotting and saving
+* OCV-rlx: improvements of the OCV-rlx tools
 * Internals: rename main classes (CellpyData -> CellpyCell, Cell -> Data)
 * Internals: rename .cell property to .data
 * Internals: allow for only one Data-object pr CellpyCell object
+* CLI: general improvements and bug fixes
+* CLI: move editing of db-file to the edit sub-command
+
 
 
 0.4.3 (2023)
 ============
 
 * Neware txt loader (supports one specific format only, other formats will have to wait for v.1.0)
```

### Comparing `cellpy-1.0.0a8/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.0a9/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/Makefile` & `cellpy-1.0.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a9/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a9/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png` & `cellpy-1.0.0a9/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-1.0.0a9/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a9/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/adapted_readme.rst` & `cellpy-1.0.0a9/docs/adapted_readme.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/conf.py` & `cellpy-1.0.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_data_structure.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_folder_structure.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_packaging_pypi.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_packaging_pypi.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_cellpy_setup.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_cellpy_setup.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_conda_package.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_conda_package.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_docs.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_docs.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_loaders_and_instruments.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_loaders_and_instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/developers_guide/dev_various.rst` & `cellpy-1.0.0a9/docs/developers_guide/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/05_configuring.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/05_configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/06_pandas.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/06_pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png` & `cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png` & `cellpy-1.0.0a9/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/tips_and_tricks.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/batch.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/ica.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/plotting.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst` & `cellpy-1.0.0a9/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/figures/cellpy-icon-bw.png` & `cellpy-1.0.0a9/docs/figures/cellpy-icon-bw.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/figures/cellpy-logo-v1.png` & `cellpy-1.0.0a9/docs/figures/cellpy-logo-v1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/index.rst` & `cellpy-1.0.0a9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/main_description/formats.rst` & `cellpy-1.0.0a9/docs/main_description/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/main_description/installation.rst` & `cellpy-1.0.0a9/docs/main_description/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/main_description/usage.rst` & `cellpy-1.0.0a9/docs/main_description/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/make.bat` & `cellpy-1.0.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.parameters.rst` & `cellpy-1.0.0a9/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.configurations.rst` & `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.configurations.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.loader_specific_modules.rst` & `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.loader_specific_modules.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.processors.rst` & `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.processors.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.readers.instruments.rst` & `cellpy-1.0.0a9/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.readers.rst` & `cellpy-1.0.0a9/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.rst` & `cellpy-1.0.0a9/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-1.0.0a9/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/docs/source/cellpy.utils.rst` & `cellpy-1.0.0a9/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a8/setup.py` & `cellpy-1.0.0a9/setup.py`

 * *Files identical despite different names*

