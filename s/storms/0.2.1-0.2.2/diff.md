# Comparing `tmp/storms-0.2.1.tar.gz` & `tmp/storms-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storms-0.2.1.tar", last modified: Wed May 24 18:54:08 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `storms-0.2.1.tar` & `storms-0.2.2.tar`

### file list

```diff
@@ -1,133 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.284590 storms-0.2.1/
--rw-rw-rw-   0        0        0    35149 2023-05-11 18:48:55.000000 storms-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      400 2023-05-11 19:30:33.000000 storms-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2364 2023-05-24 18:54:08.284590 storms-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1550 2023-05-12 14:03:47.000000 storms-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.060570 storms-0.2.1/docs/
--rw-rw-rw-   0        0        0      753 2023-05-11 18:38:49.000000 storms-0.2.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.005299 storms-0.2.1/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.004248 storms-0.2.1/docs/_build/doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.069586 storms-0.2.1/docs/_build/doctrees/nbsphinx/
--rw-rw-rw-   0        0        0   348653 2023-04-27 03:43:35.000000 storms-0.2.1/docs/_build/doctrees/nbsphinx/examples_disagg_example_5_0.png
--rw-rw-rw-   0        0        0    27031 2023-04-27 03:43:40.000000 storms-0.2.1/docs/_build/doctrees/nbsphinx/usage_28_0.png
--rw-rw-rw-   0        0        0    39629 2023-04-27 03:43:40.000000 storms-0.2.1/docs/_build/doctrees/nbsphinx/usage_30_0.png
--rw-rw-rw-   0        0        0    47107 2023-04-27 03:43:40.000000 storms-0.2.1/docs/_build/doctrees/nbsphinx/usage_34_0.png
--rw-rw-rw-   0        0        0    21294 2023-04-27 03:43:40.000000 storms-0.2.1/docs/_build/doctrees/nbsphinx/usage_8_1.png
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.007252 storms-0.2.1/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.070584 storms-0.2.1/docs/_build/html/_images/
--rw-rw-rw-   0        0        0   348653 2023-04-27 03:43:35.000000 storms-0.2.1/docs/_build/html/_images/examples_disagg_example_5_0.png
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.076571 storms-0.2.1/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-04-27 01:48:55.000000 storms-0.2.1/docs/_build/html/_static/file.png
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.078592 storms-0.2.1/docs/_build/html/_static/img/
--rw-rw-rw-   0        0        0    42067 2022-09-12 13:31:03.000000 storms-0.2.1/docs/_build/html/_static/img/output_8_1.png
--rw-rw-rw-   0        0        0       90 2023-04-27 01:48:55.000000 storms-0.2.1/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-27 01:48:55.000000 storms-0.2.1/docs/_build/html/_static/plus.png
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.009250 storms-0.2.1/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.080587 storms-0.2.1/docs/_static/img/
--rw-rw-rw-   0        0        0    42067 2022-09-12 13:31:03.000000 storms-0.2.1/docs/_static/img/output_8_1.png
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.011251 storms-0.2.1/docs/_templates/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.083586 storms-0.2.1/docs/_templates/autosummary/
--rw-rw-rw-   0        0        0      108 2022-09-12 13:31:03.000000 storms-0.2.1/docs/_templates/autosummary/base.rst
--rw-rw-rw-   0        0        0      670 2023-04-27 01:51:21.000000 storms-0.2.1/docs/_templates/autosummary/class.rst
--rw-rw-rw-   0        0        0     8128 2023-05-11 18:38:49.000000 storms-0.2.1/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.084589 storms-0.2.1/docs/examples/
--rw-rw-rw-   0        0        0      127 2023-04-27 03:22:49.000000 storms-0.2.1/docs/examples/index.rst
--rw-rw-rw-   0        0        0      206 2023-05-11 18:38:49.000000 storms-0.2.1/docs/index.rst
--rw-rw-rw-   0        0        0     1534 2023-05-11 18:38:49.000000 storms-0.2.1/docs/installation.rst
--rwxrwxrwx   0        0        0      804 2023-05-11 18:38:49.000000 storms-0.2.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.094574 storms-0.2.1/docs/reference/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.139589 storms-0.2.1/docs/reference/api/
--rw-rw-rw-   0        0        0       89 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.IDF.rst
--rw-rw-rw-   0        0        0      116 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.disaggregate.rst
--rw-rw-rw-   0        0        0      100 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.events.rst
--rw-rw-rw-   0        0        0      106 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.find_ari.rst
--rw-rw-rw-   0        0        0      115 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.find_events.rst
--rw-rw-rw-   0        0        0      124 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.find_intervals.rst
--rw-rw-rw-   0        0        0       94 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.freq.rst
--rw-rw-rw-   0        0        0      133 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.from_GlobalHourly.rst
--rw-rw-rw-   0        0        0      109 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.from_asos.rst
--rw-rw-rw-   0        0        0      106 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.from_csv.rst
--rw-rw-rw-   0        0        0      103 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.from_ff.rst
--rw-rw-rw-   0        0        0      109 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.from_swmm.rst
--rw-rw-rw-   0        0        0      109 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.get_event.rst
--rw-rw-rw-   0        0        0      137 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.get_event_by_rank.rst
--rw-rw-rw-   0        0        0      120 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.get_noaa_ari.rst
--rw-rw-rw-   0        0        0      109 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.intervals.rst
--rw-rw-rw-   0        0        0      111 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.num_years.rst
--rw-rw-rw-   0        0        0     1102 2023-04-27 01:59:56.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.rst
--rw-rw-rw-   0        0        0      108 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/api/pydro.Raingage.ts_hours.rst
--rw-rw-rw-   0        0        0      116 2022-09-12 13:31:03.000000 storms-0.2.1/docs/reference/index.rst
--rw-rw-rw-   0        0        0      108 2023-04-27 01:51:21.000000 storms-0.2.1/docs/reference/precip.rst
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.146585 storms-0.2.1/docs/reference/raindata/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.172589 storms-0.2.1/docs/reference/raindata/api/
--rw-rw-rw-   0        0        0      110 2023-04-27 01:59:56.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.ASOS.get_meta.rst
--rw-rw-rw-   0        0        0       93 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.ASOS.map.rst
--rw-rw-rw-   0        0        0      137 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.ASOS.request_dataframe.rst
--rw-rw-rw-   0        0        0      373 2023-04-27 01:59:56.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.ASOS.rst
--rw-rw-rw-   0        0        0      134 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.GlobalHourly.get_meta.rst
--rw-rw-rw-   0        0        0      117 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.GlobalHourly.map.rst
--rw-rw-rw-   0        0        0      161 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.GlobalHourly.request_dataframe.rst
--rw-rw-rw-   0        0        0      471 2023-04-27 01:59:56.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.GlobalHourly.rst
--rw-rw-rw-   0        0        0      132 2023-01-12 20:05:29.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.GlobalHourly.stations.rst
--rw-rw-rw-   0        0        0      143 2023-01-12 20:05:30.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.NEXRAD.request_dataframe.rst
--rw-rw-rw-   0        0        0      341 2023-04-27 01:59:56.000000 storms-0.2.1/docs/reference/raindata/api/pydro.precip.datasets.NEXRAD.rst
--rw-rw-rw-   0        0        0      214 2023-05-11 18:38:49.000000 storms-0.2.1/docs/reference/raindata/asos.rst
--rw-rw-rw-   0        0        0      292 2023-05-11 18:38:49.000000 storms-0.2.1/docs/reference/raindata/globalhourly.rst
--rw-rw-rw-   0        0        0      114 2023-04-27 01:51:21.000000 storms-0.2.1/docs/reference/raindata/index.rst
--rw-rw-rw-   0        0        0      172 2023-05-11 18:38:49.000000 storms-0.2.1/docs/reference/raindata/nexrad.rst
--rw-rw-rw-   0        0        0      961 2023-05-11 18:38:49.000000 storms-0.2.1/docs/reference/raingage.rst
--rw-rw-rw-   0        0        0       56 2022-09-12 13:31:03.000000 storms-0.2.1/docs/reference/streamflow.rst
--rw-rw-rw-   0        0        0       72 2022-09-12 13:31:03.000000 storms-0.2.1/docs/reference/tide.rst
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.175587 storms-0.2.1/docs/reference/tidedata/
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.183586 storms-0.2.1/docs/reference/tidedata/api/
--rw-rw-rw-   0        0        0      106 2023-01-12 20:05:30.000000 storms-0.2.1/docs/reference/tidedata/api/pydro.tide.datasets.NOAAtides.map.rst
--rw-rw-rw-   0        0        0      150 2023-01-12 20:05:30.000000 storms-0.2.1/docs/reference/tidedata/api/pydro.tide.datasets.NOAAtides.request_dataframe.rst
--rw-rw-rw-   0        0        0      401 2023-04-27 01:59:56.000000 storms-0.2.1/docs/reference/tidedata/api/pydro.tide.datasets.NOAAtides.rst
--rw-rw-rw-   0        0        0      121 2023-01-12 20:05:30.000000 storms-0.2.1/docs/reference/tidedata/api/pydro.tide.datasets.NOAAtides.stations.rst
--rw-rw-rw-   0        0        0       80 2022-09-12 13:31:03.000000 storms-0.2.1/docs/reference/tidedata/index.rst
--rw-rw-rw-   0        0        0      272 2023-05-11 18:38:49.000000 storms-0.2.1/docs/reference/tidedata/noaa.rst
--rw-rw-rw-   0        0        0     4413 2022-09-12 13:31:03.000000 storms-0.2.1/docs/storms_logoOnly.png
--rw-rw-rw-   0        0        0    23724 2023-05-11 18:37:10.000000 storms-0.2.1/docs/storms_logo_with_text.png
--rw-rw-rw-   0        0        0      616 2023-05-24 18:54:08.286600 storms-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2140 2023-05-24 18:53:11.000000 storms-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.188589 storms-0.2.1/storms/
--rw-rw-rw-   0        0        0      173 2023-05-24 18:53:17.000000 storms-0.2.1/storms/__init__.py
--rw-rw-rw-   0        0        0     6999 2023-05-11 18:38:48.000000 storms-0.2.1/storms/_datasource.py
--rw-rw-rw-   0        0        0     2265 2023-03-20 19:02:57.000000 storms-0.2.1/storms/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.227570 storms-0.2.1/storms/precip/
--rw-rw-rw-   0        0        0      265 2023-05-11 18:38:48.000000 storms-0.2.1/storms/precip/__init__.py
--rw-rw-rw-   0        0        0     5390 2023-05-11 18:38:48.000000 storms-0.2.1/storms/precip/_dashboard.py
--rw-rw-rw-   0        0        0     8091 2023-04-27 14:40:46.000000 storms-0.2.1/storms/precip/_disagg.py
--rw-rw-rw-   0        0        0    19046 2023-04-27 01:51:21.000000 storms-0.2.1/storms/precip/_rainrank.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.251572 storms-0.2.1/storms/precip/datasets/
--rw-rw-rw-   0        0        0  2667526 2022-09-12 13:31:04.000000 storms-0.2.1/storms/precip/datasets/Logan.1h
--rw-rw-rw-   0        0        0      284 2023-05-11 18:38:49.000000 storms-0.2.1/storms/precip/datasets/__init__.py
--rw-rw-rw-   0        0        0    16707 2023-05-11 18:38:49.000000 storms-0.2.1/storms/precip/datasets/_asos.py
--rw-rw-rw-   0        0        0    20851 2023-05-11 18:38:49.000000 storms-0.2.1/storms/precip/datasets/_globalhourly.py
--rw-rw-rw-   0        0        0    12764 2023-05-11 18:38:49.000000 storms-0.2.1/storms/precip/datasets/_nexrad.py
--rw-rw-rw-   0        0        0     8803 2022-09-12 13:31:04.000000 storms-0.2.1/storms/precip/datasets/_nexradmaps.py
--rw-rw-rw-   0        0        0  2990723 2022-09-12 13:31:04.000000 storms-0.2.1/storms/precip/datasets/isd_history.txt
--rw-rw-rw-   0        0        0    15164 2023-04-27 14:40:46.000000 storms-0.2.1/storms/precip/eva.py
--rw-rw-rw-   0        0        0    44601 2023-04-04 16:18:52.000000 storms-0.2.1/storms/precip/index.html
--rw-rw-rw-   0        0        0     5741 2023-05-11 18:38:48.000000 storms-0.2.1/storms/precip/network.py
--rw-rw-rw-   0        0        0    53734 2023-05-24 18:52:05.000000 storms-0.2.1/storms/precip/raingage.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.256570 storms-0.2.1/storms/tide/
--rw-rw-rw-   0        0        0       41 2023-05-11 18:38:48.000000 storms-0.2.1/storms/tide/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.261591 storms-0.2.1/storms/tide/datasets/
--rw-rw-rw-   0        0        0       50 2023-05-11 18:38:48.000000 storms-0.2.1/storms/tide/datasets/__init__.py
--rw-rw-rw-   0        0        0    12624 2023-05-11 18:38:48.000000 storms-0.2.1/storms/tide/datasets/_noaa.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.200579 storms-0.2.1/storms.egg-info/
--rw-rw-rw-   0        0        0     2364 2023-05-24 18:54:07.000000 storms-0.2.1/storms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3987 2023-05-24 18:54:07.000000 storms-0.2.1/storms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 18:54:07.000000 storms-0.2.1/storms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-11 19:00:08.000000 storms-0.2.1/storms.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2023-05-24 18:54:07.000000 storms-0.2.1/storms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 18:54:07.000000 storms-0.2.1/storms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.265598 storms-0.2.1/tests/
--rw-rw-rw-   0        0        0       37 2023-05-11 18:38:48.000000 storms-0.2.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:54:08.280575 storms-0.2.1/tests/data/
--rw-rw-rw-   0        0        0  1448697 2022-09-12 13:31:04.000000 storms-0.2.1/tests/data/Bradley.1h
--rw-rw-rw-   0        0        0  1843945 2022-09-12 13:31:04.000000 storms-0.2.1/tests/data/BrainardExcept8499.1h
--rw-rw-rw-   0        0        0  2663058 2022-09-12 13:31:04.000000 storms-0.2.1/tests/data/Logan.1h
--rw-rw-rw-   0        0        0  2297186 2022-09-12 13:31:04.000000 storms-0.2.1/tests/data/Logan.csv
--rw-rw-rw-   0        0        0     1147 2023-05-11 18:44:31.000000 storms-0.2.1/tests/test_raingage.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 storms-0.2.2/storms/__init__.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 storms-0.2.2/storms/_datasource.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 storms-0.2.2/storms/_utils.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/__init__.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/_dashboard.py
+-rw-r--r--   0        0        0     8091 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/_disagg.py
+-rw-r--r--   0        0        0    19046 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/_rainrank.py
+-rw-r--r--   0        0        0    15249 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/eva.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/hdsc-nws-noaa-gov-chain.pem
+-rw-r--r--   0        0        0    44601 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/index.html
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/network.py
+-rw-r--r--   0        0        0    54068 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/raingage.py
+-rw-r--r--   0        0        0  2667526 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/Logan.1h
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/__init__.py
+-rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/_asos.py
+-rw-r--r--   0        0        0    20865 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/_globalhourly.py
+-rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/_nexrad.py
+-rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/_nexradmaps.py
+-rw-r--r--   0        0        0  2990723 2020-02-02 00:00:00.000000 storms-0.2.2/storms/precip/datasets/isd_history.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 storms-0.2.2/storms/tide/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 storms-0.2.2/storms/tide/datasets/__init__.py
+-rw-r--r--   0        0        0    12624 2020-02-02 00:00:00.000000 storms-0.2.2/storms/tide/datasets/_noaa.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 storms-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 storms-0.2.2/tests/test_raingage.py
+-rw-r--r--   0        0        0  1448697 2020-02-02 00:00:00.000000 storms-0.2.2/tests/data/Bradley.1h
+-rw-r--r--   0        0        0  1843945 2020-02-02 00:00:00.000000 storms-0.2.2/tests/data/BrainardExcept8499.1h
+-rw-r--r--   0        0        0  2663058 2020-02-02 00:00:00.000000 storms-0.2.2/tests/data/Logan.1h
+-rw-r--r--   0        0        0  2297186 2020-02-02 00:00:00.000000 storms-0.2.2/tests/data/Logan.csv
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 storms-0.2.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 storms-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 storms-0.2.2/README.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 storms-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 storms-0.2.2/PKG-INFO
```

### Comparing `storms-0.2.1/LICENSE` & `storms-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/README.md` & `storms-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <img src="https://raw.githubusercontent.com/karosc/storms/main/docs/storms_logo_with_text.png" width=100%></img>
 
 
 # storms: a simple and effective storm event analysis toolkit
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOCS:Pages](https://github.com/karosc/storms/actions/workflows/documentation.yaml/badge.svg)](https://www.karosc.com/storms/)
 [![Latest PyPI version](https://img.shields.io/pypi/v/storms.svg)](https://pypi.python.org/pypi/storms/)
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 <!-- [![PyPI Monthly Downloads](https://img.shields.io/badge/dynamic/json.svg?label=Downloads&url=https%3A%2F%2Fpypistats.org%2Fapi%2Fpackages%2Fstorms%2Frecent&query=%24.data.last_month&colorB=green&suffix=%20last%20month)](https://pypi.python.org/pypi/storms/)
  -->
 
 ## Features
 
 - Download hourly rainfall timeseries from [NOAA ISD](https://www.ncei.noaa.gov/products/land-based-station/integrated-surface-database) 
 - Bin rainfall data timeseries into descrete events
```

### Comparing `storms-0.2.1/storms/_datasource.py` & `storms-0.2.2/storms/_datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,23 @@
         self,
         start: datetime_like,
         end: datetime_like,
         datatype: Union[str, Sequence[str]],
     ) -> Any:
         return NotImplementedError
 
+    def _sync_request_dataframe(
+        self,
+        start: datetime_like,
+        end: datetime_like,
+        process_data: bool,
+        pull_freq: str,
+    ) -> pd.DataFrame:
+        raise NotImplementedError
+
     def _sync_request_data_series(
         self, start: datetime_like, end: datetime_like, pull_freq: str = "AS", **kwargs
     ) -> pd.DataFrame:
         # convert string inputs to datetime-like
         dStart = pd.to_datetime(start)
         dEnd = pd.to_datetime(end)
 
@@ -130,14 +139,24 @@
         return data
 
     def _sync_request_data(
         self, start: datetime_like, end: datetime_like, session: Session
     ) -> Union[ndarray, str, List[dict]]:
         raise NotImplementedError
 
+    async def _async_request_dataframe(
+        self,
+        start: datetime_like,
+        end: datetime_like,
+        process_data: bool,
+        pull_freq: str,
+        conn_limit: int,
+    ) -> pd.DataFrame:
+        raise NotImplementedError
+
     async def _async_request_data_series(
         self,
         start: datetime_like,
         end: datetime_like,
         pull_freq: str = "AS",
         conn_limit: int = 30,
         **kwargs,
```

### Comparing `storms-0.2.1/storms/_utils.py` & `storms-0.2.2/storms/_utils.py`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/_dashboard.py` & `storms-0.2.2/storms/precip/_dashboard.py`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/_disagg.py` & `storms-0.2.2/storms/precip/_disagg.py`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/_rainrank.py` & `storms-0.2.2/storms/precip/_rainrank.py`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/datasets/Logan.1h` & `storms-0.2.2/storms/precip/datasets/Logan.1h`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/datasets/_asos.py` & `storms-0.2.2/storms/precip/datasets/_asos.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,16 +337,16 @@
             return "\n".join(response.text.split("\n")[1:])
 
     async def _async_request_dataframe(
         self,
         start: datetime_like,
         end: datetime_like,
         process_data: bool = True,
-        pull_freq="AS",
-        conn_limit=5,
+        pull_freq: str = "AS",
+        conn_limit: int = 5,
     ) -> pd.DataFrame:
         """
         Request precipitation DataFrame with asynchronous annual requests to Iowa Mesonet
 
         This is an async function and must be awaited as::
 
             df = await gage._async_request_dataframe(start = '1/1/2020', end = '1/1/2021')
```

### Comparing `storms-0.2.1/storms/precip/datasets/_globalhourly.py` & `storms-0.2.2/storms/precip/datasets/_globalhourly.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,16 +458,16 @@
 
     # async functions
     async def _async_request_dataframe(
         self,
         start: datetime_like,
         end: datetime_like,
         process_data: bool = True,
-        pull_freq="AS",
-        conn_limit=30,
+        pull_freq: str = "AS",
+        conn_limit: int = 30,
     ) -> pd.DataFrame:
         """
         Request precipitation DataFrame with asynchronous annual requests to NOAA V1 API.
         https://www.ncei.noaa.gov/support/access-data-service-api-user-documentation
 
         This is an async function and must be awaited as::
```

### Comparing `storms-0.2.1/storms/precip/datasets/_nexrad.py` & `storms-0.2.2/storms/precip/datasets/_nexrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,16 +263,16 @@
 
     # async functions
     async def _async_request_dataframe(
         self,
         start: datetime_like,
         end: datetime_like,
         process_data: bool = True,
-        pull_freq="5T",
-        conn_limit=30,
+        pull_freq: str = "5T",
+        conn_limit: int = 30,
     ) -> Union[pd.DataFrame, np.ndarray]:
         """
         Request nexrad data DataFrame with asynchronous requests to Iowa Mesonet.
 
 
         Request precipitation DataFrame with asynchronous annual requests to Iowa Mesonet
 
@@ -363,15 +363,16 @@
                 # print(
                 #     "Oops, the connection was dropped before we finished, retrying..."
                 # )
                 error_counter += 1
                 continue
             except:
                 raise Exception(f"error pulling {url}, retrying...")
-        print(f"Couldn't get data from {start}")
+
+        raise Exception(f"error pulling {url} after 5 retries")
 
     def _process_data(self, data: np.ndarray, index: np.ndarray) -> np.ndarray:
         """Process raw nexrad rgb values into reflectivity values using NOAA color maps
         and average values for the entire image.
 
         Parameters
         ----------
```

### Comparing `storms-0.2.1/storms/precip/datasets/_nexradmaps.py` & `storms-0.2.2/storms/precip/datasets/_nexradmaps.py`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/datasets/isd_history.txt` & `storms-0.2.2/storms/precip/datasets/isd_history.txt`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/eva.py` & `storms-0.2.2/storms/precip/eva.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,15 +340,19 @@
         -------
         Union[float, np.ndarray]
             Probability density function evaluated at `x`
         """
         return self.model.cdf(x, **self.paras)
 
 
-def plotting_position(M: int, nyrs: int, A: float = 0.4) -> float:
+def plotting_position(
+    M: Union[int, np.int64],
+    nyrs: Union[int, np.int64],
+    A: Union[float, np.float64] = 0.4,
+) -> float | np.float64:
     """
     Empirical  return  period  (plotting  position)  is  calculated  by  the  general  equation
     first proposed by Gringorten (1963) and analyzed by Cunnane (1978). From `SWMM4 Manual`_ pg 299.
 
     .. _SWMM4 Manual: http://www.dynsystem.com/netstorm/docs/swmm4manuals.pdf
 
     Parameters
```

### Comparing `storms-0.2.1/storms/precip/index.html` & `storms-0.2.2/storms/precip/index.html`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/storms/precip/network.py` & `storms-0.2.2/storms/precip/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
         self.gages: Dict[str, Raingage] = {}
         data: List[pd.Series] = []
         for i, gage in enumerate(args):
             if i == 0:
                 self._freq = gage.freq
             self.validate_gage(gage)
             data.append(gage.data)
+            if gage.ID is None:
+                raise Exception("All gages in a network must have an ID set")
             self.gages[gage.ID] = gage
 
         self.gage_names = list(self.gages.keys())
 
         self.qaqc = kwargs.get("qaqc")
         if self.qaqc:
             self.validate_gage(self.qaqc)
@@ -31,15 +33,15 @@
             )
 
         self.data = pd.concat(data, axis=1).fillna(0)
         self.data.columns = self.gage_names
         self.precip = self.data.to_numpy()
         self.datetime = self.data.index.to_numpy()
 
-    def validate_gage(self, gage: Raingage) -> NoReturn:
+    def validate_gage(self, gage: Raingage) -> None:
         if not isinstance(gage, Raingage):
             raise Exception("All network objects must be Raingages")
         if gage.ID is None:
             raise Exception("All Raingages must have an ID property")
         if gage.freq != self._freq:
             raise Exception("All gages in the network must have the same frequency.")
 
@@ -75,15 +77,15 @@
         :return: time series time step (hours)
         :rtype: float
         """
         return self.freq.nanos / 1e9 / 60 / 60
 
     def find_events(
         self, inter_event_period: float = 6, threshold_depth: float = 0.25
-    ) -> NoReturn:
+    ) -> None:
         self._events, self._event_col = eventify(
             self.precip,
             self.datetime,
             inter_event_period,
             threshold_depth,
             self.ts_hours,
         )
```

### Comparing `storms-0.2.1/storms/precip/raingage.py` & `storms-0.2.2/storms/precip/raingage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from os import cpu_count
 from typing import Optional, Sequence, Union, Tuple, Dict
 from warnings import warn
 from types import MethodType
 from io import StringIO
+import pathlib
 
 import numpy as np
 import pandas as pd
 import requests
 
 from numba import set_num_threads
 from numpy.typing import ArrayLike
@@ -20,14 +21,17 @@
 from storms.precip.eva import EVA
 from storms.precip.datasets import GlobalHourly, ASOS, NEXRAD
 from storms.precip._disagg import continuous_deterministic, continuous_stochastic
 from storms._utils import datetime_like
 from storms.precip._dashboard import rg_2_dash
 from tqdm.auto import tqdm
 
+__HERE__ = pathlib.Path(__file__).parent
+_noaa_ca_cert_path = str((__HERE__ / "hdsc-nws-noaa-gov-chain.pem").absolute())
+
 
 def dbz_to_depth(
     dbz: np.ndarray, a: float = 200, b: float = 1.6, interval: float = 300, **kwargs
 ) -> np.ndarray:
     """
     Convert radar reflectivity to depth in inches using the Marshall-Palmer Equation
 
@@ -59,15 +63,15 @@
     return (R * interval / 3600.0) / 25.4
 
 
 class Raingage(object):
     def __init__(
         self,
         data: pd.Series,
-        freq: str = None,
+        freq: Optional[str] = None,
         latlon: Optional[Tuple[float, float]] = None,
         meta: Optional[dict] = {},
         ID: Optional[str] = None,
     ):
         """Raingage class for developing IDF stats and storm time histories
 
         Parameters
@@ -122,15 +126,16 @@
 
         self._evds: Dict[str, EVA] = {}
 
         self.intervals: pd.DataFrame
         """DataFrame of sub-events found with the find_intervals method."""
 
         self._dbz_data: Dict[
-            Tuple[pd.TimeStamp, pd.TimeStamp, Union[float, int]], pd.Series
+            Tuple[pd.TimeStamp, pd.TimeStamp, float, Union[str, pd.DateOffset]],
+            pd.Series,
         ] = {}
 
     @classmethod
     def from_asos(cls, ID: str, start: datetime_like, end: datetime_like, aSync=False):
         """Create raingage object with data from NOAA's ASOS dataset.
 
         Data are collected with asynchronous annual requests to the `Iowa Mesonet API`_.
@@ -663,31 +668,31 @@
             return Raingage(series, out_freq, self.latlon, self.meta, self.ID)
 
     def _continuous_stoch(
         self,
         out_freq: pd.DateOffset,
         num_bins: int,
         inplace: bool,
-        precision: float = 2,
+        precision: int = 2,
         scale_factor: float = 0,
         **kwargs,
     ):
         """Continous stochastic disaggregation using geometric similarity to disaggregate
         data to new interval given by out_freq.
 
         Parameters
         ----------
         out_freq: pd.DateOffset
             Pandas offset string giving new output frequency.
         num_bins: int
             Number of bins to split data into every time step.
         inplace: bool
             Switch to return new Raingage object or alter current, by default True.
-        precision: float
-            The precision of output rainfall timeseries, by default 2 for hundreths of an inche.
+        precision: int
+            The precision of output rainfall timeseries, by default 2 for hundreths of an inch.
         scale_factor: float
             Spiking factor used to randomly add higher peaks to output timeseries, by default 0.
 
         Returns
         -------
         Raingage object with new freq or None if inplace=True.
         """
@@ -1239,22 +1244,21 @@
                 evt.start_date
                 + pd.to_timedelta(evt.hours_duration - self.ts_hours, "H")
             ).round("T")
         else:
             start = pd.to_datetime(start)
             end = pd.to_datetime(end)
 
-        key = (start, end, averaging_distance, freq)
+        pull_freq = freq if freq is not None else self.freq
+        key = (start, end, averaging_distance, pull_freq)
 
         if self._dbz_data.get(key) is None:
             if nex is None:
                 nex = NEXRAD(*self.latlon, averaging_distance)  # type: ignore
 
-            pull_freq = freq if freq is not None else self.freq
-
             data = nex.request_dataframe(
                 start, end, aSync=True, pull_freq=pull_freq, progress=progress
             )
             self._dbz_data[key] = data
 
         return self._dbz_data.get(key)
 
@@ -1479,40 +1483,48 @@
         dump_json: bool = True,
     ) -> None:
         rg_2_dash(
             file_path=file_path, rg=self, idf_periods=idf_periods, dump_json=dump_json
         )
 
 
-def get_pfds(lat: float, lon: float, **kwargs) -> pd.DataFrame:
+def get_pfds(
+    lat: float, lon: float, verify=_noaa_ca_cert_path, **kwargs
+) -> pd.DataFrame:
     """Pull atlas 14 PFDS and return table as DataFrame
 
     Parameters
     ----------
     lat: float
         Latitude of station in decimal degrees
     lon: float
         Longitude of station in decimal degrees
+    verify:
+        verify argument to feed into requests.get
     **kwargs
         Additional kwargs to be fed into requests.get
 
     Returns
     -------
     pd.DataFrame
         DataFrame of rainfall depths at various durations and ARIs
 
     """
     # base url of noaa pfds
     try:
         url = f"https://hdsc.nws.noaa.gov/cgi-bin/hdsc/new/fe_text_mean.csv?lat={lat}&lon={lon}&data=depth&units=english&series=pds&"
-        response = requests.get(url,**kwargs)
-        
+        response = requests.get(url, verify=verify, **kwargs)
+
         # NOAA PFDS uses ASCII encoding rather than UTF
         df = pd.read_csv(
-            StringIO(response.content.decode()), engine="python", encoding="cp1252", skiprows=13, skipfooter=2
+            StringIO(response.content.decode()),
+            engine="python",
+            encoding="cp1252",
+            skiprows=13,
+            skipfooter=2,
         )
 
         # convert string duration index to hours
         df.index = (
             pd.to_timedelta(
                 df.iloc[:, 0].str.replace("-", "").str.replace(":", "")
             ).dt.total_seconds()
```

### Comparing `storms-0.2.1/storms/tide/datasets/_noaa.py` & `storms-0.2.2/storms/tide/datasets/_noaa.py`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/tests/data/Bradley.1h` & `storms-0.2.2/tests/data/Bradley.1h`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/tests/data/BrainardExcept8499.1h` & `storms-0.2.2/tests/data/BrainardExcept8499.1h`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/tests/data/Logan.1h` & `storms-0.2.2/tests/data/Logan.1h`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/tests/data/Logan.csv` & `storms-0.2.2/tests/data/Logan.csv`

 * *Files identical despite different names*

### Comparing `storms-0.2.1/tests/test_raingage.py` & `storms-0.2.2/tests/test_raingage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,8 @@
     ]
     assert (
         BostonRaingage.events.set_index("event_num")
         .sort_values("event_total")
         .iloc[-1]
         .to_list()
         == largest24hrEvent
-    )
+    )
```

