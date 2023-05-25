# Comparing `tmp/upsies-2023.4.3.tar.gz` & `tmp/upsies-2023.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsies-2023.4.3.tar", last modified: Mon Apr  3 14:19:55 2023, max compression
+gzip compressed data, was "upsies-2023.5.25.tar", last modified: Thu May 25 13:47:13 2023, max compression
```

## Comparing `upsies-2023.4.3.tar` & `upsies-2023.5.25.tar`

### file list

```diff
@@ -1,147 +1,154 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.820104 upsies-2023.4.3/
--rw-------   0 ich       (1000) ich       (1000)    35149 2021-06-11 16:56:53.000000 upsies-2023.4.3/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     2366 2023-04-03 14:19:55.820104 upsies-2023.4.3/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1815 2023-03-10 11:08:25.000000 upsies-2023.4.3/README.rst
--rw-------   0 ich       (1000) ich       (1000)       38 2023-04-03 14:19:55.820104 upsies-2023.4.3/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1637 2023-04-01 09:23:22.000000 upsies-2023.4.3/setup.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.756104 upsies-2023.4.3/upsies/
--rw-------   0 ich       (1000) ich       (1000)     1181 2023-04-03 14:19:05.000000 upsies-2023.4.3/upsies/__init__.py
--rw-------   0 ich       (1000) ich       (1000)       73 2022-03-13 08:26:06.000000 upsies-2023.4.3/upsies/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     1399 2023-03-19 11:08:21.000000 upsies-2023.4.3/upsies/constants.py
--rw-------   0 ich       (1000) ich       (1000)     2079 2023-03-02 18:38:22.000000 upsies-2023.4.3/upsies/defaults.py
--rw-------   0 ich       (1000) ich       (1000)     6111 2023-03-02 18:50:50.000000 upsies-2023.4.3/upsies/errors.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.768104 upsies-2023.4.3/upsies/jobs/
--rw-------   0 ich       (1000) ich       (1000)      215 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/jobs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    27452 2023-04-01 17:11:12.000000 upsies-2023.4.3/upsies/jobs/base.py
--rw-------   0 ich       (1000) ich       (1000)     2165 2023-03-16 15:48:25.000000 upsies-2023.4.3/upsies/jobs/custom.py
--rw-------   0 ich       (1000) ich       (1000)    18480 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/jobs/dialog.py
--rw-------   0 ich       (1000) ich       (1000)     3707 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/jobs/imghost.py
--rw-------   0 ich       (1000) ich       (1000)     4807 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/jobs/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     7596 2023-03-09 08:41:14.000000 upsies-2023.4.3/upsies/jobs/poster.py
--rw-------   0 ich       (1000) ich       (1000)     8642 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/jobs/scene.py
--rw-------   0 ich       (1000) ich       (1000)    14316 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/jobs/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     2770 2023-03-02 16:24:04.000000 upsies-2023.4.3/upsies/jobs/set.py
--rw-------   0 ich       (1000) ich       (1000)     7977 2023-03-27 13:40:54.000000 upsies-2023.4.3/upsies/jobs/submit.py
--rw-------   0 ich       (1000) ich       (1000)    13640 2023-03-02 18:50:56.000000 upsies-2023.4.3/upsies/jobs/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    13899 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/jobs/webdb.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.772104 upsies-2023.4.3/upsies/trackers/
--rw-------   0 ich       (1000) ich       (1000)     1385 2023-02-10 10:57:50.000000 upsies-2023.4.3/upsies/trackers/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.772104 upsies-2023.4.3/upsies/trackers/base/
--rw-------   0 ich       (1000) ich       (1000)      149 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/trackers/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3032 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/trackers/base/_howto.py
--rw-------   0 ich       (1000) ich       (1000)     2638 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/trackers/base/config.py
--rw-------   0 ich       (1000) ich       (1000)    33820 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/trackers/base/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     5516 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/trackers/base/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.776104 upsies-2023.4.3/upsies/trackers/bhd/
--rw-------   0 ich       (1000) ich       (1000)      238 2021-06-22 10:11:31.000000 upsies-2023.4.3/upsies/trackers/bhd/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3643 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/trackers/bhd/config.py
--rw-------   0 ich       (1000) ich       (1000)    15605 2023-03-31 09:20:40.000000 upsies-2023.4.3/upsies/trackers/bhd/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     5162 2023-03-30 16:57:42.000000 upsies-2023.4.3/upsies/trackers/bhd/tracker.py
--rw-------   0 ich       (1000) ich       (1000)     3744 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/trackers/dummy.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.776104 upsies-2023.4.3/upsies/trackers/mtv/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/trackers/mtv/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2306 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/trackers/mtv/config.py
--rw-------   0 ich       (1000) ich       (1000)     9530 2023-04-01 09:23:22.000000 upsies-2023.4.3/upsies/trackers/mtv/jobs.py
--rw-------   0 ich       (1000) ich       (1000)    12614 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/trackers/mtv/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.780104 upsies-2023.4.3/upsies/trackers/nbl/
--rw-------   0 ich       (1000) ich       (1000)      238 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/trackers/nbl/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     1059 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/trackers/nbl/config.py
--rw-------   0 ich       (1000) ich       (1000)     1855 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/trackers/nbl/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     3969 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/trackers/nbl/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.780104 upsies-2023.4.3/upsies/trackers/ptp/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/trackers/ptp/__init__.py
--rw-------   0 ich       (1000) ich       (1000)      563 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/trackers/ptp/_ptp_tags.py
--rw-------   0 ich       (1000) ich       (1000)     1921 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/trackers/ptp/config.py
--rw-------   0 ich       (1000) ich       (1000)    17106 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/trackers/ptp/jobs.py
--rw-------   0 ich       (1000) ich       (1000)    10548 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/trackers/ptp/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.780104 upsies-2023.4.3/upsies/uis/
--rw-------   0 ich       (1000) ich       (1000)       24 2021-06-11 16:55:41.000000 upsies-2023.4.3/upsies/uis/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.784104 upsies-2023.4.3/upsies/uis/tui/
--rw-------   0 ich       (1000) ich       (1000)       55 2022-03-13 08:25:17.000000 upsies-2023.4.3/upsies/uis/tui/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.792104 upsies-2023.4.3/upsies/uis/tui/commands/
--rw-------   0 ich       (1000) ich       (1000)     1319 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/uis/tui/commands/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    15230 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/commands/base.py
--rw-------   0 ich       (1000) ich       (1000)     1942 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/commands/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     3500 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/poster.py
--rw-------   0 ich       (1000) ich       (1000)     2465 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/release_name.py
--rw-------   0 ich       (1000) ich       (1000)     2710 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/scene.py
--rw-------   0 ich       (1000) ich       (1000)     4071 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     5152 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/set.py
--rw-------   0 ich       (1000) ich       (1000)     8319 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/submit.py
--rw-------   0 ich       (1000) ich       (1000)     8288 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/upload_images.py
--rw-------   0 ich       (1000) ich       (1000)     1570 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/commands/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     3061 2022-03-13 08:27:19.000000 upsies-2023.4.3/upsies/uis/tui/headless.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.796104 upsies-2023.4.3/upsies/uis/tui/jobwidgets/
--rw-------   0 ich       (1000) ich       (1000)      947 2021-06-11 16:56:53.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6992 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/base.py
--rw-------   0 ich       (1000) ich       (1000)      252 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/config.py
--rw-------   0 ich       (1000) ich       (1000)      202 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/custom.py
--rw-------   0 ich       (1000) ich       (1000)     1902 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/dialog.py
--rw-------   0 ich       (1000) ich       (1000)      767 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/imghost.py
--rw-------   0 ich       (1000) ich       (1000)      205 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     1105 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/poster.py
--rw-------   0 ich       (1000) ich       (1000)     4143 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/scene.py
--rw-------   0 ich       (1000) ich       (1000)     1649 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)      686 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/submit.py
--rw-------   0 ich       (1000) ich       (1000)     8671 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     9727 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/jobwidgets/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     2865 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/main.py
--rw-------   0 ich       (1000) ich       (1000)     1345 2022-10-25 10:31:19.000000 upsies-2023.4.3/upsies/uis/tui/style.py
--rw-------   0 ich       (1000) ich       (1000)     9795 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/uis/tui/tui.py
--rw-------   0 ich       (1000) ich       (1000)      626 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/uis/tui/utils.py
--rw-------   0 ich       (1000) ich       (1000)    13809 2023-03-28 10:18:22.000000 upsies-2023.4.3/upsies/uis/tui/widgets.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.808104 upsies-2023.4.3/upsies/utils/
--rw-------   0 ich       (1000) ich       (1000)    12665 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5254 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/utils/argtypes.py
--rw-------   0 ich       (1000) ich       (1000)      302 2023-03-05 11:59:14.000000 upsies-2023.4.3/upsies/utils/browser.py
--rw-------   0 ich       (1000) ich       (1000)    15025 2023-03-10 18:07:23.000000 upsies-2023.4.3/upsies/utils/configfiles.py
--rw-------   0 ich       (1000) ich       (1000)     1862 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/country.py
--rw-------   0 ich       (1000) ich       (1000)     7285 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/daemon.py
--rw-------   0 ich       (1000) ich       (1000)    16331 2023-04-01 09:23:22.000000 upsies-2023.4.3/upsies/utils/fs.py
--rw-------   0 ich       (1000) ich       (1000)     1955 2023-02-02 18:17:40.000000 upsies-2023.4.3/upsies/utils/html.py
--rw-------   0 ich       (1000) ich       (1000)    23350 2023-03-30 14:13:03.000000 upsies-2023.4.3/upsies/utils/http.py
--rw-------   0 ich       (1000) ich       (1000)     8756 2023-04-01 09:23:22.000000 upsies-2023.4.3/upsies/utils/image.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.812104 upsies-2023.4.3/upsies/utils/imghosts/
--rw-------   0 ich       (1000) ich       (1000)     1391 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/imghosts/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     7453 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/imghosts/base.py
--rw-------   0 ich       (1000) ich       (1000)     1147 2021-06-11 16:56:53.000000 upsies-2023.4.3/upsies/utils/imghosts/common.py
--rw-------   0 ich       (1000) ich       (1000)     1011 2021-10-31 14:15:29.000000 upsies-2023.4.3/upsies/utils/imghosts/dummy.py
--rw-------   0 ich       (1000) ich       (1000)     1997 2021-11-27 15:46:37.000000 upsies-2023.4.3/upsies/utils/imghosts/freeimage.py
--rw-------   0 ich       (1000) ich       (1000)     2517 2021-11-26 16:53:37.000000 upsies-2023.4.3/upsies/utils/imghosts/imgbb.py
--rw-------   0 ich       (1000) ich       (1000)      912 2021-10-19 13:17:48.000000 upsies-2023.4.3/upsies/utils/imghosts/imgbox.py
--rw-------   0 ich       (1000) ich       (1000)     3154 2021-11-26 16:53:37.000000 upsies-2023.4.3/upsies/utils/imghosts/ptpimg.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.816104 upsies-2023.4.3/upsies/utils/predbs/
--rw-------   0 ich       (1000) ich       (1000)     1364 2023-03-30 16:57:42.000000 upsies-2023.4.3/upsies/utils/predbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9573 2023-03-31 09:56:10.000000 upsies-2023.4.3/upsies/utils/predbs/base.py
--rw-------   0 ich       (1000) ich       (1000)     4128 2023-03-01 11:25:29.000000 upsies-2023.4.3/upsies/utils/predbs/common.py
--rw-------   0 ich       (1000) ich       (1000)     2276 2023-03-28 07:47:06.000000 upsies-2023.4.3/upsies/utils/predbs/corruptnet.py
--rw-------   0 ich       (1000) ich       (1000)    20145 2023-04-01 09:23:22.000000 upsies-2023.4.3/upsies/utils/predbs/multi.py
--rw-------   0 ich       (1000) ich       (1000)     2174 2023-03-30 16:57:42.000000 upsies-2023.4.3/upsies/utils/predbs/predbclub.py
--rw-------   0 ich       (1000) ich       (1000)     2333 2023-03-28 07:47:07.000000 upsies-2023.4.3/upsies/utils/predbs/predbde.py
--rw-------   0 ich       (1000) ich       (1000)     2167 2023-03-30 14:14:59.000000 upsies-2023.4.3/upsies/utils/predbs/predbovh.py
--rw-------   0 ich       (1000) ich       (1000)     5207 2023-03-01 11:25:29.000000 upsies-2023.4.3/upsies/utils/predbs/query.py
--rw-------   0 ich       (1000) ich       (1000)     3434 2023-03-28 11:13:24.000000 upsies-2023.4.3/upsies/utils/predbs/srrdb.py
--rw-------   0 ich       (1000) ich       (1000)    53993 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/utils/release.py
--rw-------   0 ich       (1000) ich       (1000)     3931 2023-02-19 13:31:01.000000 upsies-2023.4.3/upsies/utils/signal.py
--rw-------   0 ich       (1000) ich       (1000)     3922 2023-03-25 10:43:29.000000 upsies-2023.4.3/upsies/utils/string.py
--rw-------   0 ich       (1000) ich       (1000)     1908 2023-03-31 14:19:32.000000 upsies-2023.4.3/upsies/utils/subproc.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2021-09-23 10:04:01.000000 upsies-2023.4.3/upsies/utils/timestamp.py
--rw-------   0 ich       (1000) ich       (1000)    18257 2023-02-22 14:50:53.000000 upsies-2023.4.3/upsies/utils/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    11165 2023-03-02 18:51:27.000000 upsies-2023.4.3/upsies/utils/types.py
--rw-------   0 ich       (1000) ich       (1000)     2927 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/update.py
--rw-------   0 ich       (1000) ich       (1000)    34608 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/utils/video.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.820104 upsies-2023.4.3/upsies/utils/webdbs/
--rw-------   0 ich       (1000) ich       (1000)     1140 2023-01-16 18:31:24.000000 upsies-2023.4.3/upsies/utils/webdbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     8549 2023-03-28 17:30:22.000000 upsies-2023.4.3/upsies/utils/webdbs/base.py
--rw-------   0 ich       (1000) ich       (1000)    12546 2023-03-03 18:20:32.000000 upsies-2023.4.3/upsies/utils/webdbs/common.py
--rw-------   0 ich       (1000) ich       (1000)    17639 2023-04-03 14:17:09.000000 upsies-2023.4.3/upsies/utils/webdbs/imdb.py
--rw-------   0 ich       (1000) ich       (1000)    11802 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/webdbs/tmdb.py
--rw-------   0 ich       (1000) ich       (1000)     9525 2023-01-16 18:34:35.000000 upsies-2023.4.3/upsies/utils/webdbs/tvmaze.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-04-03 14:19:55.756104 upsies-2023.4.3/upsies.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     2366 2023-04-03 14:19:55.000000 upsies-2023.4.3/upsies.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     3600 2023-04-03 14:19:55.000000 upsies-2023.4.3/upsies.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-04-03 14:19:55.000000 upsies-2023.4.3/upsies.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       47 2023-04-03 14:19:55.000000 upsies-2023.4.3/upsies.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)      221 2023-04-03 14:19:55.000000 upsies-2023.4.3/upsies.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)        7 2023-04-03 14:19:55.000000 upsies-2023.4.3/upsies.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.493727 upsies-2023.5.25/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2021-06-11 16:56:53.000000 upsies-2023.5.25/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     2367 2023-05-25 13:47:13.493727 upsies-2023.5.25/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1815 2023-04-25 13:55:04.000000 upsies-2023.5.25/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.473728 upsies-2023.5.25/bb/
+-rw-------   0 ich       (1000) ich       (1000)      115 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3145 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/config.py
+-rw-------   0 ich       (1000) ich       (1000)    51071 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     8450 2023-04-25 13:54:40.000000 upsies-2023.5.25/bb/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-05-25 13:47:13.493727 upsies-2023.5.25/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1664 2023-05-25 13:46:48.000000 upsies-2023.5.25/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/
+-rw-------   0 ich       (1000) ich       (1000)     1181 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)       73 2022-03-13 08:26:06.000000 upsies-2023.5.25/upsies/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     1399 2023-03-19 11:08:21.000000 upsies-2023.5.25/upsies/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     2058 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/defaults.py
+-rw-------   0 ich       (1000) ich       (1000)     6188 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/errors.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/jobs/
+-rw-------   0 ich       (1000) ich       (1000)      215 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    27889 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     2165 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/custom.py
+-rw-------   0 ich       (1000) ich       (1000)    21011 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)     3707 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)     4807 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     7596 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     8642 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/scene.py
+-rw-------   0 ich       (1000) ich       (1000)    17965 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/jobs/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     2770 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/set.py
+-rw-------   0 ich       (1000) ich       (1000)     7977 2023-04-25 14:32:10.000000 upsies-2023.5.25/upsies/jobs/submit.py
+-rw-------   0 ich       (1000) ich       (1000)    13209 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/jobs/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    13899 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/jobs/webdb.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/trackers/
+-rw-------   0 ich       (1000) ich       (1000)     1385 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies/trackers/base/
+-rw-------   0 ich       (1000) ich       (1000)      149 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3222 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/trackers/base/_howto.py
+-rw-------   0 ich       (1000) ich       (1000)     3102 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/trackers/base/config.py
+-rw-------   0 ich       (1000) ich       (1000)    33425 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/trackers/base/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     5985 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/base/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/bhd/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.5.25/upsies/trackers/bhd/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3643 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/bhd/config.py
+-rw-------   0 ich       (1000) ich       (1000)    15623 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/bhd/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     6243 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/bhd/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     3647 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/dummy.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/mtv/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/mtv/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2306 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/mtv/config.py
+-rw-------   0 ich       (1000) ich       (1000)     9488 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/mtv/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)    12862 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/mtv/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/nbl/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.5.25/upsies/trackers/nbl/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1059 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/nbl/config.py
+-rw-------   0 ich       (1000) ich       (1000)     1855 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/nbl/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     3969 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/nbl/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/trackers/ptp/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/ptp/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2146 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/trackers/ptp/config.py
+-rw-------   0 ich       (1000) ich       (1000)    27925 2023-05-25 09:30:06.000000 upsies-2023.5.25/upsies/trackers/ptp/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     2001 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/trackers/ptp/metadata.py
+-rw-------   0 ich       (1000) ich       (1000)    15920 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/trackers/ptp/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/uis/
+-rw-------   0 ich       (1000) ich       (1000)       24 2021-06-11 16:55:41.000000 upsies-2023.5.25/upsies/uis/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.481727 upsies-2023.5.25/upsies/uis/tui/
+-rw-------   0 ich       (1000) ich       (1000)       55 2022-03-13 08:25:17.000000 upsies-2023.5.25/upsies/uis/tui/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.485727 upsies-2023.5.25/upsies/uis/tui/commands/
+-rw-------   0 ich       (1000) ich       (1000)     1319 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    15230 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1942 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     3500 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     2513 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/release_name.py
+-rw-------   0 ich       (1000) ich       (1000)     2710 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     4546 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/uis/tui/commands/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     5152 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/set.py
+-rw-------   0 ich       (1000) ich       (1000)     8269 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/uis/tui/commands/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     8308 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/uis/tui/commands/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/upload_images.py
+-rw-------   0 ich       (1000) ich       (1000)     1799 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/commands/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     3061 2022-03-13 08:27:19.000000 upsies-2023.5.25/upsies/uis/tui/headless.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.485727 upsies-2023.5.25/upsies/uis/tui/jobwidgets/
+-rw-------   0 ich       (1000) ich       (1000)      947 2021-06-11 16:56:53.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6992 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/base.py
+-rw-------   0 ich       (1000) ich       (1000)      252 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/config.py
+-rw-------   0 ich       (1000) ich       (1000)      202 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/custom.py
+-rw-------   0 ich       (1000) ich       (1000)     1902 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)      767 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)      205 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     1105 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     4143 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     1649 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)      686 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     8671 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     9727 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/jobwidgets/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     2865 2023-05-22 08:06:05.000000 upsies-2023.5.25/upsies/uis/tui/main.py
+-rw-------   0 ich       (1000) ich       (1000)     1345 2022-10-25 10:31:19.000000 upsies-2023.5.25/upsies/uis/tui/style.py
+-rw-------   0 ich       (1000) ich       (1000)     9795 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/tui.py
+-rw-------   0 ich       (1000) ich       (1000)      626 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/utils.py
+-rw-------   0 ich       (1000) ich       (1000)    13814 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/uis/tui/widgets.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.489727 upsies-2023.5.25/upsies/utils/
+-rw-------   0 ich       (1000) ich       (1000)    13326 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5658 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/utils/argtypes.py
+-rw-------   0 ich       (1000) ich       (1000)      302 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/browser.py
+-rw-------   0 ich       (1000) ich       (1000)     2794 2023-05-25 09:31:21.000000 upsies-2023.5.25/upsies/utils/btclient.py
+-rw-------   0 ich       (1000) ich       (1000)    15025 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/configfiles.py
+-rw-------   0 ich       (1000) ich       (1000)     1825 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/country.py
+-rw-------   0 ich       (1000) ich       (1000)     7285 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/daemon.py
+-rw-------   0 ich       (1000) ich       (1000)    17717 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/utils/fs.py
+-rw-------   0 ich       (1000) ich       (1000)     2353 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/utils/html.py
+-rw-------   0 ich       (1000) ich       (1000)    23553 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/utils/http.py
+-rw-------   0 ich       (1000) ich       (1000)    10178 2023-05-25 13:46:48.000000 upsies-2023.5.25/upsies/utils/image.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.489727 upsies-2023.5.25/upsies/utils/imghosts/
+-rw-------   0 ich       (1000) ich       (1000)     1391 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/imghosts/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     7453 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/imghosts/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1147 2021-06-11 16:56:53.000000 upsies-2023.5.25/upsies/utils/imghosts/common.py
+-rw-------   0 ich       (1000) ich       (1000)     1011 2021-10-31 14:15:29.000000 upsies-2023.5.25/upsies/utils/imghosts/dummy.py
+-rw-------   0 ich       (1000) ich       (1000)     1997 2021-11-27 15:46:37.000000 upsies-2023.5.25/upsies/utils/imghosts/freeimage.py
+-rw-------   0 ich       (1000) ich       (1000)     2517 2021-11-26 16:53:37.000000 upsies-2023.5.25/upsies/utils/imghosts/imgbb.py
+-rw-------   0 ich       (1000) ich       (1000)      912 2021-10-19 13:17:48.000000 upsies-2023.5.25/upsies/utils/imghosts/imgbox.py
+-rw-------   0 ich       (1000) ich       (1000)     3154 2023-04-23 11:00:43.000000 upsies-2023.5.25/upsies/utils/imghosts/ptpimg.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.489727 upsies-2023.5.25/upsies/utils/predbs/
+-rw-------   0 ich       (1000) ich       (1000)     1364 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9573 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     4128 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)     2276 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/corruptnet.py
+-rw-------   0 ich       (1000) ich       (1000)    20069 2023-05-19 14:42:15.000000 upsies-2023.5.25/upsies/utils/predbs/multi.py
+-rw-------   0 ich       (1000) ich       (1000)     2174 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/predbclub.py
+-rw-------   0 ich       (1000) ich       (1000)     2333 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/predbde.py
+-rw-------   0 ich       (1000) ich       (1000)     2167 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/predbovh.py
+-rw-------   0 ich       (1000) ich       (1000)     5207 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/predbs/query.py
+-rw-------   0 ich       (1000) ich       (1000)     3434 2023-05-22 08:05:50.000000 upsies-2023.5.25/upsies/utils/predbs/srrdb.py
+-rw-------   0 ich       (1000) ich       (1000)    55868 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/release.py
+-rw-------   0 ich       (1000) ich       (1000)     3931 2023-02-19 13:31:01.000000 upsies-2023.5.25/upsies/utils/signal.py
+-rw-------   0 ich       (1000) ich       (1000)     3922 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/string.py
+-rw-------   0 ich       (1000) ich       (1000)     1908 2023-03-31 14:19:32.000000 upsies-2023.5.25/upsies/utils/subproc.py
+-rw-------   0 ich       (1000) ich       (1000)     7760 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/subtitle.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2021-09-23 10:04:01.000000 upsies-2023.5.25/upsies/utils/timestamp.py
+-rw-------   0 ich       (1000) ich       (1000)    19249 2023-04-25 14:57:27.000000 upsies-2023.5.25/upsies/utils/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    11165 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/types.py
+-rw-------   0 ich       (1000) ich       (1000)     2927 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/update.py
+-rw-------   0 ich       (1000) ich       (1000)    35045 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/video.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.493727 upsies-2023.5.25/upsies/utils/webdbs/
+-rw-------   0 ich       (1000) ich       (1000)     1140 2023-01-16 18:31:24.000000 upsies-2023.5.25/upsies/utils/webdbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     8898 2023-04-28 13:26:45.000000 upsies-2023.5.25/upsies/utils/webdbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)    12546 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/webdbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)    17839 2023-04-28 13:48:23.000000 upsies-2023.5.25/upsies/utils/webdbs/imdb.py
+-rw-------   0 ich       (1000) ich       (1000)    12105 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/webdbs/tmdb.py
+-rw-------   0 ich       (1000) ich       (1000)     9757 2023-04-25 13:55:04.000000 upsies-2023.5.25/upsies/utils/webdbs/tvmaze.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 13:47:13.477728 upsies-2023.5.25/upsies.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     2367 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     3702 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       47 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)      237 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       10 2023-05-25 13:47:13.000000 upsies-2023.5.25/upsies.egg-info/top_level.txt
```

### Comparing `upsies-2023.4.3/LICENSE` & `upsies-2023.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/PKG-INFO` & `upsies-2023.5.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2023.4.3
+Version: 2023.5.25
 Summary: Media metadata aggregator
 Home-page: https://upsies.readthedocs.io
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `upsies-2023.4.3/README.rst` & `upsies-2023.5.25/README.rst`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/setup.py` & `upsies-2023.5.25/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,21 +32,22 @@
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     ],
     python_requires='>=3.8',
     install_requires=[
         'beautifulsoup4==4.*',
         'countryguess==0.*',
-        'aiobtclientapi==1.*',
+        'aiobtclientapi==1.1.*',
         'guessit==3.*,>=3.5.0',
         'httpx==0.*,>=0.20.0',
+        'langcodes==3.*',
         'natsort==8.*',
         'packaging',
         'prompt_toolkit==3.*,>=3.0.6',
         'pyimgbox==1.*',
-        'py-memoize==1.*',
+        'async-lru==2.*',
         'pyxdg',
         'torf==4.*,>=4.1.2',
         'Unidecode==1.3.*',
     ],
     entry_points={'console_scripts': ['upsies = upsies.uis.tui:main']},
 )
```

### Comparing `upsies-2023.4.3/upsies/__init__.py` & `upsies-2023.5.25/upsies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __project_name__ = 'upsies'
 __description__ = 'Media metadata aggregator'
 __homepage__ = 'https://upsies.readthedocs.io'
-__version__ = '2023.04.03'
+__version__ = '2023.05.25'
 __author__ = 'plotski'
 __author_email__ = 'plotski@example.org'
 
 
 def application_setup(config):
     """
     This function should be called by the UI ASAP when `config` is available
```

### Comparing `upsies-2023.4.3/upsies/constants.py` & `upsies-2023.5.25/upsies/constants.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/defaults.py` & `upsies-2023.5.25/upsies/defaults.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import functools
 
-import aiobtclientapi
-
 from . import constants, trackers, utils
 
 defaults = {
     'config': {
         'main': {
             'cache_directory': utils.configfiles.config_value(
                 value=constants.DEFAULT_CACHE_DIRECTORY,
@@ -21,45 +19,43 @@
         },
         'torrent-create': {
             'reuse_torrent_paths': utils.configfiles.config_value(
                 value=[],
                 description=(
                     'List of directories to search for a *.torrent file '
                     'to get piece hashes from instead of generating the '
-                    'pieces hashes from file contents.\n'
+                    'pieces hashes from file contents.'
                 ),
             ),
         },
+        'screenshots': {
+            'optimize': utils.configfiles.config_value(
+                value=utils.types.Choice('default', options=utils.image.optimization_levels),
+                description='Whether to optimize screenshot file sizes',
+            ),
+        },
     },
 
     'trackers': {
         tracker.name: tracker.TrackerConfig()
         for tracker in trackers.trackers()
     },
 
     'imghosts': {
         imghost.name: imghost.default_config
         for imghost in utils.imghosts.imghosts()
     },
 
     'clients': {
-        client.name: {
-            'url': client.URL.default,
-            'username': '',
-            'password': '',
-            'check_after_add': utils.types.Bool('no'),
-        }
-        for client in aiobtclientapi.api_classes()
+        name: utils.btclient.client_defaults(name)
+        for name in utils.btclient.client_names()
     },
 }
 """Defaults for configuration options"""
 
-# Transmission cannot add torrent without verifying it
-defaults['clients']['transmission']['check_after_add'] = utils.types.Bool('yes')
-
 
 @functools.lru_cache(maxsize=None)
 def option_paths():
     """Tuple of configuration option paths (`<section>.<subsection>.<option>`)"""
     return utils.configfiles.ConfigFiles(defaults).paths
```

### Comparing `upsies-2023.4.3/upsies/errors.py` & `upsies-2023.5.25/upsies/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,18 @@
     """Screenshot creation failed"""
 
 
 class ImageResizeError(UpsiesError):
     """Image resizing failed"""
 
 
+class ImageOptimizeError(UpsiesError):
+    """Image optimization failed"""
+
+
 class TorrentError(UpsiesError):
     """Torrent file creation failed"""
 
 
 def SubprocessError(exception, original_traceback):
     """Attach `original_traceback` to `exception`"""
     exception.original_traceback = f'Subprocess traceback:\n{original_traceback.strip()}'
```

### Comparing `upsies-2023.4.3/upsies/jobs/base.py` & `upsies-2023.5.25/upsies/jobs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,18 +404,31 @@
         Calling this method from multiple coroutines simultaneously is safe.
 
         Subclasses must call the parent's method (``super().finish()``).
 
         This method does not block.
         """
         if not self.is_finished:
-            for task in self._tasks:
-                if not task.done():
-                    _log.debug('%s: Cancelling %r', self.name, task)
-                    task.cancel()
+
+            # Do not cancel tasks for now because it can print
+            # RuntimeWarning: coroutine ... was never awaited
+            #
+            # to stderr, for example when release-name command is already
+            # cached:
+            # $ upsies rn ...
+            # $ upsies rn ...  # Same command
+            #
+            # This may cause problems if long tasks are running when we call
+            # finish().
+
+            # for task in self._tasks:
+            #     if not task.done():
+            #         _log.debug('%s: Cancelling %r', self.name, task)
+            #         task.cancel()
+
             self._finished_event.set()
             self.signal.emit('finished', self)
             self._write_cache()
 
     @property
     def is_finished(self):
         """Whether :meth:`finish` was called"""
```

### Comparing `upsies-2023.4.3/upsies/jobs/custom.py` & `upsies-2023.5.25/upsies/jobs/custom.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/dialog.py` & `upsies-2023.5.25/upsies/jobs/dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -350,14 +350,17 @@
     @property
     def text(self):
         """Current text"""
         return getattr(self, '_text', '')
 
     @text.setter
     def text(self, text):
+        # Don't call validator here because it should be possible to set invalid
+        # texts and let the user fix it manually. We only validate when we
+        # commit to `text` (see send()).
         self._text = self._normalizer(str(text))
         self.signal.emit('text', self.text)
 
     @property
     def obscured(self):
         """
         Whether the text is unreadable, e.g. when entering passwords
@@ -387,43 +390,39 @@
         return getattr(self, '_is_loading', False)
 
     @is_loading.setter
     def is_loading(self, is_loading):
         self._is_loading = bool(is_loading)
         self.signal.emit('is_loading', self.is_loading)
 
-    @property
-    def exit_code(self):
-        """
-        Always exit with ``0``
-
-        Instead of exiting with a non-zero exit code, the application should
-        :meth:`warn` the user about invalid values. This is done by providing a
-        `validator`.
-        """
-        if self.is_finished:
-            return 0
-
-    def initialize(self, *, name, label, text='', autofinish=False,
+    def initialize(self, *, name, label,
+                   text='', default=None, finish_on_success=False, nonfatal_exceptions=(),
                    validator=None, normalizer=None, obscured=False, read_only=False):
         """
         Set internal state
 
         :param name: Name for internal use
         :param label: Name for user-facing use
         :param text: Initial text or callable (synchronous or asynchronous)
             which will be called when the job is :meth:`executed
             <upsies.jobs.base.JobBase.execute>`. The return value is used as the
             initial text.
+        :param default: Text to use if `text` is `None`, returns `None` or
+            raises `nonfatal_exceptions`
+        :param finish_on_success: Whether to call :meth:`finish` after setting
+            :attr:`text` to `text`
+
+            .. note:: :meth:`finish` is not called when :attr:`text` is set to
+                      `default`.
+        :param nonfatal_exceptions: Sequence of exception classes that may be
+            raised by `text` without crashing
 
-            .. warning:: If this is a :class:`callable` of any kind, all
-                         exceptions are raised fatally. All expected exceptions
-                         should be handled in the (asynchronous) function.
-        :param autofinish: Automatically :meth:`finish` after `text` is set
-            successfully
+            Fatal exceptions are raised immediately while non-fatal exceptions
+            are passed to :meth:`warn`, and the user can fix the situation
+            manually.
         :param validator: Callable that gets text before job is finished. If
             `ValueError` is raised, it is displayed as a warning instead of
             finishing the job.
         :type validator: callable or None
         :param normalizer: Callable that gets text and returns the new text. It
             is called before `validator`. It should not raise any exceptions.
         :type normalizer: callable or None
@@ -440,102 +439,160 @@
         self.signal.add('is_loading')
         self.signal.add('read_only')
         self.signal.add('obscured')
         self.obscured = obscured
         self.read_only = read_only
 
         if isinstance(text, str):
+            # Set text attribute immediately
             self.text = text
-        else:
-            # Get text from callable when job is executed
-            self._execute_arguments = (text, autofinish)
+
+        # Get text from callable when job is executed
+        self._execute_arguments = (text, default, finish_on_success, nonfatal_exceptions)
 
     def execute(self):
-        text, autofinish = getattr(self, '_execute_arguments', (None, None))
+        text, default, finish_on_success, nonfatal_exceptions = self._execute_arguments
 
         if inspect.isawaitable(text):
             self.attach_task(
-                self.fetch_text(coro=text, finish_on_success=autofinish),
+                self.fetch_text(
+                    coro=text,
+                    default=default,
+                    finish_on_success=finish_on_success,
+                    nonfatal_exceptions=nonfatal_exceptions,
+                )
             )
 
         elif inspect.iscoroutinefunction(text):
             self.attach_task(
-                self.fetch_text(coro=text(), finish_on_success=autofinish),
+                self.fetch_text(
+                    coro=text(),
+                    default=default,
+                    finish_on_success=finish_on_success,
+                    nonfatal_exceptions=nonfatal_exceptions,
+                )
             )
 
-        elif callable(text):
-            try:
-                self.text = text()
-            except BaseException as e:
-                self.exception(e)
-            else:
-                if autofinish:
-                    self.send(self.text)
-
-        elif text is not None:
-            self.text = text
-            if autofinish:
-                self.send(self.text)
+        else:
+            self.set_text(
+                text=text,
+                default=default,
+                finish_on_success=finish_on_success,
+                nonfatal_exceptions=nonfatal_exceptions,
+            )
 
-    def send(self, output):
+    def set_text(self, text, default=None, finish_on_success=False, nonfatal_exceptions=()):
         """
-        Validate `output` before actually sending it
+        Change :attr:`text` value
 
-        Pass `output` to `validator`. If :class:`ValueError` is raised, pass it
-        to :meth:`warn` and do not finish. Otherwise, pass `output` to
-        :meth:`~.base.JobBase.send` and :meth:`~.base.JobBase.finish` this job.
+        :param text: New text value
+
+            If this is callable, it must return the new :attr:`text` or `None`
+            to use `default`
+
+        :param default: Text to use if `text` is `None`, returns `None` or
+            raises `nonfatal_exceptions`
+
+        :param finish_on_success: Whether to call :meth:`finish` after setting
+            :attr:`text` to `text`
+
+            .. note:: :meth:`finish` is not called when :attr:`text` is set to
+                      `default`.
+
+        :param nonfatal_exceptions: Sequence of exception classes that may be
+            raised by `text` without crashing
+
+            Fatal exceptions are raised immediately while non-fatal exceptions
+            are passed to :meth:`warn`, and the user can fix the situation
+            manually.
         """
-        output = self._normalizer(output)
+        self.is_loading = self.read_only = True
         try:
-            self._validator(output)
-        except ValueError as e:
-            self.warn(e)
+            if callable(text):
+                new_text = text()
+            elif text is not None:
+                new_text = str(text)
+            else:
+                new_text = None
+        except Exception as e:
+            self._set_text(default)
+            self._handle_exception(e, nonfatal=nonfatal_exceptions)
         else:
-            super().send(output)
-            super().finish()
+            self._set_text(new_text, default=default, finish=finish_on_success)
+        finally:
+            # Always re-enable text field after we're done messing with it
+            self.is_loading = self.read_only = False
 
-    async def fetch_text(self, coro, default_text=None, finish_on_success=False, nonfatal_exceptions=()):
+    async def fetch_text(self, coro, default=None, finish_on_success=False, nonfatal_exceptions=()):
         """
         Get :attr:`text` from coroutine
 
         :param coro: Coroutine that returns the new :attr:`text` or `None` to
-            use `default_text`
-        :param default_text: String to use if `coro` raises
-            `nonfatal_exceptions` or if `coro` returns `None`
+            use `default`
+
+        :param default: Text to use if `text` is `None`, returns `None` or
+            raises `nonfatal_exceptions`
+
         :param finish_on_success: Whether to call :meth:`finish` after setting
             :attr:`text` to `coro` return value
+
+            .. note:: :meth:`finish` is not called when :attr:`text` is set to
+                      `default`.
+
         :param nonfatal_exceptions: Sequence of exception classes that may be
-            raised by `coro` without indicating failure
+            raised by `coro` without crashing
 
-            Non-fatal exceptions are passed to :meth:`warn` while fatal
-            exceptions are raised.
+            Fatal exceptions are raised immediately while non-fatal exceptions
+            are passed to :meth:`warn`, and the user can fix the situation
+            manually.
         """
         self.is_loading = self.read_only = True
-
         try:
-            text = await coro
-
+            new_text = await coro
         except Exception as e:
-            if default_text is not None:
-                self.text = default_text
-
-            if isinstance(e, nonfatal_exceptions):
-                # Display error and allow user to adjust the default text
-                self.warn(e)
-            else:
-                self.finish()
-                raise e
-
+            _log.debug('CAUGHT EXCEPTION: %r', e)
+            self._set_text(default)
+            self._handle_exception(e, nonfatal=nonfatal_exceptions)
         else:
-            if text is not None:
-                self.text = text
-            elif default_text is not None:
-                self.text = default_text
-
-            # We must call send() because it handles output caching, and it also
-            # finishes the job.
-            if finish_on_success and text is not None:
-                self.send(text)
-
+            self._set_text(new_text, default=default, finish=finish_on_success)
         finally:
             # Always re-enable text field after we're done messing with it
             self.is_loading = self.read_only = False
+
+    def _set_text(self, text, default=None, finish=False):
+        # Fill in text
+        if text is not None:
+            self.text = text
+            # Only finish if the intended text was set
+            if finish:
+                # We must call send() because it handles output caching, and it also
+                # finishes the job.
+                self.send(text)
+
+        elif default is not None:
+            self.text = default
+
+    def _handle_exception(self, exception, nonfatal=()):
+        # Display error and allow user to manually fix the situation
+        if isinstance(exception, nonfatal):
+            self.warn(exception)
+
+        # An exception we didn't expect
+        else:
+            raise exception
+
+    def send(self, output):
+        """
+        Validate `output` before actually sending it
+
+        Pass `output` to `validator`. If :class:`ValueError` is raised, pass it
+        to :meth:`warn` and do not finish. Otherwise, pass `output` to
+        :meth:`~.base.JobBase.send` and :meth:`~.base.JobBase.finish` this job.
+        """
+        output = self._normalizer(output)
+        try:
+            self._validator(output)
+        except ValueError as e:
+            self.warn(e)
+        else:
+            super().send(output)
+            super().finish()
```

### Comparing `upsies-2023.4.3/upsies/jobs/imghost.py` & `upsies-2023.5.25/upsies/jobs/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/mediainfo.py` & `upsies-2023.5.25/upsies/jobs/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/poster.py` & `upsies-2023.5.25/upsies/jobs/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/scene.py` & `upsies-2023.5.25/upsies/jobs/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/screenshots.py` & `upsies-2023.5.25/upsies/jobs/screenshots.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,16 @@
             total number of screenshots as a positional argument.
     """
 
     name = 'screenshots'
     label = 'Screenshots'
     cache_id = None
 
-    def initialize(self, *, content_path, exclude_files=(), timestamps=(), count=0, from_all_videos=False):
+    def initialize(self, *, content_path, exclude_files=(), timestamps=(), count=0,
+                   from_all_videos=False, optimize='default'):
         """
         Set internal state
 
         :param str content_path: Path to file or directory or sequence of paths
         :param exclude_files: Sequence of glob patterns (:class:`str`) and
             :class:`re.Pattern` objects (return value from :func:`re.compile`)
             that are matched against the relative path beneath `content_path`
@@ -51,76 +52,128 @@
         :type timestamps: sequence of "[[H+:]M+:]S+" strings or seconds
         :param count: How many screenshots to make
         :param bool from_all_videos: Whether to take `count` screenshots from
             each video file or only from the first video
 
             See :func:`.video.find_videos` for more information.
 
+        :param optimize: `level` argument for :func:`~image.optimize`
+
+            If this is ``"default"``, missing optimization dependencies are
+            silently ignored.
+
         If `timestamps` and `count` are not given, screenshot positions are
         picked at even intervals. If `count` is larger than the number of
         `timestamps`, more timestamps are added.
         """
         self._content_path = content_path
         self._exclude_files = exclude_files
         self._screenshots_created = 0
         self._screenshots_total = -1
         self._timestamps = timestamps
         self._count = count
         self._from_all_videos = from_all_videos
+        self._optimize = optimize
         self._screenshots_process = None
+        self._optimize_process = None
         self._screenshots_by_file = collections.defaultdict(lambda: [])
         self.signal.add('screenshots_total', record=True)
 
     def execute(self):
         """
         Execute screenshot creation subprocess
 
         The subprocess also picks video file(s) and timestamps.
         """
+        if self._optimize not in ('none', None):
+            self._execute_screenshots_process()
+            self._execute_optimize_process()
+        else:
+            self._execute_screenshots_process()
+
+    def _execute_screenshots_process(self):
         self._screenshots_process = daemon.DaemonProcess(
-            name=self.name,
+            name='_screenshots_process',
             target=_screenshots_process,
             kwargs={
                 'content_path': self._content_path,
                 'exclude_files': self._exclude_files,
                 'timestamps': self._timestamps,
                 'count': self._count,
                 'from_all_videos': self._from_all_videos,
                 'output_dir': self.home_directory,
                 'overwrite': self.ignore_cache,
             },
             info_callback=self._handle_info,
             error_callback=self._handle_error,
-            finished_callback=self.finish,
         )
         self._screenshots_process.start()
 
-    def finish(self):
-        """Terminate screenshot creation subprocess and finish"""
-        if self._screenshots_process:
-            self._screenshots_process.stop()
-        super().finish()
+    def _execute_optimize_process(self):
+        self._optimize_process = daemon.DaemonProcess(
+            name='_optimize_process',
+            target=_optimize_process,
+            kwargs={
+                # Use default optimization level if None is provided
+                'level': self._optimize,
+                # Ignore missing dependecy if we do "default" optimization
+                'ignore_dependency_error': (
+                    True
+                    if self._optimize == 'default' else
+                    False
+                ),
+            },
+            info_callback=self._handle_info,
+            error_callback=self._handle_error,
+        )
+        self._optimize_process.start()
 
     def _handle_info(self, info):
         if not self.is_finished:
             if 'screenshots_total' in info:
                 self._screenshots_total = info['screenshots_total']
                 self.signal.emit('screenshots_total', self._screenshots_total)
 
             if 'screenshot_path' in info:
-                self._screenshots_created += 1
                 self._screenshots_by_file[info['video_path']].append(info['screenshot_path'])
-                self.send(info['screenshot_path'])
+
+                if self._optimize_process:
+                    _log.debug('Optimizing %s: %.2f KiB',
+                               info['screenshot_path'],
+                               fs.file_size(info['screenshot_path']) / 1024)
+                    self._optimize_process.send(daemon.MsgType.info, info['screenshot_path'])
+
+                else:
+                    self._screenshots_created += 1
+                    self.send(info['screenshot_path'])
+
+            elif 'optimized_screenshot_path' in info:
+                _log.debug('Optimized %s: %.2f KiB',
+                           info['optimized_screenshot_path'],
+                           fs.file_size(info['optimized_screenshot_path']) / 1024)
+                self._screenshots_created += 1
+                self.send(info['optimized_screenshot_path'])
+
+            if self.screenshots_created == self.screenshots_total:
+                self.finish()
 
     def _handle_error(self, error):
         if isinstance(error, BaseException):
             self.exception(error)
         else:
             self.error(error)
 
+    def finish(self):
+        """Terminate screenshot creation subprocess and finish"""
+        if self._screenshots_process:
+            self._screenshots_process.stop()
+        if self._optimize_process:
+            self._optimize_process.stop()
+        super().finish()
+
     @property
     def exit_code(self):
         """`0` if all screenshots were made, `1` otherwise, `None` if unfinished"""
         if self.is_finished:
             if self.screenshots_total < 0:
                 # Job is finished but _screenshots_process() never sent us
                 # timestamps. That means we're either using previously cached
@@ -298,14 +351,49 @@
         )
     except SystemExit:
         # _maybe_terminate signals termination by raising SystemExit. This
         # shouldn't cause any issues as long as we actually exit here.
         pass
 
 
+def _optimize_process(output_queue, input_queue, *, level, ignore_dependency_error):
+    # Get as many queued screenshots as possible. Check if there's a termination
+    # sentinel before optimizing each screenshot to avoid processing all the
+    # screenshots before Ctrl-C takes effect.
+    msgs = []
+    while True:
+        new_msgs = _read_queue_until_empty(input_queue=input_queue)
+        msgs.extend(new_msgs)
+
+        if any(typ is daemon.MsgType.terminate for typ, msg_ in msgs):
+            break
+
+        elif msgs:
+            typ_, screenshot_file = msgs.pop(0)
+            try:
+                image.optimize(screenshot_file, level=level)
+
+            except errors.ImageOptimizeError as e:
+                output_queue.put((daemon.MsgType.error, str(e)))
+
+            except errors.DependencyError as e:
+                if ignore_dependency_error:
+                    # Act like we optimized `screenshot_file`
+                    output_queue.put((daemon.MsgType.info, {
+                        'optimized_screenshot_path': screenshot_file,
+                    }))
+                else:
+                    raise e
+
+            else:
+                output_queue.put((daemon.MsgType.info, {
+                    'optimized_screenshot_path': screenshot_file,
+                }))
+
+
 def _get_video_files(output_queue, *, content_path, exclude_files):
     # Make list of appropriate video file(s) from `content_path`
     try:
         filtered_files = torrent.filter_files(content_path, exclude=exclude_files)
         return video.filter_main_videos(filtered_files)
     except errors.ContentError as e:
         output_queue.put((daemon.MsgType.error, str(e)))
@@ -418,7 +506,18 @@
     try:
         typ, msg = input_queue.get_nowait()
     except queue.Empty:
         pass
     else:
         if typ == daemon.MsgType.terminate:
             raise SystemExit('Terminated')
+
+
+def _read_queue_until_empty(*, input_queue):
+    msgs = []
+    while True:
+        try:
+            typ, msg = input_queue.get(timeout=0.01)
+        except queue.Empty:
+            return msgs
+        else:
+            msgs.append((typ, msg))
```

### Comparing `upsies-2023.4.3/upsies/jobs/set.py` & `upsies-2023.5.25/upsies/jobs/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/submit.py` & `upsies-2023.5.25/upsies/jobs/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/jobs/torrent.py` & `upsies-2023.5.25/upsies/jobs/torrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,22 +126,23 @@
 
     def _start_torrent_creation_process(self, announce_url):
         self._torrent_process = daemon.DaemonProcess(
             name=self.name,
             target=_torrent_process,
             kwargs={
                 'content_path': self._content_path,
-                'torrent_path': self._torrent_path,
-                'piece_size_min': self._tracker.TrackerJobs.torrent_piece_size_min,
-                'piece_size_max': self._tracker.TrackerJobs.torrent_piece_size_max,
-                'reuse_torrent_path': self._reuse_torrent_path,
-                'use_cache': not self.ignore_cache,
                 'announce': announce_url,
                 'source': self._tracker.options['source'],
+                'torrent_path': self._torrent_path,
                 'exclude': self._exclude_files,
+                'use_cache': not self.ignore_cache,
+                'reuse_torrent_path': self._reuse_torrent_path,
+                'randomize_infohash': self._tracker.options['randomize_infohash'],
+                'piece_size_calculator': self._tracker.calculate_piece_size,
+                'piece_size_min_max_calculator': self._tracker.calculate_piece_size_min_max,
             },
             init_callback=self._handle_files,
             info_callback=self._handle_info_update,
             error_callback=self._handle_error,
             result_callback=self._handle_torrent_created,
             finished_callback=self.finish,
         )
@@ -260,48 +261,37 @@
             argument.
     """
 
     name = 'add-torrent'
     label = 'Add Torrent'
     cache_id = None  # Don't cache output
 
-    def initialize(self, *, client_api, download_path=None, check_after_add=False, enqueue=()):
+    def initialize(self, *, btclient, enqueue=()):
         """
         Set internal state
 
-        :param client_api: :class:`aiobtclientapi.clients.APIBase` subclass
-            instance
-        :param download_path: Path to the torrent's download location or `None`
-            to use the client's default path
-        :param bool check_after_add: Whether to hash torrent's existing files
-            after torrent is added
+        :param btclient: :class:`~.btclient.BtClient` instance
         :param enqueue: Sequence of torrent file paths to add
 
         If `enqueue` is given and not empty, this job is finished as soon as its
         last item is added.
         """
-        self._client_api = client_api
-        self._download_path = download_path
-        self._check_after_add = check_after_add
+        self._btclient = btclient
         self.signal.add('adding')
         self.signal.add('added')
         self.signal.register('adding', lambda tp: setattr(self, 'info', f'Adding {fs.basename(tp)}'))
         self.signal.register('added', lambda _: setattr(self, 'info', ''))
         self.signal.register('finished', lambda _: setattr(self, 'info', ''))
         self.signal.register('error', lambda _: setattr(self, 'info', ''))
 
     async def handle_input(self, torrent_path):
-        _log.debug('Adding %s to %s', torrent_path, self._client_api.name)
+        _log.debug('Adding %s to %s', torrent_path, self._btclient.name)
         self.signal.emit('adding', torrent_path)
 
-        response = await self._client_api.add(
-            torrent_path,
-            location=self._download_path,
-            verify=self._check_after_add,
-        )
+        response = await self._btclient.add_torrent(torrent_path)
 
         for warning in response.warnings:
             self.warn(warning)
 
         for error in response.errors:
             self.error(error)
```

### Comparing `upsies-2023.4.3/upsies/jobs/webdb.py` & `upsies-2023.5.25/upsies/jobs/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/__init__.py` & `upsies-2023.5.25/upsies/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/base/_howto.py` & `upsies-2023.5.25/upsies/trackers/base/_howto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 Standardized configuration and setup howto
 """
 
-import aiobtclientapi
-
-from ... import utils
+from ... import __project_name__, utils
 
 
 class Howto:
     def __init__(self, tracker_cls):
         self._tracker_cls = tracker_cls
         self._section = 0
 
@@ -39,50 +37,51 @@
     @property
     def screenshots(self):
         return self._autobump((
             (
                 f'{self._section}. Screenshots (Optional)\n'
                 '\n'
                 f'   {self._section}.1 Specify how many screenshots to make.\n'
-                f'       $ upsies set trackers.{self._tracker_cls.name}.screenshots NUMBER_OF_SCREENSHOTS\n'
+                f'       $ {__project_name__} set trackers.{self._tracker_cls.name}.screenshots NUMBER_OF_SCREENSHOTS\n'
             ),
             (
                 f'   {self._section}.2 Specify where to host images.\n'
-                f'       $ upsies set trackers.{self._tracker_cls.name}.image_host IMAGE_HOST\n'
+                f'       $ {__project_name__} set trackers.{self._tracker_cls.name}.image_host IMAGE_HOST\n'
                 f'       Supported services: ' + ', '.join(utils.imghosts.imghost_names()) + '\n'
                 '\n'
                 f'   {self._section}.3 Configure image hosting service.\n'
-                f'       $ upsies upload-images IMAGE_HOST --help\n'
+                f'       $ {__project_name__} upload-images IMAGE_HOST --help\n'
             ),
         ))
 
     @property
     def autoseed(self):
         return self._autobump((
             (
                 f'{self._section}. Add Uploaded Torrents To Client (Optional)\n'
                 '\n'
                 f'   {self._section}.1 Specify which client to add uploaded torrents to.\n'
-                f'       $ upsies set trackers.{self._tracker_cls.name}.add_to CLIENT_NAME\n'
-                f'       Supported clients: ' + ', '.join(aiobtclientapi.client_names()) + '\n'
+                f'       $ {__project_name__} set trackers.{self._tracker_cls.name}.add_to CLIENT_NAME\n'
+                f'       Supported clients: ' + ', '.join(utils.btclient.client_names()) + '\n'
             ),
             (
                 f'   {self._section}.2 Specify your client connection.\n'
-                '       $ upsies set clients.CLIENT_NAME.url URL\n'
-                '       $ upsies set clients.CLIENT_NAME.username USERNAME\n'
-                '       $ upsies set clients.CLIENT_NAME.password PASSWORD\n'
+                f'       $ {__project_name__} set clients.CLIENT_NAME.url URL\n'
+                f'       $ {__project_name__} set clients.CLIENT_NAME.username USERNAME\n'
+                f'       $ {__project_name__} set clients.CLIENT_NAME.password PASSWORD\n'
                 '\n'
                 f'{self._section + 1}. Copy Uploaded Torrents To Directory (Optional)\n'
                 '\n'
-                f'   $ upsies set trackers.{self._tracker_cls.name}.copy_to /path/to/directory\n'
+                f'   $ {__project_name__} set trackers.{self._tracker_cls.name}.copy_to /path/to/directory\n'
             ),
         ))
 
     @property
     def upload(self):
         return self._autobump((
             (
                 f'{self._section}. Upload\n'
                 '\n'
-                f'   $ upsies submit {self._tracker_cls.name} /path/to/content\n'
+                f'   $ {__project_name__} submit {self._tracker_cls.name} --help\n'
+                f'   $ {__project_name__} submit {self._tracker_cls.name} /path/to/content\n'
             ),
         ))
```

### Comparing `upsies-2023.4.3/upsies/trackers/base/config.py` & `upsies-2023.5.25/upsies/trackers/base/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 Base class for tracker configuration
 """
 
-import aiobtclientapi
-
 from ... import utils
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class TrackerConfigBase(dict):
@@ -19,26 +17,36 @@
 
     # Options that are available for all trackers
     _common_defaults = {
         'source': utils.configfiles.config_value(
             value='',
             description='Value of the "source" field in generated torrents.',
         ),
+        'randomize_infohash': utils.configfiles.config_value(
+            value=utils.types.Bool('no'),
+            description=(
+                'Whether the info hash of generated torrents is randomized '
+                'by including a random number in the metadata.\n'
+                'WARNING: The tracker may choke on the non-standard field '
+                'or remove the random number, forcing you to manually download '
+                'the torrent.'
+            ),
+        ),
         'exclude': utils.configfiles.config_value(
             value=utils.types.ListOf(
                 item_type=utils.types.RegEx,
                 iterable=(),
             ),
             description='List of regular expressions. Matching files are excluded from generated torrents.',
         ),
         'add_to': utils.configfiles.config_value(
             value=utils.types.Choice(
                 value='',
                 empty_ok=True,
-                options=aiobtclientapi.client_names(),
+                options=utils.btclient.client_names(),
             ),
             description='BitTorrent client to add torrent to after submission.',
         ),
         'copy_to': utils.configfiles.config_value(
             value='',
             description='Directory path to copy torrent to after submission.',
         ),
```

### Comparing `upsies-2023.4.3/upsies/trackers/base/jobs.py` & `upsies-2023.5.25/upsies/trackers/base/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Abstract base class for tracker jobs
 """
 
 import abc
 import builtins
 import collections
 import functools
-import os
 import pathlib
 
 from ... import errors, jobs, utils
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
@@ -30,24 +29,25 @@
     Subclasses that need to run background tasks should pass them to
     :meth:`.JobBase.attach_task` or to :meth:`.TrackerBase.attach_task`.
 
     For a description of the arguments see the corresponding properties.
     """
 
     def __init__(self, *, content_path, tracker,
-                 reuse_torrent_path=None, torrent_destination=None, check_after_add=False,
-                 exclude_files=(), options=None, image_host=None,
-                 bittorrent_client=None, common_job_args=None):
+                 reuse_torrent_path=None, exclude_files=(),
+                 btclient=None, torrent_destination=None,
+                 screenshots_optimization=None, image_host=None,
+                 options=None, common_job_args=None):
         self._content_path = content_path
         self._reuse_torrent_path = reuse_torrent_path
         self._tracker = tracker
+        self._screenshots_optimization = screenshots_optimization
         self._image_host = image_host
-        self._bittorrent_client = bittorrent_client
+        self._btclient = btclient
         self._torrent_destination = torrent_destination
-        self._check_after_add = check_after_add
         self._exclude_files = exclude_files
         self._common_job_args = common_job_args or {}
         self._options = options or {}
         self._signal = utils.signal.Signal('warning', 'error', 'exception')
 
     @property
     def content_path(self):
@@ -82,19 +82,14 @@
         Where to copy the generated torrent file to or `None`
 
         This is the same object that was passed as a initialization argument.
         """
         return self._torrent_destination
 
     @property
-    def check_after_add(self):
-        """Whether to hash existing files after adding the torrent to a client"""
-        return self._check_after_add
-
-    @property
     def exclude_files(self):
         """
         Sequence of glob and regular expression patterns to exclude from the
         generated torrent
 
         See the ``exclude_files`` argument of
         :meth:`.CreateTorrentJob.initialize`.
@@ -119,21 +114,21 @@
         :class:`~.base.ImageHostBase` instance or `None`
 
         This is the same object that was passed as a initialization argument.
         """
         return self._image_host
 
     @property
-    def bittorrent_client(self):
+    def btclient(self):
         """
-        :class:`~.base.ClientApiBase` instance or `None`
+        :class:`~.btclient.BtClient` instance or `None`
 
         This is the same object that was passed as a initialization argument.
         """
-        return self._bittorrent_client
+        return self._btclient
 
     def common_job_args(self, **overload):
         """
         Keyword arguments that are passed to all jobs or empty `dict`
 
         :param overload: Keyword arguments add or replace values from the
             initialization argument
@@ -314,54 +309,49 @@
         cached output from another tracker's job with the same name.
 
         Standard jobs have names so that cached output will be re-used by other
         trackers if possible. This function is mainly for unique and custom jobs
         that are only used for one tracker but might share the same name with
         other trackers.
         """
-        prefix = f'{self.tracker.name}-'
-        if name.startswith(prefix):
+        suffix = f'.{self.tracker.name}'
+        if name.endswith(suffix):
             return name
         else:
-            return f'{prefix}{name}'
+            return f'{name}{suffix}'
 
     @functools.cached_property
     def create_torrent_job(self):
         """:class:`~.jobs.torrent.CreateTorrentJob` instance"""
         return jobs.torrent.CreateTorrentJob(
             content_path=self.content_path,
             reuse_torrent_path=self.reuse_torrent_path,
             tracker=self.tracker,
             exclude_files=self.exclude_files,
             precondition=self.make_precondition('create_torrent_job'),
             **self.common_job_args(),
         )
 
-    torrent_piece_size_min = 2**20  # 1 MiB
-    """Minimum torrent piece size for this tracker"""
-
-    torrent_piece_size_max = 16 * 2**20  # 16 MiB
-    """Maximum torrent piece size for this tracker"""
-
     @functools.cached_property
     def add_torrent_job(self):
         """:class:`~.jobs.torrent.AddTorrentJob` instance"""
-        if self.bittorrent_client and self.create_torrent_job:
+        if self._btclient and self.create_torrent_job:
             add_torrent_job = jobs.torrent.AddTorrentJob(
                 autostart=False,
-                client_api=self.bittorrent_client,
-                download_path=utils.fs.dirname(os.path.abspath(self.content_path)),
-                check_after_add=self.check_after_add,
+                btclient=self._btclient,
                 precondition=self.make_precondition('add_torrent_job'),
                 **self.common_job_args(),
             )
+
             # Pass CreateTorrentJob output to AddTorrentJob input.
             self.create_torrent_job.signal.register('output', add_torrent_job.enqueue)
+
             # Tell AddTorrentJob to finish the current upload and then finish.
             self.create_torrent_job.signal.register('finished', self.finalize_add_torrent_job)
+
             return add_torrent_job
 
     def finalize_add_torrent_job(self, _):
         self.add_torrent_job.finalize()
 
     @functools.cached_property
     def copy_torrent_job(self):
@@ -428,14 +418,15 @@
 
         This is a convenience wrapper around :meth:`.ReleaseName.fetch_info` and
         :meth:`.TextFieldJob.fetch_text`.
         """
         await self.release_name_job.fetch_text(
             coro=self.release_name.fetch_info(webdb=webdb, webdb_id=webdb_id),
             nonfatal_exceptions=(errors.RequestError,),
+            default=str(self.release_name),
         )
         _log.debug('Updated release name: %s', self.release_name)
 
     @functools.cached_property
     def imdb_job(self):
         """:class:`~.jobs.webdb.WebDbSearchJob` instance"""
         return jobs.webdb.WebDbSearchJob(
@@ -540,33 +531,35 @@
         await self.update_release_name_from(webdb, webdb_id)
 
     @functools.cached_property
     def screenshots_job(self):
         """
         :class:`~.jobs.screenshots.ScreenshotsJob` instance
 
-        The number of screenshots to make is taken from the ``screenshots``
-        value in :attr:`options`.
+        The number of screenshots to make is taken the :attr:`screenshots_count`
+        attribute.
         """
         return jobs.screenshots.ScreenshotsJob(
             content_path=self.content_path,
             exclude_files=self.exclude_files,
             count=self.screenshots_count,
             from_all_videos=self.screenshots_from_all_videos,
+            optimize=self._screenshots_optimization,
             precondition=self.make_precondition('screenshots_job'),
             **self.common_job_args(),
         )
 
     @property
     def screenshots_count(self):
         """
         How many screenshots to make
 
         The default implementation uses :attr:`options`\\ ``["screenshots"]``
-        with `None` as the default value.
+        with `None` as the default value, which creates a default number of
+        screenshots.
         """
         return self.options.get('screenshots')
 
     @property
     def screenshots_from_all_videos(self):
         """
         Whether to make :attr:`screenshots_count` screenshots from all
```

### Comparing `upsies-2023.4.3/upsies/trackers/base/tracker.py` & `upsies-2023.5.25/upsies/trackers/base/tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,14 +153,30 @@
         """Whether a user session is active"""
         return getattr(self, '_is_logged_in', False)
 
     @abc.abstractmethod
     async def get_announce_url(self):
         """Get announce URL from tracker website"""
 
+    calculate_piece_size = None
+    """
+    :class:`staticmethod` that takes a torrent's content size and returns
+    the corresponding piece size
+
+    If this is `None`, the default implementation is used.
+    """
+
+    calculate_piece_size_min_max = None
+    """
+    :class:`staticmethod` that takes a torrent's content size and returns
+    the corresponding allowed minimum and maximum piece sizes
+
+    If this is `None`, the default implementation is used.
+    """
+
     @abc.abstractmethod
     async def upload(self, tracker_jobs):
         """
         Upload torrent and other metadata from jobs
 
         :param TrackerJobsBase tracker_jobs: :attr:`TrackerJobs` instance
         """
```

### Comparing `upsies-2023.4.3/upsies/trackers/bhd/config.py` & `upsies-2023.5.25/upsies/trackers/bhd/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/bhd/jobs.py` & `upsies-2023.5.25/upsies/trackers/bhd/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             self.scene_check_job,
             self.tags_job,
         )
 
     @property
     def isolated_jobs(self):
         """
-        Sequence of attribute names (e.g. "imdb_job") that were singled out by the
-        user, e.g. with a CLI argument
+        Sequence of job attribute names (e.g. "imdb_job") that were singled
+        out by the user, e.g. with a CLI argument
         """
         if self.options.get('only_description', False):
             return self.get_job_and_dependencies(
                 self.description_job,
                 # `screenshots_job` is needed by `upload_screenshots_job`, but
                 # `upload_screenshots_job` is a `QueueJobBase`, which doesn't
                 # know anything about the job it gets input from and therefore
@@ -195,15 +195,15 @@
             precondition=self.make_precondition('description_job'),
             prejobs=(
                 self.upload_screenshots_job,
                 self.mediainfo_job,
             ),
             text=self.generate_description,
             hidden=True,
-            autofinish=True,
+            finish_on_success=True,
             read_only=True,
             **self.common_job_args(ignore_cache=True),
         )
 
     image_host_config = {
         'common': {'thumb_width': 350},
     }
@@ -278,15 +278,15 @@
             label='Tags',
             precondition=self.make_precondition('tags_job'),
             prejobs=(
                 self.release_name_job,
                 self.scene_check_job,
             ),
             text=self.generate_tags,
-            autofinish=True,
+            finish_on_success=True,
             read_only=True,
             **self.common_job_args(),
         )
 
     async def generate_tags(self):
         assert self.release_name_job.is_finished
         assert self.scene_check_job.is_finished
```

### Comparing `upsies-2023.4.3/upsies/trackers/bhd/tracker.py` & `upsies-2023.5.25/upsies/trackers/bhd/tracker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Concrete :class:`~.base.TrackerBase` subclass for BHD
 """
 
 import re
 
-from ... import errors, utils
+from ... import __project_name__, errors, utils
 from ..base import TrackerBase
 from .config import BhdTrackerConfig
 from .jobs import BhdTrackerJobs
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
@@ -18,31 +18,32 @@
     label = 'BHD'
 
     setup_howto_template = (
         '{howto.introduction}\n'
         '\n'
         '{howto.current_section}. Announce Passkey\n'
         '\n'
-        '   {howto.current_section}.1 On the website, go to My Security -> Passkey and copy\n'
-        '       your personal PASSKEY.\n'
+        '   {howto.current_section}.1 On the website, go to My Settings -> Security -> Passkey\n'
+        '       and copy your personal PASSKEY.\n'
         '   {howto.current_section}.2 $ upsies set trackers.bhd.announce_passkey PASSKEY\n'
         '{howto.bump_section}'
         '\n'
         '{howto.current_section}. API key\n'
         '\n'
-        '   {howto.current_section}.1 On the website, go to My Security -> API Key and copy\n'
-        '       your personal API_KEY.\n'
+        '   {howto.current_section}.1 On the website, go to My Settings -> Security -> API Key\n'
+        '       and copy your personal API_KEY.\n'
         '   {howto.current_section}.2 $ upsies set trackers.bhd.apikey API_KEY\n'
         '{howto.bump_section}'
         '\n'
         '{howto.screenshots}\n'
         '\n'
         '{howto.autoseed}\n'
         '\n'
         '{howto.upload}\n'
+        f'   $ {__project_name__} submit bhd /path/to/content --draft\n'
     )
 
     TrackerConfig = BhdTrackerConfig
     TrackerJobs = BhdTrackerJobs
 
     async def _login(self):
         pass
@@ -144,7 +145,30 @@
 
     def _torrent_page_url_from_download_url(self, torrent_download_url):
         # Download URL: .../torrent/download/<torrent name>.123456.d34db33f
         # Website URL: .../torrents/<torrent name>.123456
         torrent_page_url = torrent_download_url.replace('/torrent/download/', '/torrents/')
         torrent_page_url = re.sub(r'\.[a-zA-Z0-9]+$', '', torrent_page_url)
         return torrent_page_url
+
+    @staticmethod
+    def calculate_piece_size(bytes):
+        # Upload page says:
+        #
+        #  4 -   8 GB = 1 MB piece size
+        #  8 -  16 GB = 2 MB piece size
+        # 16 -  72 GB = 4 MB piece size
+        # 72 - 190 GB = 8 MB piece size
+        #
+        # We assume "[MG]B" means "[MG]iB" because piece sizes in MB would be
+        # considered invalid by most BitTorrent clients.
+
+        piece_size_map = {
+            (0, 8 * 1024 * 1024 * 1024 - 1): 1 * 1024 * 1024,                         # 1 MiB
+            (8 * 1024 * 1024 * 1024, 16 * 1024 * 1024 * 1024 - 1): 2 * 1024 * 1024,   # 2 MiB
+            (16 * 1024 * 1024 * 1024, 72 * 1024 * 1024 * 1024 - 1): 4 * 1024 * 1024,  # 4 MiB
+            (72 * 1024 * 1024 * 1024, float('inf')): 8 * 1024 * 1024,                 # 8 MiB
+        }
+
+        for (min_size, max_size), piece_size in piece_size_map.items():
+            if min_size <= bytes <= max_size:
+                return piece_size
```

### Comparing `upsies-2023.4.3/upsies/trackers/dummy.py` & `upsies-2023.5.25/upsies/trackers/dummy.py`

 * *Files 18% similar despite different names*

```diff
@@ -48,17 +48,14 @@
             },
         },
     }
 
 
 class DummyTrackerJobs(base.TrackerJobsBase):
 
-    torrent_piece_size_min = 4 * 2**20  # 4 MiB
-    torrent_piece_size_max = 8 * 2**20  # 8 MiB
-
     @functools.cached_property
     def jobs_before_upload(self):
         return (
             self.create_torrent_job,
             self.screenshots_job,
             self.upload_screenshots_job,
             self.poster_job,
```

### Comparing `upsies-2023.4.3/upsies/trackers/mtv/config.py` & `upsies-2023.5.25/upsies/trackers/mtv/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/mtv/jobs.py` & `upsies-2023.5.25/upsies/trackers/mtv/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
 class MtvTrackerJobs(TrackerJobsBase):
 
-    torrent_piece_size_max = 8 * 2**20  # 8 MiB
-
     @functools.cached_property
     def jobs_before_upload(self):
         return (
             # Background jobs
             self.create_torrent_job,
             self.mediainfo_job,
             self.screenshots_job,
@@ -145,21 +143,21 @@
 
         Unlike :attr:`~.TrackerJobsBase.release_name_job`, this uses the
         original scene release name for movie and episode scene releases.
         """
         return jobs.dialog.TextFieldJob(
             name=self.get_job_name('title'),
             label='Title',
+            precondition=self.make_precondition('title_job'),
             prejobs=(
                 self.category_job,
                 self.scene_check_job,
                 self.imdb_job,
             ),
             text=self.generate_title,
-            precondition=self.make_precondition('title_job'),
             **self.common_job_args(),
         )
 
     async def generate_title(self):
         assert self.scene_check_job.is_finished
         assert self.imdb_job.is_finished
 
@@ -180,21 +178,21 @@
     }
 
     @functools.cached_property
     def description_job(self):
         return jobs.dialog.TextFieldJob(
             name=self.get_job_name('description'),
             label='Description',
+            precondition=self.make_precondition('description_job'),
             prejobs=(
                 self.mediainfo_job,
                 self.upload_screenshots_job,
             ),
             text=self.generate_description,
-            precondition=self.make_precondition('description_job'),
-            autofinish=True,
+            finish_on_success=True,
             read_only=True,
             hidden=True,
             # Don't cache job output because the number of screenshots can be
             # changed by the user between runs.
             **self.common_job_args(ignore_cache=True),
         )
```

### Comparing `upsies-2023.4.3/upsies/trackers/mtv/tracker.py` & `upsies-2023.5.25/upsies/trackers/mtv/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,22 @@
                     raise errors.RequestError(f'Failed to find announce URL - set it manually: {cmd}')
             finally:
                 # TODO: If we logout, we can't login again for some reason. The
                 #       error message is: Unauthorized: Expired session await
                 # self.logout()
                 pass
 
+    @staticmethod
+    def calculate_piece_size_min_max(bytes):
+        """Anything from 32 KiB to 8 MiB is fine, regardless of content size"""
+        return (
+            32 * 1024,        # 32 KiB
+            8 * (1024 ** 2),  # 8 MiB
+        )
+
     async def upload(self, tracker_jobs):
         autofill_post_data = await self._make_autofill_request(tracker_jobs)
         _log.debug('Autofill data: %r', autofill_post_data)
 
         torrent_page_url = await self._make_upload_request(tracker_jobs, autofill_post_data)
         _log.debug('Torrent page URL: %r', torrent_page_url)
         return torrent_page_url
```

### Comparing `upsies-2023.4.3/upsies/trackers/nbl/config.py` & `upsies-2023.5.25/upsies/trackers/nbl/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/nbl/jobs.py` & `upsies-2023.5.25/upsies/trackers/nbl/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/nbl/tracker.py` & `upsies-2023.5.25/upsies/trackers/nbl/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/trackers/ptp/config.py` & `upsies-2023.5.25/upsies/trackers/ptp/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,9 +47,14 @@
             ('--screenshots', '--ss'): {
                 'help': 'How many screenshots to make per video file',
                 'type': argtypes.number_of_screenshots(min=1, max=10),
             },
             ('--upload-token', '--ut'): {
                 'help': 'Upload token from staff',
             },
+            ('--only-description', '--od'): {
+                'help': 'Only generate description (do not upload anything)',
+                'action': 'store_true',
+                'group': 'generate-metadata',
+            },
         },
     }
```

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/__init__.py` & `upsies-2023.5.25/upsies/uis/tui/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/base.py` & `upsies-2023.5.25/upsies/uis/tui/commands/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/mediainfo.py` & `upsies-2023.5.25/upsies/uis/tui/commands/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/poster.py` & `upsies-2023.5.25/upsies/uis/tui/commands/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/release_name.py` & `upsies-2023.5.25/upsies/uis/tui/commands/release_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     def _update_release_name(self, imdb_id):
         self.release_name_job.attach_task(
             self.release_name_job.fetch_text(
                 coro=self.release_name.fetch_info(webdb=self.imdb, webdb_id=imdb_id),
                 nonfatal_exceptions=(
                     errors.RequestError,
                 ),
+                default=str(self.release_name),
             ),
         )
 
     @functools.cached_property
     def imdb_job(self):
         # To be able to fetch the original title, year, etc, we need to ask for
         # an ID first. IMDb seems to be best.
```

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/scene.py` & `upsies-2023.5.25/upsies/uis/tui/commands/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/screenshots.py` & `upsies-2023.5.25/upsies/uis/tui/commands/screenshots.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,14 +45,20 @@
             'help': 'How many screenshots to make in total',
             'default': 0,
         },
         ('--from-all-videos', '-a'): {
             'action': 'store_true',
             'help': 'Make NUMBER screenshots from each video file beneath CONTENT',
         },
+        ('--optimize', '--opt'): {
+            'type': utils.argtypes.one_of(utils.image.optimization_levels),
+            'default': None,
+            'metavar': 'LEVEL',
+            'help': f'File size optimization level: {", ".join(utils.image.optimization_levels)}',
+        },
         ('--upload-to', '-u'): {
             'type': utils.argtypes.imghost,
             'metavar': 'IMAGEHOST',
             'help': ('Case-insensitive name of image hosting service\n'
                      'Supported services: ' + ', '.join(utils.imghosts.imghost_names())),
         },
         ('--output-directory', '-o'): {
@@ -72,14 +78,19 @@
             exclude_files=(
                 tuple(self.args.exclude_files)
                 + tuple(self.args.exclude_files_regex)
             ),
             timestamps=self.args.timestamps,
             count=self.args.number,
             from_all_videos=self.args.from_all_videos,
+            optimize=(
+                self.args.optimize
+                if self.args.optimize is not None else
+                self.config['config']['screenshots']['optimize']
+            ),
         )
 
     @functools.cached_property
     def upload_screenshots_job(self):
         if self.args.upload_to:
             imghost_job = jobs.imghost.ImageHostJob(
                 home_directory=self.home_directory,
```

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/set.py` & `upsies-2023.5.25/upsies/uis/tui/commands/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/submit.py` & `upsies-2023.5.25/upsies/uis/tui/commands/submit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Generate all required metadata and upload to tracker
 """
 
 import functools
-
-import aiobtclientapi
+import os
 
 from .... import __project_name__, constants, jobs, trackers, utils
 from . import base
 
 
 class submit(base.CommandBase):
     """Generate all required metadata and upload to TRACKER"""
@@ -76,15 +75,15 @@
                         'type': utils.argtypes.existing_path,
                         'default': (),
                     },
                     ('--add-to', '-a'): {
                         'type': utils.argtypes.client,
                         'metavar': 'CLIENT',
                         'help': ('Case-insensitive BitTorrent client name\n'
-                                 'Supported clients: ' + ', '.join(aiobtclientapi.client_names())),
+                                 'Supported clients: ' + ', '.join(utils.btclient.client_names())),
                     },
                     ('--copy-to', '-c'): {
                         'metavar': 'PATH',
                         'help': 'Copy the created torrent to PATH (file or directory)',
                     },
                 },
                 # Custom arguments defined by tracker for this command
@@ -144,18 +143,18 @@
             options=self.tracker_options,
             content_path=self.args.CONTENT,
             reuse_torrent_path=(
                 tuple(self.args.reuse_torrent)
                 + tuple(self.config['config']['torrent-create']['reuse_torrent_paths'])
             ),
             tracker=self.tracker,
+            screenshots_optimization=self.config['config']['screenshots']['optimize'],
             image_host=self._get_imghost(),
-            bittorrent_client=self._get_btclient(),
+            btclient=self._get_btclient(),
             torrent_destination=self._get_torrent_destination(),
-            check_after_add=self._get_check_after_add(),
             exclude_files=(
                 tuple(self.config['trackers'][self.tracker.name]['exclude'])
                 + tuple(self.args.exclude_files)
                 + tuple(self.args.exclude_files_regex)
             ),
             common_job_args={
                 'home_directory': self.home_directory,
@@ -183,26 +182,23 @@
 
     def _get_btclient_name(self):
         return (getattr(self.args, 'add_to', None)
                 or self.tracker_options.get('add_to', None)
                 or None)
 
     def _get_btclient(self):
-        btclient_name = self._get_btclient_name()
-        if btclient_name:
-            options = self.get_options('clients', btclient_name)
-            return aiobtclientapi.api(
-                name=btclient_name,
+        client_name = self._get_btclient_name()
+        if client_name:
+            options = self.get_options('clients', client_name)
+            return utils.btclient.BtClient(
+                name=client_name,
                 url=options['url'],
                 username=options['username'],
                 password=options['password'],
+                download_path=utils.fs.dirname(os.path.abspath(self.args.CONTENT)),
+                check_after_add=options['check_after_add'],
             )
 
     def _get_torrent_destination(self):
         return (getattr(self.args, 'copy_to', None)
                 or self.tracker_options.get('copy_to', None)
                 or None)
-
-    def _get_check_after_add(self):
-        btclient_config = self.config['clients'].get(self._get_btclient_name())
-        if btclient_config:
-            return btclient_config['check_after_add']
```

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/torrent.py` & `upsies-2023.5.25/upsies/uis/tui/commands/torrent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """
 Commands related to torrent files
 """
 
 import functools
 import os
 
-import aiobtclientapi
-
 from .... import constants, jobs, trackers, utils
 from .base import CommandBase
 
 
 class torrent_add(CommandBase):
     """Add torrent file to BitTorrent client"""
 
     names = ('torrent-add', 'ta')
 
     argument_definitions = {
         'CLIENT': {
             'type': utils.argtypes.client,
             'help': ('Case-insensitive BitTorrent client name\n'
-                     'Supported clients: ' + ', '.join(aiobtclientapi.client_names())),
+                     'Supported clients: ' + ', '.join(utils.btclient.client_names())),
         },
         'TORRENT': {
             'nargs': '+',
             'help': 'Path to torrent file',
         },
         ('--download-path', '-p'): {
             'help': "Parent directory of the torrent's content",
@@ -37,22 +35,22 @@
         client_name = self.args.CLIENT
         options = self.get_options('clients', client_name)
         return (
             jobs.torrent.AddTorrentJob(
                 home_directory=self.home_directory,
                 cache_directory=self.cache_directory,
                 ignore_cache=self.args.ignore_cache,
-                client_api=aiobtclientapi.api(
+                btclient=utils.btclient.BtClient(
                     name=client_name,
                     url=options['url'],
                     username=options['username'],
                     password=options['password'],
+                    download_path=self.args.download_path,
+                    check_after_add=options['check_after_add'],
                 ),
-                download_path=self.args.download_path,
-                check_after_add=options['check_after_add'],
                 enqueue=self.args.TORRENT,
             ),
         )
 
 
 class torrent_create(CommandBase):
     """
@@ -101,23 +99,23 @@
                         'nargs': '+',
                         'metavar': 'TORRENT',
                         'help': ('Use hashed pieces from TORRENT instead of generating '
                                  'them again or getting them from '
                                  f'{utils.fs.tildify_path(constants.GENERIC_TORRENTS_DIRPATH)}\n'
                                  'TORRENT may also be a directory, which is searched recursively '
                                  'for a matching *.torrent file.\n'
-                                 "NOTE: This option is ignored if TORRENT doesn't match properly."),
+                                 "NOTE: This option is ignored if TORRENT doesn't match CONTENT properly."),
                         'type': utils.argtypes.existing_path,
                         'default': (),
                     },
                     ('--add-to', '-a'): {
                         'type': utils.argtypes.client,
                         'metavar': 'CLIENT',
                         'help': ('Case-insensitive BitTorrent client name\n'
-                                 'Supported clients: ' + ', '.join(aiobtclientapi.client_names())),
+                                 'Supported clients: ' + ', '.join(utils.btclient.client_names())),
                     },
                     ('--copy-to', '-c'): {
                         'metavar': 'PATH',
                         'help': 'Copy the created torrent to PATH (file or directory)',
                     },
                 },
                 # Custom arguments defined by tracker for this command
@@ -159,34 +157,37 @@
             ),
         )
 
     @functools.cached_property
     def add_torrent_job(self):
         if self.args.add_to:
             client_name = self.args.add_to
-            config = self.config['clients'][client_name]
+            options = self.get_options('clients', client_name)
             add_torrent_job = jobs.torrent.AddTorrentJob(
                 home_directory=self.home_directory,
                 cache_directory=self.cache_directory,
                 ignore_cache=self.args.ignore_cache,
-                client_api=aiobtclientapi.api(
+                btclient=utils.btclient.BtClient(
                     name=client_name,
-                    url=config['url'],
-                    username=config['username'],
-                    password=config['password'],
+                    url=options['url'],
+                    username=options['username'],
+                    password=options['password'],
+                    download_path=utils.fs.dirname(os.path.abspath(self.args.CONTENT)),
+                    check_after_add=options['check_after_add'],
                 ),
-                download_path=utils.fs.dirname(os.path.abspath(self.args.CONTENT)),
-                check_after_add=config['check_after_add'],
             )
+
             # Pass CreateTorrentJob output to AddTorrentJob input.
             self.create_torrent_job.signal.register('output', add_torrent_job.enqueue)
+
             # Finish AddTorrentJob when CreateTorrentJob is finished. The
             # torrent will be enqueued and AddTorrentJob will finish after
             # adding the enqueued torrent.
             self.create_torrent_job.signal.register('finished', lambda _: add_torrent_job.finalize())
+
             return add_torrent_job
 
     @functools.cached_property
     def copy_torrent_job(self):
         if self.args.copy_to:
             copy_torrent_job = jobs.torrent.CopyTorrentJob(
                 home_directory=self.home_directory,
```

### Comparing `upsies-2023.4.3/upsies/uis/tui/commands/upload_images.py` & `upsies-2023.5.25/upsies/uis/tui/commands/upload_images.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/headless.py` & `upsies-2023.5.25/upsies/uis/tui/headless.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/__init__.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/base.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/dialog.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/dialog.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/imghost.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/poster.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/scene.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/screenshots.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/submit.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/torrent.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/jobwidgets/webdb.py` & `upsies-2023.5.25/upsies/uis/tui/jobwidgets/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/main.py` & `upsies-2023.5.25/upsies/uis/tui/main.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/style.py` & `upsies-2023.5.25/upsies/uis/tui/style.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/tui.py` & `upsies-2023.5.25/upsies/uis/tui/tui.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/utils.py` & `upsies-2023.5.25/upsies/uis/tui/utils.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/uis/tui/widgets.py` & `upsies-2023.5.25/upsies/uis/tui/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,23 +127,27 @@
     def text(self):
         return self.buffer.text
 
     @text.setter
     def text(self, text):
         self.set_text(text)
 
-    def set_text(self, text, ignore_callback=False, preserve_cursor_position=True):
+    def set_text(self, text, ignore_callback=False, preserve_cursor_position=False):
         if preserve_cursor_position:
             curpos = self.buffer.cursor_position
+
         if ignore_callback:
             handlers = self.buffer.on_text_changed._handlers
             self.buffer.on_text_changed._handlers = []
+
         self.buffer.set_document(Document(text), bypass_readonly=True)
+
         if ignore_callback:
             self.buffer.on_text_changed._handlers = handlers
+
         if preserve_cursor_position:
             self.buffer.cursor_position = curpos
 
     @property
     def read_only(self):
         return self._read_only
```

### Comparing `upsies-2023.4.3/upsies/utils/__init__.py` & `upsies-2023.5.25/upsies/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,18 +197,40 @@
         return self._list == other
 
     def __repr__(self):
         return f'{type(self).__name__}({repr(self._list)}, callback={self._callback!r})'
 
 
 class ImmutableMapping(collections.abc.Mapping):
-    """:class:`dict`-like that can't be changed after initialization"""
+    """
+    :class:`dict`-like that can't be changed after initialization
+
+    All values are also made immutable recursively. Keys should already be
+    immutable because the must be hashable.
+    """
 
     def __init__(self, *args, **kwargs):
-        self._dct = dict(*args, **kwargs)
+        self._dct = {
+            k: self._make_immutable(v)
+            for k, v in dict(*args, **kwargs).items()
+        }
+
+    def _make_immutable(self, obj):
+        if isinstance(obj, str):
+            # Catch strings early because they are also sequences
+            return obj
+
+        elif isinstance(obj, collections.abc.Sequence):
+            return tuple(self._make_immutable(item) for item in obj)
+
+        elif isinstance(obj, collections.abc.Mapping):
+            return ImmutableMapping(obj)
+
+        else:
+            return obj
 
     def __getitem__(self, key):
         return self._dct[key]
 
     def __iter__(self):
         return iter(self._dct)
 
@@ -423,27 +445,29 @@
     return await loop.run_in_executor(None, wrapped)
 
 
 # We must import these here to prevent circular imports
 from . import (  # noqa: E402 isort:skip
     argtypes,
     browser,
+    btclient,
     configfiles,
     country,
     daemon,
     fs,
     html,
     http,
     image,
     imghosts,
     predbs,
     release,
     signal,
     string,
     subproc,
+    subtitle,
     timestamp,
     torrent,
     types,
     update,
     video,
     webdbs,
 )
```

### Comparing `upsies-2023.4.3/upsies/utils/argtypes.py` & `upsies-2023.5.25/upsies/utils/argtypes.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,18 @@
                     raise argparse.ArgumentTypeError(f'Invalid value: {string}')
         return values
 
     return comma_separated
 
 
 def client(value):
-    """Name of a BitTorrent client supported by :mod:`aiobtclientapi`"""
-    import aiobtclientapi
+    """Name of a supported BitTorrent client"""
+    from . import btclient
     name = value.lower()
-    if name in aiobtclientapi.client_names():
+    if name in btclient.client_names():
         return name
     else:
         raise argparse.ArgumentTypeError(f'Unsupported client: {value}')
 
 
 def content(value):
     """Existing path to release file(s)"""
@@ -106,14 +106,33 @@
     from .. import defaults
     if value in defaults.option_paths():
         return value.lower()
     else:
         raise argparse.ArgumentTypeError(f'Unknown option: {value}')
 
 
+@functools.lru_cache(maxsize=None)
+def one_of(values):
+    """
+    Return function that returns an item of `values` or raises
+    :class:`argparse.ArgumentTypeError`
+
+    :param values: Allowed values
+    """
+    values = tuple(values)
+
+    def one_of_values(value):
+        if value in values:
+            return value
+        else:
+            raise argparse.ArgumentTypeError(f'Invalid value: {value}')
+
+    return one_of_values
+
+
 def regex(value):
     """:class:`re.Pattern` object"""
     import re
     try:
         return re.compile(str(value))
     except re.error as e:
         msg = f'Invalid regular expression: {value}: {e}'
```

### Comparing `upsies-2023.4.3/upsies/utils/configfiles.py` & `upsies-2023.5.25/upsies/utils/configfiles.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/country.py` & `upsies-2023.5.25/upsies/utils/country.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Lookup country information
+Look up country information
 """
 
 import functools
 
 from countryguess import guess_country as _guess_country
 
 
@@ -58,11 +58,8 @@
     :param country: Country name or code, e.g. "Russian Federation" (official
         name), "USA" (common abbreviation), "Korea" (short name), "fr"
         (2-character country code), etc.
     :type country: str or sequence
 
     :return: Country TLD or `country` if it can't be associated with any country
     """
-    def as_tld(tld):
-        return ('uk' if tld == 'GB' else tld).lower()
-
-    return as_tld(iso2(country))
+    return _guess_country(country, attribute='cctld', default=country)
```

### Comparing `upsies-2023.4.3/upsies/utils/daemon.py` & `upsies-2023.5.25/upsies/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/fs.py` & `upsies-2023.5.25/upsies/utils/fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,22 +177,25 @@
 
 def mkdir(path):
     """
     Create directory and its parents
 
     Existing directories are ignored.
 
+    If `path` is empty, no directory is created.
+
     :raise ContentError: if directory creation fails
     """
-    try:
-        os.makedirs(path, exist_ok=True)
-    except OSError as e:
-        raise errors.ContentError(f'{path}: {e.strerror or e}')
-    else:
-        assert_dir_usable(path)
+    if path:
+        try:
+            os.makedirs(path, exist_ok=True)
+        except OSError as e:
+            raise errors.ContentError(f'{path}: {e.strerror or e}')
+        else:
+            assert_dir_usable(path)
 
 
 def basename(path, parents=0):
     """
     Return last segment in `path`
 
     Unlike :func:`os.path.basename`, this removes any trailing directory
@@ -350,28 +353,45 @@
         try:
             return os.path.getsize(path)
         except OSError:
             pass
     return None
 
 
+def path_size(path):
+    """
+    Combined size of all files beneath `path`
+
+    Returns the same value as :func:`file_size` if `path` is not a directory.
+
+    Symbolic links are ignored.
+    """
+    filepaths = file_list(path, follow_dirlinks=False)
+    return sum(
+        file_size(f) or 0
+        for f in filepaths
+        if not os.path.islink(f)
+    )
+
+
 def file_list(path, extensions=(), min_age=None, max_age=None, follow_dirlinks=False):
     """
     List naturally sorted files in `path` and any subdirectories
 
     If `path` is not a directory, it is returned as a single item in a list
     unless `extensions` are given and they don't match.
 
     If `path` is any falsy value (e.g. ``""`` or `None`), return an empty
     sequence.
 
     Unreadable directories are excluded.
 
     :param str path: Path to a directory
     :param str extensions: Only include files with one of these extensions
+        (matched case-insensitively)
     :param min_age: Exclude files that are younger than this
     :type min_age: int or float
     :param max_age: Exclude files that are older than this
     :type max_age: int or float
     :param follow_dirlinks: Whether to include the contents of symbolic links to
         directories or the links themselves
 
@@ -422,14 +442,40 @@
                 if os.path.islink(dirpath):
                     del dirnames[dirnames.index(dirname)]
                     files.append(dirpath)
 
     return tuple(natsort.natsorted(files, key=str.casefold))
 
 
+def find_name(name, path, validator=None):
+    """
+    Return first path (in human sort order) to `name` anywhere beneath
+    `path` or `None`
+
+    :param str name: Exact name of the file or directory
+    :param str path: Base path to search for `name`
+
+    :param validator: Callable that gets a path that ends with `name` and
+        returns whether it is a match or not
+
+        For example, you can use :func:`os.path.isfile` or :func:`os.path.isdir`
+        to only find files or directories.
+    """
+    for root_, dirnames_, filenames_ in natsort.natsorted(
+            os.walk(path, topdown=True, followlinks=False),
+    ):
+        names_ = natsort.natsorted(filenames_ + dirnames_)
+        for name_ in names_:
+            path_ = os.path.join(root_, name_)
+            if name_ == name and (
+                    not validator or validator(path_)
+            ):
+                return path_
+
+
 # Stolen from torf-cli
 # https://github.com/rndusr/torf-cli/blob/master/torfcli/_utils.py
 
 _DOWN       = '\u2502'  # noqa: E221  # │
 _DOWN_RIGHT = '\u251C'  # noqa: E221  # ├
 _RIGHT      = '\u2500'  # noqa: E221  # ─
 _CORNER     = '\u2514'  # noqa: E221  # └
```

### Comparing `upsies-2023.4.3/upsies/utils/html.py` & `upsies-2023.5.25/upsies/utils/html.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 HTML parsing
 """
 
 import re
+import warnings
 
 from . import LazyModule
 
 bs4 = LazyModule(module='bs4', namespace=globals())
 
 
 def parse(string):
@@ -16,15 +17,20 @@
     :param string: HTML document
 
     :raise ContentError: if `string` is invalid HTML
     """
     if isinstance(string, bs4.element.Tag):
         return string
     else:
-        return bs4.BeautifulSoup(string, features='html.parser')
+        # Disable bs4 warnings, e.g. "MarkupResemblesLocatorWarning: The input
+        # looks more like a filename than markup. You may want to open this file
+        # and pass the filehandle into Beautiful Soup."
+        with warnings.catch_warnings():
+            warnings.simplefilter(action='ignore', category=UserWarning)
+            return bs4.BeautifulSoup(string, features='html.parser')
 
 
 def dump(html, filepath):
     """
     Write `html` to `filepath` for debugging
 
     :param html: String or :class:`~.bs4.BeautifulSoup` instance
@@ -61,14 +67,15 @@
         if soup is None:
             return None
     return soup
 
 
 def as_text(html):
     """Strip HTML tags from string and return text without markup"""
+    html = re.sub(r'<br\s*/?>', '\n', str(html))
     text = parse(html).get_text()
     text = re.sub(r'(\s)\s+', r'\1', text, flags=re.MULTILINE).strip()
     return text
 
 
 def purge_javascript(html):
     """
```

### Comparing `upsies-2023.4.3/upsies/utils/http.py` & `upsies-2023.5.25/upsies/utils/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,20 @@
         verify=bool(verify),
     )
     async with client:
         # Create request object
         if isinstance(data, (bytes, str)):
             build_request_args = {'content': data}
         else:
-            build_request_args = {'data': data}
+            # Remove fields with a value of `None`
+            build_request_args = {'data': {
+                k: v
+                for k, v in data.items()
+                if v is not None
+            }}
         request = client.build_request(
             method=str(method),
             url=str(url),
             cookies=_load_session_cookies(httpx.URL(url).host),
             params=params,
             files=_open_files(files),
             timeout=timeout,
@@ -407,14 +412,15 @@
         _log.debug('Request headers: %r', r.headers)
         _log.debug('Request data: %r', content)
     else:
         _log.debug('Received response: %r', r)
         _log.debug('Response headers: %r', r.headers)
         _log.debug('Response data: %r', content)
 
+    utils.fs.mkdir(os.path.dirname(filepath))
     if isinstance(content, str):
         utils.html.dump(content, f'{filepath}.html')
     elif isinstance(content, bytes):
         with open(f'{filepath}.content', 'wb') as f:
             f.write(content)
     elif isinstance(content, str):
         with open(f'{filepath}.content', 'w') as f:
```

### Comparing `upsies-2023.4.3/upsies/utils/image.py` & `upsies-2023.5.25/upsies/utils/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -252,7 +252,53 @@
     cmd = _make_resize_cmd(image_file, ffmpeg_params, target_filepath)
     output = utils.subproc.run(cmd, ignore_errors=True, join_stderr=True)
     if not os.path.exists(target_filepath):
         error = output or 'Unknown reason'
         raise errors.ImageResizeError(f'Failed to resize: {error}')
     else:
         return str(target_filepath)
+
+
+# NOTE: Most of the optimization is achieved at level 1 with ~40 % smaller
+#       files. Anything higher seems to only reduce by tens of kB or less.
+_optimization_levels = {
+    'low': '1',
+    'medium': '2',
+    'high': '4',
+    'placebo': 'max',
+}
+
+optimization_levels = tuple(_optimization_levels) + ('none', 'default')
+"""Valid `level` arguments for :func:`optimize`"""
+
+
+def optimize(image_file, level=4):
+    """
+    Optimize PNG image size
+
+    `image_file` is overwritten with the smaller image data.
+
+    :path image_file: Path to PNG File
+
+    :path str,int level: Optimiziation level (``"low"``, ``"medium"``,
+        ``"high"``) or ``"default"`` to use recommended level or ``"none"`` /
+        `None` to not do any optimization
+    """
+    if level not in ('none', None):
+        if level == 'default':
+            level = 'medium'
+
+        try:
+            opt = _optimization_levels[str(level)]
+        except KeyError:
+            raise errors.ImageOptimizeError(f'Invalid optimization level: {level}')
+
+        cmd = [
+            'oxipng', '--quiet', '--preserve',
+            '--opt', opt,
+            '--interlace', '0',  # Remove any interlacing
+            '--strip', 'safe',   # Remove irrelevant metadata
+            str(image_file),
+        ]
+        error = utils.subproc.run(cmd, join_stderr=True)
+        if error:
+            raise errors.ImageOptimizeError(f'Failed to optimize: {error}')
```

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/__init__.py` & `upsies-2023.5.25/upsies/utils/imghosts/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/base.py` & `upsies-2023.5.25/upsies/utils/imghosts/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/common.py` & `upsies-2023.5.25/upsies/utils/imghosts/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/dummy.py` & `upsies-2023.5.25/upsies/utils/imghosts/dummy.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/freeimage.py` & `upsies-2023.5.25/upsies/utils/imghosts/freeimage.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/imgbb.py` & `upsies-2023.5.25/upsies/utils/imghosts/imgbb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/imgbox.py` & `upsies-2023.5.25/upsies/utils/imghosts/imgbox.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/imghosts/ptpimg.py` & `upsies-2023.5.25/upsies/utils/imghosts/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/__init__.py` & `upsies-2023.5.25/upsies/utils/predbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/base.py` & `upsies-2023.5.25/upsies/utils/predbs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/common.py` & `upsies-2023.5.25/upsies/utils/predbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/corruptnet.py` & `upsies-2023.5.25/upsies/utils/predbs/corruptnet.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/multi.py` & `upsies-2023.5.25/upsies/utils/predbs/multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import collections
 import difflib
 import os
 import re
 
-import memoize.wrapper
+import async_lru
 
 from ... import constants, errors, utils
 from . import SceneCheckResult
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
@@ -95,15 +95,15 @@
             try:
                 result = await coro
             except (NotImplementedError, errors.RequestError) as e:
                 yield e
             else:
                 yield result
 
-    @memoize.wrapper.memoize()
+    @async_lru.alru_cache
     async def search(self, *args, **kwargs):
         """
         Search multiple predbs concurrently and return first non-empty results
 
         See :meth:`~.PredbApiBase.search`.
         """
         exceptions = []
@@ -119,35 +119,34 @@
             # All predbs are unreachable or don't have `method_name` implemented.
             # Raise combined RequestErrors.
             self._raise(exceptions, method_name='search')
         else:
             # No search results
             return []
 
-    @memoize.wrapper.memoize()
+    @async_lru.alru_cache
     async def release_files(self, *args, **kwargs):
         """See :meth:`~.PredbApiBase.release_files`"""
         return await self._for_each_predb('release_files', *args, **kwargs)
 
     _nogroup_regexs = (
         re.compile(r'^$'),
         re.compile(r'^(?i:nogroup)$'),
         re.compile(r'^(?i:nogrp)$'),
     )
 
-    @memoize.wrapper.memoize()
+    @async_lru.alru_cache
     async def is_scene_release(self, release):
         """
         Return whether `release` is a scene release or not
 
         .. note:: A renamed or otherwise altered scene release is still
             considered a scene release.
 
-        :param release: Release name, path to release or
-            :class:`~.release.ReleaseInfo` instance
+        :param release: Release name, path to release
 
         :return: :class:`~.types.SceneCheckResult`
         """
         if isinstance(release, str):
             release_info = utils.release.ReleaseInfo(release)
         else:
             release_info = release
```

### Comparing `upsies-2023.4.3/upsies/utils/predbs/predbclub.py` & `upsies-2023.5.25/upsies/utils/predbs/predbclub.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/predbde.py` & `upsies-2023.5.25/upsies/utils/predbs/predbde.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/predbovh.py` & `upsies-2023.5.25/upsies/utils/predbs/predbovh.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/query.py` & `upsies-2023.5.25/upsies/utils/predbs/query.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/predbs/srrdb.py` & `upsies-2023.5.25/upsies/utils/predbs/srrdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/release.py` & `upsies-2023.5.25/upsies/utils/release.py`

 * *Files 4% similar despite different names*

```diff
@@ -474,15 +474,47 @@
     @edition.setter
     def edition(self, value):
         self._info['edition'] = [str(v) for v in value]
 
     @_translated_property
     def source(self):
         '''Original source (e.g. "BluRay", "WEB-DL") or "UNKNOWN_SOURCE"'''
-        return self._info.get('source') or 'UNKNOWN_SOURCE'
+        source = None
+
+        # DVD
+        video_ts_path = utils.fs.find_name('VIDEO_TS', self._path, validator=os.path.isdir)
+        if video_ts_path:
+            # Include VIDEO_TS siblings (e.g. "cover")
+            release_size = utils.fs.path_size(os.path.dirname(video_ts_path))
+            _log.debug('VIDEO_TS size: %r: %r', video_ts_path, release_size)
+            if release_size <= 4_700_000_000:
+                source = 'DVD5'
+            else:
+                source = 'DVD9'
+
+        if source is None:
+            # Blu-ray
+            bdmv_path = utils.fs.find_name('BDMV', self._path, validator=os.path.isdir)
+            if bdmv_path:
+                # Include BDMV siblings (e.g. "CERTIFICATE", and "ANY!")
+                release_size = utils.fs.path_size(os.path.dirname(bdmv_path))
+                _log.debug('Blu-ray size: %r: %r', bdmv_path, release_size)
+                if release_size <= 25e9:
+                    source = 'BD25'
+                elif release_size <= 50e9:
+                    source = 'BD50'
+                elif release_size <= 66e9:
+                    source = 'BD66'
+                else:
+                    source = 'BD100'
+
+        if source is None:
+            source = self._info.get('source') or 'UNKNOWN_SOURCE'
+
+        return source
 
     @source.setter
     def source(self, value):
         self._info['source'] = str(value)
 
     @_translated_property
     def resolution(self):
@@ -672,14 +704,25 @@
 
     _needed_attrs = {
         ReleaseType.movie: ('title', 'year', 'resolution', 'source', 'video_format'),
         ReleaseType.season: ('title', 'episodes', 'resolution', 'source', 'video_format'),
         ReleaseType.episode: ('title', 'episodes', 'resolution', 'source', 'video_format'),
     }
 
+    @functools.cached_property
+    def dvd_encoding(self):
+        """"PAL", "NTSC" or `None`"""
+        if self.source in ('DVD', 'DVD5', 'DVD9', 'DVDRip'):
+            frame_rate = utils.video.frame_rate(self._path, default=0)
+            if frame_rate:
+                if frame_rate <= 25:
+                    return 'PAL'
+                elif frame_rate <= 30:
+                    return 'NTSC'
+
     @property
     def is_complete(self):
         """
         Whether all needed information is known and the string returned by
         :meth:`format` will not contain "UNKNOWN_*"
 
         This always returns `False` if :attr:`type` is
@@ -819,15 +862,18 @@
             The typical use case would be ``.``.
         """
         parts = [self.title_with_aka_and_year]
 
         if self.type in (ReleaseType.season, ReleaseType.episode) and not self.date:
             parts.append(str(self.episodes))
 
-        parts.append(self.resolution)
+        if self.dvd_encoding:
+            parts.append(self.dvd_encoding)
+        else:
+            parts.append(self.resolution)
 
         if self.service:
             parts.append(self.service)
 
         parts.append(self.source)
 
         if self.edition:
@@ -845,14 +891,16 @@
 
         # Separator (usually " " or ".")
         sep = separator if separator is not None else self.separator
         if sep != ' ':
             joined = joined.replace(' ', sep)
 
         if sep == '.':
+            # Replace "&" with "and" before "&" gets removed
+            joined = re.sub(r'&', 'and', joined)
             # Remove non-word characters like (e.g.: ,:) with some exceptions
             joined = re.sub(r'[^ \w\.-]', '', joined)
             # Deduplicate "."
             joined = re.sub(r'\.+', '.', joined)
 
         return joined
 
@@ -1402,15 +1450,16 @@
             {'': ('1', '2'), '3': ('4', '5')}
             >>> Episodes.from_string('S09E08S03E06S9E1')
             {'9': ('1', '8',), '3': ('6',)}
             >>> Episodes.from_string('E01S03E06.bar.E02')
             {'': ('1', '2',), '3': ('6',)}
         """
         def extract_number(string):
-            return ''.join(c for c in string if c in '0123456789').lstrip('0')
+            n = ''.join(c for c in string if c in '0123456789').lstrip('0')
+            return '0' if n == '' else n
 
         def split_episodes(string):
             return {extract_number(e) for e in string.split('E') if e.strip()}
 
         # Extract episode information to get "S..E.." string without any other
         # characters. The original value might have delimiters,
         # e.g. "...S09E14-E15...", and we want "S09E14E15".
```

### Comparing `upsies-2023.4.3/upsies/utils/signal.py` & `upsies-2023.5.25/upsies/utils/signal.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/string.py` & `upsies-2023.5.25/upsies/utils/string.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/subproc.py` & `upsies-2023.5.25/upsies/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/timestamp.py` & `upsies-2023.5.25/upsies/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/torrent.py` & `upsies-2023.5.25/upsies/utils/torrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,28 @@
 SKIP_SEARCHING = 'skip_searching'
 """
 Return value for the `progress_callback` to stop searching for a reusable
 torrent (see :func:`create`)
 """
 
 
-def create(*, content_path, announce, source, torrent_path,
-           use_cache=True, exclude=(), reuse_torrent_path=None,
-           piece_size_min=None, piece_size_max=None,
+def create(*, content_path, announce, source,
+           torrent_path, exclude=(), use_cache=True,
+           reuse_torrent_path=None, randomize_infohash=True,
+           piece_size_calculator=None, piece_size_min_max_calculator=None,
            init_callback, progress_callback):
     """
     Generate and write torrent file
 
     :param str content_path: Path to the torrent's payload
     :param str announce: Announce URL
     :param str source: Value of the ``source`` field in the torrent. This makes
         the torrent unique for each tracker to avoid cross-seeding issues, so it
         is usually the tracker's abbreviated name.
     :param str torrent_path: Path of the generated torrent file
-    :param int piece_size_min: Minimum piece size
-    :param int piece_size_max: Maximum piece size
-    :param init_callback: Callable that is called once before torrent generation
-        commences with a :class:`Files` object
-    :param progress_callback: Callable that is called at regular intervals with
-        a :class:`CreateTorrentProgress` or :class:`FindTorrentProgress` object
-        as a positional argument
     :param exclude: Sequence of glob patterns (:class:`str`) and
         :class:`re.Pattern` objects (return value from :func:`re.compile`)
 
         Files beneath `content_path` are excluded from the torrent.
 
         Glob patterns are matched case-insensitively.
     :param bool use_cache: Whether to get piece hashes from previously created
@@ -59,14 +53,32 @@
         and use the first one that matches.
 
         Non-existing or otherwise unreadable paths as well as falsy values
         (e.g. ``""`` or `None`) are silently ignored.
 
         If this is a sequence, its items are expected to be directory or file
         paths and handled as described above.
+    :param randomize_infohash: Whether the torrent is made unique by randomizing
+        the infohash
+
+        This is done by including a random number in the torrent.
+    :param piece_size_calculator: Function that takes the torrent's content size
+        in bytes and returns the piece size
+
+        If this is `None`, the default implementation is used.
+    :param piece_size_min_max_calculator: Function that takes the torrent's
+        content size in bytes and returns the allowed minimum and maximum piece
+        sizes
+
+        If this is `None`, the default minimum and maximum piece sizes are used.
+    :param init_callback: Callable that is called once before torrent generation
+        commences with a :class:`Files` object
+    :param progress_callback: Callable that is called at regular intervals with
+        a :class:`CreateTorrentProgress` or :class:`FindTorrentProgress` object
+        as a positional argument
 
     Callbacks can cancel the torrent creation by returning `True` or any other
     truthy value. If `progress_callback` returns :data:`SKIP_SEARCHING`, the
     search for a reusable torrent is cancelled and pieces are hashed normally.
 
     :raise TorrentError: if anything goes wrong
 
@@ -79,17 +91,25 @@
 
     # Create Torrent object
     torrent = _get_torrent(
         content_path=content_path,
         exclude=_get_exclude_regexs(exclude),
         announce=announce,
         source=source,
-        piece_size_min=piece_size_min,
-        piece_size_max=piece_size_max,
+        randomize_infohash=randomize_infohash,
     )
+
+    # Custom piece_size management
+    if piece_size_min_max_calculator:
+        # Calculate custom piece_size boundaries based on torrent's content size
+        torrent.piece_size_min, torrent.piece_size_max = piece_size_min_max_calculator(torrent.size)
+    if piece_size_calculator:
+        # Calculate custom piece_size based on torrent's content size
+        torrent.piece_size = piece_size_calculator(torrent.size)
+
     # Report files with `exclude` applied
     cancelled = init_callback(Files(torrent))
     if cancelled:
         return None
 
     if use_cache:
         # Try to get piece hashes from existing torrent
@@ -127,23 +147,22 @@
         elif isinstance(pattern, str):
             regexs.append(re.compile(fnmatch.translate(str(pattern)), flags=re.IGNORECASE))
         else:
             raise TypeError(f'Unexpected exclude type: {pattern!r}')
     return regexs
 
 
-def _get_torrent(*, content_path, exclude, announce, source, piece_size_min, piece_size_max):
+def _get_torrent(*, content_path, exclude, announce, source, randomize_infohash):
     try:
         return torf.Torrent(
             path=content_path,
             exclude_regexs=exclude,
-            piece_size_min=piece_size_min,
-            piece_size_max=piece_size_max,
             trackers=((announce,),),
             source=source,
+            randomize_infohash=randomize_infohash,
             private=True,
             created_by=f'{__project_name__} {__version__}',
             creation_date=time.time(),
         )
     except torf.TorfError as e:
         raise errors.TorrentError(str(e))
 
@@ -158,14 +177,18 @@
     except torf.TorfError as e:
         raise errors.TorrentError(str(e))
     else:
         return wrapped_callback.return_value
 
 
 def _find_hashes(*, torrent, reuse_torrent_path, callback):
+    if not torrent.files:
+        # All files are excluded (let someone deal with it)
+        return False
+
     wrapped_callback = _FindTorrentCallback(callback)
     try:
         torrent.reuse(
             _get_reuse_torrent_paths(torrent, reuse_torrent_path),
             callback=wrapped_callback,
             interval=1.0,
         )
@@ -521,14 +544,13 @@
     """
     try:
         torrent = _get_torrent(
             content_path=content_path,
             exclude=_get_exclude_regexs(exclude),
             announce='http://dummy.local',
             source=None,
-            piece_size_min=None,
-            piece_size_max=None,
+            randomize_infohash=False,
         )
     except errors.TorrentError as e:
         raise errors.ContentError(e)
     else:
         return [str(f) for f in torrent.filepaths]
```

### Comparing `upsies-2023.4.3/upsies/utils/types.py` & `upsies-2023.5.25/upsies/utils/types.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/update.py` & `upsies-2023.5.25/upsies/utils/update.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/video.py` & `upsies-2023.5.25/upsies/utils/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     ``mediainfo`` output as a string
 
     The parent directory of `path` is redacted.
 
     :param str path: Path to video file or directory
     :param bool only_first: Whether to return mediainfo for each video file as a
         :class:`list` or to return mediainfo of the first video file (see
-        :func:`find_video`)
+        :func:`find_videos`)
 
     :raise ContentError: if anything goes wrong
     """
     def remove_parent_directory(mi, parent_directory=utils.fs.dirname(path)):
         if parent_directory:
             return mi.replace(parent_directory + os.sep, '')
         else:
@@ -141,15 +141,27 @@
     :param default: Return value if `path` doesn't exist, raise
         :exc:`~.ContentError` if not provided
 
     :raise ContentError: if anything goes wrong
     """
     if default is not NO_DEFAULT_VALUE and not os.path.exists(path):
         return default
-    return _tracks(find_videos(path)[0])
+
+    try:
+        main_videos = find_videos(path)
+    except errors.ContentError:
+        # No video file found - use path as is. This allows us to get tracks
+        # from an .IFO file, which isn't a video, so find_videos() raises
+        # ContentError. _tracks()/_run_mediainfo() will still raise ContentError
+        # if `path` mediainfo can't handle it.
+        video_filepath = path
+    else:
+        video_filepath = main_videos[0]
+
+    return _tracks(video_filepath)
 
 def _tracks(video_file_path):
     stdout = _run_mediainfo(video_file_path, '--Output=JSON')
     tracks = {}
     try:
         for track in json.loads(stdout)['media']['track']:
             if track['@type'] not in tracks:
```

### Comparing `upsies-2023.4.3/upsies/utils/webdbs/__init__.py` & `upsies-2023.5.25/upsies/utils/webdbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/webdbs/base.py` & `upsies-2023.5.25/upsies/utils/webdbs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,24 +53,33 @@
     @property
     @abc.abstractmethod
     def default_config(self):
         """Default user configuration as a dictionary"""
 
     def sanitize_query(self, query):
         """
-        Modify :class:`~.common.Query` for specific DB
+        Modify :class:`.Query` for specific DB
 
-        See :meth:`.TvmazeApi.sanitize_query` for an example.
+        If :meth:`get_id_from_text` finds an ID in :attr:`.Query.title`,
+        :attr:`.Query.id` is set to that ID, which means all other query
+        parameters are ignored.
         """
         if not isinstance(query, Query):
             raise TypeError(f'Not a Query instance: {query!r}')
         else:
+            id_from_url = self.get_id_from_text(query.title)
+            if id_from_url:
+                query.id = id_from_url
             return query
 
     @abc.abstractmethod
+    def get_id_from_text(self, text):
+        """Return ID found in `text` or `None`"""
+
+    @abc.abstractmethod
     async def search(self, query):
         """
         Search DB
 
         :param query: :class:`~.common.Query` instance
 
         :return: List of :class:`~.common.SearchResult` instances
```

### Comparing `upsies-2023.4.3/upsies/utils/webdbs/common.py` & `upsies-2023.5.25/upsies/utils/webdbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.4.3/upsies/utils/webdbs/imdb.py` & `upsies-2023.5.25/upsies/utils/webdbs/imdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,23 +23,26 @@
     default_config = {}
 
     _url_base = 'https://www.imdb.com'
     _soup_cache = {}
 
     async def _get_soup(self, path, params={}):
         path = path.rstrip('/')
+
         cache_id = (path, tuple(sorted(params.items())))
         if cache_id in self._soup_cache:
             return self._soup_cache[cache_id]
+
         text = await utils.http.get(
-            url=f'{self._url_base}/{path}',
+            url=f'{self._url_base}/{path}/',
             params=params,
             user_agent=await utils.http.get_popular_user_agent(),
             cache=True,
         )
+
         self._soup_cache[cache_id] = utils.html.parse(text)
         return self._soup_cache[cache_id]
 
     _title_types = {
         ReleaseType.movie: 'feature,tv_movie,documentary,short,video,tv_short',
         ReleaseType.season: 'tv_series,tv_miniseries',
         # Searching for single episodes is currently not supported
@@ -60,14 +63,20 @@
         query = super().sanitize_query(query)
         query.title = re.sub(r'\s(?i:and)(\s)', r'\1', query.title)
         query.title = re.sub(r'\b(?i:dont)(\b)', "don't", query.title)
         query.title = re.sub(r'\b(?i:cant)(\b)', "can't", query.title)
         query.title = re.sub(r'\b(?i:wont)(\b)', "won't", query.title)
         return query
 
+    def get_id_from_text(self, text):
+        # Example: https://www.imdb.com/title/tt0048918/
+        match = re.search(r'\b(tt\d+)\b', text)
+        if match:
+            return match.group(1)
+
     async def search(self, query):
         _log.debug('Searching IMDb for %s', query)
 
         if query.id:
             title_english = await self.title_english(query.id)
             title_original = await self.title_original(query.id)
             return [_ImdbSearchResult(
```

### Comparing `upsies-2023.4.3/upsies/utils/webdbs/tmdb.py` & `upsies-2023.5.25/upsies/utils/webdbs/tmdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,22 @@
             params=params,
             user_agent=await http.get_popular_user_agent(),
             cache=True,
         )
         self._soup_cache[cache_id] = html.parse(text)
         return self._soup_cache[cache_id]
 
+    def get_id_from_text(self, text):
+        # Examples:
+        # https://www.themoviedb.org/movie/334536-the-blackcoat-s-daughter
+        # https://www.themoviedb.org/tv/45016-bron-broen
+        match = re.search(r'\b((?i:movie|tv)/\d+)\b', text)
+        if match:
+            return match.group(1)
+
     async def search(self, query):
         _log.debug('Searching TMDb for %s', query)
 
         if query.id:
             async def generate_result(id):
                 _log.debug('Getting ID: %r', id)
                 title_english = await self.title_english(id)
```

### Comparing `upsies-2023.4.3/upsies/utils/webdbs/tvmaze.py` & `upsies-2023.5.25/upsies/utils/webdbs/tvmaze.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 API for tvmaze.com
 """
 
 import collections
 import functools
 import json
+import re
 
 from ... import errors, utils
 from .. import html, http
 from ..types import ReleaseType
 from . import common
 from .base import WebDbApiBase
 
@@ -28,14 +29,20 @@
 
     def sanitize_query(self, query):
         """Set :attr:`~.common.Query.type` to :attr:`~.types.ReleaseType.unknown`"""
         query = super().sanitize_query(query)
         query.type = ReleaseType.unknown
         return query
 
+    def get_id_from_text(self, text):
+        # Example: https://www.tvmaze.com/shows/36906/gary-and-his-demons
+        match = re.search(r'\b(?i:shows)/(\d+)\b', text)
+        if match:
+            return match.group(1)
+
     async def search(self, query):
         _log.debug('Searching TVmaze for %s', query)
 
         if query.id:
             show = await self._get_show(query.id)
             return [_TvmazeSearchResult(show=show, tvmaze_api=self)]
```

### Comparing `upsies-2023.4.3/upsies.egg-info/PKG-INFO` & `upsies-2023.5.25/upsies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2023.4.3
+Version: 2023.5.25
 Summary: Media metadata aggregator
 Home-page: https://upsies.readthedocs.io
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `upsies-2023.4.3/upsies.egg-info/SOURCES.txt` & `upsies-2023.5.25/upsies.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 LICENSE
 README.rst
 setup.py
+bb/__init__.py
+bb/config.py
+bb/jobs.py
+bb/tracker.py
 upsies/__init__.py
 upsies/__main__.py
 upsies/constants.py
 upsies/defaults.py
 upsies/errors.py
 upsies.egg-info/PKG-INFO
 upsies.egg-info/SOURCES.txt
@@ -41,17 +45,17 @@
 upsies/trackers/mtv/jobs.py
 upsies/trackers/mtv/tracker.py
 upsies/trackers/nbl/__init__.py
 upsies/trackers/nbl/config.py
 upsies/trackers/nbl/jobs.py
 upsies/trackers/nbl/tracker.py
 upsies/trackers/ptp/__init__.py
-upsies/trackers/ptp/_ptp_tags.py
 upsies/trackers/ptp/config.py
 upsies/trackers/ptp/jobs.py
+upsies/trackers/ptp/metadata.py
 upsies/trackers/ptp/tracker.py
 upsies/uis/__init__.py
 upsies/uis/tui/__init__.py
 upsies/uis/tui/headless.py
 upsies/uis/tui/main.py
 upsies/uis/tui/style.py
 upsies/uis/tui/tui.py
@@ -81,25 +85,27 @@
 upsies/uis/tui/jobwidgets/screenshots.py
 upsies/uis/tui/jobwidgets/submit.py
 upsies/uis/tui/jobwidgets/torrent.py
 upsies/uis/tui/jobwidgets/webdb.py
 upsies/utils/__init__.py
 upsies/utils/argtypes.py
 upsies/utils/browser.py
+upsies/utils/btclient.py
 upsies/utils/configfiles.py
 upsies/utils/country.py
 upsies/utils/daemon.py
 upsies/utils/fs.py
 upsies/utils/html.py
 upsies/utils/http.py
 upsies/utils/image.py
 upsies/utils/release.py
 upsies/utils/signal.py
 upsies/utils/string.py
 upsies/utils/subproc.py
+upsies/utils/subtitle.py
 upsies/utils/timestamp.py
 upsies/utils/torrent.py
 upsies/utils/types.py
 upsies/utils/update.py
 upsies/utils/video.py
 upsies/utils/imghosts/__init__.py
 upsies/utils/imghosts/base.py
```

