# Comparing `tmp/RobertCommonBasic-0.1.39.tar.gz` & `tmp/RobertCommonBasic-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonBasic-0.1.39.tar", last modified: Tue May 16 09:43:02 2023, max compression
+gzip compressed data, was "RobertCommonBasic-0.1.40.tar", last modified: Thu May 25 09:14:25 2023, max compression
```

## Comparing `RobertCommonBasic-0.1.39.tar` & `RobertCommonBasic-0.1.40.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.231700 RobertCommonBasic-0.1.39/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.39/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.39/MANIFEST.in
--rw-rw-rw-   0        0        0     1739 2023-05-16 09:43:02.231700 RobertCommonBasic-0.1.39/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.39/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.111766 RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/
--rw-rw-rw-   0        0        0     1739 2023-05-16 09:43:01.000000 RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4427 2023-05-16 09:43:01.000000 RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:43:01.000000 RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2023-05-16 09:43:01.000000 RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-16 09:43:01.000000 RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      187 2023-04-19 11:40:39.000000 RobertCommonBasic-0.1.39/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.112766 RobertCommonBasic-0.1.39/robertcommonbasic/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.39/robertcommonbasic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.113764 RobertCommonBasic-0.1.39/robertcommonbasic/basic/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.115767 RobertCommonBasic-0.1.39/robertcommonbasic/basic/base/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/base/__init__.py
--rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/base/constant.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.116764 RobertCommonBasic-0.1.39/robertcommonbasic/basic/cache/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/cache/__init__.py
--rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/cache/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.118768 RobertCommonBasic-0.1.39/robertcommonbasic/basic/cls/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/cls/__init__.py
--rw-rw-rw-   0        0        0    12320 2023-05-09 08:30:50.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/cls/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.129160 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/__init__.py
--rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/conversion.py
--rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/crc16.py
--rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/csv.py
--rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/datatuple.py
--rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/frame.py
--rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/nametuple.py
--rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/type.py
--rw-rw-rw-   0        0        0     5064 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.133351 RobertCommonBasic-0.1.39/robertcommonbasic/basic/decorator/
--rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/decorator/__init__.py
--rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/decorator/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.136762 RobertCommonBasic-0.1.39/robertcommonbasic/basic/dt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/dt/__init__.py
--rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/dt/schedule.py
--rw-rw-rw-   0        0        0    10445 2023-04-10 06:28:17.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/dt/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.143768 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/__init__.py
--rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/aes.py
--rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/dsa.py
--rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/hash.py
--rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/md5.py
--rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.145768 RobertCommonBasic-0.1.39/robertcommonbasic/basic/error/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/error/__init__.py
--rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/error/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.148768 RobertCommonBasic-0.1.39/robertcommonbasic/basic/exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/exector/__init__.py
--rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/exector/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.157770 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/
--rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/__init__.py
--rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/csv.py
--rw-rw-rw-   0        0        0     4951 2023-05-16 08:36:24.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/ini.py
--rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/log.py
--rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/xml.py
--rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/yaml.py
--rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.161768 RobertCommonBasic-0.1.39/robertcommonbasic/basic/log/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/log/__init__.py
--rw-rw-rw-   0        0        0     6070 2023-04-10 02:23:47.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/log/utils.py
--rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/log/watch.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.163768 RobertCommonBasic-0.1.39/robertcommonbasic/basic/net/
--rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/net/__init__.py
--rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/net/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.171128 RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/__init__.py
--rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/cmd.py
--rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/env.py
--rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/file.py
--rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/path.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.173492 RobertCommonBasic-0.1.39/robertcommonbasic/basic/process/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/process/__init__.py
--rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/process/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.176175 RobertCommonBasic-0.1.39/robertcommonbasic/basic/profile/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/profile/__init__.py
--rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/profile/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.179197 RobertCommonBasic-0.1.39/robertcommonbasic/basic/re/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/re/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-02-09 02:47:33.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/re/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.185323 RobertCommonBasic-0.1.39/robertcommonbasic/basic/safetext/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/safetext/__init__.py
--rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/safetext/converter.py
--rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/safetext/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.187338 RobertCommonBasic-0.1.39/robertcommonbasic/basic/sugar/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/sugar/__init__.py
--rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/sugar/funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.190330 RobertCommonBasic-0.1.39/robertcommonbasic/basic/validation/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/validation/__init__.py
--rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.39/robertcommonbasic/basic/validation/input.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.192330 RobertCommonBasic-0.1.39/robertcommonbasic/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.193330 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.195434 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_cls/
--rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_cls/__init__.py
--rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.203773 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/
--rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/__init__.py
--rw-rw-rw-   0        0        0      729 2022-06-23 09:21:24.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
--rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
--rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_frame.py
--rw-rw-rw-   0        0        0     3568 2023-04-11 13:11:50.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.206780 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_dt/
--rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_dt/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-02-20 02:34:17.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.213025 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/
--rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
--rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
--rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
--rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.214527 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_exector/
--rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_exector/__init__.py
--rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.221083 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/__init__.py
--rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/test_csv.py
--rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/test_xml.py
--rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/test_zip.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.223082 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_net/
--rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_net/__init__.py
--rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_net/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.226379 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_os/
--rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_os/__init__.py
--rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_os/test_env.py
--rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_os/test_file.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.228397 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_re/
--rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_re/__init__.py
--rw-rw-rw-   0        0        0      605 2023-04-11 09:07:57.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_re/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:43:02.230702 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_validation/
--rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_validation/__init__.py
--rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_validation/test_input.py
--rw-rw-rw-   0        0        0       42 2023-05-16 09:43:02.233069 RobertCommonBasic-0.1.39/setup.cfg
--rw-rw-rw-   0        0        0     3876 2023-05-16 05:38:22.000000 RobertCommonBasic-0.1.39/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.400530 RobertCommonBasic-0.1.40/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonBasic-0.1.40/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonBasic-0.1.40/MANIFEST.in
+-rw-rw-rw-   0        0        0     1739 2023-05-25 09:14:25.400530 RobertCommonBasic-0.1.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2022-01-13 05:29:18.000000 RobertCommonBasic-0.1.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.279205 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/
+-rw-rw-rw-   0        0        0     1739 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4467 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-25 09:14:25.000000 RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      187 2023-05-23 06:22:21.000000 RobertCommonBasic-0.1.40/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.280208 RobertCommonBasic-0.1.40/robertcommonbasic/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonBasic-0.1.40/robertcommonbasic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.281205 RobertCommonBasic-0.1.40/robertcommonbasic/basic/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.282714 RobertCommonBasic-0.1.40/robertcommonbasic/basic/base/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:39:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/base/__init__.py
+-rw-rw-rw-   0        0        0      471 2023-01-04 02:45:25.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/base/constant.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.285151 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/__init__.py
+-rw-rw-rw-   0        0        0      667 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.287153 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/__init__.py
+-rw-rw-rw-   0        0        0    12320 2023-05-09 08:30:50.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.298418 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/__init__.py
+-rw-rw-rw-   0        0        0    13611 2023-01-31 14:01:59.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/conversion.py
+-rw-rw-rw-   0        0        0     4537 2022-11-14 07:54:50.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/crc16.py
+-rw-rw-rw-   0        0        0     2169 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/csv.py
+-rw-rw-rw-   0        0        0    39297 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/datatuple.py
+-rw-rw-rw-   0        0        0     2528 2023-05-25 09:05:54.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/express.py
+-rw-rw-rw-   0        0        0     8304 2022-11-14 09:43:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/frame.py
+-rw-rw-rw-   0        0        0     1097 2022-11-14 09:48:07.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/nametuple.py
+-rw-rw-rw-   0        0        0       62 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/type.py
+-rw-rw-rw-   0        0        0    12943 2023-05-23 08:43:23.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.300422 RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/
+-rw-rw-rw-   0        0        0        0 2021-12-08 01:56:09.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/__init__.py
+-rw-rw-rw-   0        0        0     1250 2022-12-05 08:07:43.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.303420 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/__init__.py
+-rw-rw-rw-   0        0        0     4474 2022-12-28 02:51:52.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/schedule.py
+-rw-rw-rw-   0        0        0    10445 2023-05-18 03:32:13.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.309851 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/__init__.py
+-rw-rw-rw-   0        0        0      583 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/aes.py
+-rw-rw-rw-   0        0        0     3856 2022-11-14 07:41:26.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/dsa.py
+-rw-rw-rw-   0        0        0      716 2023-03-09 07:09:06.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/hash.py
+-rw-rw-rw-   0        0        0      338 2022-11-14 07:14:55.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/md5.py
+-rw-rw-rw-   0        0        0     2661 2022-11-14 07:25:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/rsa.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.312238 RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/__init__.py
+-rw-rw-rw-   0        0        0     2354 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.315245 RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:25:14.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/__init__.py
+-rw-rw-rw-   0        0        0     3641 2022-11-14 09:50:44.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.327165 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 02:39:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-04-28 09:36:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/csv.py
+-rw-rw-rw-   0        0        0     4951 2023-05-18 08:56:41.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/ini.py
+-rw-rw-rw-   0        0        0     1035 2022-11-18 06:23:07.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/log.py
+-rw-rw-rw-   0        0        0     3157 2022-11-24 03:18:18.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/xml.py
+-rw-rw-rw-   0        0        0      339 2022-11-18 06:47:46.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/yaml.py
+-rw-rw-rw-   0        0        0     3039 2023-03-08 07:31:52.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/zip.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.334249 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/__init__.py
+-rw-rw-rw-   0        0        0     6070 2023-05-05 06:04:36.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/utils.py
+-rw-rw-rw-   0        0        0     1366 2022-12-05 08:20:54.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/watch.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.337467 RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 12:44:36.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/__init__.py
+-rw-rw-rw-   0        0        0     8521 2023-05-16 03:07:09.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.343541 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-12-14 09:03:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/cmd.py
+-rw-rw-rw-   0        0        0      400 2022-06-29 09:34:23.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/env.py
+-rw-rw-rw-   0        0        0     3446 2023-03-16 09:00:41.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/file.py
+-rw-rw-rw-   0        0        0      533 2023-02-06 07:51:13.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/path.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.346423 RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/__init__.py
+-rw-rw-rw-   0        0        0     8845 2022-12-14 08:53:18.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.348426 RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/__init__.py
+-rw-rw-rw-   0        0        0     1264 2022-11-18 02:27:39.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.351863 RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.355482 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-02-03 07:26:22.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/converter.py
+-rw-rw-rw-   0        0        0      377 2022-11-18 02:33:07.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/safetext/funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.360399 RobertCommonBasic-0.1.40/robertcommonbasic/basic/sugar/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/sugar/__init__.py
+-rw-rw-rw-   0        0        0      377 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/sugar/funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.362542 RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/__init__.py
+-rw-rw-rw-   0        0        0    36389 2023-02-21 08:51:30.000000 RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/input.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.363549 RobertCommonBasic-0.1.40/robertcommonbasic/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.365549 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:18.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.367550 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/
+-rw-rw-rw-   0        0        0        0 2022-04-22 02:07:10.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/__init__.py
+-rw-rw-rw-   0        0        0     1291 2023-03-02 14:03:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.373794 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/
+-rw-rw-rw-   0        0        0        0 2022-01-19 07:38:20.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/__init__.py
+-rw-rw-rw-   0        0        0      928 2023-05-25 08:51:36.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_conversion.py
+-rw-rw-rw-   0        0        0     5920 2022-04-21 06:58:53.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py
+-rw-rw-rw-   0        0        0     2456 2022-01-27 05:56:15.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_frame.py
+-rw-rw-rw-   0        0        0     4649 2023-05-23 08:03:46.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.375953 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/
+-rw-rw-rw-   0        0        0        0 2022-03-08 05:59:28.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/__init__.py
+-rw-rw-rw-   0        0        0     2313 2023-05-25 08:43:02.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.381126 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/
+-rw-rw-rw-   0        0        0        0 2021-07-30 08:42:35.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/__init__.py
+-rw-rw-rw-   0        0        0    32599 2022-07-03 01:41:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py
+-rw-rw-rw-   0        0        0      270 2022-07-03 01:04:51.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_md5.py
+-rw-rw-rw-   0        0        0     3004 2022-11-22 07:10:43.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.383337 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/
+-rw-rw-rw-   0        0        0        0 2022-08-31 08:24:08.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-12-05 09:33:27.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.389344 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:48:14.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/__init__.py
+-rw-rw-rw-   0        0        0     1090 2023-02-03 06:30:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_csv.py
+-rw-rw-rw-   0        0        0     4285 2023-02-02 03:00:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_xml.py
+-rw-rw-rw-   0        0        0      705 2023-03-08 07:17:17.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_zip.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.392343 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/
+-rw-rw-rw-   0        0        0        0 2022-06-29 13:56:13.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/__init__.py
+-rw-rw-rw-   0        0        0      637 2023-05-16 02:40:06.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.395529 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/
+-rw-rw-rw-   0        0        0        0 2022-03-25 04:05:00.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-06-29 09:29:01.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/test_env.py
+-rw-rw-rw-   0        0        0      449 2022-11-14 02:56:25.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_os/test_file.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.397530 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/
+-rw-rw-rw-   0        0        0        0 2022-05-18 02:57:45.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/__init__.py
+-rw-rw-rw-   0        0        0      670 2023-05-23 08:45:26.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:14:25.399530 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_validation/
+-rw-rw-rw-   0        0        0        0 2021-11-19 07:34:54.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_validation/__init__.py
+-rw-rw-rw-   0        0        0      218 2022-05-10 03:46:33.000000 RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_validation/test_input.py
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:14:25.401529 RobertCommonBasic-0.1.40/setup.cfg
+-rw-rw-rw-   0        0        0     3876 2023-05-25 09:11:33.000000 RobertCommonBasic-0.1.40/setup.py
```

### Comparing `RobertCommonBasic-0.1.39/LICENSE` & `RobertCommonBasic-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/PKG-INFO` & `RobertCommonBasic-0.1.40/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.39
+Version: 0.1.40
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.39/README.md` & `RobertCommonBasic-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/PKG-INFO` & `RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonBasic
-Version: 0.1.39
+Version: 0.1.40
 Summary: Robert Common Basic Library
 Home-page: https://github.com/hun0423/RobertCommonBasic
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonBasic-0.1.39/RobertCommonBasic.egg-info/SOURCES.txt` & `RobertCommonBasic-0.1.40/RobertCommonBasic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 robertcommonbasic/basic/cls/__init__.py
 robertcommonbasic/basic/cls/utils.py
 robertcommonbasic/basic/data/__init__.py
 robertcommonbasic/basic/data/conversion.py
 robertcommonbasic/basic/data/crc16.py
 robertcommonbasic/basic/data/csv.py
 robertcommonbasic/basic/data/datatuple.py
+robertcommonbasic/basic/data/express.py
 robertcommonbasic/basic/data/frame.py
 robertcommonbasic/basic/data/nametuple.py
 robertcommonbasic/basic/data/type.py
 robertcommonbasic/basic/data/utils.py
 robertcommonbasic/basic/decorator/__init__.py
 robertcommonbasic/basic/decorator/utils.py
 robertcommonbasic/basic/dt/__init__.py
```

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/cache/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/cache/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/cls/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/cls/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/conversion.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/conversion.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/crc16.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/crc16.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/csv.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/datatuple.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/datatuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/frame.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/data/nametuple.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/data/nametuple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/decorator/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/decorator/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/dt/schedule.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/schedule.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/dt/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/dt/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/aes.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/aes.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/dsa.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/hash.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/hash.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/encrypt/rsa.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/encrypt/rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/error/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/error/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/exector/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/exector/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/csv.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/ini.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/log.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/log.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/xml.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/file/zip.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/file/zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/log/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/log/watch.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/log/watch.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/net/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/net/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/file.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/os/path.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/os/path.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/process/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/process/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/profile/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/profile/utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/re/utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/re/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 # 匹配搜索
 # \w{3}:.*?;;\n   reg:testdtu;;\n
 #  QQ交流群:(?P<QQ>\d+) blog地址:(?P<blog>.*?) 欢迎收藏
 def search_match(value: str, pattern: str = r'(?P<xxx>.*?)') -> dict:
     return re.search(pattern, value).groupdict()
 
 
-# 匹配查找
 def contain_match(value: str, filters: str = '') -> bool:
+    """模糊匹配"""
     pattern = '.*?'.join(filters.split('&'))
     if re.compile(f".*?{pattern}.*?").search(value):
         return True
     return False
 
 
 # 查找全部
```

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/basic/validation/input.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/basic/validation/input.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_cls/test_utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_cls/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_datatupple.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_frame.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_frame.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_data/test_utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_data/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import sys
 from robertcommonbasic.basic.data.utils import format_value, revert_exp, chunk_list, SimpleEval, DEFAULT_FUNCTIONS
 
+
 def test_format_value():
 
     print(f"format_value('1.234', '1') = {format_value('1.234', '1')}")
     print(f"format_value('1.234', '-2.0') = {format_value('1.234', '-2.0')}")
     print(f"format_value('-1.234', '2.0') = {format_value('-1.234', '2.0')}")
     print(f"format_value('-1.234', 'v*3') = {format_value('-1.234', 'v*3')}")
     print(f"format_value('测试', '1') = {format_value('测试', '1')}")
@@ -16,43 +17,67 @@
     print(f"format_value('1.234', 'int(v)') = {format_value('1.234', 'int(v)')}")
     print(f"format_value('2, 'bit(v, 1)') = {format_value('2', 'bit(v, 1)')}")   #取位操作
     print(f"format_value('35535, 'signed(v)') = {format_value('35535', 'signed(v)')}")  # 取位操作
     print(f"format_value('1.234', '1 if v == 20.1234 else 0') = {format_value('1.234', '1 if v == 1.234 else 0')}")
 
     print()
 
+
+def test_format_value1():
+
+    #print(f"format_value('1.234', '1') = {format_value('1.234', '1')}")
+    print(f"format_value('1.234', '1', revert=True) = {format_value('1.234', '1', revert=True)}")
+
+    #print(f"format_value('4', 'v*3') = {format_value('4', 'v*3')}")
+    print(f"format_value('12', 'v*3', revert=True) = {format_value('12', 'v*3', revert=True)}")
+
+    #print(f"format_value('1.234', 'int(v)') = {format_value('1.234', 'int(v)')}")
+    print(f"format_value('1.234', 'int(v)', revert=True) = {format_value('1.234', '-v', revert=True)}")
+
+    #print(f"format_value('2, 'bit(v, 1)') = {format_value('2', 'bit(v, 1)')}")   #取位操作
+    print(f"format_value('2, 'bit(v, 1)', revert=True) = {format_value('2', 'bit(v, 1)', revert=True)}")  # 取位操作
+
+    #print(f"format_value('1.234', '1 if v == 20.1234 else 0') = {format_value('1.234', '1 if v == 1.234 else 0')}")
+    print(f"format_value('1.234', '1 if v == 20.1234 else 0', revert=True) = {format_value('1.234', '1 if v == 1.234 else 0', revert=True)}")
+
+    print()
+
+
 def test_format_value2():
     print(format_value('5.0', '1 if v == 5 else 0'))
     print(format_value('2', '_or(bit(v, 1), bit(v, 0), _and(bit(v, 0),bit(v, 1)))'))
 
 
 def test_float_value():
     values = ['123456789.0', '-123456789.0', '9.0', '9.1', '9.12334567', '-9.0', '-9.12300000', '-0.00000567', '-0.000005670001000']
     for value in values:
         print(f"{value} {format_value(value, '1', 7)}")
     print()
 
+
 def test_format_value3():
     a = format_value('255', 'bit(v, 0)*2+bit(v, 1)')
     print(format_value('255', 'bit(v, 0)'))
     print(format_value('255', 'bit(v, 1)'))
     print(format_value('255', 'bit(v, 2)'))
     print(format_value('2', '_or(bit(v, 1), bit(v, 0), _and(bit(v, 0),bit(v, 1)))'))
 
+
 def test_format_value31():
     a = format_value(str(int(0x7B)), 'bit(v, 0)*2+bit(v, 1)')
     print(format_value('255', 'bit(v, 0)'))
     print(format_value('255', 'bit(v, 1)'))
     print(format_value('255', 'bit(v, 2)'))
     print(format_value(str(int(0x7B)), '_or(bit(v, 1), bit(v, 0), _and(bit(v, 0),bit(v, 1)))'))
 
     datas = bytes([0x7B])
     freq_ant = int(format_value(str(int(datas[0])), 'bit(v, 0)') + format_value(str(int(datas[0])), 'bit(v, 1)'))
     print(freq_ant)
 
+
 def test_nvn_value():
     result = format_value('952', '(max(4, v*3.3*1000/(4095*150))-4)/16*100', 2)
     print('{:g}'.format(6.96))
     print(format_value('2', '(max(4, v*3.3*1000/(4095*150))-4)/16*100', 3))
 
 
 def test_conver():
@@ -82,8 +107,8 @@
         expression = 'Bucket Brigade Real4 > 0'
         vs = {'Bucket Brigade Real4': 2}
         return SimpleEval(None, DEFAULT_FUNCTIONS.copy(), vs).eval(expression)
     except Exception as e:
         return None
 
 
-print(test_express())
+print(test_format_value1())
```

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_dt/test_utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_dt/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,8 +57,15 @@
 
 def test_timestamp1():
     tm = int(1676217900000 / 1000)
     data_time = convert_time(tm, 'Asia/Shanghai', 'Asia/Shanghai').replace(second=0).strftime("%Y-%m-%d %H:%M:%S")
     print(data_time)
 
 
-test_timestamp1()
+def test_zone():
+    print(datetime.now())
+    print(get_datetime())
+    print(get_datetime('Asia/Shanghai'))
+    print(get_datetime('UTC'))
+
+
+test_zone()
```

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_dsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_encrypt/test_rsa.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_exector/test_utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_exector/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/test_csv.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_csv.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/test_xml.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_xml.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_file/test_zip.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_file/test_zip.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_net/test_utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_net/test_utils.py`

 * *Files identical despite different names*

### Comparing `RobertCommonBasic-0.1.39/robertcommonbasic/tests/test_basic/test_re/test_utils.py` & `RobertCommonBasic-0.1.40/robertcommonbasic/tests/test_basic/test_re/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from robertcommonbasic.basic.re.utils import format_name, find_match
+from robertcommonbasic.basic.re.utils import format_name, find_match, contain_match, search_match
 from robertcommonbasic.basic.dt.utils import parse_time
 
 
 def test():
     name = 'Bldg3_Area1_hourly_SiteId_08-14-2021-23_00_00_PM_EDT.zip'
     time = format_name(name, r'[^0-9]+', '')
     tm = parse_time(time)
     print(tm)
 
 
 def get_expression_points(expression: str, pattern: str = r'<%(.*?)%>') -> list:
     return find_match(expression, pattern)
 
 
-points = get_expression_points('if <%Bucket Brigade.Real4%> and <%Bucket@Brigade_Real5%>')
+#points = get_expression_points('if <%Bucket Brigade.Real4%> and <%Bucket@Brigade_Real5%>')
 #points = get_expression_points('<%Bucket Brigade.Real4%>')
-print(points)
+print(find_match('bit(v,1)', r'bit\(v,(.*?)\)'))
```

### Comparing `RobertCommonBasic-0.1.39/setup.py` & `RobertCommonBasic-0.1.40/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonBasic'
 DESCRIPTION = 'Robert Common Basic Library'
 URL = 'https://github.com/hun0423/RobertCommonBasic'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.39'
-DATE = '2023-05-16'
+VERSION = '0.1.40'
+DATE = '2023-05-25'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

