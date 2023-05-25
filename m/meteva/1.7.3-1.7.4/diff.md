# Comparing `tmp/meteva-1.7.3.tar.gz` & `tmp/meteva-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\meteva-1.7.3.tar", last modified: Fri Nov 25 08:58:46 2022, max compression
+gzip compressed data, was "dist\meteva-1.7.4.tar", last modified: Wed Mar 22 11:47:59 2023, max compression
```

## Comparing `meteva-1.7.3.tar` & `meteva-1.7.4.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:46.000000 meteva-1.7.3/
--rw-rw-rw-   0        0        0      513 2022-11-25 08:58:46.000000 meteva-1.7.3/PKG-INFO
--rw-rw-rw-   0        0        0      109 2022-10-23 13:40:12.000000 meteva-1.7.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva/
--rw-rw-rw-   0        0        0      254 2022-11-25 08:58:27.000000 meteva-1.7.3/meteva/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva/base/
--rw-rw-rw-   0        0        0      174 2020-03-12 03:56:51.000000 meteva-1.7.3/meteva/base/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva/base/basicdata/
--rw-rw-rw-   0        0        0      143 2021-04-20 14:24:26.000000 meteva-1.7.3/meteva/base/basicdata/__init__.py
--rw-rw-rw-   0        0        0     1151 2022-07-18 07:42:19.000000 meteva-1.7.3/meteva/base/basicdata/const.py
--rw-rw-rw-   0        0        0     7330 2022-06-10 14:01:03.000000 meteva-1.7.3/meteva/base/basicdata/ctl.py
--rw-rw-rw-   0        0        0    19196 2021-11-06 13:46:18.000000 meteva-1.7.3/meteva/base/basicdata/dicts.py
--rw-rw-rw-   0        0        0    11020 2022-07-08 11:04:01.000000 meteva-1.7.3/meteva/base/basicdata/grid.py
--rw-rw-rw-   0        0        0    31390 2022-03-02 03:34:57.000000 meteva-1.7.3/meteva/base/basicdata/grid_data.py
--rw-rw-rw-   0        0        0      669 2020-03-20 01:16:06.000000 meteva-1.7.3/meteva/base/basicdata/keys.py
--rw-rw-rw-   0        0        0     7163 2022-09-17 14:18:55.000000 meteva-1.7.3/meteva/base/basicdata/sta_data.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva/base/fun/
--rw-rw-rw-   0        0        0      532 2022-05-08 03:56:06.000000 meteva-1.7.3/meteva/base/fun/__init__.py
--rw-rw-rw-   0        0        0    29698 2022-08-14 02:45:14.000000 meteva-1.7.3/meteva/base/fun/combining.py
--rw-rw-rw-   0        0        0    27984 2022-08-24 03:18:31.000000 meteva-1.7.3/meteva/base/fun/computing.py
--rw-rw-rw-   0        0        0    18474 2022-09-27 06:32:06.000000 meteva-1.7.3/meteva/base/fun/diagnosing.py
--rw-rw-rw-   0        0        0    29962 2022-08-13 12:24:01.000000 meteva-1.7.3/meteva/base/fun/grouping.py
--rw-rw-rw-   0        0        0    30978 2022-10-28 07:38:54.000000 meteva-1.7.3/meteva/base/fun/interpolating.py
--rw-rw-rw-   0        0        0    13572 2022-07-10 12:09:39.000000 meteva-1.7.3/meteva/base/fun/nearing.py
--rw-rw-rw-   0        0        0    46996 2022-07-17 12:33:00.000000 meteva-1.7.3/meteva/base/fun/selecting.py
--rw-rw-rw-   0        0        0    31088 2022-06-23 03:13:55.000000 meteva-1.7.3/meteva/base/fun/statisticing.py
--rw-rw-rw-   0        0        0    10676 2022-08-09 06:51:25.000000 meteva-1.7.3/meteva/base/fun/timing.py
--rw-rw-rw-   0        0        0     6241 2022-08-13 01:19:17.000000 meteva-1.7.3/meteva/base/fun/transformating.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva/base/io/
--rw-rw-rw-   0        0        0    21279 2022-10-27 01:46:57.000000 meteva-1.7.3/meteva/base/io/CMADaasAccess.py
--rw-rw-rw-   0        0        0    13513 2020-03-04 02:07:45.000000 meteva-1.7.3/meteva/base/io/DataBlock_pb2.py
--rw-rw-rw-   0        0        0     1085 2020-03-04 02:07:45.000000 meteva-1.7.3/meteva/base/io/GDS_data_service.py
--rw-rw-rw-   0        0        0     1288 2020-11-12 11:24:12.000000 meteva-1.7.3/meteva/base/io/SignGenUtil.py
--rw-rw-rw-   0        0        0      471 2022-08-08 08:44:26.000000 meteva-1.7.3/meteva/base/io/__init__.py
--rw-rw-rw-   0        0        0     2987 2020-09-15 02:05:05.000000 meteva-1.7.3/meteva/base/io/clienthandler.py
--rw-rw-rw-   0        0        0     1649 2020-07-06 02:31:29.000000 meteva-1.7.3/meteva/base/io/encoding.py
--rw-rw-rw-   0        0        0    16712 2021-02-15 14:14:53.000000 meteva-1.7.3/meteva/base/io/ftpconn.py
--rw-rw-rw-   0        0        0     1749 2021-04-29 03:15:02.000000 meteva-1.7.3/meteva/base/io/httpclient.py
--rw-rw-rw-   0        0        0     7967 2021-02-15 14:14:53.000000 meteva-1.7.3/meteva/base/io/httpconn.py
--rw-rw-rw-   0        0        0     4709 2021-02-15 14:14:53.000000 meteva-1.7.3/meteva/base/io/loglib.py
--rw-rw-rw-   0        0        0     6048 2022-08-12 07:45:29.000000 meteva-1.7.3/meteva/base/io/print_grib_info.py
--rw-rw-rw-   0        0        0    20392 2021-06-02 08:38:42.000000 meteva-1.7.3/meteva/base/io/read_graphydata.py
--rw-rw-rw-   0        0        0    83269 2022-10-09 03:44:56.000000 meteva-1.7.3/meteva/base/io/read_griddata.py
--rw-rw-rw-   0        0        0    89024 2022-09-26 06:48:16.000000 meteva-1.7.3/meteva/base/io/read_stadata.py
--rw-rw-rw-   0        0        0     4340 2021-10-04 12:35:27.000000 meteva-1.7.3/meteva/base/io/write_array.py
--rw-rw-rw-   0        0        0    10035 2022-10-09 06:20:34.000000 meteva-1.7.3/meteva/base/io/write_griddata.py
--rw-rw-rw-   0        0        0    10076 2021-05-07 14:09:50.000000 meteva-1.7.3/meteva/base/io/write_stadata.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/base/tool/
--rw-rw-rw-   0        0        0     1200 2022-10-28 14:46:41.000000 meteva-1.7.3/meteva/base/tool/__init__.py
--rw-rw-rw-   0        0        0    42601 2022-10-27 14:56:03.000000 meteva-1.7.3/meteva/base/tool/color_tools.py
--rw-rw-rw-   0        0        0    13819 2022-02-26 00:32:32.000000 meteva-1.7.3/meteva/base/tool/copy_tools.py
--rw-rw-rw-   0        0        0     1227 2022-01-26 03:14:18.000000 meteva-1.7.3/meteva/base/tool/frprmn2.py
--rw-rw-rw-   0        0        0     4695 2022-02-26 00:32:32.000000 meteva-1.7.3/meteva/base/tool/grib_tools.py
--rw-rw-rw-   0        0        0     8797 2022-05-30 02:19:44.000000 meteva-1.7.3/meteva/base/tool/maskout.py
--rw-rw-rw-   0        0        0    11223 2022-11-09 03:04:49.000000 meteva-1.7.3/meteva/base/tool/math_tools.py
--rw-rw-rw-   0        0        0    12484 2022-05-09 13:56:16.000000 meteva-1.7.3/meteva/base/tool/path_tools.py
--rw-rw-rw-   0        0        0   173722 2022-11-01 07:20:25.000000 meteva-1.7.3/meteva/base/tool/plot_tools.py
--rw-rw-rw-   0        0        0    32624 2022-11-13 03:35:24.000000 meteva-1.7.3/meteva/base/tool/plot_tools_adv.py
--rw-rw-rw-   0        0        0     4851 2022-02-27 12:00:59.000000 meteva-1.7.3/meteva/base/tool/process_tools.py
--rw-rw-rw-   0        0        0     3647 2020-09-18 14:05:02.000000 meteva-1.7.3/meteva/base/tool/station_tools.py
--rw-rw-rw-   0        0        0     5637 2021-09-29 03:54:03.000000 meteva-1.7.3/meteva/base/tool/time_tools.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/Vector/
--rw-rw-rw-   0        0        0      588 2022-08-19 06:02:40.000000 meteva-1.7.3/meteva/method/Vector/__init__.py
--rw-rw-rw-   0        0        0    19121 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/Vector/plot.py
--rw-rw-rw-   0        0        0    46040 2022-08-19 06:02:13.000000 meteva-1.7.3/meteva/method/Vector/score.py
--rw-rw-rw-   0        0        0      385 2022-07-18 08:30:17.000000 meteva-1.7.3/meteva/method/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/continuous/
--rw-rw-rw-   0        0        0      928 2022-09-27 08:48:55.000000 meteva-1.7.3/meteva/method/continuous/__init__.py
--rw-rw-rw-   0        0        0    37480 2022-04-21 03:32:28.000000 meteva-1.7.3/meteva/method/continuous/plot.py
--rw-rw-rw-   0        0        0    41277 2022-10-06 08:41:29.000000 meteva-1.7.3/meteva/method/continuous/score.py
--rw-rw-rw-   0        0        0     1272 2022-08-11 06:12:59.000000 meteva-1.7.3/meteva/method/continuous/skill.py
--rw-rw-rw-   0        0        0     5086 2022-05-19 09:07:12.000000 meteva-1.7.3/meteva/method/continuous/table.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/ensemble/
--rw-rw-rw-   0        0        0      211 2021-08-16 08:04:20.000000 meteva-1.7.3/meteva/method/ensemble/__init__.py
--rw-rw-rw-   0        0        0     4412 2022-02-26 23:44:42.000000 meteva-1.7.3/meteva/method/ensemble/plot.py
--rw-rw-rw-   0        0        0     4630 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/ensemble/score.py
--rw-rw-rw-   0        0        0        0 2020-03-04 02:07:36.000000 meteva-1.7.3/meteva/method/ensemble/table.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/multi_category/
--rw-rw-rw-   0        0        0      543 2021-06-02 08:05:58.000000 meteva-1.7.3/meteva/method/multi_category/__init__.py
--rw-rw-rw-   0        0        0    15473 2022-11-14 03:23:59.000000 meteva-1.7.3/meteva/method/multi_category/plot.py
--rw-rw-rw-   0        0        0    21927 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/multi_category/score.py
--rw-rw-rw-   0        0        0     7803 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/multi_category/table.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/probability/
--rw-rw-rw-   0        0        0      308 2022-03-02 14:27:29.000000 meteva-1.7.3/meteva/method/probability/__init__.py
--rw-rw-rw-   0        0        0    21703 2022-10-23 06:25:47.000000 meteva-1.7.3/meteva/method/probability/plot.py
--rw-rw-rw-   0        0        0     7341 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/probability/score.py
--rw-rw-rw-   0        0        0     2628 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/probability/table.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/
--rw-rw-rw-   0        0        0      310 2022-11-23 02:18:40.000000 meteva-1.7.3/meteva/method/space/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/fss/
--rw-rw-rw-   0        0        0     1725 2021-11-23 02:49:29.000000 meteva-1.7.3/meteva/method/space/fss/__init__.py
--rw-rw-rw-   0        0        0     8025 2022-06-15 13:39:04.000000 meteva-1.7.3/meteva/method/space/fss/fss.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/mode/
--rw-rw-rw-   0        0        0     1955 2022-06-14 12:27:50.000000 meteva-1.7.3/meteva/method/space/mode/__init__.py
--rw-rw-rw-   0        0        0      161 2021-02-04 10:20:28.000000 meteva-1.7.3/meteva/method/space/mode/angles_psp.py
--rw-rw-rw-   0        0        0      384 2021-02-04 10:20:28.000000 meteva-1.7.3/meteva/method/space/mode/as_psp.py
--rw-rw-rw-   0        0        0      910 2021-03-10 13:04:02.000000 meteva-1.7.3/meteva/method/space/mode/bearing.py
--rw-rw-rw-   0        0        0     4059 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/censqdelta.py
--rw-rw-rw-   0        0        0    11638 2022-05-30 12:33:28.000000 meteva-1.7.3/meteva/method/space/mode/centmatch.py
--rw-rw-rw-   0        0        0     9067 2022-11-12 03:01:53.000000 meteva-1.7.3/meteva/method/space/mode/consistent.py
--rw-rw-rw-   0        0        0     3537 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/data_pre.py
--rw-rw-rw-   0        0        0     1497 2022-02-25 08:34:50.000000 meteva-1.7.3/meteva/method/space/mode/deltametric.py
--rw-rw-rw-   0        0        0     3541 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/deltamm.py
--rw-rw-rw-   0        0        0    18089 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/deltammSqCen.py
--rw-rw-rw-   0        0        0     3530 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/deltamm_bak.py
--rw-rw-rw-   0        0        0     4801 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/distmap.py
--rw-rw-rw-   0        0        0     6072 2022-06-10 07:13:19.000000 meteva-1.7.3/meteva/method/space/mode/feature_axis.py
--rw-rw-rw-   0        0        0     4087 2022-06-24 14:09:57.000000 meteva-1.7.3/meteva/method/space/mode/feature_comps.py
--rw-rw-rw-   0        0        0    31716 2022-07-19 07:56:52.000000 meteva-1.7.3/meteva/method/space/mode/feature_finder.py
--rw-rw-rw-   0        0        0    10095 2022-06-22 08:33:01.000000 meteva-1.7.3/meteva/method/space/mode/feature_match_analyzer.py
--rw-rw-rw-   0        0        0     2456 2022-06-10 12:47:16.000000 meteva-1.7.3/meteva/method/space/mode/feature_props.py
--rw-rw-rw-   0        0        0     5142 2022-06-11 09:04:30.000000 meteva-1.7.3/meteva/method/space/mode/feature_table.py
--rw-rw-rw-   0        0        0    10478 2022-06-30 15:07:24.000000 meteva-1.7.3/meteva/method/space/mode/interester.py
--rw-rw-rw-   0        0        0      748 2022-02-24 23:16:53.000000 meteva-1.7.3/meteva/method/space/mode/intersect.py
--rw-rw-rw-   0        0        0      201 2021-02-04 10:20:28.000000 meteva-1.7.3/meteva/method/space/mode/lengths_psp.py
--rw-rw-rw-   0        0        0     1225 2022-06-14 13:03:13.000000 meteva-1.7.3/meteva/method/space/mode/load.py
--rw-rw-rw-   0        0        0     1365 2021-02-04 10:20:28.000000 meteva-1.7.3/meteva/method/space/mode/loc_list_setup.py
--rw-rw-rw-   0        0        0     3987 2022-02-25 08:35:16.000000 meteva-1.7.3/meteva/method/space/mode/locperf.py
--rw-rw-rw-   0        0        0     7803 2022-02-25 06:16:09.000000 meteva-1.7.3/meteva/method/space/mode/make_SpatialVx_bak.py
--rw-rw-rw-   0        0        0     7943 2022-02-24 23:16:53.000000 meteva-1.7.3/meteva/method/space/mode/make_spatialVx.py
--rw-rw-rw-   0        0        0    11321 2022-06-30 15:12:30.000000 meteva-1.7.3/meteva/method/space/mode/merge_force.py
--rw-rw-rw-   0        0        0      203 2022-02-24 23:16:53.000000 meteva-1.7.3/meteva/method/space/mode/midpoints_psp.py
--rw-rw-rw-   0        0        0    18185 2022-02-24 23:16:53.000000 meteva-1.7.3/meteva/method/space/mode/minboundmatch.py
--rw-rw-rw-   0        0        0     5729 2022-07-19 07:58:01.000000 meteva-1.7.3/meteva/method/space/mode/operater.py
--rw-rw-rw-   0        0        0    32002 2022-11-18 15:03:34.000000 meteva-1.7.3/meteva/method/space/mode/plot.py
--rw-rw-rw-   0        0        0     7757 2022-02-27 12:41:23.000000 meteva-1.7.3/meteva/method/space/mode/regress2.py
--rw-rw-rw-   0        0        0     2226 2022-06-10 07:15:34.000000 meteva-1.7.3/meteva/method/space/mode/sma.py
--rw-rw-rw-   0        0        0     9347 2022-11-13 01:17:32.000000 meteva-1.7.3/meteva/method/space/mode/tran_to_dataframe.py
--rw-rw-rw-   0        0        0      519 2021-02-04 10:20:28.000000 meteva-1.7.3/meteva/method/space/mode/utils.py
--rw-rw-rw-   0        0        0     4489 2020-08-22 13:00:57.000000 meteva-1.7.3/meteva/method/space/point_to_area.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/rigider/
--rw-rw-rw-   0        0        0      394 2021-11-01 03:34:12.000000 meteva-1.7.3/meteva/method/space/rigider/__init__.py
--rw-rw-rw-   0        0        0    10874 2021-11-02 02:23:51.000000 meteva-1.7.3/meteva/method/space/rigider/fint2d.py
--rw-rw-rw-   0        0        0     8093 2021-10-29 08:05:10.000000 meteva-1.7.3/meteva/method/space/rigider/fint2d_old.py
--rw-rw-rw-   0        0        0     1114 2021-10-28 01:37:41.000000 meteva-1.7.3/meteva/method/space/rigider/imomenter.py
--rw-rw-rw-   0        0        0      431 2021-10-24 18:01:18.000000 meteva-1.7.3/meteva/method/space/rigider/mij.py
--rw-rw-rw-   0        0        0      191 2021-10-24 18:01:18.000000 meteva-1.7.3/meteva/method/space/rigider/q_loss_rigid.py
--rw-rw-rw-   0        0        0      465 2021-11-01 13:32:37.000000 meteva-1.7.3/meteva/method/space/rigider/rigid_transform.py
--rw-rw-rw-   0        0        0    13373 2021-11-02 02:16:32.000000 meteva-1.7.3/meteva/method/space/rigider/rigider.py
--rw-rw-rw-   0        0        0      275 2021-10-24 18:01:18.000000 meteva-1.7.3/meteva/method/space/rigider/zapsmall.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/saller/
--rw-rw-rw-   0        0        0      329 2021-04-17 00:33:40.000000 meteva-1.7.3/meteva/method/space/saller/__init__.py
--rw-rw-rw-   0        0        0     5904 2022-07-27 01:17:46.000000 meteva-1.7.3/meteva/method/space/saller/saller.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/significance/
--rw-rw-rw-   0        0        0     4074 2022-11-08 08:43:59.000000 meteva-1.7.3/meteva/method/space/significance/LocSig.py
--rw-rw-rw-   0        0        0      214 2022-11-24 08:03:54.000000 meteva-1.7.3/meteva/method/space/significance/__init__.py
--rw-rw-rw-   0        0        0     3646 2022-11-03 07:56:35.000000 meteva-1.7.3/meteva/method/space/significance/bootstrap.py
--rw-rw-rw-   0        0        0     1670 2022-11-03 08:11:48.000000 meteva-1.7.3/meteva/method/space/significance/bootstrap_ci.py
--rw-rw-rw-   0        0        0     4023 2022-11-20 14:11:12.000000 meteva-1.7.3/meteva/method/space/significance/is_sig.py
--rw-rw-rw-   0        0        0      854 2022-11-20 14:11:12.000000 meteva-1.7.3/meteva/method/space/significance/sig_coverage.py
--rw-rw-rw-   0        0        0    13422 2022-11-25 08:07:10.000000 meteva-1.7.3/meteva/method/space/significance/significance.py
--rw-rw-rw-   0        0        0     2506 2022-11-20 14:16:05.000000 meteva-1.7.3/meteva/method/space/significance/spatbiasFS.py
--rw-rw-rw-   0        0        0     1748 2022-11-03 08:16:02.000000 meteva-1.7.3/meteva/method/space/significance/tsboot.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/space/vgm/
--rw-rw-rw-   0        0        0      164 2022-11-03 08:11:48.000000 meteva-1.7.3/meteva/method/space/vgm/__init__.py
--rw-rw-rw-   0        0        0     1692 2022-02-27 00:17:20.000000 meteva-1.7.3/meteva/method/space/vgm/rdist.py
--rw-rw-rw-   0        0        0    13416 2022-02-27 00:17:20.000000 meteva-1.7.3/meteva/method/space/vgm/structurogram.py
--rw-rw-rw-   0        0        0     7840 2022-02-27 00:17:20.000000 meteva-1.7.3/meteva/method/space/vgm/structurogram_matrix.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/weather_system/
--rw-rw-rw-   0        0        0       29 2022-07-18 08:29:19.000000 meteva-1.7.3/meteva/method/weather_system/__init__.py
--rw-rw-rw-   0        0        0     9933 2022-07-28 06:07:19.000000 meteva-1.7.3/meteva/method/weather_system/identify.py
--rw-rw-rw-   0        0        0        0 2022-07-18 11:29:15.000000 meteva-1.7.3/meteva/method/weather_system/plot.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/method/yes_or_no/
--rw-rw-rw-   0        0        0      788 2021-11-21 07:43:31.000000 meteva-1.7.3/meteva/method/yes_or_no/__init__.py
--rw-rw-rw-   0        0        0    11060 2022-02-27 00:17:20.000000 meteva-1.7.3/meteva/method/yes_or_no/plot.py
--rw-rw-rw-   0        0        0    35049 2022-08-11 01:07:24.000000 meteva-1.7.3/meteva/method/yes_or_no/score.py
--rw-rw-rw-   0        0        0     2998 2021-10-22 07:58:05.000000 meteva-1.7.3/meteva/method/yes_or_no/skill.py
--rw-rw-rw-   0        0        0     7738 2022-04-21 02:55:24.000000 meteva-1.7.3/meteva/method/yes_or_no/table.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:45.000000 meteva-1.7.3/meteva/perspact/
--rw-rw-rw-   0        0        0       53 2022-07-26 13:58:05.000000 meteva-1.7.3/meteva/perspact/__init__.py
--rw-rw-rw-   0        0        0    25896 2022-10-23 13:22:56.000000 meteva-1.7.3/meteva/perspact/middle_prepare.py
--rw-rw-rw-   0        0        0    33946 2022-10-25 01:26:10.000000 meteva-1.7.3/meteva/perspact/score.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:46.000000 meteva-1.7.3/meteva/product/
--rw-rw-rw-   0        0        0      216 2022-07-10 01:42:40.000000 meteva-1.7.3/meteva/product/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:46.000000 meteva-1.7.3/meteva/product/application/
--rw-rw-rw-   0        0        0      533 2022-02-25 22:41:50.000000 meteva-1.7.3/meteva/product/application/__init__.py
--rw-rw-rw-   0        0        0    10138 2022-05-26 01:55:16.000000 meteva-1.7.3/meteva/product/application/data_collection.py
--rw-rw-rw-   0        0        0     3846 2020-06-10 05:57:46.000000 meteva-1.7.3/meteva/product/application/data_distribute.py
--rw-rw-rw-   0        0        0    24083 2022-10-27 01:45:33.000000 meteva-1.7.3/meteva/product/application/data_prepare.py
--rw-rw-rw-   0        0        0     2240 2021-09-20 08:13:53.000000 meteva-1.7.3/meteva/product/application/fun.py
--rw-rw-rw-   0        0        0     2951 2021-11-08 11:47:14.000000 meteva-1.7.3/meteva/product/application/terrain_height_correction.py
--rw-rw-rw-   0        0        0     9895 2020-03-04 02:07:44.000000 meteva-1.7.3/meteva/product/application/time_compare.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:46.000000 meteva-1.7.3/meteva/product/presentation/
--rw-rw-rw-   0        0        0        0 2022-02-25 22:41:49.000000 meteva-1.7.3/meteva/product/presentation/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:46.000000 meteva-1.7.3/meteva/product/program/
--rw-rw-rw-   0        0        0     1201 2022-07-10 03:13:50.000000 meteva-1.7.3/meteva/product/program/__init__.py
--rw-rw-rw-   0        0        0    19061 2022-05-19 07:32:32.000000 meteva-1.7.3/meteva/product/program/diurnal.py
--rw-rw-rw-   0        0        0    17966 2022-02-27 12:41:23.000000 meteva-1.7.3/meteva/product/program/error_ana_list.py
--rw-rw-rw-   0        0        0     5761 2022-02-27 12:41:23.000000 meteva-1.7.3/meteva/product/program/error_ana_scatter.py
--rw-rw-rw-   0        0        0    28305 2022-10-30 14:45:02.000000 meteva-1.7.3/meteva/product/program/fun.py
--rw-rw-rw-   0        0        0     6584 2020-12-23 09:44:56.000000 meteva-1.7.3/meteva/product/program/plot.py
--rw-rw-rw-   0        0        0      971 2022-06-07 02:04:19.000000 meteva-1.7.3/meteva/product/program/sample_statistic.py
--rw-rw-rw-   0        0        0    40438 2022-11-11 08:35:13.000000 meteva-1.7.3/meteva/product/program/score.py
--rw-rw-rw-   0        0        0   147251 2022-07-21 11:10:00.000000 meteva-1.7.3/meteva/product/program/space_compare.py
--rw-rw-rw-   0        0        0     1960 2020-09-27 01:08:16.000000 meteva-1.7.3/meteva/product/program/table.py
--rw-rw-rw-   0        0        0    61214 2022-07-05 07:34:53.000000 meteva-1.7.3/meteva/product/program/time_compare.py
--rw-rw-rw-   0        0        0     5564 2022-07-11 14:46:12.000000 meteva-1.7.3/meteva/product/program/time_space_compare.py
--rw-rw-rw-   0        0        0     2407 2022-06-14 06:00:20.000000 meteva-1.7.3/meteva/product/program/typhoon.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:46.000000 meteva-1.7.3/meteva/product/regulation/
--rw-rw-rw-   0        0        0      206 2022-08-11 06:12:59.000000 meteva-1.7.3/meteva/product/regulation/__init__.py
--rw-rw-rw-   0        0        0     8570 2022-05-20 03:12:02.000000 meteva-1.7.3/meteva/product/regulation/environment.py
--rw-rw-rw-   0        0        0     7069 2020-12-26 09:01:13.000000 meteva-1.7.3/meteva/product/regulation/short_term_heavy_rainfall.py
--rw-rw-rw-   0        0        0     3011 2022-08-11 07:10:19.000000 meteva-1.7.3/meteva/product/regulation/temperature.py
--rw-rw-rw-   0        0        0    16261 2021-03-14 02:43:06.000000 meteva-1.7.3/meteva/product/regulation/thunderstrom_gale.py
-drwxrwxrwx   0        0        0        0 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva.egg-info/
--rw-rw-rw-   0        0        0      513 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6536 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-25 08:58:44.000000 meteva-1.7.3/meteva.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-25 08:58:46.000000 meteva-1.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2125 2022-11-16 07:54:20.000000 meteva-1.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/
+-rw-rw-rw-   0        0        0      513 2023-03-22 11:47:59.000000 meteva-1.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2022-10-23 13:40:12.000000 meteva-1.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva/
+-rw-rw-rw-   0        0        0      254 2022-12-18 15:12:23.000000 meteva-1.7.4/meteva/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva/base/
+-rw-rw-rw-   0        0        0      174 2020-03-12 03:56:51.000000 meteva-1.7.4/meteva/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva/base/basicdata/
+-rw-rw-rw-   0        0        0      143 2021-04-20 14:24:26.000000 meteva-1.7.4/meteva/base/basicdata/__init__.py
+-rw-rw-rw-   0        0        0     1151 2022-07-18 07:42:19.000000 meteva-1.7.4/meteva/base/basicdata/const.py
+-rw-rw-rw-   0        0        0     7385 2022-12-18 14:39:13.000000 meteva-1.7.4/meteva/base/basicdata/ctl.py
+-rw-rw-rw-   0        0        0    19196 2021-11-06 13:46:18.000000 meteva-1.7.4/meteva/base/basicdata/dicts.py
+-rw-rw-rw-   0        0        0    11165 2022-12-20 01:27:25.000000 meteva-1.7.4/meteva/base/basicdata/grid.py
+-rw-rw-rw-   0        0        0    31585 2022-12-20 01:27:25.000000 meteva-1.7.4/meteva/base/basicdata/grid_data.py
+-rw-rw-rw-   0        0        0      669 2020-03-20 01:16:06.000000 meteva-1.7.4/meteva/base/basicdata/keys.py
+-rw-rw-rw-   0        0        0     7163 2022-09-17 14:18:55.000000 meteva-1.7.4/meteva/base/basicdata/sta_data.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva/base/fun/
+-rw-rw-rw-   0        0        0      532 2022-05-08 03:56:06.000000 meteva-1.7.4/meteva/base/fun/__init__.py
+-rw-rw-rw-   0        0        0    29905 2023-01-15 03:35:48.000000 meteva-1.7.4/meteva/base/fun/combining.py
+-rw-rw-rw-   0        0        0    27984 2022-08-24 03:18:31.000000 meteva-1.7.4/meteva/base/fun/computing.py
+-rw-rw-rw-   0        0        0    18474 2022-09-27 06:32:06.000000 meteva-1.7.4/meteva/base/fun/diagnosing.py
+-rw-rw-rw-   0        0        0    29962 2022-08-13 12:24:01.000000 meteva-1.7.4/meteva/base/fun/grouping.py
+-rw-rw-rw-   0        0        0    30978 2022-10-28 07:38:54.000000 meteva-1.7.4/meteva/base/fun/interpolating.py
+-rw-rw-rw-   0        0        0    13572 2022-07-10 12:09:39.000000 meteva-1.7.4/meteva/base/fun/nearing.py
+-rw-rw-rw-   0        0        0    47186 2023-01-18 01:17:34.000000 meteva-1.7.4/meteva/base/fun/selecting.py
+-rw-rw-rw-   0        0        0    31088 2022-06-23 03:13:55.000000 meteva-1.7.4/meteva/base/fun/statisticing.py
+-rw-rw-rw-   0        0        0    10676 2022-08-09 06:51:25.000000 meteva-1.7.4/meteva/base/fun/timing.py
+-rw-rw-rw-   0        0        0     6241 2022-08-13 01:19:17.000000 meteva-1.7.4/meteva/base/fun/transformating.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva/base/io/
+-rw-rw-rw-   0        0        0    21279 2022-10-27 01:46:57.000000 meteva-1.7.4/meteva/base/io/CMADaasAccess.py
+-rw-rw-rw-   0        0        0    13513 2020-03-04 02:07:45.000000 meteva-1.7.4/meteva/base/io/DataBlock_pb2.py
+-rw-rw-rw-   0        0        0     1085 2020-03-04 02:07:45.000000 meteva-1.7.4/meteva/base/io/GDS_data_service.py
+-rw-rw-rw-   0        0        0     1288 2020-11-12 11:24:12.000000 meteva-1.7.4/meteva/base/io/SignGenUtil.py
+-rw-rw-rw-   0        0        0      471 2022-08-08 08:44:26.000000 meteva-1.7.4/meteva/base/io/__init__.py
+-rw-rw-rw-   0        0        0     2987 2020-09-15 02:05:05.000000 meteva-1.7.4/meteva/base/io/clienthandler.py
+-rw-rw-rw-   0        0        0     1649 2020-07-06 02:31:29.000000 meteva-1.7.4/meteva/base/io/encoding.py
+-rw-rw-rw-   0        0        0    16712 2021-02-15 14:14:53.000000 meteva-1.7.4/meteva/base/io/ftpconn.py
+-rw-rw-rw-   0        0        0     1749 2021-04-29 03:15:02.000000 meteva-1.7.4/meteva/base/io/httpclient.py
+-rw-rw-rw-   0        0        0     7967 2021-02-15 14:14:53.000000 meteva-1.7.4/meteva/base/io/httpconn.py
+-rw-rw-rw-   0        0        0     4709 2021-02-15 14:14:53.000000 meteva-1.7.4/meteva/base/io/loglib.py
+-rw-rw-rw-   0        0        0     6048 2022-08-12 07:45:29.000000 meteva-1.7.4/meteva/base/io/print_grib_info.py
+-rw-rw-rw-   0        0        0    20392 2021-06-02 08:38:42.000000 meteva-1.7.4/meteva/base/io/read_graphydata.py
+-rw-rw-rw-   0        0        0    83725 2023-03-07 02:22:54.000000 meteva-1.7.4/meteva/base/io/read_griddata.py
+-rw-rw-rw-   0        0        0    89025 2022-11-30 09:06:26.000000 meteva-1.7.4/meteva/base/io/read_stadata.py
+-rw-rw-rw-   0        0        0     4670 2023-03-02 08:36:03.000000 meteva-1.7.4/meteva/base/io/write_array.py
+-rw-rw-rw-   0        0        0    10035 2022-10-09 06:20:34.000000 meteva-1.7.4/meteva/base/io/write_griddata.py
+-rw-rw-rw-   0        0        0    12422 2023-02-28 07:04:31.000000 meteva-1.7.4/meteva/base/io/write_stadata.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/base/tool/
+-rw-rw-rw-   0        0        0     1216 2023-03-01 02:53:13.000000 meteva-1.7.4/meteva/base/tool/__init__.py
+-rw-rw-rw-   0        0        0    42601 2023-02-22 23:21:34.000000 meteva-1.7.4/meteva/base/tool/color_tools.py
+-rw-rw-rw-   0        0        0    13819 2022-02-26 00:32:32.000000 meteva-1.7.4/meteva/base/tool/copy_tools.py
+-rw-rw-rw-   0        0        0     1227 2022-01-26 03:14:18.000000 meteva-1.7.4/meteva/base/tool/frprmn2.py
+-rw-rw-rw-   0        0        0     4695 2022-02-26 00:32:32.000000 meteva-1.7.4/meteva/base/tool/grib_tools.py
+-rw-rw-rw-   0        0        0     8797 2022-05-30 02:19:44.000000 meteva-1.7.4/meteva/base/tool/maskout.py
+-rw-rw-rw-   0        0        0    11223 2022-11-09 03:04:49.000000 meteva-1.7.4/meteva/base/tool/math_tools.py
+-rw-rw-rw-   0        0        0    12484 2022-05-09 13:56:16.000000 meteva-1.7.4/meteva/base/tool/path_tools.py
+-rw-rw-rw-   0        0        0   174697 2023-03-01 03:01:25.000000 meteva-1.7.4/meteva/base/tool/plot_tools.py
+-rw-rw-rw-   0        0        0    32623 2023-03-21 05:41:09.000000 meteva-1.7.4/meteva/base/tool/plot_tools_adv.py
+-rw-rw-rw-   0        0        0     4851 2022-02-27 12:00:59.000000 meteva-1.7.4/meteva/base/tool/process_tools.py
+-rw-rw-rw-   0        0        0     3647 2020-09-18 14:05:02.000000 meteva-1.7.4/meteva/base/tool/station_tools.py
+-rw-rw-rw-   0        0        0     5637 2021-09-29 03:54:03.000000 meteva-1.7.4/meteva/base/tool/time_tools.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/method/Vector/
+-rw-rw-rw-   0        0        0      611 2023-02-10 01:19:01.000000 meteva-1.7.4/meteva/method/Vector/__init__.py
+-rw-rw-rw-   0        0        0    29852 2023-02-28 08:38:01.000000 meteva-1.7.4/meteva/method/Vector/plot.py
+-rw-rw-rw-   0        0        0    46040 2022-08-19 06:02:13.000000 meteva-1.7.4/meteva/method/Vector/score.py
+-rw-rw-rw-   0        0        0      385 2022-07-18 08:30:17.000000 meteva-1.7.4/meteva/method/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/continuous/
+-rw-rw-rw-   0        0        0      994 2023-02-05 08:50:06.000000 meteva-1.7.4/meteva/method/continuous/__init__.py
+-rw-rw-rw-   0        0        0    38272 2023-01-16 07:31:13.000000 meteva-1.7.4/meteva/method/continuous/plot.py
+-rw-rw-rw-   0        0        0    43537 2023-02-05 10:56:45.000000 meteva-1.7.4/meteva/method/continuous/score.py
+-rw-rw-rw-   0        0        0     1272 2022-08-11 06:12:59.000000 meteva-1.7.4/meteva/method/continuous/skill.py
+-rw-rw-rw-   0        0        0     5086 2022-05-19 09:07:12.000000 meteva-1.7.4/meteva/method/continuous/table.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/ensemble/
+-rw-rw-rw-   0        0        0      211 2021-08-16 08:04:20.000000 meteva-1.7.4/meteva/method/ensemble/__init__.py
+-rw-rw-rw-   0        0        0     4412 2022-02-26 23:44:42.000000 meteva-1.7.4/meteva/method/ensemble/plot.py
+-rw-rw-rw-   0        0        0     4630 2022-04-21 02:55:24.000000 meteva-1.7.4/meteva/method/ensemble/score.py
+-rw-rw-rw-   0        0        0        0 2020-03-04 02:07:36.000000 meteva-1.7.4/meteva/method/ensemble/table.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/multi_category/
+-rw-rw-rw-   0        0        0      543 2021-06-02 08:05:58.000000 meteva-1.7.4/meteva/method/multi_category/__init__.py
+-rw-rw-rw-   0        0        0    15473 2022-11-14 03:23:59.000000 meteva-1.7.4/meteva/method/multi_category/plot.py
+-rw-rw-rw-   0        0        0    21927 2022-04-21 02:55:24.000000 meteva-1.7.4/meteva/method/multi_category/score.py
+-rw-rw-rw-   0        0        0     7803 2022-12-28 08:27:35.000000 meteva-1.7.4/meteva/method/multi_category/table.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/probability/
+-rw-rw-rw-   0        0        0      308 2022-03-02 14:27:29.000000 meteva-1.7.4/meteva/method/probability/__init__.py
+-rw-rw-rw-   0        0        0    21703 2022-10-23 06:25:47.000000 meteva-1.7.4/meteva/method/probability/plot.py
+-rw-rw-rw-   0        0        0     7341 2022-04-21 02:55:24.000000 meteva-1.7.4/meteva/method/probability/score.py
+-rw-rw-rw-   0        0        0     2628 2022-04-21 02:55:24.000000 meteva-1.7.4/meteva/method/probability/table.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/space/
+-rw-rw-rw-   0        0        0      310 2022-11-23 02:18:40.000000 meteva-1.7.4/meteva/method/space/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/space/fss/
+-rw-rw-rw-   0        0        0     1725 2021-11-23 02:49:29.000000 meteva-1.7.4/meteva/method/space/fss/__init__.py
+-rw-rw-rw-   0        0        0     8025 2022-06-15 13:39:04.000000 meteva-1.7.4/meteva/method/space/fss/fss.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/space/mode/
+-rw-rw-rw-   0        0        0     1933 2023-02-07 03:25:04.000000 meteva-1.7.4/meteva/method/space/mode/__init__.py
+-rw-rw-rw-   0        0        0      161 2021-02-04 10:20:28.000000 meteva-1.7.4/meteva/method/space/mode/angles_psp.py
+-rw-rw-rw-   0        0        0      384 2021-02-04 10:20:28.000000 meteva-1.7.4/meteva/method/space/mode/as_psp.py
+-rw-rw-rw-   0        0        0      910 2021-03-10 13:04:02.000000 meteva-1.7.4/meteva/method/space/mode/bearing.py
+-rw-rw-rw-   0        0        0     4059 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/censqdelta.py
+-rw-rw-rw-   0        0        0    11638 2022-05-30 12:33:28.000000 meteva-1.7.4/meteva/method/space/mode/centmatch.py
+-rw-rw-rw-   0        0        0     9067 2022-11-12 03:01:53.000000 meteva-1.7.4/meteva/method/space/mode/consistent.py
+-rw-rw-rw-   0        0        0     3537 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/data_pre.py
+-rw-rw-rw-   0        0        0     1497 2022-02-25 08:34:50.000000 meteva-1.7.4/meteva/method/space/mode/deltametric.py
+-rw-rw-rw-   0        0        0     3541 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/deltamm.py
+-rw-rw-rw-   0        0        0    18089 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/deltammSqCen.py
+-rw-rw-rw-   0        0        0     3530 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/deltamm_bak.py
+-rw-rw-rw-   0        0        0     4801 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/distmap.py
+-rw-rw-rw-   0        0        0     6072 2022-06-10 07:13:19.000000 meteva-1.7.4/meteva/method/space/mode/feature_axis.py
+-rw-rw-rw-   0        0        0     4087 2022-06-24 14:09:57.000000 meteva-1.7.4/meteva/method/space/mode/feature_comps.py
+-rw-rw-rw-   0        0        0    31716 2022-07-19 07:56:52.000000 meteva-1.7.4/meteva/method/space/mode/feature_finder.py
+-rw-rw-rw-   0        0        0    10157 2023-02-07 02:37:08.000000 meteva-1.7.4/meteva/method/space/mode/feature_match_analyzer.py
+-rw-rw-rw-   0        0        0     2456 2022-06-10 12:47:16.000000 meteva-1.7.4/meteva/method/space/mode/feature_props.py
+-rw-rw-rw-   0        0        0     5142 2022-06-11 09:04:30.000000 meteva-1.7.4/meteva/method/space/mode/feature_table.py
+-rw-rw-rw-   0        0        0    10478 2022-06-30 15:07:24.000000 meteva-1.7.4/meteva/method/space/mode/interester.py
+-rw-rw-rw-   0        0        0      748 2022-02-24 23:16:53.000000 meteva-1.7.4/meteva/method/space/mode/intersect.py
+-rw-rw-rw-   0        0        0      201 2021-02-04 10:20:28.000000 meteva-1.7.4/meteva/method/space/mode/lengths_psp.py
+-rw-rw-rw-   0        0        0     1269 2023-02-07 07:23:55.000000 meteva-1.7.4/meteva/method/space/mode/load.py
+-rw-rw-rw-   0        0        0     1365 2021-02-04 10:20:28.000000 meteva-1.7.4/meteva/method/space/mode/loc_list_setup.py
+-rw-rw-rw-   0        0        0     3987 2022-02-25 08:35:16.000000 meteva-1.7.4/meteva/method/space/mode/locperf.py
+-rw-rw-rw-   0        0        0     7803 2022-02-25 06:16:09.000000 meteva-1.7.4/meteva/method/space/mode/make_SpatialVx_bak.py
+-rw-rw-rw-   0        0        0     7943 2022-02-24 23:16:53.000000 meteva-1.7.4/meteva/method/space/mode/make_spatialVx.py
+-rw-rw-rw-   0        0        0    11321 2022-06-30 15:12:30.000000 meteva-1.7.4/meteva/method/space/mode/merge_force.py
+-rw-rw-rw-   0        0        0      203 2022-02-24 23:16:53.000000 meteva-1.7.4/meteva/method/space/mode/midpoints_psp.py
+-rw-rw-rw-   0        0        0    18185 2022-02-24 23:16:53.000000 meteva-1.7.4/meteva/method/space/mode/minboundmatch.py
+-rw-rw-rw-   0        0        0     5727 2023-02-07 02:37:07.000000 meteva-1.7.4/meteva/method/space/mode/operater.py
+-rw-rw-rw-   0        0        0    32002 2022-11-18 15:03:34.000000 meteva-1.7.4/meteva/method/space/mode/plot.py
+-rw-rw-rw-   0        0        0     7757 2022-02-27 12:41:23.000000 meteva-1.7.4/meteva/method/space/mode/regress2.py
+-rw-rw-rw-   0        0        0     2226 2022-06-10 07:15:34.000000 meteva-1.7.4/meteva/method/space/mode/sma.py
+-rw-rw-rw-   0        0        0    10131 2023-02-07 03:23:11.000000 meteva-1.7.4/meteva/method/space/mode/tran_to_dataframe.py
+-rw-rw-rw-   0        0        0      519 2021-02-04 10:20:28.000000 meteva-1.7.4/meteva/method/space/mode/utils.py
+-rw-rw-rw-   0        0        0     4595 2023-03-20 12:31:25.000000 meteva-1.7.4/meteva/method/space/point_to_area.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/space/rigider/
+-rw-rw-rw-   0        0        0      394 2021-11-01 03:34:12.000000 meteva-1.7.4/meteva/method/space/rigider/__init__.py
+-rw-rw-rw-   0        0        0    10874 2021-11-02 02:23:51.000000 meteva-1.7.4/meteva/method/space/rigider/fint2d.py
+-rw-rw-rw-   0        0        0     8093 2021-10-29 08:05:10.000000 meteva-1.7.4/meteva/method/space/rigider/fint2d_old.py
+-rw-rw-rw-   0        0        0     1114 2021-10-28 01:37:41.000000 meteva-1.7.4/meteva/method/space/rigider/imomenter.py
+-rw-rw-rw-   0        0        0      431 2021-10-24 18:01:18.000000 meteva-1.7.4/meteva/method/space/rigider/mij.py
+-rw-rw-rw-   0        0        0      191 2021-10-24 18:01:18.000000 meteva-1.7.4/meteva/method/space/rigider/q_loss_rigid.py
+-rw-rw-rw-   0        0        0      465 2021-11-01 13:32:37.000000 meteva-1.7.4/meteva/method/space/rigider/rigid_transform.py
+-rw-rw-rw-   0        0        0    13373 2021-11-02 02:16:32.000000 meteva-1.7.4/meteva/method/space/rigider/rigider.py
+-rw-rw-rw-   0        0        0      275 2021-10-24 18:01:18.000000 meteva-1.7.4/meteva/method/space/rigider/zapsmall.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:58.000000 meteva-1.7.4/meteva/method/space/saller/
+-rw-rw-rw-   0        0        0      329 2021-04-17 00:33:40.000000 meteva-1.7.4/meteva/method/space/saller/__init__.py
+-rw-rw-rw-   0        0        0     5904 2022-07-27 01:17:46.000000 meteva-1.7.4/meteva/method/space/saller/saller.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/method/space/significance/
+-rw-rw-rw-   0        0        0     4074 2022-11-08 08:43:59.000000 meteva-1.7.4/meteva/method/space/significance/LocSig.py
+-rw-rw-rw-   0        0        0      214 2022-11-24 08:03:54.000000 meteva-1.7.4/meteva/method/space/significance/__init__.py
+-rw-rw-rw-   0        0        0     3646 2022-11-03 07:56:35.000000 meteva-1.7.4/meteva/method/space/significance/bootstrap.py
+-rw-rw-rw-   0        0        0     1670 2022-11-03 08:11:48.000000 meteva-1.7.4/meteva/method/space/significance/bootstrap_ci.py
+-rw-rw-rw-   0        0        0     4023 2022-11-20 14:11:12.000000 meteva-1.7.4/meteva/method/space/significance/is_sig.py
+-rw-rw-rw-   0        0        0      854 2022-11-20 14:11:12.000000 meteva-1.7.4/meteva/method/space/significance/sig_coverage.py
+-rw-rw-rw-   0        0        0    13422 2022-11-25 08:07:10.000000 meteva-1.7.4/meteva/method/space/significance/significance.py
+-rw-rw-rw-   0        0        0     2506 2022-11-20 14:16:05.000000 meteva-1.7.4/meteva/method/space/significance/spatbiasFS.py
+-rw-rw-rw-   0        0        0     1748 2022-11-03 08:16:02.000000 meteva-1.7.4/meteva/method/space/significance/tsboot.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/method/space/vgm/
+-rw-rw-rw-   0        0        0      164 2022-11-03 08:11:48.000000 meteva-1.7.4/meteva/method/space/vgm/__init__.py
+-rw-rw-rw-   0        0        0     1692 2022-02-27 00:17:20.000000 meteva-1.7.4/meteva/method/space/vgm/rdist.py
+-rw-rw-rw-   0        0        0    13416 2022-02-27 00:17:20.000000 meteva-1.7.4/meteva/method/space/vgm/structurogram.py
+-rw-rw-rw-   0        0        0     7840 2022-02-27 00:17:20.000000 meteva-1.7.4/meteva/method/space/vgm/structurogram_matrix.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/method/weather_system/
+-rw-rw-rw-   0        0        0       29 2022-07-18 08:29:19.000000 meteva-1.7.4/meteva/method/weather_system/__init__.py
+-rw-rw-rw-   0        0        0     9933 2022-07-28 06:07:19.000000 meteva-1.7.4/meteva/method/weather_system/identify.py
+-rw-rw-rw-   0        0        0        0 2022-07-18 11:29:15.000000 meteva-1.7.4/meteva/method/weather_system/plot.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/method/yes_or_no/
+-rw-rw-rw-   0        0        0      788 2021-11-21 07:43:31.000000 meteva-1.7.4/meteva/method/yes_or_no/__init__.py
+-rw-rw-rw-   0        0        0    11060 2022-02-27 00:17:20.000000 meteva-1.7.4/meteva/method/yes_or_no/plot.py
+-rw-rw-rw-   0        0        0    35049 2023-03-07 00:53:25.000000 meteva-1.7.4/meteva/method/yes_or_no/score.py
+-rw-rw-rw-   0        0        0     2995 2023-03-03 07:52:23.000000 meteva-1.7.4/meteva/method/yes_or_no/skill.py
+-rw-rw-rw-   0        0        0     7738 2022-04-21 02:55:24.000000 meteva-1.7.4/meteva/method/yes_or_no/table.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/perspact/
+-rw-rw-rw-   0        0        0       53 2022-07-26 13:58:05.000000 meteva-1.7.4/meteva/perspact/__init__.py
+-rw-rw-rw-   0        0        0    26617 2023-02-05 11:17:51.000000 meteva-1.7.4/meteva/perspact/middle_prepare.py
+-rw-rw-rw-   0        0        0    36277 2023-02-05 10:59:22.000000 meteva-1.7.4/meteva/perspact/score.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/product/
+-rw-rw-rw-   0        0        0      216 2022-07-10 01:42:40.000000 meteva-1.7.4/meteva/product/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/product/application/
+-rw-rw-rw-   0        0        0      533 2022-02-25 22:41:50.000000 meteva-1.7.4/meteva/product/application/__init__.py
+-rw-rw-rw-   0        0        0    10138 2022-05-26 01:55:16.000000 meteva-1.7.4/meteva/product/application/data_collection.py
+-rw-rw-rw-   0        0        0     3846 2020-06-10 05:57:46.000000 meteva-1.7.4/meteva/product/application/data_distribute.py
+-rw-rw-rw-   0        0        0    24149 2022-12-02 02:34:12.000000 meteva-1.7.4/meteva/product/application/data_prepare.py
+-rw-rw-rw-   0        0        0     2240 2021-09-20 08:13:53.000000 meteva-1.7.4/meteva/product/application/fun.py
+-rw-rw-rw-   0        0        0     2951 2021-11-08 11:47:14.000000 meteva-1.7.4/meteva/product/application/terrain_height_correction.py
+-rw-rw-rw-   0        0        0     9895 2020-03-04 02:07:44.000000 meteva-1.7.4/meteva/product/application/time_compare.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/product/presentation/
+-rw-rw-rw-   0        0        0        0 2022-02-25 22:41:49.000000 meteva-1.7.4/meteva/product/presentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/product/program/
+-rw-rw-rw-   0        0        0     1201 2022-07-10 03:13:50.000000 meteva-1.7.4/meteva/product/program/__init__.py
+-rw-rw-rw-   0        0        0    19079 2023-01-13 06:11:18.000000 meteva-1.7.4/meteva/product/program/diurnal.py
+-rw-rw-rw-   0        0        0    17966 2022-02-27 12:41:23.000000 meteva-1.7.4/meteva/product/program/error_ana_list.py
+-rw-rw-rw-   0        0        0     5761 2022-02-27 12:41:23.000000 meteva-1.7.4/meteva/product/program/error_ana_scatter.py
+-rw-rw-rw-   0        0        0    28305 2022-10-30 14:45:02.000000 meteva-1.7.4/meteva/product/program/fun.py
+-rw-rw-rw-   0        0        0     6663 2023-01-13 02:52:16.000000 meteva-1.7.4/meteva/product/program/plot.py
+-rw-rw-rw-   0        0        0      971 2022-06-07 02:04:19.000000 meteva-1.7.4/meteva/product/program/sample_statistic.py
+-rw-rw-rw-   0        0        0    40787 2023-02-23 06:03:50.000000 meteva-1.7.4/meteva/product/program/score.py
+-rw-rw-rw-   0        0        0   147630 2022-12-21 03:21:41.000000 meteva-1.7.4/meteva/product/program/space_compare.py
+-rw-rw-rw-   0        0        0     1960 2020-09-27 01:08:16.000000 meteva-1.7.4/meteva/product/program/table.py
+-rw-rw-rw-   0        0        0    61214 2022-07-05 07:34:53.000000 meteva-1.7.4/meteva/product/program/time_compare.py
+-rw-rw-rw-   0        0        0     5564 2022-07-11 14:46:12.000000 meteva-1.7.4/meteva/product/program/time_space_compare.py
+-rw-rw-rw-   0        0        0     2407 2022-06-14 06:00:20.000000 meteva-1.7.4/meteva/product/program/typhoon.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:59.000000 meteva-1.7.4/meteva/product/regulation/
+-rw-rw-rw-   0        0        0      206 2022-08-11 06:12:59.000000 meteva-1.7.4/meteva/product/regulation/__init__.py
+-rw-rw-rw-   0        0        0     8570 2022-05-20 03:12:02.000000 meteva-1.7.4/meteva/product/regulation/environment.py
+-rw-rw-rw-   0        0        0     7069 2020-12-26 09:01:13.000000 meteva-1.7.4/meteva/product/regulation/short_term_heavy_rainfall.py
+-rw-rw-rw-   0        0        0     3011 2022-08-11 07:10:19.000000 meteva-1.7.4/meteva/product/regulation/temperature.py
+-rw-rw-rw-   0        0        0    16261 2021-03-14 02:43:06.000000 meteva-1.7.4/meteva/product/regulation/thunderstrom_gale.py
+drwxrwxrwx   0        0        0        0 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva.egg-info/
+-rw-rw-rw-   0        0        0      513 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6536 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-22 11:47:57.000000 meteva-1.7.4/meteva.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-22 11:47:59.000000 meteva-1.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2172 2022-12-28 03:00:34.000000 meteva-1.7.4/setup.py
```

### Comparing `meteva-1.7.3/PKG-INFO` & `meteva-1.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteva
-Version: 1.7.3
+Version: 1.7.4
 Summary: A collections of functions for meteorological verification.
 Home-page: UNKNOWN
 Author: liucouhua,daikan,wangbaoli,tangbuxing
 Author-email: liucouhua@163.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `meteva-1.7.3/meteva/base/basicdata/const.py` & `meteva-1.7.4/meteva/base/basicdata/const.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/basicdata/ctl.py` & `meteva-1.7.4/meteva/base/basicdata/ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
                             nlevel = 1
                         onev["nlevel"] = nlevel
                         onev["type"] = int(strs[2])
                         onev["discription"] = strs[3]
                         onev["start_bolck_index"] = cumulate
                         cumulate += nlevel
                         ctl["vars"].append(onev)
+                    ctl["cumulate_levels"] = cumulate
 
             line = file.readline()
         if "edef" not in ctl.keys():
             ctl["edef"] = [0]
             ctl["nensemble"] = 1
         if "ntime" not in ctl.keys():
             ctl["ntime"] = 1
```

### Comparing `meteva-1.7.3/meteva/base/basicdata/dicts.py` & `meteva-1.7.4/meteva/base/basicdata/dicts.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/basicdata/grid.py` & `meteva-1.7.4/meteva/base/basicdata/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,8 +269,13 @@
 
 def reset_grid(grid0):
     if grid0.dlat <0:
         grid0.dlat = - grid0.dlat
         tran = grid0.slat
         grid0.slat = grid0.elat
         grid0.elat = tran
+    if grid0.dlon <0:
+        grid0.dlon = - grid0.dlon
+        tran = grid0.slon
+        grid0.slon = grid0.elon
+        grid0.elon = tran
     return
```

### Comparing `meteva-1.7.3/meteva/base/basicdata/grid_data.py` & `meteva-1.7.4/meteva/base/basicdata/grid_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,15 +873,21 @@
     return da
 
 
 
 
 def reset(grd):
     lats = grd["lat"].values
-
     if lats[0]>lats[1]:
         lats = grd["lat"].values[::-1]
         grd['lat'] = lats
         dat = grd.values[:, :, :, :, ::-1, :]
         grd.values = dat
 
+    lons = grd["lon"].values
+    if lons[0]>lons[1]:
+        lons = grd["lon"].values[::-1]
+        grd['lon'] = lons
+        dat = grd.values[:, :, :, :, :, ::-1]
+        grd.values = dat
+
     return
```

### Comparing `meteva-1.7.3/meteva/base/basicdata/keys.py` & `meteva-1.7.4/meteva/base/basicdata/keys.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/basicdata/sta_data.py` & `meteva-1.7.4/meteva/base/basicdata/sta_data.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/__init__.py` & `meteva-1.7.4/meteva/base/fun/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/combining.py` & `meteva-1.7.4/meteva/base/fun/combining.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,14 +401,15 @@
     :param sta_fo_list:
     :return:
     '''
     if not isinstance(sta_fo_list, list):
         print("the second args shold be a list")
         return
     sta_all = None
+
     if g =="id":
         grouped_ob = dict(list(sta_ob.groupby("id")))
         nfo = len(sta_fo_list)
         grouped_fo_list=[]
         for i in range(nfo):
             grouped_fo_list.append(dict(list(sta_fo_list[i].groupby("id"))))
         id_ob = list(grouped_ob.keys())
@@ -445,15 +446,14 @@
         grouped_fo_list = []
         dtime_list = []
         for i in range(nfo):
             dict1 = dict(list(sta_fo_list[i].groupby("dtime")))
             grouped_fo_list.append(dict1)
             dtime_list.extend(list(dict1.keys()))
         dtime_list = list(set(dtime_list))
-        print(dtime_list)
         sys._clear_type_cache()
         gc.collect()
         sta_list = []
         n_dtime = len(dtime_list)
 
         for i in range(n_dtime):
             rate = int((i/n_dtime)*100)
@@ -479,14 +479,20 @@
         sta_all = concat(sta_list)
         del sta_list
     if sta_all is not None:
         sta_all = sta_all.fillna(meteva.base.IV)
     sta_all.attrs = copy.deepcopy(sta_ob.attrs)
     sta_all.drop_duplicates(subset=["level","time","dtime","id"],inplace=True)
     sta_all.sort_values(by=["level", "time", "dtime", "id"], inplace=True)
+
+    names = meteva.base.get_stadata_names(sta_ob)
+    for i in range(len(sta_fo_list)):
+        names.extend(meteva.base.get_stadata_names(sta_fo_list[i]))
+    sta_all = meteva.base.in_member_list(sta_all,member_list=names)
+
     return sta_all
 
 
 def combine_on_obTime(sta_ob,sta_fo_list,need_match_ob = False):
     if not isinstance(sta_fo_list, list):
         sta_fo_list = [sta_fo_list]
```

### Comparing `meteva-1.7.3/meteva/base/fun/computing.py` & `meteva-1.7.4/meteva/base/fun/computing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/diagnosing.py` & `meteva-1.7.4/meteva/base/fun/diagnosing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/grouping.py` & `meteva-1.7.4/meteva/base/fun/grouping.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/interpolating.py` & `meteva-1.7.4/meteva/base/fun/interpolating.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/nearing.py` & `meteva-1.7.4/meteva/base/fun/nearing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/selecting.py` & `meteva-1.7.4/meteva/base/fun/selecting.py`

 * *Files 1% similar despite different names*

```diff
@@ -712,30 +712,32 @@
 
     p_set = ["member","level","time","time_range","year","month","day","dayofyear","hour", "ob_time","ob_time_range" ,"ob_year",
               "ob_month", "ob_day","ob_dayofyear","ob_hour","dtime","dtime_range","dday","dhour" ,
               "lon","lat", "id","grid","gxy", "gxyz" ,"stadata","ob_stadata","value","drop_IV","last" , "last_range","drop_last","province_name"]
 
 
     sta1 = data
-    data_names = meteva.base.get_stadata_names(data)
-    p_set.extend(data_names)
-    data_names_range = []
-    for data_name in data_names:
-        data_names_range.append(str(data_name)+"_range")
-    p_set.extend(data_names_range)
-    for key in s.keys():
-        if key in data_names:
-            value_one = s[key]
-            if not isinstance(value_one,list):
-                value_one = [value_one]
-            sta1 = in_one_column_value_list(sta1,key, value_one)
-        elif key in data_names_range:
-            value_one = s[key]
-            data_name = key.split("_")[0]
-            sta1 = between_one_column_value_range(sta1,data_name,value_one[0],value_one[1])
+
+    if isinstance(data, pd.DataFrame):
+        data_names = meteva.base.get_stadata_names(data)
+        p_set.extend(data_names)
+        data_names_range = []
+        for data_name in data_names:
+            data_names_range.append(str(data_name)+"_range")
+        p_set.extend(data_names_range)
+        for key in s.keys():
+            if key in data_names:
+                value_one = s[key]
+                if not isinstance(value_one,list):
+                    value_one = [value_one]
+                sta1 = in_one_column_value_list(sta1,key, value_one)
+            elif key in data_names_range:
+                value_one = s[key]
+                data_name = key[0:-6]
+                sta1 = between_one_column_value_range(sta1,data_name,value_one[0],value_one[1])
 
 
     key_set = s.keys() #set(list(s.keys()))
     if(not set(p_set) >= key_set):
         print("参数s的字典中包含本程序不能识别的关键词")
         return None
 
@@ -925,32 +927,31 @@
     :param value: 提取所有数据列都在给定取值范围的数据，列表形式，第一个元素为数据最低值，第二个为数据最高值
     :param drop_IV: 该参数为True时，删除包含缺省值的行
     :param last_range: 包含起始值和结束值的列表，取出最后一列取值在该取值范围的数据，并删除最后一列的数据
     :param last: 取出最后一列包含lastL的行，如何选择多个类型，lastL采用列表形式，并删除最后一列的数据
     :return:  [站点数据](https://www.showdoc.cc/nmc?page_id=3744334022014027)
     '''
     sta1 = data
-
-    data_names = meteva.base.get_stadata_names(data)
-    data_names_range = []
-    for data_name in data_names:
-        data_names_range.append(str(data_name)+"_range")
-    for key in kwargs.keys():
-        if key in data_names:
-            value_one = kwargs[key]
-            if not isinstance(value_one,list):
-                value_one = [value_one]
-            sta1 = in_one_column_value_list(sta1,key, value_one)
-        elif key in data_names_range:
-            value_one = kwargs[key]
-            data_name = key.split("_")[0]
-            sta1 = between_one_column_value_range(sta1,data_name,value_one[0],value_one[1])
-        else:
-            print("输入的参数"+key+"不是数据选取函数可接受的参数")
-
+    if isinstance(data, pd.DataFrame):
+        data_names = meteva.base.get_stadata_names(data)
+        data_names_range = []
+        for data_name in data_names:
+            data_names_range.append(str(data_name)+"_range")
+        for key in kwargs.keys():
+            if key in data_names:
+                value_one = kwargs[key]
+                if not isinstance(value_one,list):
+                    value_one = [value_one]
+                sta1 = in_one_column_value_list(sta1,key, value_one)
+            elif key in data_names_range:
+                value_one = kwargs[key]
+                data_name = key[0:-6]
+                sta1 = between_one_column_value_range(sta1,data_name,value_one[0],value_one[1])
+            else:
+                print("输入的参数"+key+"不是数据选取函数可接受的参数")
 
     if member is not None:
         sta1 = in_member_list(sta1,member)
     if level is not None:
         sta1 = in_level_list(sta1,level)
     if time is not None:
         sta1 = in_time_list(sta1, time)
```

### Comparing `meteva-1.7.3/meteva/base/fun/statisticing.py` & `meteva-1.7.4/meteva/base/fun/statisticing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/timing.py` & `meteva-1.7.4/meteva/base/fun/timing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/fun/transformating.py` & `meteva-1.7.4/meteva/base/fun/transformating.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/CMADaasAccess.py` & `meteva-1.7.4/meteva/base/io/CMADaasAccess.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/DataBlock_pb2.py` & `meteva-1.7.4/meteva/base/io/DataBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/GDS_data_service.py` & `meteva-1.7.4/meteva/base/io/GDS_data_service.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/SignGenUtil.py` & `meteva-1.7.4/meteva/base/io/SignGenUtil.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/clienthandler.py` & `meteva-1.7.4/meteva/base/io/clienthandler.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/encoding.py` & `meteva-1.7.4/meteva/base/io/encoding.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/ftpconn.py` & `meteva-1.7.4/meteva/base/io/ftpconn.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/httpclient.py` & `meteva-1.7.4/meteva/base/io/httpclient.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/httpconn.py` & `meteva-1.7.4/meteva/base/io/httpconn.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/loglib.py` & `meteva-1.7.4/meteva/base/io/loglib.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/print_grib_info.py` & `meteva-1.7.4/meteva/base/io/print_grib_info.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/read_graphydata.py` & `meteva-1.7.4/meteva/base/io/read_graphydata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/read_griddata.py` & `meteva-1.7.4/meteva/base/io/read_griddata.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,16 @@
             else:
                 #如果传入函数有grid信息，就需要进行一次双线性插值，按照grid信息进行提取网格信息。
                 da1 = meteva.base.interp_gg_linear(da, grid)
                 if show:
                     print("success read from " + filename)
                 return da1
         else:
+            print("自描述信息中的网格数是：" +str(nlon1) + "*" + str(nlat1) +"="+ str(nlon1 * nlat1))
+            print("实际数据大小为："+str(len(strs) - 22))
             print("m4 文件式错误，文件自描述信息中网格数和实际数据大小不一致")
             return None
     except:
         if show:
             exstr = traceback.format_exc()
             print(exstr)
         print(filename + "文件格式不能识别。可能原因：文件未按micaps4格式存储")
@@ -1734,23 +1736,29 @@
             if data_name is not None:
                 meteva.base.set_griddata_coords(grd, member_list=[data_name])
             return grd
 
         else:
             grid0 = meteva.base.grid(ctl["glon"],ctl["glat"])
             blocksize_xy = grid0.nlon * grid0.nlat * 4
-            ensembel_size = 1
+
+            data_list = []
+            blocksize_one_time = ctl["cumulate_levels"] *blocksize_xy
             nlevel = ctl["vars"][value_index]["nlevel"]
-            blocksize_time_ensemble = blocksize_xy *  ctl["ntime"] * ctl["nensemble"]
-            start_index = ctl["vars"][value_index]["start_bolck_index"] * blocksize_time_ensemble
-            position = file.seek(start_index)
-            blocksize_one_value = blocksize_time_ensemble * nlevel
-            content = file.read(blocksize_one_value)
-            data = np.frombuffer(content, dtype=endian +"f")
+            for nn in range(ctl["nensemble"]):
+                for t in range(ctl["ntime"]):
+                    start_index =blocksize_one_time *ctl["ntime"] * nn +  t * blocksize_one_time + ctl["vars"][value_index][
+                        "start_bolck_index"] * blocksize_xy
+                    position = file.seek(start_index)
+                    blocksize_one_value = blocksize_xy * nlevel
+                    content = file.read(blocksize_one_value)
+                    data1 = np.frombuffer(content, dtype=endian + "f")
+                    data_list.append(data1)
 
+            data = np.array(data_list)
             data = data.reshape(ctl["nensemble"], ctl["ntime"], nlevel, ctl["nlat"], ctl["nlon"])
             data = data.transpose(0,2,1,3,4)
             if nlevel != len(ctl["zdef"]):
                 level_list = np.arange(ctl["vars"][value_index]["nlevel"])
             else:
                 level_list =ctl["zdef"]
```

### Comparing `meteva-1.7.3/meteva/base/io/read_stadata.py` & `meteva-1.7.4/meteva/base/io/read_stadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1039,15 +1039,15 @@
                 record_head_dtype = [
                    ('lon', 'f4'), ('lat', 'f4'), ('numb', 'i2')]
                 records = []
                 #if station is None or len(station.index) * 100 > station_number:
                 for i in range(station_number):
                     string_id_record_length = np.frombuffer( byteArray[ind:(ind + 2)],dtype="i2")[0]
                     dtype1 = "S" + str(string_id_record_length)
-                    print(string_id_record_length)
+                    #print(string_id_record_length)
                     if string_id_record_length==0:
                         string_id ="999999"
                     else:
                         string_id = np.frombuffer(byteArray[ind+2:(ind + 2+string_id_record_length)],dtype=dtype1)[0]
                         string_id = string_id.decode()
                     ind += (2+string_id_record_length)
                     record_head = np.frombuffer(
```

### Comparing `meteva-1.7.3/meteva/base/io/write_array.py` & `meteva-1.7.4/meteva/base/io/write_array.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pandas as pd
 import numpy as np
+import meteva
 def write_array_to_excel(array,save_path,name_list_dict,columns = None,index = None):
     shape = array.shape
     keys = list(name_list_dict.keys())
     if len(shape) ==1:
         rows = [[keys[0]],name_list_dict[keys[0]]]
         table_data = pd.DataFrame(array,index=pd.MultiIndex.from_product(rows))
         table_data.to_excel(save_path, sheet_name='sheet1')
@@ -84,25 +85,31 @@
             print("axis 参数的取值必须是name_list_dict的key")
         newshape = (keys.index(sheet),keys.index(index),keys.index(columns))
         data = array.transpose(newshape)
         table_data_list = []
         cols= [[columns],name_list_dict[columns]]
         rows = [[index],name_list_dict[index]]
         sheet_list = name_list_dict[sheet]
-
+        if isinstance(sheet_list[0],pd._libs.tslibs.timestamps.Timestamp):
+            print(type(sheet_list[0]))
+            sheet_list1 = []
+            for name in sheet_list:
+                name1 = meteva.base.all_type_time_to_str(name)
+                sheet_list1.append(name1)
+            sheet_list = sheet_list1
         for s in range(len(sheet_list)):
             # table_data = pd.DataFrame(array[:,:,s])
             table_data = pd.DataFrame(data[s,:, :],
                                       columns=pd.MultiIndex.from_product(cols),
                                       index=pd.MultiIndex.from_product(rows)
                                       )
             table_data_list.append(table_data)
         with pd.ExcelWriter(save_path) as writer:
             for i in range(len(sheet_list)):
-                str1 = str(name_list_dict[sheet][i])
+                str1 = str(sheet_list[i])
                 str1 = str1.replace("[","【")
                 #print(str1)
                 table_data_list[i].to_excel(writer, sheet_name=sheet + '_' + str1)
     else:
         print("array不能超过3维")
         return
```

### Comparing `meteva-1.7.3/meteva/base/io/write_griddata.py` & `meteva-1.7.4/meteva/base/io/write_griddata.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/io/write_stadata.py` & `meteva-1.7.4/meteva/base/io/write_stadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -252,14 +252,78 @@
     dict1 = {}
     dict1["attrs"] = sta1.attrs
     dict1["data"] = sta1.to_dict(orient='index')
     str_data = json.dumps(dict1)
     return str_data'''
 
 
+def write_stadata_to_micaps2(sta_speed,sta_angle,save_path = "a.txt",creat_dir = False, type = 0,effectiveNum = 4,show = False,title = None):
+    """
+    生成micaps3格式的文件
+    :param sta0:站点数据信息
+    :param save_path 需要保存的文件路径和名称
+    :param type 类型：默认：1
+    :param effectiveNum 有效数字 默认为：4
+    :return:保存为micaps3格式的文件
+    """
+    try:
+
+        dir = os.path.split(os.path.abspath(save_path))[0]
+        if not os.path.isdir(dir):
+            if not creat_dir:
+                print("文件夹：" + dir + "不存在")
+                return False
+            else:
+                meteva.base.tool.path_tools.creat_path(save_path)
+
+        br = open(save_path,'w')
+        end = len(save_path)
+        start = max(0, end-16)
+        sta = meteva.base.combine_on_all_coords(sta_angle,sta_speed)
+        nsta =len(sta.index)
+        time = sta['time'].iloc[0]
+        if isinstance(time,np.datetime64) or isinstance(time,datetime.datetime):
+            time_str = meteva.base.tool.time_tools.time_to_str(time)
+            time_str = time_str[0:4] + " " +time_str[4:6] + " " + time_str[6:8] + " " + time_str[8:10] + " "
+        else:
+            time_str = "2099 01 01 0 "
+
+        if np.isnan(sta['level'].iloc[0]):
+            level = 0
+        else:
+            level = int(sta['level'].iloc[0])
+        if type<0 or level == np.NaN or level ==pd.NaT:
+            level = int(type)
+
+        if title is None:
+            str1=("diamond 2 " + save_path[start:end] + "\n"+ time_str + str(level) +" " + str(nsta) + "\n")
+        else:
+            str1 = ("diamond 2 " + title + "\n" + time_str + str(level) +" "  + str(nsta) + "\n")
+        br.write(str1)
+        br.close()
+
+        df = copy.deepcopy(sta[['id','lon','lat']])
+        df['alt'] = 0
+        df["d0"] = 1
+        df["d1"] = 9999
+        df["d2"] = 9999
+        df["d3"] = 9999
+        df["angle"] = sta.iloc[:,6]
+        df["speed"] = sta.iloc[:, 7]
+
+        effectiveNum_str = "%." + '%d'% effectiveNum + "f"
+        df.to_csv(save_path,mode='a',header=None,sep = "\t",float_format=effectiveNum_str,index = None)
+        if show:
+            print('成功输出至' + save_path)
+        return True
+    except:
+        exstr = traceback.format_exc()
+        print(exstr)
+        return False
+
+
 
 if __name__ == "__main__":
-    meteva.base.print_gds_file_values_names(r"H:\test_data\20210220160000.000")
-    sta = meteva.base.read_stadata_from_gdsfile(r"H:\test_data\20210220160000.000",element_id=603)
-    sta.attrs["description"] = "Temp"
-    print(sta)
-    write_stadata_to_gds_file(sta,save_path=r"H:\test_data\output\meb\m3_gds_test.000")
+    path = r"D:\book\test_data\charpter11\ob_with_noisy\22010102.000"
+    sta = pd.read_csv(path, parse_dates=["time"])
+    speed,angle = meteva.base.wind_to_speed_angle(sta)
+    write_stadata_to_micaps2(speed,angle,r"D:\book\test_data\charpter11\a.txt")
```

### Comparing `meteva-1.7.3/meteva/base/tool/__init__.py` & `meteva-1.7.4/meteva/base/tool/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 from .copy_tools import copy_m4_to_nc,copy_data
 from .time_tools import all_type_time_to_datetime,all_type_time_to_time64,all_type_time_to_str
 from .time_tools import all_type_timedelta_to_timedelta64,all_type_timedelta_to_timedelta
 from .grib_tools import grib_to_nc
 from .station_tools import get_station_id_name_dict,station_id_name_dict,station_name_id_dict,find_station_id_by_city_name,get_station_format_province_set
 from .process_tools import multi_run
-from .plot_tools import contourf_2d_grid,pcolormesh_2d_grid,scatter_sta,bar,plot,mesh,set_customized_shpfile_list,add_scatter,bar_line,myheatmap,contourf
+from .plot_tools import contourf_2d_grid,pcolormesh_2d_grid,scatter_sta,bar,plot,mesh,set_customized_shpfile_list,add_scatter,bar_line,myheatmap,contourf,barbs_grid_wind
 from .color_tools import cmaps,def_cmap_clevs,merge_cmap_clevs,get_seprated_rgb_method1,get_seprated_rgb_method2,set_plot_color_dict_method0,set_plot_color_dict_method1,set_plot_color_dict_method2
 from .maskout import *
 from .plot_tools_adv import *
```

### Comparing `meteva-1.7.3/meteva/base/tool/color_tools.py` & `meteva-1.7.4/meteva/base/tool/color_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         clev_list.append(1 + v * 0.2)
         cmap_list.append(white * (1 - v * 0.2) + yellow * v * 0.2)
 
     for v in range(1,6):
         clev_list.append(2 + v * 0.2)
         cmap_list.append(yellow * (1 - v * 0.2) + red * v * 0.2)
 
-    for v in range(1,11):
+    for v in range(1,10):
         clev_list.append(3 + v * 0.5)
         cmap_list.append(red * (1 - v * 0.1) + pink * v * 0.1)
 
     for value in range(8, int(vmax + 1), 1):
         clev_list.append(value)
         cmap_list.append((pink * (vmax - value) + black * (value - 2)) / (vmax - 2))
     cmap = colors.ListedColormap(cmap_list, 'indexed')
```

### Comparing `meteva-1.7.3/meteva/base/tool/copy_tools.py` & `meteva-1.7.4/meteva/base/tool/copy_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/frprmn2.py` & `meteva-1.7.4/meteva/base/tool/frprmn2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/grib_tools.py` & `meteva-1.7.4/meteva/base/tool/grib_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/maskout.py` & `meteva-1.7.4/meteva/base/tool/maskout.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/math_tools.py` & `meteva-1.7.4/meteva/base/tool/math_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/path_tools.py` & `meteva-1.7.4/meteva/base/tool/path_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/plot_tools.py` & `meteva-1.7.4/meteva/base/tool/plot_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,16 +358,25 @@
     else:
         width_all_plot = width - width_colorbar - width_left_yticks - (ncol - 1) * width_wspace
         width_map = width_all_plot / ncol
         height_map = width_map * rlat / rlon
         height_all_plot = height_map * nrow + (nrow-1) * height_hspace
         height = height_all_plot + height_title + height_bottem_xticsk
 
+    if clevs is None and vmin is None and vmax is None:
+        vmax = -1e30
+        vmin = 1e30
+        for grd in grd_list:
+            vmax1 = np.max(grd.values)
+            if vmax < vmax1:
+                vmax = vmax1
+            vmin1 = np.min(grd.values)
+            if vmin > vmin1:
+                vmin = vmin1
     cmap1, clevs1 = meteva.base.tool.color_tools.def_cmap_clevs(cmap=cmap, clevs=clevs, vmin=vmin, vmax=vmax)
-    #print(clevs1)
     norm = BoundaryNorm(clevs1, ncolors=cmap1.N-1)
 
     vmax = elon
     vmin = slon
     r = rlon
     if r <= 1:
         inte = 0.1
@@ -794,14 +803,16 @@
 
     cmap1,clevs1 = meteva.base.tool.color_tools.def_cmap_clevs(cmap=cmap,clevs=clevs,vmin=vmin_v,vmax = vmax_v)
     #clevs1, cmap1 = meteva.base.tool.color_tools.def_cmap_clevs(clevs=clevs, cmap=cmap, vmin = None, vmax=None)
     #meteva.base.tool.color_tools.show_cmap_clev(cmap1,clevs1)
 
     norm = BoundaryNorm(clevs1, ncolors=cmap1.N-1)
 
+
+
     if point_size is None:
 
         sta_id1 = sta0.drop_duplicates(['id'])
         sta_dis = meteva.base.sta_dis_ensemble_near_by_sta(sta_id1,nearNum=2)
         dis_values = sta_dis["data1"].values
         dis_values.sort()
         dis1 = dis_values[int(len(dis_values) * 0.02) + 1]
@@ -871,15 +882,14 @@
 
 
     if subplot is None:
 
         split = ["level","time","dtime","member"]
         sta_list = meteva.base.split(sta0,used_coords=split)
         nplot = len(sta_list)
-
         #nplot = len(plot_data_names)
         if isinstance(title, list):
             if nplot != len(title):
                 print("手动设置的title数目和要绘制的图形数目不一致")
                 return
         if save_path is not None:
             if isinstance(save_path,str):
@@ -1418,16 +1428,16 @@
             ax_min.spines["top"].set_linewidth(0.3)
             ax_min.spines["bottom"].set_linewidth(0.3)
             ax_min.spines["right"].set_linewidth(0.3)
             ax_min.spines["left"].set_linewidth(0.3)
             add_china_map_2basemap(ax_min, name="world", edgecolor='k', lw=0.2, encoding='gbk', grid0=None)  # "国界"
             add_china_map_2basemap(ax_min, name="nation", edgecolor='k', lw=0.2, encoding='gbk', grid0=None)  # "省界"
 
-        if print_max >0 or print_min >0:
-            print(title1)
+        #if print_max >0 or print_min >0:
+        #    print(title1)
         if print_max > 0:
             print("取值最大的" + str(print_max) + "个站点：")
             indexs = value.argsort()[-print_max:][::-1]
             for index in indexs:
                 print("id:" + str(sta_one_member.iloc[index, 3]) + "   lon:" + str(
                     sta_one_member.iloc[index, 4]) + "  lat:" + str(sta_one_member.iloc[index, 5]) +
                       " value:" + str(sta_one_member.iloc[index, 6]))
@@ -4130,14 +4140,30 @@
             if show:
                 plt.show()
             plt.close()
             kk += 1
     return
 
 
+def barbs_grid_wind(grid_wind,width = None,height = None,sup_fontsize = 12,dpi = 300,skip = None,save_path = None,show = False):
+    grid1 = meteva.base.get_grid_of_data(grid_wind)
+    axs = meteva.base.creat_axs(1, map_extend=grid1, add_minmap=False, ncol=2, width=width,height=height,sup_fontsize=sup_fontsize,dpi=dpi)
+    meteva.base.add_barbs(axs[0], grid_wind,skip=skip)
+
+    if save_path is None:
+        show = True
+    else:
+        meteva.base.creat_path(save_path)
+        plt.savefig(save_path,bbox_inches='tight')
+        print("检验结果已以图片形式保存至" + save_path)
+    if show:
+        plt.show()
+    plt.close()
+
+
 def add_scatter(ax,map_extend,sta0,cmap = None,clevs = None,point_size = None,fix_size = True,title = None,threshold = 2,min_spot_value = 0,mean_value = 2,
                 grid = False,add_colorbar = True,alpha = None):
     sta = sta0
     if isinstance(map_extend, list):
         slon = map_extend[0]
         elon = map_extend[1]
         slat = map_extend[2]
```

### Comparing `meteva-1.7.3/meteva/base/tool/plot_tools_adv.py` & `meteva-1.7.4/meteva/base/tool/plot_tools_adv.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,14 @@
 
     vmax_v = np.max(sta_without_iv.iloc[:,-1].values)
     vmin_v = np.min(sta_without_iv.iloc[:,-1].values)
     clevs1 = None
     cmap1 = None
     if cmap is not None:
         cmap1, clevs1 = meteva.base.tool.color_tools.def_cmap_clevs(cmap=cmap, clevs=clevs, vmin=vmin_v, vmax=vmax_v)
-
     fig = plt.gcf()
     fmt_tag = "%." + str(tag) + "f"
 
     if cmap1 is None:
         nsta = len(sta_without_iv.index)
         for i in range(nsta):
             x = sta_without_iv.iloc[i,4]
@@ -564,15 +563,15 @@
             else:
                 ax.text(x, y, fmt_tag % v, ha="center", va="center",fontsize=font_size,color = color, clip_on=True,alpha = alpha, zorder=1000)
     else:
         x = sta_without_iv.iloc[:, 4].values
         y = sta_without_iv.iloc[:, 5].values
         v = sta_without_iv.iloc[:, -1].values
         for k in range(len(clevs1)-1):
-            index = np.where((v>clevs1[k])&(v<clevs1[k+1]))
+            index = np.where((v>=clevs1[k])&(v<clevs1[k+1]))
             if len(index[0])>0:
                 x1 = x[index]
                 y1 = y[index]
                 v1 = v[index]
                 color = cmap1(k)
                 for j in range(x1.size):
                     if isinstance(v1[j],str):
```

### Comparing `meteva-1.7.3/meteva/base/tool/process_tools.py` & `meteva-1.7.4/meteva/base/tool/process_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/station_tools.py` & `meteva-1.7.4/meteva/base/tool/station_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/base/tool/time_tools.py` & `meteva-1.7.4/meteva/base/tool/time_tools.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/Vector/__init__.py` & `meteva-1.7.4/meteva/method/Vector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import score
 from . import plot
 
-from .plot import  scatter_uv,scatter_uv_error,statisitic_uv
+from .plot import  scatter_uv,scatter_uv_error,statisitic_uv,probability_density_uv
 from .score import acd_nas,acs_nasws,acz_na,acs,acz,nas_d,nasws_s,na_ds,scd_nas,scd,scs,scs_nasws,acd
 from .score import wind_weaker_rate,wind_severer_rate,wind_severer_rate_nasws,wind_weaker_rate_nasws
 from .score import nasws_uv,na_uv,acd_uv,acs_uv,acz_uv,nas_uv,scd_uv,scs_uv,wind_severer_rate_uv,wind_weaker_rate_uv
 from .score import distance_tdis,distance,tdis
 from .score import tase_angle,tase_angle_uv,me_angle,me_angle_uv,mae_angle,mae_angle_uv,rmse_angle,rmse_angle_uv
```

### Comparing `meteva-1.7.3/meteva/method/Vector/plot.py` & `meteva-1.7.4/meteva/product/program/error_ana_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,548 +1,472 @@
+import numpy as np
 import matplotlib.pyplot as plt
-import os
+plt.rcParams['font.sans-serif']=['SimHei'] #用来正常显示中文标签\
+plt.rcParams['axes.unicode_minus']=False #用来正常显示负号
 import math
-import numpy as np
 import meteva
-from matplotlib.colors import BoundaryNorm
+import json
+
+def error_boxplot(sta_ob_and_fos0,s = None, g = None, gll=None,
+                  group_name_list=None,threshold = 2,save_dir=None,save_path = None,show = False,dpi = 200,title="误差综合分析图",
+                  vmin  = None,vmax = None,spasify_xticks = None,sup_fontsize =10,width = None,height = None,json_dir = None,json_path = None,
+                  **kwargs):
+    '''
 
+    :param sta_ob_and_fos0:
+    :param s:
+    :param g:
+    :param gll:
+    :param save_dir:
+    :param group_name_list:
+    :param threshold:
+    :param show:
+    :param title:
+    :return:
+    '''
+    if s is not None:
+        if g is not None:
+            if g == "last_range" or g == "last_step":
+                s["drop_last"] = False
+            else:
+                s["drop_last"] = True
 
-def scatter_uv_error(u_ob,u_fo,v_ob,v_fo,member_list = None,title = "风矢量误差散点分布图"
-              , vmax=None, ncol=None, save_path=None, show=False, dpi=300,
-               sup_fontsize=10, width=None, height=None):
-
-
-    if vmax is None:
-        du = u_fo - u_ob
-        dv = v_fo - v_ob
-        speed_d= np.sqrt(du * du + dv * dv)
-        vmax = np.max(speed_d)
-        vmax = math.ceil(vmax)
-
-    Fo_shape = u_fo.shape
-    Ob_shape = u_ob.shape
-    Ob_shpe_list = list(Ob_shape)
-    size = len(Ob_shpe_list)
-    ind = -size
-    Fo_Ob_index = list(Fo_shape[ind:])
-    if Fo_Ob_index != Ob_shpe_list:
-        print('预报数据和观测数据维度不匹配')
+
+    sta_ob_and_fos = meteva.base.sele_by_dict(sta_ob_and_fos0, s)
+    if(len(sta_ob_and_fos.index) == 0):
+        print("there is no data to verify")
         return
-    Ob_shpe_list.insert(0, -1)
-    new_Fo_shape = tuple(Ob_shpe_list)
-    new_u_Fo = u_fo.reshape(new_Fo_shape)
-    new_v_Fo = v_fo.reshape(new_Fo_shape)
-    new_Fo_shape = new_u_Fo.shape
-    sub_plot_num = new_Fo_shape[0]
-
-
-
-    height_title = sup_fontsize * 0.01
-    height_bottem_xticsk = sup_fontsize * 0.05
-    height_hspace = sup_fontsize * 0.07
-
-    width_wspace = height_hspace
-
-    width_colorbar = 0.5
-    width_left_yticks = sup_fontsize * 0.1
-
-
-    if ncol is None:
-        if sub_plot_num ==1:
-            ncol = 1
-        elif sub_plot_num %2 == 0:
-            ncol = 2
-        else:
-            ncol = 3
-
-    if title is None:
-        sup_height_title = 0
-    else:
-        sup_height_title = sup_fontsize * 0.12
-    nrow = math.ceil(new_Fo_shape[0] / ncol)
-    if width is None and height is None:
-        if sub_plot_num ==1:
-            width = 5
-        else:
-            width = 10
-
-
-    if width is None:
-        height_all_plot = height - height_title - height_bottem_xticsk - (nrow-1) * height_hspace + sup_height_title
-        height_axis = height_all_plot / nrow
-        width_axis = height_axis
-        width_all_plot = width_axis * ncol + (ncol-1) * width_wspace
-        width = width_all_plot + width_colorbar + width_left_yticks
-    else:
-        width_all_plot = width - width_colorbar - width_left_yticks - (ncol - 1) * width_wspace
-        width_axis = width_all_plot / ncol
-        height_axis = width_axis
-        height_all_plot = height_axis * nrow + (nrow-1) * height_hspace
-        height = height_all_plot + height_title + height_bottem_xticsk + sup_height_title
-
-
-    fig = plt.figure(figsize=(width, height), dpi=dpi)
-    plt.subplots_adjust(hspace = 0.3,wspace = 0.3)
-    u1 = u_ob.flatten()
-    v1 = v_ob.flatten()
-
-    if member_list is None:
-        member_list = []
-        for line in range(new_Fo_shape[0]):
-            member_list.append("预报" + str(line))
-
-    colors = meteva.base.color_tools.get_color_list(new_Fo_shape[0]+1)
-
-    for line in range(new_Fo_shape[0]):
-        pi = line % ncol
-        pj = int(line / ncol)
-        rect1 = [(width_left_yticks + pi * (width_axis + width_wspace))/width,
-                 (height_bottem_xticsk + (nrow -1- pj) * (height_axis + height_hspace))/height,
-                 width_axis / width,
-                 height_axis / height]
-        ax = plt.axes(rect1)
-
-        u2 = new_u_Fo[line, :].flatten()
-        v2 = new_v_Fo[line, :].flatten()
-
-
-        markersize = 5 * width_axis * height_axis / np.sqrt(u_ob.size)
-
-        if markersize < 1:
-            markersize = 1
-        elif markersize > 20:
-            markersize = 20
-        #plt.subplot(nrows, ncols, line + 1)
-
-
-        plt.plot(u2-u1,v2-v1,'.',color = colors[line+1], markersize=markersize)
-        #plt.plot(u1,v1,'.',color= 'b',  markersize=markersize)
-        plt.xlabel("U分量",fontsize = sup_fontsize *0.9)
-        plt.ylabel("V分量",fontsize = sup_fontsize *0.9)
-        plt.title(member_list[line],fontsize = sup_fontsize)
-
-        #print(maxs)
-        plt.xlim(-vmax,vmax)
-        plt.ylim(-vmax,vmax)
-        #plt.legend()
-        angles = np.arange(0,360,45)
-        for i in range(len(angles)):
-            angle = angles[i] * 3.1415926 /180
-            r = np.arange(0,vmax+1,vmax * 0.1)
-            x = r * np.sin(angle)
-            y = r * np.cos(angle)
-            plt.plot(x,y,"--",color = "k",linewidth = 0.5)
-
-        rs = np.arange(0,vmax+1,1)
-        for i in range(len(rs)):
-            r = rs[i]
-            angle = np.arange(0,360) * 3.1415926 /180
-            x = r * np.sin(angle)
-            y = r * np.cos(angle)
-            plt.plot(x,y,"--",color = "k",linewidth = 0.5)
-
-    y_sup_title = (height_bottem_xticsk + (nrow) * (height_axis + height_hspace)) / height
-    if title is not None:
-        plt.suptitle(title, y = y_sup_title,fontsize=sup_fontsize * 1.2)
-
-    if(save_path is not None):
-        file1,extension = os.path.splitext(save_path)
-        extension = extension[1:]
-        plt.savefig(save_path,format = extension)
-    else:
-        show = True
-    if show:
-        plt.show()
-    plt.close()
-
-
-def scatter_uv(u_ob,u_fo,v_ob,v_fo,member_list = None,title = "风矢量散点分布图"
-               , vmax=None, ncol=None, save_path=None, show=False, dpi=300,
-               sup_fontsize=10, width=None, height=None,add_randn_to_ob = 0.0):
-
-
-    if vmax is None:
-        speed_ob = np.sqrt(u_ob * u_ob + v_ob * v_ob)
-        speed_fo = np.sqrt(u_fo * u_fo + v_fo * v_fo)
-        vmax = max(np.max(speed_ob), np.max(speed_fo))
-        vmax = math.ceil(vmax)
-
-    Fo_shape = u_fo.shape
-    Ob_shape = u_ob.shape
-    Ob_shpe_list = list(Ob_shape)
-    size = len(Ob_shpe_list)
-    ind = -size
-    Fo_Ob_index = list(Fo_shape[ind:])
-    if Fo_Ob_index != Ob_shpe_list:
-        print('预报数据和观测数据维度不匹配')
+    sta_ob_and_fos_list, gll1 = meteva.base.fun.group(sta_ob_and_fos, g, gll)
+    data_names = meteva.base.get_stadata_names(sta_ob_and_fos_list[0])
+    if(len(data_names) ==1):
+        print("error infomation: only one data column, can't caculate error")
         return
-    Ob_shpe_list.insert(0, -1)
-    new_Fo_shape = tuple(Ob_shpe_list)
-    new_u_Fo = u_fo.reshape(new_Fo_shape)
-    new_v_Fo = v_fo.reshape(new_Fo_shape)
-    new_Fo_shape = new_u_Fo.shape
-    sub_plot_num = new_Fo_shape[0]
-
-    height_title = sup_fontsize * 0.01
-    height_bottem_xticsk = sup_fontsize * 0.05
-    height_hspace = sup_fontsize * 0.07
-
-    width_wspace = height_hspace
-
-    width_colorbar = 0.5
-    width_left_yticks = sup_fontsize * 0.1
-
-
-    if ncol is None:
-        if sub_plot_num ==1:
-            ncol = 1
-        elif sub_plot_num %2 == 0:
-            ncol = 2
-        else:
-            ncol = 3
-
-
-    if title is None:
-        sup_height_title = 0
-    else:
-        sup_height_title = sup_fontsize * 0.12
-    nrow = math.ceil(new_Fo_shape[0] / ncol)
-    if width is None and height is None:
-        if sub_plot_num ==1:
-            width = 5
-        else:
-            width = 10
-
-
-    if width is None:
-        height_all_plot = height - height_title - height_bottem_xticsk - (nrow-1) * height_hspace + sup_height_title
-        height_axis = height_all_plot / nrow
-        width_axis = height_axis
-        width_all_plot = width_axis * ncol + (ncol-1) * width_wspace
-        width = width_all_plot + width_colorbar + width_left_yticks
-    else:
-        width_all_plot = width - width_colorbar - width_left_yticks - (ncol - 1) * width_wspace
-        width_axis = width_all_plot / ncol
-        height_axis = width_axis
-        height_all_plot = height_axis * nrow + (nrow-1) * height_hspace
-        height = height_all_plot + height_title + height_bottem_xticsk + sup_height_title
-
-
-    u1 = u_ob.flatten() + np.random.randn(len(u_ob))*add_randn_to_ob
-    v1 = v_ob.flatten() + np.random.randn(len(v_ob))*add_randn_to_ob
-
-    if member_list is None:
-        member_list = []
-        for line in range(new_Fo_shape[0]):
-            member_list.append("预报" + str(line))
-
-
-
-    fig = plt.figure(figsize=(width, height), dpi=dpi)
-    colors = meteva.base.color_tools.get_color_list(new_Fo_shape[0]+1)
-
-    for line in range(new_Fo_shape[0]):
-        pi = line % ncol
-        pj = int(line / ncol)
-        rect1 = [(width_left_yticks + pi * (width_axis + width_wspace))/width,
-                 (height_bottem_xticsk + (nrow -1- pj) * (height_axis + height_hspace))/height,
-                 width_axis / width,
-                 height_axis / height]
-        ax = plt.axes(rect1)
-        u2 = new_u_Fo[line, :].flatten()
-        v2 = new_v_Fo[line, :].flatten()
-        markersize = 15 * width_axis * height_axis / np.sqrt(u_ob.size)
-        if markersize < 1:
-            markersize = 1
-        elif markersize > 20:
-            markersize = 20
-        #plt.subplot(nrow, ncols, line + 1)
-        plt.plot(u1,v1,'.',color= "r", markeredgewidth = 0, markersize=markersize,alpha = 0.5,label = "OBS")
-        plt.plot(u2,v2,'.',color= "b", markeredgewidth = 0,  markersize=markersize,alpha = 0.5,label = "FCT")
-
-        plt.xlabel("U分量",fontsize = sup_fontsize *0.9)
-        plt.ylabel("V分量",fontsize = sup_fontsize *0.9)
-        plt.title(member_list[line],fontsize = sup_fontsize)
-
-
-        plt.xlim(-vmax,vmax)
-        plt.ylim(-vmax,vmax)
-        plt.legend(loc = 2,fontsize = sup_fontsize * 0.7)
-        angles = np.arange(0,360,45)
-        for i in range(len(angles)):
-            angle = angles[i] * 3.1415926 /180
-            r = np.arange(0,vmax+1,vmax * 0.1)
-            x = r * np.sin(angle)
-            y = r * np.cos(angle)
-            plt.plot(x,y,"--",color = "k",linewidth = 0.5)
-
-        rs = np.arange(0,vmax+1,1)
-        for i in range(len(rs)):
-            r = rs[i]
-            angle = np.arange(0,360) * 3.1415926 /180
-            x = r * np.sin(angle)
-            y = r * np.cos(angle)
-            plt.plot(x,y,"--",color = "k",linewidth = 0.5)
-        plt.xticks(fontsize = 0.8 * sup_fontsize)
-        plt.yticks(fontsize = 0.8 * sup_fontsize)
-
-    y_sup_title = (height_bottem_xticsk + (nrow) * (height_axis + height_hspace)) / height
-    if title is not None:
-        plt.suptitle(title, y = y_sup_title,fontsize=sup_fontsize * 1.2)
-
-    if(save_path is not None):
-        file1,extension = os.path.splitext(save_path)
-        extension = extension[1:]
-        plt.savefig(save_path,format = extension)
-    else:
-        show = True
-    if show:
-        plt.show()
-    plt.close()
 
+    if isinstance(title, list):
+        if len(data_names) -1 != len(title):
+            print("手动设置的title数目和要绘制的图形数目不一致")
+            return
+
+
+
+    if save_path is not None:
+        if isinstance(save_path,str):
+            save_path = [save_path]
+        if len(data_names) -1 != len(save_path):
+            print("手动设置的save_path数目和要绘制的图形数目不一致")
+            return
+
+    if json_path is not None:
+        if isinstance(json_path,str):
+            json_path = [json_path]
+        if len(data_names) -1 != len(json_path):
+            print("手动设置的json_path数目和要绘制的图形数目不一致")
+            return
+
+    if group_name_list is None:
+        group_name_list = meteva.product.program.get_group_name(gll1)
+
+    for v in range(len(data_names)-1):
+        combineData = []
+        boxgroup = []
+        right_rate = []
+        tcount = []
+        me_list = []
+        mae_list = []
+        rmse_list = []
+        max_list = []
+        min_list = []
+        if gll1 is None:
+            gll1 = [[0]]
+        picture_ele_dict = {}
+        picture_ele_dict["box_data"] ={}
+
+        for i in range(len(gll1)):
+            dat = sta_ob_and_fos_list[i].values[:, 7+v] - sta_ob_and_fos_list[i].values[:, 6]
+            #picture_ele_dict["box_data"][i] = dat.tolist()
+            if vmax is None:
+                max_list.append(np.max(dat))
+            if vmin is None:
+                min_list.append(np.min(dat))
+            me_list.append(np.mean(dat))
+            mae_list.append(np.mean(np.abs(dat)))
+            rmse_list.append(np.sqrt(np.mean(np.power(dat,2))))
+            tt = len(dat)
+            index = np.where((dat <= threshold) & (dat >= -threshold))
+            rcount = len(index[0])
+            right_rate.append(rcount / tt)
+            tcount.append(tt)
+            combineData.append(dat)
+            bg = np.ones(tt) * i
+            boxgroup.append(bg)
+
+
+        picture_ele_dict["me"] = me_list
+        picture_ele_dict["mae"] = mae_list
+        picture_ele_dict["rmse"] = rmse_list
+        picture_ele_dict["correct_rate"] = right_rate
+        picture_ele_dict["sample_count"] = tcount
+        picture_ele_dict["xticklabels"] = group_name_list
 
-def uv_frequent_statistic(u,v,ngrade = 16,half_span = 22.5,rate = 20,smtime = 50):
-    '''
+        right_rate = np.array(right_rate)
+        tcount = np.array(tcount)
 
-    :param u: 输入的u分量列表
-    :param v: 输入的v分量列表
-    :param ngrade:  统计的时候对360度均匀分布的ngrade个不同角度进行统计
-    :param half_span:  统计的角度范围，围绕一个中心角度两侧的扇形角度
-    :param rate:  将统计结果加密成连续变化的结果，加密的比例，
-    :param smtime:  对一圈统计结果进行平滑的次数
-    :return:
-    '''
-    s1,a1 = meteva.base.tool.math_tools.u_v_to_s_d(u,v)
 
-    step = 360 / ngrade
-    ms1 = np.zeros(ngrade)
-    ma1 = np.zeros(ngrade)
-    mf1 = np.zeros(ngrade)
-    mstd1 = np.zeros(ngrade)
-    for i in range(ngrade):
-
-        mid_angle = i * step
-        d_angle = 180 - np.abs(np.abs(a1 - mid_angle) - 180)
-        s2 = s1[d_angle<=half_span]
-        if s2.size == 0:
-            ms1[i] = 0
-            mf1[i] = 0
-            ma1[i] = 0
-            mstd1[i] = 0.5
-        else:
-            ms1[i] = np.mean(s2)
-            mf1[i] = len(s2)
-            ma1[i] = mid_angle
-            mstd1[i] = np.std(s2)
-
-    mu1,mv1 = meteva.base.math_tools.s_d_to_u_v(ms1,ma1)
-
-    ngrade2 = ngrade * rate
-    x = np.arange(ngrade2)/ rate
-    ig = x.astype(dtype='int16')
-    dx = x - ig
-    ig1 = ig + 1
-    ii = ig % ngrade
-    ii1 = ig1 % ngrade
-    mu2 = mu1[ii] * (1-dx) + mu1[ii1] * dx
-    mv2 = mv1[ii] * (1-dx) + mv1[ii1] * dx
-    mf2 = mf1[ii] * (1-dx) + mf1[ii1] * dx
-    mstd2 = mstd1[ii] * (1-dx) + mstd1[ii1] * dx
-
-
-    ig = np.arange(ngrade2)
-    ig1 = (ig + 1) % ngrade2
-    ig_1 = (ig + ngrade2 - 1) % ngrade2
-    for k in range(smtime):
-        mu2 = (mu2 * 2 + mu2[ig1] + mu2[ig_1])/4
-        mv2 = (mv2 * 2 + mv2[ig1] + mv2[ig_1]) / 4
-        mf2 = (mf2 * 2 + mf2[ig1] + mf2[ig_1]) / 4
-        mstd2 = (mstd2 * 2 + mstd2[ig1] + mstd2[ig_1]) / 4
-
-    mf2 = 10 * (360/half_span) * (mf2/u.size)
-    return mu2,mv2,mf2,mstd2
-
-def statisitic_uv(u_ob,u_fo,v_ob,v_fo,member_list = None,title = "风矢量分布统计图"
-               ,vmax=None, ncol=None, save_path=None, show=False, dpi=300,
-               sup_fontsize=10, width=None, height=None):
-
-
-    Fo_shape = u_fo.shape
-    Ob_shape = u_ob.shape
-    Ob_shpe_list = list(Ob_shape)
-    size = len(Ob_shpe_list)
-    ind = -size
-    Fo_Ob_index = list(Fo_shape[ind:])
-    if Fo_Ob_index != Ob_shpe_list:
-        print('预报数据和观测数据维度不匹配')
+        if vmin is None:
+            vmin1 = np.min(np.array(min_list))
+        else:
+            vmin1 = vmin
+        if vmax is None:
+            vmax1 = np.max(np.array(max_list))
+        else:
+            vmax1 = vmax
+        dmax = vmax1 - vmin1
+        if vmin is None:
+            if vmin1 < 0:
+                vmin1 = vmin1 - 0.1 * dmax
+        if vmax is None:
+            vmax1 = vmax1 + 0.2 * dmax
+
+        picture_ele_dict["vmin"] = vmin1
+        picture_ele_dict["vmax"] = vmax1
+
+
+
+        # 计算最大的横坐标字符串
+        #max_str_len = 5
+        #for k in range(1, len(group_name_list)):
+        #    index = group_name_list[k]
+        #    if not type(index) == str:
+        #        index = str(index)
+        #    indexs = index.split("\n")
+        #    for i in range(len(indexs)):
+        #        str1 = indexs[i]
+        #        if max_str_len < len(str1):
+        #            max_str_len = len(str1)
+
+        width_axis_labels = meteva.base.plot_tools.caculate_axis_width(group_name_list, sup_fontsize, 1)
+        width_wspace = 2
+        width_one_subplot = width_axis_labels + width_wspace
+        if width_one_subplot < 2: width_one_subplot = 2
+        if width is None:
+            width = max(4,min(width_one_subplot,8))
+
+        spasify = 1
+        if width_one_subplot > width:
+            spasify = int(math.ceil(width_axis_labels / (width - width_wspace)))
+        if spasify_xticks is not None:
+            xticks_font = sup_fontsize * 0.8 * spasify_xticks * (width - width_wspace) / (width_axis_labels)
+            spasify = spasify_xticks
+        else:
+            xticks_font = sup_fontsize * 0.8
+
+        x = np.arange(1, len(tcount) + 1)
+        xticks = x[::spasify]
+        xticks_labels = group_name_list[::spasify]
+
+        #if width is None:
+        #    width = 0.5 + (1 + max_str_len) * 0.06 * len(group_name_list)
+        #    if width < 4:width = 4
+        #    if width >8:width = 8
+
+        if height is None:
+            height = 4
+
+        fig = plt.figure(figsize=(width, height),dpi = dpi)
+
+        grid_plt = plt.GridSpec(6, 1, hspace=0)
+        plt.rcParams['xtick.direction'] = 'in'
+        plt.rcParams['ytick.direction'] = 'in'
+        ax1 = plt.subplot(grid_plt[0:5, 0])
+
+        bplot = ax1.boxplot(combineData, boxgroup, patch_artist=True, sym='.',**kwargs)
+        for i, item in enumerate(bplot["boxes"]):
+            item.set_facecolor("lightblue")
+        plt.subplots_adjust(left=0.5 / width, right=1 - 0.1 / width)
+        plt.ylabel("误差值", fontsize=sup_fontsize *0.9)
+        plt.yticks(fontsize = sup_fontsize * 0.8)
+        plt.plot(x,me_list,'g',label = '平均误差',zorder = 3)
+        plt.plot(x, mae_list, 'b', label='平均绝对误差',zorder = 3)
+        plt.plot(x, rmse_list, 'r', label='均方根误差',zorder = 3)
+        plt.hlines(0, 1, len(group_name_list), linewidth=1, color="k", linestyles="dashed")
+        plt.hlines(threshold, 1, len(group_name_list), linewidth=1, color="k", linestyles="dashed")
+        plt.hlines(-threshold, 1, len(group_name_list), linewidth=1, color="k", linestyles="dashed")
+        plt.ylim(vmin1,vmax1)
+        plt.legend(fontsize =sup_fontsize * 0.8,ncol = 3,loc = "upper center")
+
+
+        if isinstance(title,list):
+            title1 = title[v]
+        else:
+            title1 = meteva.product.program.get_title_from_dict(title, s, None, None,
+                                                                data_names[v + 1])
+
+        plt.title(title1, fontsize=14)
+
+        ax2 = plt.subplot(grid_plt[5, 0])
+        plt.rcParams['xtick.direction'] = 'in'
+        plt.rcParams['ytick.direction'] = 'in'
+        plt.bar(x, tcount,width=0.5,label = "样本数")
+        plt.legend(fontsize=sup_fontsize * 0.5, loc="upper left")
+        xlabel_1 = meteva.product.program.get_x_label(g)
+
+        plt.xlabel(xlabel_1, fontsize=sup_fontsize *0.9)
+        plt.xlim(0.5, len(tcount) + 0.5)
+        plt.ylim(0, np.max(tcount) * 1.5)
+
+
+        plt.xticks(xticks, xticks_labels,fontsize = xticks_font)
+        plt.yticks(fontsize=sup_fontsize *0.8)
+        plt.ylabel("样本数", fontsize=sup_fontsize * 0.9)
+        ax2 = ax2.twinx()
+        plt.plot(x, right_rate*100, "r",linestyle = "--", linewidth=1.5,label = "准确率")
+        plt.legend(fontsize=sup_fontsize * 0.5, loc="upper right")
+        plt.ylim(0, 100)
+        plt.yticks([0,25,50,75,100],fontsize=sup_fontsize *0.8)
+        plt.ylabel("准确率(%)", fontsize = sup_fontsize * 0.9)
+
+        save_path1 = None
+        if save_path is None:
+            if save_dir is None:
+                show = True
+            else:
+                save_path1 = save_dir + "/" + data_names[v + 1] + ".png"
+        else:
+            save_path1 = save_path[v]
+        if save_path1 is not None:
+            meteva.base.tool.path_tools.creat_path(save_path1)
+            plt.savefig(save_path1,bbox_inches='tight')
+            print("图片已保存至" + save_path1)
+        if show:
+            plt.show()
+        plt.close()
+
+
+        json_path1 = None
+        if json_path is None:
+            if json_dir is None:
+                pass
+            else:
+                json_path1 = json_dir + "/" + data_names[v + 1] + ".json"
+        else:
+            json_path1 = json_path[v]
+        if json_path1 is not None:
+            meteva.base.tool.path_tools.creat_path(json_path1)
+            file = open(json_path1, "w")
+            json.dump(picture_ele_dict, file)
+            print("have printed pictrue elements to " + json_path1)
+
+
+
+def error_boxplot_abs(sta_ob_and_fos0,s = None, g = None, gll=None,
+                  group_name_list=None,threshold = 2,save_dir=None,save_path = None,show = False,dpi = 200,title="绝对误差综合分析图",
+                    vmin = None, vmax = None, spasify_xticks = None, sup_fontsize = 10, width = None, height = None
+                      ,json_dir = None,json_path = None,**kwargs):
+
+    if s is not None:
+        if g is not None:
+            if g == "last_range" or g == "last_step":
+                s["drop_last"] = False
+            else:
+                s["drop_last"] = True
+
+    sta_ob_and_fos = meteva.base.sele_by_dict(sta_ob_and_fos0, s)
+    if(len(sta_ob_and_fos.index) == 0):
+        print("there is no data to verify")
         return
-    Ob_shpe_list.insert(0, -1)
-    new_Fo_shape = tuple(Ob_shpe_list)
-    new_u_Fo = u_fo.reshape(new_Fo_shape)
-    new_v_Fo = v_fo.reshape(new_Fo_shape)
-    new_Fo_shape = new_u_Fo.shape
-    sub_plot_num = new_Fo_shape[0]
-
-
-    height_title = sup_fontsize * 0.01
-    height_bottem_xticsk = sup_fontsize * 0.05
-    height_hspace = sup_fontsize * 0.07
-
-    width_wspace = height_hspace
-
-    width_colorbar = 1
-    width_left_yticks = sup_fontsize * 0.1
-
-
-    if ncol is None:
-        if sub_plot_num ==1:
-            ncol = 1
-        elif sub_plot_num %2 == 0:
-            ncol = 2
-        else:
-            ncol = 3
-
-    if title is None:
-        sup_height_title = 0
-    else:
-        sup_height_title = sup_fontsize * 0.12
-    nrow = math.ceil(new_Fo_shape[0] / ncol)
-    if width is None and height is None:
-        if sub_plot_num ==1:
-            width = 5
-        else:
-            width = 10
-
-
-    if width is None:
-        height_all_plot = height - height_title - height_bottem_xticsk - (nrow-1) * height_hspace + sup_height_title
-        height_axis = height_all_plot / nrow
-        width_axis = height_axis
-        width_all_plot = width_axis * ncol + (ncol-1) * width_wspace
-        width = width_all_plot + width_colorbar + width_left_yticks
-    else:
-        width_all_plot = width - width_colorbar - width_left_yticks - (ncol - 1) * width_wspace
-        width_axis = width_all_plot / ncol
-        height_axis = width_axis
-        height_all_plot = height_axis * nrow + (nrow-1) * height_hspace
-        height = height_all_plot + height_title + height_bottem_xticsk + sup_height_title
-
-
-    fig = plt.figure(figsize=(width, height), dpi=dpi)
-    #plt.subplots_adjust(hspace = 0.3,wspace = 0.30)
-    u1 = u_ob.flatten()
-    v1 = v_ob.flatten()
-
-
-    mu1,mv1,mf1,mstd1 = uv_frequent_statistic(u1,v1)
-    ms1,ma1 = meteva.base.math_tools.u_v_to_s_d(mu1,mv1)
-
-    gray1 = ms1/(ms1+mstd1)
-    cmap1, clevs1 = meteva.base.tool.color_tools.def_cmap_clevs(cmap="autumn", vmin=0.5, vmax=1)
-    norm1= BoundaryNorm(clevs1, ncolors=cmap1.N-1)
-
-    cmap2, clevs2= meteva.base.tool.color_tools.def_cmap_clevs(cmap="winter",  vmin=0.5, vmax=1)
-    norm2= BoundaryNorm(clevs2, ncolors=cmap1.N-1)
-
-    if member_list is None:
-        member_list = []
-        for line in range(new_Fo_shape[0]):
-            member_list.append("预报" + str(line))
-
-    ms_list = [ms1]
-    mu2_list = []
-    mv2_list = []
-    mf2_list = []
-    mgray2_list = []
-    for line in range(new_Fo_shape[0]):
-        u2 = new_u_Fo[line, :].flatten()
-        v2 = new_v_Fo[line, :].flatten()
-        mu2, mv2, mf2, mstd2 = uv_frequent_statistic(u2, v2)
-        ms2, ma2 = meteva.base.math_tools.u_v_to_s_d(mu2, mv2)
-        ms_list.append(ms2)
-        mu2_list.append(mu2)
-        mv2_list.append(mv2)
-        mf2_list.append(mf2)
-        gray2 = ms2 / (ms2 + mstd2)
-        mgray2_list.append(gray2)
-
-    if vmax is None:
-        vmax = np.max(np.array(ms_list)) * 1.2
-
-    ax_ob = None
-    ax_fo = None
-    for line in range(new_Fo_shape[0]):
-        print(member_list[line])
-        pi = line % ncol
-        pj = int(line / ncol)
-        rect1 = [(width_left_yticks + pi * (width_axis + width_wspace))/width,
-                 (height_bottem_xticsk + (nrow -1- pj) * (height_axis + height_hspace))/height,
-                 width_axis / width,
-                 height_axis / height]
-        ax = plt.axes(rect1)
-
-        ax_ob = plt.scatter(mu1, mv1, c=gray1,s = mf1,cmap = cmap1,norm=norm1)
-        ax_fo = plt.scatter(mu2_list[line], mv2_list[line], c=mgray2_list[line],s = mf2_list[line],cmap = cmap2,norm = norm2)
-
-        plt.xlabel("U分量",fontsize = sup_fontsize *0.9)
-        plt.ylabel("V分量",fontsize = sup_fontsize *0.9)
-        plt.title(member_list[line],fontsize = sup_fontsize)
-
-        #print(maxs)
-        plt.xlim(-vmax,vmax)
-        plt.ylim(-vmax,vmax)
-        #plt.legend()
-        angles = np.arange(0,360,45)
-        for i in range(len(angles)):
-            angle = angles[i] * 3.1415926 /180
-            r = np.arange(0,vmax+1,vmax * 0.1)
-            x = r * np.sin(angle)
-            y = r * np.cos(angle)
-            plt.plot(x,y,"--",color = "k",linewidth = 0.5)
-
-        rs = np.arange(0,vmax+1,1)
-        for i in range(len(rs)):
-            r = rs[i]
-            angle = np.arange(0,360) * 3.1415926 /180
-            x = r * np.sin(angle)
-            y = r * np.cos(angle)
-            plt.plot(x,y,"--",color = "k",linewidth = 0.5)
-
-
-    left_low = (width_left_yticks + ncol * width_axis  + (ncol-1)*width_wspace+0.1)/width
-    #print(left_low)
-    colorbar_position_grid = fig.add_axes([left_low, height_bottem_xticsk / height,0.02, 0.455*height_all_plot/height])  # 位置[左,下,宽,高]
-
-
-
-    #colorbar_position_grid = fig.add_axes([0.92, 0.50, 0.02, 0.32])  # 位置[左,下,宽,高]
-    colorbar_ob = plt.colorbar(ax_ob, cax=colorbar_position_grid)
-    colorbar_ob.ax.tick_params(labelsize=sup_fontsize * 0.5)  # 改变bar标签字体大小
-
-    colorbar_ob.set_label('观测风速的一致性',fontsize = sup_fontsize * 0.7)
-    #colorbar_position_grid = fig.add_axes([0.92, 0.15, 0.02, 0.32])  # 位置[左,下,宽,高]
-    colorbar_position_grid = fig.add_axes([left_low, (height_bottem_xticsk+0.545 * height_all_plot) / height,
-                                           0.02, 0.455*height_all_plot/height])  # 位置[左,下,宽,高]
-
-
-    colorbar_fo = plt.colorbar(ax_fo, cax=colorbar_position_grid)
-    colorbar_fo.ax.tick_params(labelsize=sup_fontsize * 0.5)  # 改变bar标签字体大小
-    colorbar_fo.set_label('预报风速的一致性',fontsize = sup_fontsize * 0.7)
-    y_sup_title = (height_bottem_xticsk + (nrow) * (height_axis + height_hspace)) / height
-    if title is not None:
-        plt.suptitle(title, y = y_sup_title,fontsize=sup_fontsize * 1.2)
-    if(save_path is not None):
-        file1,extension = os.path.splitext(save_path)
-        extension = extension[1:]
-        plt.savefig(save_path,format = extension)
-    else:
-        show = True
-    if show:
-        plt.show()
-    plt.close()
+    data_names = meteva.base.get_stadata_names(sta_ob_and_fos)
+    if(len(data_names) ==1):
+        print("error infomation: only one data column, can't caculate error")
+        return
+
+    if save_path is not None:
+        if isinstance(save_path,str):
+            save_path = [save_path]
+        if len(data_names) -1 != len(save_path):
+            print("手动设置的save_path数目和要绘制的图形数目不一致")
+            return
+
+    if isinstance(title, list):
+        if len(data_names) -1 != len(title):
+            print("手动设置的title数目和要绘制的图形数目不一致")
+            return
+
+    if json_path is not None:
+        if isinstance(json_path,str):
+            json_path = [json_path]
+        if len(data_names) -1 != len(json_path):
+            print("手动设置的json_path数目和要绘制的图形数目不一致")
+            return
+
+    sta_ob_and_fos_list, gll1 = meteva.base.fun.group(sta_ob_and_fos, g, gll)
+    if group_name_list is None:
+        group_name_list = meteva.product.program.get_group_name(gll1)
+    if gll1 is None:
+        gll1 = [[0]]
+    for v in range(len(data_names)-1):
+        combineData = []
+        boxgroup = []
+        right_rate = []
+        tcount = []
+        maxlist = []
+
+        me_list = []
+        mae_list = []
+        rmse_list = []
+        max_list = []
+
+        picture_ele_dict = {}
+        picture_ele_dict["box_data"] ={}
+
+        for i in range(len(gll1)):
+            dat = sta_ob_and_fos_list[i].values[:, 7+v] - sta_ob_and_fos_list[i].values[:, 6]
+            me_list.append(np.mean(dat))
+            dat = np.abs(dat)
+            if vmax is None:
+                max_list.append(np.max(dat))
+            mae_list.append(np.mean(dat))
+            rmse_list.append(np.sqrt(np.mean(dat * dat)))
+
+            maxlist.append(np.max(dat))
+            tt = len(dat)
+            index = np.where(dat <= threshold)
+            rcount = len(index[0])
+            right_rate.append(rcount / tt)
+            tcount.append(tt)
+            combineData.append(dat)
+            bg = np.ones(tt) * i
+            boxgroup.append(bg)
+        right_rate = np.array(right_rate)
+        tcount = np.array(tcount)
+        maxarray = np.array(maxlist)
+        maxerror = np.max(maxarray)
+
+        picture_ele_dict["me"] = me_list
+        picture_ele_dict["mae"] = mae_list
+        picture_ele_dict["rmse"] = rmse_list
+        picture_ele_dict["correct_rate"] = right_rate
+        picture_ele_dict["sample_count"] = tcount
+        picture_ele_dict["xticklabels"] = group_name_list
+
+        if vmin is None:
+            vmin1 = np.min(np.array(me_list))
+        else:
+            vmin1 = vmin
+        if vmax is None:
+            vmax1 = np.max(np.array(max_list))
+        else:
+            vmax1 = vmax
+        dmax = vmax1 - vmin1
+        if vmin is None:
+            if vmin1 < 0:
+                vmin1 = vmin1 - 0.1 * dmax
+        if vmax is None:
+            vmax1 = vmax1 + 0.2 * dmax
+
+        picture_ele_dict["vmin"] = vmin1
+        picture_ele_dict["vmax"] = vmax1
 
 
-def frequent_distribution_uv():
-    pass
 
-def regress_uv():
-    pass
+        # 计算最大的横坐标字符串
+        width_axis_labels = meteva.base.plot_tools.caculate_axis_width(group_name_list, sup_fontsize, 1)
+        width_wspace = 2
+        width_one_subplot = width_axis_labels + width_wspace
+        if width_one_subplot < 2: width_one_subplot = 2
+        if width is None:
+            width = max(4,min(width_one_subplot,8))
+
+        spasify = 1
+        if width_one_subplot > width:
+            spasify = int(math.ceil(width_axis_labels / (width - width_wspace)))
+        if spasify_xticks is not None:
+            xticks_font = sup_fontsize * 0.8 * spasify_xticks / spasify
+            spasify = spasify_xticks
+        else:
+            xticks_font = sup_fontsize * 0.8
+
+
+        x = np.arange(1, len(tcount) + 1)
+        xticks = x[::spasify]
+        xticks_labels = group_name_list[::spasify]
+        if height is None:
+            height = 4
+
+        fig = plt.figure(figsize=(width, height),dpi = dpi)
+        grid_plt = plt.GridSpec(5, 1, hspace=0)
+        x = np.arange(1, len(tcount) + 1)
+        plt.rcParams['xtick.direction'] = 'in'
+        plt.rcParams['ytick.direction'] = 'in'
+        ax1 = plt.subplot(grid_plt[0:4, 0])
+        bplot = ax1.boxplot(combineData, boxgroup,  patch_artist=True, sym='.',**kwargs)
+        for i, item in enumerate(bplot["boxes"]):
+            item.set_facecolor("lightblue")
+        plt.subplots_adjust(left=0.5 / width, right=1 - 0.1 / width)
+        plt.ylabel("误差绝对值", fontsize=sup_fontsize *0.9)
+
+        plt.yticks(fontsize=sup_fontsize * 0.8)
+        plt.ylim(vmin1,vmax1)
+        plt.plot(x,me_list,'g',label = '平均误差',zorder = 3)
+        plt.plot(x, mae_list, 'b', label='平均绝对误差',zorder = 3)
+        plt.plot(x, rmse_list, 'r', label='均方根误差',zorder = 3)
+        plt.legend(fontsize=sup_fontsize * 0.8, ncol=3, loc="upper center")
+
+        if isinstance(title,list):
+            title1 = title[v]
+        else:
+            title1 = meteva.product.program.get_title_from_dict(title, s, None, None,
+                                                                data_names[v + 1])
+
+
+        plt.title(title1, fontsize=sup_fontsize)
+
+        plt.hlines(threshold, 1, len(group_name_list), linewidth=1, color="k", linestyles="dashed")
+        plt.hlines(0, 1, len(group_name_list), linewidth=1, color="k", linestyles="dashed")
+        ax2 = plt.subplot(grid_plt[4, 0])
+        plt.rcParams['xtick.direction'] = 'in'
+        plt.rcParams['ytick.direction'] = 'in'
+        plt.bar(x, tcount,width=0.5,label = "样本数")
+        plt.legend(fontsize=sup_fontsize * 0.5, loc="upper left")
+        xlabel_1 = meteva.product.program.get_x_label(g)
+        plt.xlabel(xlabel_1, fontsize=sup_fontsize *0.9)
+        plt.xlim(0.5, len(tcount) + 0.5)
+        plt.ylim(0, np.max(tcount) * 1.5)
+        plt.xticks(xticks, xticks_labels,fontsize = xticks_font)
+        plt.yticks(fontsize=sup_fontsize * 0.8)
+        plt.ylabel("样本数", fontsize=sup_fontsize * 0.9)
+        ax3 = ax2.twinx()
+        plt.plot(x, right_rate*100, "r",linestyle = "--", linewidth=1.5,label = "准确率")
+        plt.legend(fontsize=sup_fontsize * 0.5, loc="upper right")
+        plt.ylim(0, 100)
+        plt.yticks([0,25,50,75,100],fontsize=sup_fontsize *0.8)
+        plt.ylabel("准确率(%)", fontsize=sup_fontsize * 0.9)
+
+        save_path1 = None
+        if save_path is None:
+            if save_dir is None:
+                show = True
+            else:
+                save_path1 = save_dir + "/" + data_names[v + 1] + ".png"
+        else:
+            save_path1 = save_path[v]
+        if save_path1 is not None:
+            meteva.base.tool.path_tools.creat_path(save_path1)
+            plt.savefig(save_path1,bbox_inches='tight')
+            print("图片已保存至" + save_path1)
+        if show:
+            plt.show()
+        plt.close()
+
+
+        json_path1 = None
+        if json_path is None:
+            if json_dir is None:
+                pass
+            else:
+                json_path1 = json_dir + "/" + data_names[v + 1] + ".json"
+        else:
+            json_path1 = json_path[v]
+        if json_path1 is not None:
+            meteva.base.tool.path_tools.creat_path(json_path1)
+            file = open(json_path1, "w")
+            json.dump(picture_ele_dict, file)
+            print("have printed pictrue elements to " + json_path1)
```

### Comparing `meteva-1.7.3/meteva/method/Vector/score.py` & `meteva-1.7.4/meteva/method/Vector/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/continuous/__init__.py` & `meteva-1.7.4/meteva/method/continuous/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,12 +4,13 @@
 from . import plot
 from . import skill
 
 from .table import *
 from .plot import scatter_regress,pdf_plot,box_plot_continue,taylor_diagram,frequency_histogram_error,accumulation_change_with_strenght,frequency_change_with_strenght
 from .skill import mre_skill,sme,sst
 from .score import sample_count,ob_mean,fo_mean,tase,me,mae,mse,rmse,me_tase,mae_tase,mse_tase,rmse_tase,tc_count
-from .score import bias_m,bias_tmmsss,corr,corr_tmmsss,tmmsss,tmmsss_merge,toar,nse,nse_tase_tmmsss,mre,mre_toar,correct_rate,correct_rate_tc
+from .score import bias_m,bias_tmmsss,corr,corr_tmmsss,tmmsss,tmmsss_merge,toar,nse,nse_tase_tmmsss,nse_tmmsss,mre,mre_toar,correct_rate,correct_rate_tc
 from .score import ob_fo_mean,ob_fo_std,ob_fo_max,ob_fo_min,ob_fo_cv
 from .score import wrong_rate,wrong_rate_tc,residual_error,residual_error_tmmsss,residual_error_rate,residual_error_rate_tmmsss
 from .score import max_abs_error,max_error,min_error
-from .score import ob_fo_sum,rmsf,tlfo,corr_rank,rmsf_tlfo,ob_fo_quantile,ob_fo_precipitation_strenght
+from .score import ob_fo_sum,rmsf,tlfo,corr_rank,rmsf_tlfo,ob_fo_quantile,ob_fo_precipitation_strenght
+from .score import ob_fo_sum_tmmsss,ob_fo_mean_tmmsss
```

### Comparing `meteva-1.7.3/meteva/method/continuous/plot.py` & `meteva-1.7.4/meteva/method/continuous/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     plt.close()
     return None
 
 
 
 
 def pdf_plot(ob, fo,member_list = None,vmax = None,vmin = None, save_path=None,  show = False,dpi = 300,title="频率匹配检验图",
-             sup_fontsize = 10,width = None,height = None,yscale = None):
+             sup_fontsize = 10,width = None,height = None,yscale = None,grid = False):
     '''
     sorted_ob_fo 将传入的两组数据先进行排序
     然后画出折线图
     ----------------
     :param Ob: 实况数据  任意维numpy数组
     :param Fo: 预测数据 任意维numpy数组,Fo.shape 和Ob.shape一致
     :param save_path: 图片保存路径，缺省时不输出图片，而是以默认绘图窗口形式展示
@@ -286,15 +286,16 @@
 
     if yscale == "logit":
         minfnq = min(fnq)/ob_sorted_smooth.size
         plt.ylim(minfnq,1)
 
 
         #plt.yscale('logit')
-
+    if grid:
+        plt.grid()
 
     plt.subplot(1, 2, 2)
     ob_line = np.arange(num_min, num_max, dmm / 30)
     plt.plot(ob_line, ob_line, '--')
     for line in range(new_Fo_shape[0]):
         if member_list is None:
             if new_Fo_shape[0] == 1:
@@ -313,15 +314,16 @@
         plt.ylabel("观测", fontsize=0.9 * sup_fontsize)
         plt.title("频率匹配映射关系图", fontsize=0.9 * sup_fontsize)
         plt.legend(loc="lower right", fontsize=0.9 * sup_fontsize)
         plt.yticks(fontsize=0.8 * sup_fontsize)
         plt.xticks(fontsize=0.8 * sup_fontsize)
     if title is not None:
         plt.suptitle(title + "\n", y=1.00, fontsize=sup_fontsize)
-
+    if grid:
+        plt.grid()
     if save_path is None:
         show = True
     else:
         plt.savefig(save_path,bbox_inches='tight')
         print("检验结果已以图片形式保存至" + save_path)
     if show is True:
         plt.show()
@@ -927,15 +929,19 @@
                                     width = width,height = height,sup_fontsize= sup_fontsize,log_y = log_y)
 
 
 
 
 
 def accumulation_change_with_strenght(ob,fo,member_list = None,save_path=None,  show = False,dpi = 300,title="降水量随强度变化图",
-             sup_fontsize = 14,width = None,height = None,y_log = False):
+             sup_fontsize = 14,width = None,height = None,log_y = False,y_log = None,max_x = None):
+    if y_log is not None:
+        print(
+            "warning: the argument y_log will be abolished, please use log_y instead\n警告：为保持和其它函数的名称一致，参数log_y将被废除，以后请使用参数log_y代替")
+        log_y = y_log
 
     accu_stren = meteva.method.continuous.table.accumulation_strenght_table(ob,fo)
     min_not_zero = np.min(accu_stren[accu_stren>0])
     maxv = np.max(accu_stren)
     shape = accu_stren.shape
     grade = np.arange(1,shape[1]+1,1)
     nfo = shape[0]-1
@@ -954,26 +960,29 @@
         labels = ["观测"]
         labels.extend(member_list)
     for line in range(len(labels)):
         plt.plot(grade,accu_stren[line], label=labels[line],marker = ".")
         plt.xlabel("降水强度(毫米/小时)", fontsize=0.9 * sup_fontsize)
         plt.ylabel("累计降水量", fontsize=0.9 * sup_fontsize)
         plt.title(title, fontsize=0.9 * sup_fontsize)
-        if(y_log):
+        if(log_y):
             ax_one = plt.gca()
             for tick in ax_one.yaxis.get_major_ticks():
                 tick.label1.set_fontproperties('stixgeneral')
             plt.yscale('log')
         plt.xticks(fontsize=0.8 * sup_fontsize)
         plt.legend(loc="upper right")
 
 
 
     # 设置次刻度间隔
-    maxx = len(grade)
+    if max_x is not None:
+        maxx = max_x
+    else:
+        maxx = len(grade)
     if(maxx <20):
         xmi = 1
         Xmi = 1
     elif(maxx <50):
         xmi = 1
         Xmi = 5
     elif (maxx <100):
@@ -990,30 +999,35 @@
         Xmi = 200
     ax1 = plt.gca()
     xmajorLocator = mpl.ticker.MultipleLocator(Xmi)  # 将x主刻度标签设置为次刻度10倍
     ax1.xaxis.set_major_locator(xmajorLocator)
     xminorLocator = mpl.ticker.MultipleLocator(xmi)  # 将x轴次刻度标签设置xmi
     ax1.xaxis.set_minor_locator(xminorLocator)
     plt.xlim(0,maxx)
-    if y_log:
+    if log_y:
         plt.ylim(min_not_zero,maxv * 3)
     else:
         plt.ylim(0,maxv * 1.1)
     if save_path is None:
         show = True
     else:
         plt.savefig(save_path, bbox_inches='tight')
         print("检验结果已以图片形式保存至" + save_path)
     if show is True:
         plt.show()
     plt.close()
     return accu_stren
 
-def frequency_change_with_strenght(ob,fo,member_list = None,save_path=None,  show = False,dpi = 300,title="降水量随强度变化图",
-             sup_fontsize = 14,width = None,height = None,y_log = False):
+def frequency_change_with_strenght(ob,fo,member_list = None,save_path=None,  show = False,dpi = 300,title="降水频次随强度变化图",
+             sup_fontsize = 14,width = None,height = None,log_y = False,y_log = None,max_x = None):
+
+    if y_log is not None:
+        print(
+            "warning: the argument y_log will be abolished, please use log_y instead\n警告：为保持和其它函数的名称一致，参数log_y将被废除，以后请使用参数log_y代替")
+        log_y = y_log
 
     accu_stren = meteva.method.continuous.table.frequency_strenght_table(ob,fo)
     min_not_zero = np.min(accu_stren[accu_stren>0])
     maxv = np.max(accu_stren)
     shape = accu_stren.shape
     grade = np.arange(1,shape[1]+1,1)
     nfo = shape[0]-1
@@ -1032,26 +1046,29 @@
         labels = ["观测"]
         labels.extend(member_list)
     for line in range(len(labels)):
         plt.plot(grade,accu_stren[line], label=labels[line],marker = ".")
         plt.xlabel("降水强度(毫米/小时)", fontsize=0.9 * sup_fontsize)
         plt.ylabel("降水频次", fontsize=0.9 * sup_fontsize)
         plt.title(title, fontsize=0.9 * sup_fontsize)
-        if(y_log):
+        if(log_y):
             ax_one = plt.gca()
             for tick in ax_one.yaxis.get_major_ticks():
                 tick.label1.set_fontproperties('stixgeneral')
             plt.yscale('log')
         plt.xticks(fontsize=0.8 * sup_fontsize)
         plt.legend(loc="upper right")
 
 
 
     # 设置次刻度间隔
-    maxx = len(grade)
+    if max_x is not None:
+        maxx = max_x
+    else:
+        maxx = len(grade)
     if(maxx <20):
         xmi = 1
         Xmi = 1
     elif(maxx <50):
         xmi = 1
         Xmi = 5
     elif (maxx <100):
@@ -1068,15 +1085,15 @@
         Xmi = 200
     ax1 = plt.gca()
     xmajorLocator = mpl.ticker.MultipleLocator(Xmi)  # 将x主刻度标签设置为次刻度10倍
     ax1.xaxis.set_major_locator(xmajorLocator)
     xminorLocator = mpl.ticker.MultipleLocator(xmi)  # 将x轴次刻度标签设置xmi
     ax1.xaxis.set_minor_locator(xminorLocator)
     plt.xlim(0,maxx)
-    if y_log:
+    if log_y:
         plt.ylim(min_not_zero,maxv * 3)
     else:
         plt.ylim(0,maxv * 1.1)
     if save_path is None:
         show = True
     else:
         plt.savefig(save_path, bbox_inches='tight')
```

### Comparing `meteva-1.7.3/meteva/method/continuous/score.py` & `meteva-1.7.4/meteva/method/continuous/score.py`

 * *Files 4% similar despite different names*

```diff
@@ -1039,14 +1039,56 @@
         if sxxsyy == 0:
             sxxsyy = 1e-10
     else:
         sxxsyy[sxxsyy == 0] = 1e-10
     corr = sxy / sxxsyy
     return corr
 
+def ob_fo_sum_tmmsss(tmmsss_array):
+    '''
+    相关系数，求实况数据还和预测数据之间的相关系数
+    :param tmmsss_array: 包含命中空报和漏报的多维数组，其中最后一维长度为6，分别记录了（count,mx,my,sxx,syy,sxy）
+    :return:
+    '''
+    if len(tmmsss_array.shape) == 1:
+        tmmsss_array = tmmsss_array.reshape(1, 1, 6)
+    mx = tmmsss_array[..., 1]
+    my = tmmsss_array[..., 2]
+    shape1 = list(tmmsss_array.shape)
+    if len(tmmsss_array.shape) == 2:
+        result = np.zeros((2, shape1[0]))
+        result[0, :] = mx * tmmsss_array[..., 0]
+        result[1, :] = my * tmmsss_array[..., 0]
+    else:
+        result = np.zeros((1 + shape1[0], shape1[1]))
+        result[0, :] = mx * tmmsss_array[..., 0]
+        result[1:, :] = my * tmmsss_array[..., 0]
+    return result
+
+def ob_fo_mean_tmmsss(tmmsss_array):
+    '''
+    相关系数，求实况数据还和预测数据之间的相关系数
+    :param tmmsss_array: 包含命中空报和漏报的多维数组，其中最后一维长度为6，分别记录了（count,mx,my,sxx,syy,sxy）
+    :return:
+    '''
+
+    if len(tmmsss_array.shape) == 1:
+        tmmsss_array = tmmsss_array.reshape(1, 1, 6)
+    mx = tmmsss_array[..., 1]
+    my = tmmsss_array[..., 2]
+    shape1 = list(tmmsss_array.shape)
+    if len(tmmsss_array.shape) == 2:
+        result = np.zeros((2, shape1[0]))
+        result[0, :] = mx
+        result[1, :] = my
+    else:
+        result = np.zeros((1 + shape1[0], shape1[1]))
+        result[0, :] = mx
+        result[1:, :] = my
+    return result
 
 def tmmsss(Ob, Fo):
     '''
     统计相关系数等检验量所需的中间变量
     :param Ob: 实况数据  任意维numpy数组
     :param Fo: 预测数据 任意维numpy数组,Fo.shape 和Ob.shape一致
     :return: numpy 一维数组，其元素为根据Ob和Fo
@@ -1089,17 +1131,17 @@
 def tmmsss_merge(tmmsss0, tmmsss1):
     '''
     将两份包含样本数、平均值和方差、协方差的中间结果合并
     :param tmmsss0: 长度6的一维数组，分别记录了（count,mx,my,sxx,syy,sxy）
     :param tmmsss1: 长度6的一维数组，分别记录了（count,mx,my,sxx,syy,sxy）
     :return: 长度6的一维数组，分别记录了（count,mx,my,sxx,syy,sxy）
     '''
-    if np.isnan(tmmsss0[0]):
+    if np.isnan(tmmsss0[0]).any():
         return tmmsss1
-    elif np.isnan(tmmsss1[0]):
+    elif np.isnan(tmmsss1[0]).any():
         return tmmsss0
     tmmsss_array_list = []
     tmmsss0_shape = list(tmmsss0.shape)
     tmmsss1_shape = list(tmmsss1.shape)
     if tmmsss0_shape != tmmsss1_shape:
         print('tmmsss0和tmmsss1维度不匹配')
         return
@@ -1302,7 +1344,35 @@
         sum = sxx + 0
         sum[sxx == 0] = 1e-10
         mse0 = tase_array[..., 3] / tase_array[..., 0]
         nse0 = 1 - mse0 / sum
         nse0[sxx == 0] = IV
     return nse0
 
+def nse_tmmsss(tmmsss_array):
+    '''
+    :param tase_array:
+    :param tmmsss_array:
+    :return:
+    '''
+
+    sxx = tmmsss_array[..., 3] + 0
+    syy = tmmsss_array[..., 4] + 0
+    sxy = tmmsss_array[..., 5] + 0
+    mx = tmmsss_array[..., 1] + 0
+    my = tmmsss_array[..., 2] + 0
+    exy = sxx + syy - 2 * sxy + (mx - my) * (mx - my)
+
+
+
+    if sxx.size == 1:
+        if sxx == 0:
+            nse0 = IV
+        else:
+            nse0 = 1 - exy / sxx
+    else:
+        sum = sxx + 0
+        sum[sxx == 0] = 1e-10
+        mse0 = exy
+        nse0 = 1 - mse0 / sum
+        nse0[sxx == 0] = IV
+    return nse0
```

### Comparing `meteva-1.7.3/meteva/method/continuous/skill.py` & `meteva-1.7.4/meteva/method/continuous/skill.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/continuous/table.py` & `meteva-1.7.4/meteva/method/continuous/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/ensemble/plot.py` & `meteva-1.7.4/meteva/method/ensemble/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/ensemble/score.py` & `meteva-1.7.4/meteva/method/ensemble/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/multi_category/__init__.py` & `meteva-1.7.4/meteva/method/multi_category/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/multi_category/plot.py` & `meteva-1.7.4/meteva/method/multi_category/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/multi_category/score.py` & `meteva-1.7.4/meteva/method/multi_category/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/multi_category/table.py` & `meteva-1.7.4/meteva/method/multi_category/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/probability/plot.py` & `meteva-1.7.4/meteva/method/probability/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/probability/score.py` & `meteva-1.7.4/meteva/method/probability/score.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/probability/table.py` & `meteva-1.7.4/meteva/method/probability/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/fss/__init__.py` & `meteva-1.7.4/meteva/method/space/fss/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/fss/fss.py` & `meteva-1.7.4/meteva/method/space/fss/fss.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/__init__.py` & `meteva-1.7.4/meteva/method/space/mode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,9 +46,9 @@
 from .feature_comps import feature_comps
 from .feature_match_analyzer import  feature_merged_analyzer,get_summary
 from .plot import plot_value,plot_label,plot_value_and_label,plot_interest,plot_feature,plot_value_list,plot_label_list,plot_value_and_label_list
 from .utils import get_attributes_for_feat,remove_key_from_list
 from .interester import interester
 from .operater import operate
 from .load import load_feature_summary,load_feature_summary_list
-from .tran_to_dataframe import features_list_to_df,features_list_to_df_c
+from .tran_to_dataframe import features_list_to_df
 from .consistent import combined_near_labels,unimatch,unimerge
```

### Comparing `meteva-1.7.3/meteva/method/space/mode/bearing.py` & `meteva-1.7.4/meteva/method/space/mode/bearing.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/censqdelta.py` & `meteva-1.7.4/meteva/method/space/mode/censqdelta.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/centmatch.py` & `meteva-1.7.4/meteva/method/space/mode/centmatch.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/consistent.py` & `meteva-1.7.4/meteva/method/space/mode/consistent.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/data_pre.py` & `meteva-1.7.4/meteva/method/space/mode/data_pre.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/deltametric.py` & `meteva-1.7.4/meteva/method/space/mode/deltametric.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/deltamm.py` & `meteva-1.7.4/meteva/method/space/mode/deltamm.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/deltammSqCen.py` & `meteva-1.7.4/meteva/method/space/mode/deltammSqCen.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/deltamm_bak.py` & `meteva-1.7.4/meteva/method/space/mode/deltamm_bak.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/distmap.py` & `meteva-1.7.4/meteva/method/space/mode/distmap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/feature_axis.py` & `meteva-1.7.4/meteva/method/space/mode/feature_axis.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/feature_comps.py` & `meteva-1.7.4/meteva/method/space/mode/feature_comps.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/feature_finder.py` & `meteva-1.7.4/meteva/method/space/mode/feature_finder.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/feature_match_analyzer.py` & `meteva-1.7.4/meteva/method/space/mode/feature_match_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     return out
 
 def feature_merged_analyzer(look_merge,summary =True):
     nmatch = look_merge["match_count"]
     out = {}
     out["time"] = meteva.base.all_type_time_to_str(look_merge["grd_fo"]["time"].values[0])
     out["dtime"] = int(look_merge["grd_fo"]["dtime"].values[0])
+    out["member"] = look_merge["grd_fo"]["member"].values[0]
     out["match_count"] = nmatch
     f_table = feature_table(look_merge)
     out["feature_table"] = f_table
     interest = interester(look_merge)
     out["interester"] = interest
 
     label_list_matched = look_merge["label_list_matched"]
```

### Comparing `meteva-1.7.3/meteva/method/space/mode/feature_props.py` & `meteva-1.7.4/meteva/method/space/mode/feature_props.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/feature_table.py` & `meteva-1.7.4/meteva/method/space/mode/feature_table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/interester.py` & `meteva-1.7.4/meteva/method/space/mode/interester.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/intersect.py` & `meteva-1.7.4/meteva/method/space/mode/intersect.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/load.py` & `meteva-1.7.4/meteva/method/space/mode/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     strs = file.read()
     feature = json.loads(strs)
     file.close()
     feature1 = {}
     feature1["match_count"] = feature["match_count"]
     feature1["time"] = feature["time"]
     feature1["dtime"] = feature["dtime"]
+    feature1["member"] = feature["member"]
     feature1["feature_table"] = feature["feature_table"]
     feature1["interester"] = feature["interester"]
 
 
     label_list_matched = feature["label_list_matched"]
     feature1["label_list_matched"] = label_list_matched
     for id in label_list_matched:
```

### Comparing `meteva-1.7.3/meteva/method/space/mode/loc_list_setup.py` & `meteva-1.7.4/meteva/method/space/mode/loc_list_setup.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/locperf.py` & `meteva-1.7.4/meteva/method/space/mode/locperf.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/make_SpatialVx_bak.py` & `meteva-1.7.4/meteva/method/space/mode/make_SpatialVx_bak.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/make_spatialVx.py` & `meteva-1.7.4/meteva/method/space/mode/make_spatialVx.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/merge_force.py` & `meteva-1.7.4/meteva/method/space/mode/merge_force.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/minboundmatch.py` & `meteva-1.7.4/meteva/method/space/mode/minboundmatch.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/operater.py` & `meteva-1.7.4/meteva/method/space/mode/operater.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         look_ob = feature_finder_and_merge(grd_ob,smooth[0],threshold[0],minsize[0],compare = compare,near_dis=near_dis[0],
                                            near_rate = near_rate[0])
         look_fo = feature_finder_and_merge(grd_fo, smooth[1], threshold[1], minsize[1], compare=compare,
                                            near_dis=near_dis[1],
                                            near_rate=near_rate[1])
         matched_fo = unimatch(look_ob,look_fo,cover_dis,cover_rate)
         look_merge = unimerge(look_ob,matched_fo)
-
     else:
         look_ff = feature_finder(grd_ob,grd_fo,smooth=smooth,threshold=threshold,minsize=minsize,compare=compare)
         loof_match = match_method(look_ff)
         look_merge = merge_force(loof_match)
     features = feature_merged_analyzer(look_merge,summary=summary)
     time1 = meteva.base.all_type_time_to_datetime(grd_fo["time"].values[0])
     dtime1 = grd_fo["dtime"].values[0]
```

### Comparing `meteva-1.7.3/meteva/method/space/mode/plot.py` & `meteva-1.7.4/meteva/method/space/mode/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/regress2.py` & `meteva-1.7.4/meteva/method/space/mode/regress2.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/sma.py` & `meteva-1.7.4/meteva/method/space/mode/sma.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/mode/tran_to_dataframe.py` & `meteva-1.7.4/meteva/method/space/mode/tran_to_dataframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 import pandas as pd
 import meteva
 
 def features_tran(features):
+    if "member" not in features.keys():
+        print("警告：输入的检验属性数据中没有包含预报名称，请使用升级1.7.5版本以上MetEva重新运行MODE方法输出检验结果后，再检验数据载入和分析")
+        return None,None
     try:
         time1 = meteva.base.all_type_time_to_time64(features["time"])
         tabel = features["feature_table"]["contingency_table_yesorno"]
+
+            # hmfc = pd.DataFrame({
+            #     "level":[0],"time":[time1],"dtime":[features["dtime"]],"id":[meteva.base.IV],
+            #     "lon":[meteva.base.IV],"lat":[meteva.base.IV],
+            #     "H":[tabel["Hits"]],
+            #     "F":[tabel["False alarms"]],
+            #     "M":[tabel["Misses"]],
+            #     "C":[tabel["Correct negatives"]]
+            # })
+        #升级后删除了id，lon，lat列，增加了member列，方便调用透视分析模块
         hmfc = pd.DataFrame({
-            "level":[0],"time":[time1],"dtime":[features["dtime"]],"id":[meteva.base.IV],
-            "lon":[meteva.base.IV],"lat":[meteva.base.IV],
+            "level":[0],"time":[time1],"dtime":[features["dtime"]],"member":[features["member"]],
             "H":[tabel["Hits"]],
             "F":[tabel["False alarms"]],
             "M":[tabel["Misses"]],
             "C":[tabel["Correct negatives"]]
         })
         hmfc = hmfc.sort_values(by = ["level","time","dtime"])
         nmatch = features["match_count"]
@@ -143,15 +155,15 @@
             df = None
         return  df
     except:
         print("将以下检验概要信息转换成DataFrame失败")
         print(features)
 
 
-def features_list_to_df(feature_list):
+def features_list_to_df_old(feature_list):
     hit_list = []
     hmfc_list = []
     for i in range(len(feature_list)):
         features = feature_list[i]
         hmfc,hit = features_tran(features)
         if hmfc is not None and hit is not None:
             hit_list.append(hit)
@@ -164,22 +176,24 @@
         hmfc_all = hmfc_all.reset_index(drop=True)
         return hmfc_all,df_hit
     else:
         return None,None
 
 
 
-def features_list_to_df_c(feature_list):
+def features_list_to_df(feature_list):
     hit_list = []
     hmfc_list = []
     mis_list = []
     fal_list = []
     for i in range(len(feature_list)):
         features = feature_list[i]
         hmfc,hit = features_tran(features)
+        if hmfc is None:
+            return None,None,None,None
         mis = features_tran_miss(features)
         fal = features_tran_false_alarm(features)
         hit_list.append(hit)
         hmfc_list.append(hmfc)
         mis_list.append(mis)
         fal_list.append(fal)
```

### Comparing `meteva-1.7.3/meteva/method/space/mode/utils.py` & `meteva-1.7.4/meteva/method/space/mode/utils.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/point_to_area.py` & `meteva-1.7.4/meteva/method/space/point_to_area.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import meteva
 import pandas as pd
-
+import numpy as np
 
 def p2p_vto01(sta_all,threshold = 1e-30,compair = ">="):
     '''
 
     :param sta_fo_all: 将预报数据处理成0-1数据
     :param threshold: 大于等于该阈值参数的站点值将转换成1，否则转换成0，缺省值仍然保持为缺省值
     :return:
@@ -14,27 +14,29 @@
         return
 
     sta_happen_all = sta_all.copy()
     fo_names = meteva.base.get_stadata_names(sta_all)
 
     if isinstance(threshold,pd.DataFrame):
         sta_compair = meteva.base.combine_expand_IV(sta_happen_all,threshold)
+        print(sta_compair.iloc[-10:-1,:])
         for i in range(len(fo_names)):
             name = fo_names[i]
+            hap = np.zeros(len(sta_all.index))
             if compair == ">=":
-                sta_happen_all.loc[:,name] = 0 + (sta_compair.loc[:,name] >= sta_compair.iloc[:,-1])
+                hap[sta_compair.loc[:,name].values >= sta_compair.iloc[:,-1].values] = 1
             elif compair =="<=":
-                sta_happen_all.loc[:, name] = 0 + (sta_compair.loc[:, name] <= sta_compair.iloc[:, -1])
+                hap[sta_compair.loc[:,name].values <= sta_compair.iloc[:,-1].values] = 1
             elif compair ==">":
-                sta_happen_all.loc[:, name] = 0 + (sta_compair.loc[:, name] > sta_compair.iloc[:, -1])
+                hap[sta_compair.loc[:,name].values > sta_compair.iloc[:,-1].values] = 1
             else:
-                sta_happen_all.loc[:, name] = 0 + (sta_compair.loc[:, name] < sta_compair.iloc[:, -1])
-
+                hap[sta_compair.loc[:,name].values < sta_compair.iloc[:,-1].values] = 1
 
-            sta_happen_all.loc[sta_compair.loc[:,name] == meteva.base.IV, name] = meteva.base.IV
+            sta_happen_all.loc[:, name] =hap[:]
+            sta_happen_all.loc[sta_compair.loc[:,name].values == meteva.base.IV, name] = meteva.base.IV
     else:
         for i in range(len(fo_names)):
             name = fo_names[i]
             if compair == ">=":
                 sta_happen_all.loc[:,name] = 0 + (sta_happen_all.loc[:,name] >= threshold)
             elif compair ==">":
                 sta_happen_all.loc[:,name] = 0 + (sta_happen_all.loc[:,name] > threshold)
```

### Comparing `meteva-1.7.3/meteva/method/space/rigider/fint2d.py` & `meteva-1.7.4/meteva/method/space/rigider/fint2d.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/rigider/fint2d_old.py` & `meteva-1.7.4/meteva/method/space/rigider/fint2d_old.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/rigider/imomenter.py` & `meteva-1.7.4/meteva/method/space/rigider/imomenter.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/rigider/rigider.py` & `meteva-1.7.4/meteva/method/space/rigider/rigider.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/saller/saller.py` & `meteva-1.7.4/meteva/method/space/saller/saller.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/LocSig.py` & `meteva-1.7.4/meteva/method/space/significance/LocSig.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/bootstrap.py` & `meteva-1.7.4/meteva/method/space/significance/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/bootstrap_ci.py` & `meteva-1.7.4/meteva/method/space/significance/bootstrap_ci.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/is_sig.py` & `meteva-1.7.4/meteva/method/space/significance/is_sig.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/sig_coverage.py` & `meteva-1.7.4/meteva/method/space/significance/sig_coverage.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/significance.py` & `meteva-1.7.4/meteva/method/space/significance/significance.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/spatbiasFS.py` & `meteva-1.7.4/meteva/method/space/significance/spatbiasFS.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/significance/tsboot.py` & `meteva-1.7.4/meteva/method/space/significance/tsboot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/vgm/rdist.py` & `meteva-1.7.4/meteva/method/space/vgm/rdist.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/vgm/structurogram.py` & `meteva-1.7.4/meteva/method/space/vgm/structurogram.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/space/vgm/structurogram_matrix.py` & `meteva-1.7.4/meteva/method/space/vgm/structurogram_matrix.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/weather_system/identify.py` & `meteva-1.7.4/meteva/method/weather_system/identify.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/yes_or_no/__init__.py` & `meteva-1.7.4/meteva/method/yes_or_no/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/yes_or_no/plot.py` & `meteva-1.7.4/meteva/method/yes_or_no/plot.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/method/yes_or_no/score.py` & `meteva-1.7.4/meteva/method/yes_or_no/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,15 @@
 
 def hfmc(Ob, Fo, grade_list=[1e-30],compare =">=",compair = None):
     '''
     预报列联表
     :param Ob: 实况数据  任意维numpy数组
     :param Fo: 预测数据 任意维numpy数组,Fo.shape 和Ob.shape一致
     :param grade_list: 多个阈值同时检验时的等级参数
-    :return: python numpy数组，其中最后一维长度为4，分别记录了（命中数，漏报数，空报数，正确否定数）
+    :return: python numpy数组，其中最后一维长度为4，分别记录了（命中数，空报数，漏报数，正确否定数）
     '''
     if compair is not None:
         print("warning: the argument compair will be abolished, please use compare instead\n警告：参数compair 将被废除，以后请使用参数compare代替")
         compare = compair
     if compare not in [">=",">","<","<="]:
         print("compare 参数只能是 >=   >  <  <=  中的一种")
         return
```

### Comparing `meteva-1.7.3/meteva/method/yes_or_no/skill.py` & `meteva-1.7.4/meteva/method/yes_or_no/skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,16 @@
         skill = (far_base - far)/far_base
         return round(skill,3)
 
 
 def spo(pod,pod_base):
     '''
 
-    :param far: 省台空报率
-    :param far_base: 中央台空报率
+    :param pod: 省命中率
+    :param pod_base: 中央台命中率
     :return: 省台相对于中央台的预报技巧
     '''
     if pod_base == 1:
         if pod ==1:
             return 0
         else:
             return -IV
```

### Comparing `meteva-1.7.3/meteva/method/yes_or_no/table.py` & `meteva-1.7.4/meteva/method/yes_or_no/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/perspact/middle_prepare.py` & `meteva-1.7.4/meteva/perspact/middle_prepare.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 
 method_coluns_dict = {
     "hfmc_of_sun_rain":["Hsr","Fsr","Msr","Csr"],
     "hfmc" :  ["H","F","M","C"],
     "tase":["T", "E", "A", "S"],
     "tc_count":["T", "C"],
+    "tlfo":["T","LFO"],
+    "toar":["T","OAR"],
     "tmmsss": ["T", "MX","MY","SX","SY","SXY"],
     "tbask":["T","BASK"],
     "nasws_uv": ["T", "AC", "SCORE", "SEVERER", "WEAK"],
     "nas_uv": ["T", "AC", "SCORE"],
     "na_uv":["T","AC"],
     "nasws_s": ["T", "AC", "SCORE", "SEVERER", "WEAK"]
 
@@ -27,34 +29,42 @@
         meteva.method.r,meteva.method.hss_yesorno,meteva.method.pofd,meteva.method.pod,
         meteva.method.dts,meteva.method.orss,meteva.method.pc,meteva.method.roc,meteva.method.sr,
         meteva.method.hk_yesorno,meteva.method.odds_ratio,meteva.method.ob_fo_hr,meteva.method.ob_fo_hc
     ]
     hfmc_of_sum_rain_list = [meteva.method.pc_of_sun_rain]
     tase_list = [meteva.method.me, meteva.method.mae, meteva.method.mse, meteva.method.rmse]
     tc_list = [meteva.method.correct_rate,meteva.method.wrong_rate]
-    tmmsss_list = [meteva.method.residual_error, meteva.method.residual_error_rate,meteva.method.corr]
+    tmmsss_list = [meteva.method.residual_error, meteva.method.residual_error_rate,meteva.method.corr,
+                    meteva.method.nse,meteva.method.ob_fo_mean,meteva.method.ob_fo_sum]
     tbask_list = [meteva.product.regulation.temperature.temp_forecaster_score]
     nasws_s_list = [meteva.method.acs, meteva.method.scs, meteva.method.wind_weaker_rate,
                      meteva.method.wind_severer_rate]
     nasws_uv_list = [meteva.method.acs_uv,meteva.method.scs_uv,meteva.method.wind_weaker_rate_uv,meteva.method.wind_severer_rate_uv]
     nas_uv_list = [meteva.method.acd_uv,meteva.method.scd_uv]
     na_uv_list = [meteva.method.acz_uv]
+    toar_list = [meteva.method.mre]
+    tlfo_list = [meteva.method.rmsf]
 
     method_mid = None
     method_name = method.__name__
+
     if method in hfmc_of_sum_rain_list:
         method_mid = getattr(meteva.method, method_name + "_hfmc")
     elif method in hfmc_list:
         method_mid  = getattr(meteva.method, method_name +"_hfmc")
     elif method in tase_list:
         method_mid = getattr(meteva.method, method_name + "_tase")
     elif method in tc_list:
         method_mid = getattr(meteva.method, method_name + "_tc")
     elif method in tmmsss_list:
         method_mid = getattr(meteva.method, method_name + "_tmmsss")
+    elif method in toar_list:
+        method_mid = getattr(meteva.method, method_name + "_toar")
+    elif method in tlfo_list:
+        method_mid = getattr(meteva.method, method_name + "_tlfo")
     elif method in tbask_list:
         method_mid = getattr(meteva.product, method_name + "_tbask")
     elif method in nasws_s_list:
         method_mid = getattr(meteva.method, method_name + "_nasws")
     elif method in nasws_uv_list:
         method_name1 = method_name.replace("_uv","_nasws")
         method_mid = getattr(meteva.method, method_name1)
@@ -74,15 +84,18 @@
         meteva.method.r,meteva.method.hss_yesorno,meteva.method.pofd,meteva.method.pod,
         meteva.method.dts,meteva.method.orss,meteva.method.pc,meteva.method.roc,meteva.method.sr,
         meteva.method.hk_yesorno,meteva.method.odds_ratio,meteva.method.ob_fo_hr,meteva.method.ob_fo_hc
     ]
     hfmc_of_sum_rain_list = [meteva.method.pc_of_sun_rain]
     tase_list = [meteva.method.me, meteva.method.mae, meteva.method.mse, meteva.method.rmse]
     tc_list = [meteva.method.correct_rate,meteva.method.wrong_rate]
-    tmmsss_list = [meteva.method.residual_error, meteva.method.residual_error_rate,meteva.method.corr]
+    tmmsss_list = [meteva.method.residual_error, meteva.method.residual_error_rate,meteva.method.corr,meteva.method.ob_fo_sum,meteva.method.ob_fo_mean,
+                   meteva.method.nse]
+    toar_list = [meteva.method.mre]
+    tlfo_list = [meteva.method.rmsf]
     tbask_list = [meteva.product.regulation.temperature.temp_forecaster_score]
     nasws_s_list = [meteva.method.acs,meteva.method.scs,meteva.method.wind_weaker_rate,meteva.method.wind_severer_rate]
     nasws_uv_list = [meteva.method.acs_uv,meteva.method.scs_uv,meteva.method.wind_weaker_rate_uv,meteva.method.wind_severer_rate_uv]
     nas_uv_list = [meteva.method.acd_uv,meteva.method.scd_uv]
     na_uv_list = [meteva.method.acz_uv]
 
     method_mid = None
@@ -92,14 +105,18 @@
         method_mid  = meteva.method.hfmc
     elif method in tase_list:
         method_mid = meteva.method.tase
     elif method in tc_list:
         method_mid = meteva.method.tc_count
     elif method in tmmsss_list:
         method_mid = meteva.method.tmmsss
+    elif method in toar_list:
+        method_mid = meteva.method.toar
+    elif method in tlfo_list:
+        method_mid = meteva.method.tlfo
     elif method in tbask_list:
         method_mid = meteva.product.regulation.temperature.tbask
     elif method in nasws_s_list:
         method_mid = meteva.method.nasws_s
     elif method in nasws_uv_list:
         method_mid = meteva.method.nasws_uv
     elif method in nas_uv_list:
```

### Comparing `meteva-1.7.3/meteva/perspact/score.py` & `meteva-1.7.4/meteva/perspact/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import xarray as xr
 import datetime
 import collections
 import copy
 
 
 # 实现任意纬度分类的函数
-def score_df(df, method, s = None,g=None,gll_dict = None,plot = None,first = True,**kwargs):
+def score_df(df, method, s = None,g=None,gll_dict = None,plot = None,excel_path = None,first = True,**kwargs):
     '''
 
     :param df:
     :param method:
     :param g:
     :return:
     '''
@@ -26,26 +26,34 @@
     column_df = df.columns
     if not set(column_list) <= set(column_df):
         print("input pandas.DataFrame must contains columns in list of "+ str(column_list) + " for mem." + method_name + " caculation")
         return None,None
 
     if s is not None:
         if "member" in s.keys():
-            df0  = df0.loc[df0['member'].isin(s["member"])]
+            if isinstance(s["member"],list):
+                members = s["member"]
+            else:
+                members = [s["member"]]
+            df0  = df0.loc[df0['member'].isin(members)]
             s.pop("member")
     df1 = meteva.base.sele_by_dict(df0, s)
 
     if method_name.find("ob_fo_") >= 0 and first:
         df_ob = copy.deepcopy(df1)
         df_ob["member"] = "OBS"
         if method_mid.__name__ == "hfmc":
             df_ob["H"] = df1["H"] + df1["M"]
             df_ob["F"] = 0
             df_ob["M"] = 0
             df_ob["C"] = df1["F"] + df1["C"]
+        if method_mid.__name__ =="tmmsss":
+            df_ob["T"] = df1["T"]
+            df_ob["MY"] = df1["MX"]
+            pass
         df_ob.drop_duplicates(subset=None, keep='first', inplace=True)
         df1 = pd.concat([df_ob,df1],axis=0)
         if g is None:
             g = ["member"]
 
         if "member" not in g:
             print("统计"+method_name+"时，参数g中必须包含“member")
@@ -129,30 +137,33 @@
             score_list.append(score1)
             if gll is None:
                 gll_str = "None"
             else:
                 gll_str = str(gll[i])
             gll_i_dict[gll_str] = i
 
+
         if gll0 is None:
             score_list_with_iv = score_list
         else:
             score_list_with_iv = []
             for j in range(len(gll0)):
                 gll_str = str(gll0[j])
                 if gll_str in gll_i_dict.keys():
                     score2 = score_list[gll_i_dict[gll_str]]
                 else:
                     score2 = score1 * 0 + meteva.base.IV
                 score_list_with_iv.append(score2)
-        score_array = np.array(score_list_with_iv)
 
+        score_array = np.array(score_list_with_iv)
         if method_name.find("ob_fo_")>=0:
              score_array = score_array[...,1,0]
 
+
+
         if plot is not None:meteva.base.plot_tools.plot_bar(plot,score_array,name_list_dict=gll_dict,**kwargs)
 
         return  score_array,gll_dict
     else:
         if len(g) == 2:
             g_left = g[1]
         else:
@@ -177,14 +188,16 @@
                 score2 = score_all_list[gll_i_dict[gll_str]]
             else:
                 score2 = score_array * 0 + meteva.base.IV
             score_list_with_iv.append(score2)
         score_all_array = np.array(score_list_with_iv)
 
         if plot is not None:meteva.base.plot_tools.plot_bar(plot,score_all_array,name_list_dict=gll_dict,**kwargs)
+        if excel_path is not None:
+            meteva.base.write_array_to_excel(score_all_array,excel_path,gll_dict)
 
         return score_all_array,gll_dict
 
 def sele_by_dict(ds0,s):
     if s is None:
         return ds0
     else:
@@ -757,42 +770,52 @@
             g_list = [g]
     g_list.append("id")
 
     if s is not None:
         if "member" in s.keys():
             df_mid  = df_mid.loc[df_mid['member'].isin(s["member"])]
             s.pop("member")
+        if "grade" in s.keys():
+            df_mid = df_mid.loc[df_mid['grade']== s["grade"]]
+            s.pop("grade")
     #print(df_mid)
     df_mid = meteva.base.sele_by_dict(df_mid, s)
     score_array,g_dict =score_df(df_mid,method,g = g_list,gll_dict = gll_dict)
     grd_list = []
 
+    g_time = ["time","year","month","day","hour","minute","dtime","xun","hou",
+              "ob_time","ob_year","ob_month","ob_day","ob_hour","ob_minute","ob_xun","ob_hou"]
+
     region_ids = g_dict["id"]
     max_id = np.max(region_ids)
     min_id = np.min(region_ids)
 
     max_ = max(max_id,abs(min_id))
     if max_ <1000000:
         lat = np.round(region_ids  / 1000)
         lon = region_ids - lat * 1000
     else:
         lat = np.round(region_ids / 10000)
         lon = region_ids - lat * 10000
         lon /=10
         lat /=10
-    score_grd = None
+    score_grd_list = None
+    gnames0 = None
     if len(g_list) == 1:
         dict1 = {"level":df_mid["level"].values[0],"time":df_mid["time"].values[0],"dtime":df_mid["dtime"].values[0],
             "id": region_ids, "lon": lon, "lat": lat,  "score": score_array}
         df = pd.DataFrame(dict1)
         score_sta = meteva.base.sta_data(df)
         score_grd = meteva.base.trans_sta_to_grd(score_sta)
-        score_grd.values[score_grd.values == meteva.base.IV] = 0
-        meteva.base.plot_tools.contourf_2d_grid(score_grd, save_path,**kwargs)
+        score_grd_list.append(score_grd)
+        #score_grd.values[score_grd.values == meteva.base.IV] = 0
+        #meteva.base.plot_tools.contourf_2d_grid(score_grd, save_path,**kwargs)
+        #return [score_grd],None
     elif len(g_list) == 2:
+
         gnames0 = g_dict[g_list[0]]
         #print(gnames0)
         ng0 = len(gnames0)
         if g_list[0] =="grade":
             grd_list = []
             vmin = 10e30
             vmax = -10e30
@@ -804,22 +827,39 @@
                                    "lon": lon, "lat": lat, name: value})
                 score_sta = meteva.base.sta_data(df)
 
                 score_grd = meteva.base.trans_sta_to_grd(score_sta)
                 score_grd.values[score_grd.values == meteva.base.IV] = 0
                 grd_list.append(score_grd)
 
-                vmax1 = np.max(score_grd.values)
-                vmin1 = np.max(score_grd.values)
-                if vmax1 > vmax: vmax = vmax1
-                if vmin1 < vmin: vmin = vmin1
+                # vmax1 = np.max(score_grd.values)
+                # vmin1 = np.max(score_grd.values)
+                # if vmax1 > vmax: vmax = vmax1
+                # if vmin1 < vmin: vmin = vmin1
 
-            meteva.base.plot_tools.plot_2d_grid_list(grd_list,save_path=save_path,vmax=vmax,vmin = vmin,**kwargs)
+            #meteva.base.plot_tools.plot_2d_grid_list(grd_list,save_path=save_path,vmax=vmax,vmin = vmin,**kwargs)
 
+        elif g_list[0] in g_time:
+            for i in range(ng0):
+                #name = gnames0[i]
+                value = score_array[i, :]
 
+                dict1 = {"id": region_ids, "lon": lon, "lat": lat,  "score": value}
+                if "level" not in dict1:
+                    dict1["level"] = df_mid["level"].values[0]
+                if "time" not in dict1:
+                    dict1["time"] = df_mid["time"].values[0]
+                if "dtime" not in dict1:
+                    dict1["dtime"] = df_mid["dtime"].values[0]
+                df = pd.DataFrame(dict1)
+                score_sta = meteva.base.sta_data(df)
+                score_grd = meteva.base.trans_sta_to_grd(score_sta)
+                grd_list.append(score_grd)
+                #title_list.append(g_list[0] + ":" + str(name))
+            #meteva.base.plot_tools.plot_2d_grid_list(grd_list, save_path,title = title_list,type="mesh")
         else:
             for i in range(ng0):
                 name = gnames0[i]
                 value = score_array[i,:]
                 if g_list[0] == "member":
                     df = pd.DataFrame({"level":df_mid["level"].values[0],"time":df_mid["time"].values[0],"dtime":df_mid["dtime"].values[0],"id":region_ids,
                                        "lon": lon, "lat": lat, name: value})
@@ -833,19 +873,35 @@
                         dict1["dtime"] = df_mid["dtime"].values[0]
                     df = pd.DataFrame(dict1)
                 score_sta = meteva.base.sta_data(df)
 
                 score_grd = meteva.base.trans_sta_to_grd(score_sta)
                 grd_list.append(score_grd)
             score_grd = meteva.base.concat(grd_list)
-            title = score_grd.coords[g_list[0]].values.tolist()
-            kwargs["title"]  = title
-            score_grd.values[score_grd.values == meteva.base.IV] = 0
-            meteva.base.plot_tools.contourf_2d_grid(score_grd,save_path,subplot=g_list[0],**kwargs)
-        return score_grd
+            #title_list = score_grd.coords[g_list[0]].values.tolist()
+            #kwargs["title"]  = title
+            #score_grd.values[score_grd.values == meteva.base.IV] = 0
+            #meteva.base.plot_tools.plot_2d_grid_list(grd_list, save_path,title = title_list,type="mesh")
+
+
+    grd_list_plot = []
+    for i in range(len(grd_list)):
+        score_grd = grd_list[i].copy()
+        score_grd.values[score_grd.values == meteva.base.IV] = 0
+        grd_list_plot.append(score_grd)
+    if gnames0 is None:
+        title_list = None
+    else:
+        title_list = []
+        for i in range(len(gnames0)):
+            title_list.append(g_list[0] + ":" + str(gnames0[i]))
+        kwargs["title"] = title_list
+    meteva.base.plot_tools.plot_2d_grid_list(grd_list_plot, type="mesh", save_path = save_path, **kwargs)
+
+    return grd_list,gnames0
 
 
 if __name__ =="__main__":
     import pandas as pd
     #path = r"O:\data\hdf\gongbao\wind3h_update12h_station2k\wind3h_update12h_station2k.h5"
     path = r"H:/a.txt"
     uv = pd.read_hdf(path)
```

### Comparing `meteva-1.7.3/meteva/product/application/__init__.py` & `meteva-1.7.4/meteva/product/application/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/application/data_collection.py` & `meteva-1.7.4/meteva/product/application/data_collection.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/application/data_distribute.py` & `meteva-1.7.4/meteva/product/application/data_distribute.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/application/data_prepare.py` & `meteva-1.7.4/meteva/product/application/data_prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,16 +512,16 @@
                                 dat = interp(dat,station)
                             if reasonable_value is not None:
                                 dat = meteva.base.sele_by_para(dat,value=reasonable_value)
                             data_name0 = meteva.base.get_stadata_names(dat)
                             if len(data_name0) == 1:
                                 meteva.base.set_stadata_names(dat,data_name)
                             meteva.base.set_stadata_coords(dat,time = time1)
-
                             sta_list.append(dat)
+                            print("success read data from "+ path)
                         else:
                             print("fail read data from " + path)
                     except:
                         print("fail read data from " + path)
                 else:
                     print(path +  "does not exist")
     if(len(sta_list)==0):return None
```

### Comparing `meteva-1.7.3/meteva/product/application/fun.py` & `meteva-1.7.4/meteva/product/application/fun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/application/terrain_height_correction.py` & `meteva-1.7.4/meteva/product/application/terrain_height_correction.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/application/time_compare.py` & `meteva-1.7.4/meteva/product/application/time_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/__init__.py` & `meteva-1.7.4/meteva/product/program/__init__.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/diurnal.py` & `meteva-1.7.4/meteva/product/program/diurnal.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,22 @@
             fo_name = data_name[1:]
 
     fo_num = len(fo_name)
 
     gll_valid = []
     result_list =[]
     for i in range(len(gll1)):
-        result_all,hour_list = meteva.product.program.score(sta_ob_and_fos_list[i],method,g = "ob_hour",gll = ob_hours_list)
+        result_all,hour_list = meteva.product.program.score(sta_ob_and_fos_list[i],method,g = "ob_hour",gll = ob_hours_list,**method_args)
         hours = np.array(hour_list)
         if len(hour_list) == ob_hour_count:
             gll_valid.append(gll1[i])
             result_max_index = np.argmax(result_all,axis=0)
             result_max = hours[result_max_index]
             result_list.append(result_max)
+
     result = np.array(result_list)
     group_num = len(gll_valid)
 
     if plot is not None or excel_path is not None:
 
         name_list_dict = {}
         if g is None:
@@ -182,14 +183,15 @@
         #设置成员名称
 
         name_list_dict["member"] = fo_name
         if fo_num==0:
             fo_num = 1
             name_list_dict["member"] = ["OBS"]
         result_plot = result.reshape((group_num,fo_num,grade_num))
+
         #设置等级名称
         name_list_dict["grade"] = grade_names
         keys = list(name_list_dict.keys())
         if fo_num ==1:
             if grade_num > 1:
                 if group_num>1:
                     legend = keys[2]
```

### Comparing `meteva-1.7.3/meteva/product/program/error_ana_scatter.py` & `meteva-1.7.4/meteva/product/program/error_ana_scatter.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/fun.py` & `meteva-1.7.4/meteva/product/program/fun.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/plot.py` & `meteva-1.7.4/meteva/product/program/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 def plot(sta_ob_and_fos0,method,s = None,g = None,gll = None,save_dir = None,save_path = None,title =None,**kwargs):
     if s is not None:
         if g is not None:
             if g == "last_range" or g == "last_step":
                 s["drop_last"] = False
             else:
                 s["drop_last"] = True
-    sta_ob_and_fos = sele_by_dict(sta_ob_and_fos0, s)
+
+    sta_ob_and_fos = meteva.base.sele_by_para(sta_ob_and_fos0, drop_IV=True)
+    sta_ob_and_fos = sele_by_dict(sta_ob_and_fos, s)
     #discription_uni = get_unique_coods(sta_ob_and_fos)
     sta_ob_and_fos_list,gll1 = group(sta_ob_and_fos,g,gll)
     data_name = meteva.base.get_stadata_names(sta_ob_and_fos_list[0])
 
     group_num = len(sta_ob_and_fos_list)
     #title = None
     #if "title" in kwargs.keys():
```

### Comparing `meteva-1.7.3/meteva/product/program/sample_statistic.py` & `meteva-1.7.4/meteva/product/program/sample_statistic.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/score.py` & `meteva-1.7.4/meteva/product/program/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,14 +521,17 @@
             sta_result = []
             coord_names.extend(fo_name)
             member_num = result.shape[1]
             for i in range(result.shape[2]):
                 sta_result1 = sta_merge.loc[:, coord_names]
                 sta_result1.iloc[:, -member_num:] = result[:,:,i]
                 sta_result.append(sta_result1)
+        sup_title = None
+        if "sup_title" in plot_args.keys():
+            sup_title = copy.deepcopy(plot_args["sup_title"])
 
         for i in range(len(sta_result)):
             sta_result1 = sta_result[i]
             if "var_name" in sta_ob_and_fos0.attrs.keys():
                 sta_result1.attrs["var_name"] =sta_ob_and_fos0.attrs["var_name"]
             else:
                 sta_result1.attrs["var_name"] = ""
@@ -554,25 +557,30 @@
                             title1 += "(grade_" + str(grade_names[i])+")"
                         title1_list.append(title1)
 
 
                 if plot == "scatter" or plot =="contourf":
                     if "sup_title" not in plot_args.keys():
                         plot_args["sup_title"] = ""
+                    elif isinstance(sup_title,list):
+                        plot_args["sup_title"] = sup_title[i]
                     save_path1 = None
                     if save_path is None:
                         if save_dir is None:
                             show = True
                         else:
                             save_path1 = []
                             for i in range(len(title1_list)):
                                 fileName = title1_list[i].replace("\n", "").replace(":", "")
                                 save_path1.append(save_dir + "/" + fileName + ".png")
+                    elif subplot=="member":
+                        save_path1 = save_path[i]
                     else:
                         save_path1 = save_path[k * fo_num: (k + 1) * fo_num]
+
                     if plot=="scatter":
                         if "fix_size" not in plot_args.keys():
                             plot_args["fix_size"] = False
                         meteva.base.tool.plot_tools.scatter_sta(sta_result1, save_path=save_path1, show=show,
                                                             title=title1_list, print_max=print_max,
                                                             print_min=print_min
                                                             , add_county_line=add_county_line,
@@ -596,15 +604,15 @@
                             dlat0 = 1
                         slon = slon0 - dlon0
                         elon = elon0 + dlon0
                         slat = slat0 - dlat0
                         elat = elat0 + dlat0
                         grid1 = meteva.base.grid([slon,elon,dlon0],[slat,elat,dlat0])
 
-                        grd = meteva.base.interp_sg_idw_delta(sta_result1,grid1,halfR=100,nearNum=4)
+                        grd = meteva.base.interp_sg_idw_delta(sta_result1,grid1,halfR=300,nearNum=8)
                         meteva.base.tool.plot_tools.contourf_2d_grid(grd, save_path=save_path1, show=show,
                                                             title=title1_list
                                                             , add_county_line=add_county_line,
                                                               dpi=dpi,subplot = subplot,ncol = ncol,**plot_args)
                 if plot == "micaps":
                     meteva.base.put_stadata_to_micaps(sta_result1,layer_description=title1_list)
```

### Comparing `meteva-1.7.3/meteva/product/program/space_compare.py` & `meteva-1.7.4/meteva/product/program/space_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,21 @@
                 if ob_time1 in ob_time_list:
                     dtimes_valid.append(dtime1)
                     fo_time_valid.append(fo_time)
                     ob_time_valid.append(ob_time1)
                     break
         if len(set(ob_time_valid))>1 and len(set(fo_time_valid))>1:
             print("参数x_y=dtime_member时，暂时不能支持多个起报时间和多个观测时间对应情况下的检验")
+            return
 
+        if sup_title is None:
+            if len(set(ob_time_valid))==1:
+                sup_title = meteva.base.get_path("YY年MM月DD日HH时的观测和不同时效预报对比",ob_time_valid[0])
+            elif len(set(fo_time_valid))==1:
+                sup_title = meteva.base.get_path("YY年MM月DD日HH时的起报的不时效预报和观测对比", fo_time_valid[0])
         if x_y == "dtime_member":
             x = grd_fo['lon'].values
             slon = x[0]
             elon = x[-1]
             y = grd_fo['lat'].values
             slat = y[0]
             elat = y[-1]
@@ -341,14 +347,16 @@
             cmap1, clevs1 = meteva.base.tool.color_tools.def_cmap_clevs(cmap=colors_sta, clevs=clevs, vmin=vmin, vmax=vmax)
             norm = BoundaryNorm(clevs, cmap1.N - 1)
 
             ax_up_right = None
             ylabel_seted = 0
             #print(ncol)
             #print(nrow)
+
+
             for pi in range(ncol):
                 #print(str(pi) + " ---")
                 if len(ob_time_valid) == 1:
                     dtime1 = dtimes_valid[ncol - pi - 1]
                     ob_time = ob_time_valid[0]
                     fo_time1 = None
                     for time1 in fo_time_valid:
@@ -392,14 +400,15 @@
 
                     add_china_map_2basemap(ax, name="nation", edgecolor='k', lw=0.3, encoding='gbk', grid0=None)  # "省界"
                     add_china_map_2basemap(ax, edgecolor='k', lw=0.3, encoding='gbk')  # "省界"
                     if add_county_line:
                         add_china_map_2basemap(ax, name="county", edgecolor='k', lw=0.2, encoding='gbk', grid0=None)  # "县界"
                     ax.set_xlim((slon, elon))
                     ax.set_ylim((slat, elat))
+
                     if pj ==0:
                         if valid_time == 0:
                             ax.set_title(dtime1)
                         else:
                             dtime_str = str(dtime1 - valid_time) + "-"+ str(dtime1)
                             ax.set_title(dtime_str)
 
@@ -431,36 +440,33 @@
                     plt.text(xt, yt, ts_str, color = "#FF0000", fontsize=sup_fontsize, zorder=100)
 
 
                 ylabel_seted = 1
 
             height_colorbar =0.95 * (ax_up_right.bbox.y1 - ax.bbox.y0) / fig.dpi / height/2
 
-
             location = [ax.bbox.x1 / fig.dpi / width + 0.005, ax.bbox.y0 / fig.dpi / height, 0.01,
                         height_colorbar]
 
             colorbar_position = fig.add_axes(location)  # 位置[左,下,宽,高]
             colorbar_fo = plt.colorbar(im1, cax=colorbar_position)
             colorbar_fo.set_label('预报', fontsize=sup_fontsize * 0.9)
 
             #cb.ax.tick_params(labelsize=sup_fontsize * 0.8)  # 设置色标刻度字体大小。
 
-            y_sup_title = (height_bottem_xticsk + (nrow) * (height_map + height_hspace)) / height
-
-
+            y_sup_title = (height_bottem_xticsk + (nrow) * (height_map + height_hspace)+sup_fontsize*0.03) / height
 
             location = [ax.bbox.x1 / fig.dpi / width + 0.005, ax_up_right.bbox.y1 / fig.dpi / height - height_colorbar, 0.01,
                        height_colorbar]
             colorbar_position = fig.add_axes(location)  # 位置[左,下,宽,高]
             colorbar_ob = plt.colorbar(im2, cax=colorbar_position)
             colorbar_ob.set_label('观测', fontsize=sup_fontsize * 0.9)
 
-            if sup_title is not None:
-                plt.suptitle(sup_title, y=y_sup_title, fontsize=sup_fontsize * 1.2)
+
+            plt.suptitle(sup_title, y=y_sup_title, fontsize=sup_fontsize * 1.2)
 
             if save_path is None:
                 show = True
 
             if save_path is not None:
                 meteva.base.tool.path_tools.creat_path(save_path)
                 file1, extension = os.path.splitext(save_path)
```

### Comparing `meteva-1.7.3/meteva/product/program/table.py` & `meteva-1.7.4/meteva/product/program/table.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/time_compare.py` & `meteva-1.7.4/meteva/product/program/time_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/time_space_compare.py` & `meteva-1.7.4/meteva/product/program/time_space_compare.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/program/typhoon.py` & `meteva-1.7.4/meteva/product/program/typhoon.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/regulation/environment.py` & `meteva-1.7.4/meteva/product/regulation/environment.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/regulation/short_term_heavy_rainfall.py` & `meteva-1.7.4/meteva/product/regulation/short_term_heavy_rainfall.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/regulation/temperature.py` & `meteva-1.7.4/meteva/product/regulation/temperature.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva/product/regulation/thunderstrom_gale.py` & `meteva-1.7.4/meteva/product/regulation/thunderstrom_gale.py`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/meteva.egg-info/PKG-INFO` & `meteva-1.7.4/meteva.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteva
-Version: 1.7.3
+Version: 1.7.4
 Summary: A collections of functions for meteorological verification.
 Home-page: UNKNOWN
 Author: liucouhua,daikan,wangbaoli,tangbuxing
 Author-email: liucouhua@163.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `meteva-1.7.3/meteva.egg-info/SOURCES.txt` & `meteva-1.7.4/meteva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meteva-1.7.3/setup.py` & `meteva-1.7.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     install_requires=[
                       'numpy>=1.12.1',
                       'pandas>=1.0.4',
                       "netCDF4>=1.4.2",
                       'scipy>=0.19.0',
                       'xarray>=0.10.0',
+                      'scikit-learn>=0.21.2',
                       'matplotlib>=3.0.0',
                       "httplib2>=0.12.0",
                       "protobuf<3.20.0",
                       "pyshp>=2.1.0",
                       "tables>=3.4.4",
                       "urllib3>=1.21.1"
                       #"JPype1>=1.4.0"
```

