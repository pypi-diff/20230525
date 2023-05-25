# Comparing `tmp/klu-0.1.3.tar.gz` & `tmp/klu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klu-0.1.3.tar", max compression
+gzip compressed data, was "klu-0.1.4.tar", max compression
```

## Comparing `klu-0.1.3.tar` & `klu-0.1.4.tar`

### file list

```diff
@@ -1,81 +1,82 @@
--rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.3/LICENSE
--rw-r--r--   0        0        0     2901 2023-05-17 21:55:04.290201 klu-0.1.3/README.md
--rw-r--r--   0        0        0      156 2023-05-07 13:13:15.007463 klu-0.1.3/klu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/action/__init__.py
--rw-r--r--   0        0        0     8899 2023-05-22 09:47:26.992552 klu-0.1.3/klu/action/client.py
--rw-r--r--   0        0        0      240 2023-05-12 01:09:37.128918 klu-0.1.3/klu/action/constants.py
--rw-r--r--   0        0        0      542 2023-05-01 22:54:25.386914 klu-0.1.3/klu/action/errors.py
--rw-r--r--   0        0        0     1556 2023-05-17 21:20:44.320408 klu-0.1.3/klu/action/models.py
--rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.3/klu/api/__init__.py
--rw-r--r--   0        0        0     2974 2023-05-18 00:16:38.076364 klu-0.1.3/klu/api/client.py
--rw-r--r--   0        0        0      199 2023-05-16 02:22:01.505533 klu-0.1.3/klu/api/config.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.3/klu/application/__init__.py
--rw-r--r--   0        0        0     4495 2023-05-22 09:47:26.996122 klu-0.1.3/klu/application/client.py
--rw-r--r--   0        0        0      230 2023-05-07 22:43:35.165346 klu-0.1.3/klu/application/constants.py
--rw-r--r--   0        0        0      325 2023-05-18 00:09:26.025264 klu-0.1.3/klu/application/errors.py
--rw-r--r--   0        0        0     1303 2023-05-16 01:32:56.622223 klu-0.1.3/klu/application/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/client/__init__.py
--rw-r--r--   0        0        0      714 2023-05-16 00:56:56.414877 klu-0.1.3/klu/client/klu.py
--rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.3/klu/common/__init__.py
--rw-r--r--   0        0        0     3103 2023-05-17 23:44:49.628180 klu-0.1.3/klu/common/client.py
--rw-r--r--   0        0        0     2967 2023-05-18 00:09:26.039775 klu-0.1.3/klu/common/errors.py
--rw-r--r--   0        0        0     2268 2023-05-07 22:15:35.049953 klu-0.1.3/klu/common/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/data/__init__.py
--rw-r--r--   0        0        0     2240 2023-05-17 21:42:29.875608 klu-0.1.3/klu/data/client.py
--rw-r--r--   0        0        0       24 2023-04-20 00:36:52.119366 klu-0.1.3/klu/data/constants.py
--rw-r--r--   0        0        0      281 2023-05-18 00:09:26.054468 klu-0.1.3/klu/data/errors.py
--rw-r--r--   0        0        0     2537 2023-05-16 00:57:12.476673 klu-0.1.3/klu/data/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/data_index/__init__.py
--rw-r--r--   0        0        0     8382 2023-05-21 21:56:32.827298 klu-0.1.3/klu/data_index/client.py
--rw-r--r--   0        0        0      289 2023-05-15 02:29:51.422572 klu-0.1.3/klu/data_index/constants.py
--rw-r--r--   0        0        0      316 2023-05-18 00:09:26.046973 klu-0.1.3/klu/data_index/errors.py
--rw-r--r--   0        0        0     3263 2023-05-21 21:41:28.245219 klu-0.1.3/klu/data_index/models.py
--rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.3/klu/klu.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/model/__init__.py
--rw-r--r--   0        0        0     3306 2023-05-16 00:57:12.491877 klu-0.1.3/klu/model/client.py
--rw-r--r--   0        0        0       27 2023-04-22 00:45:10.009144 klu-0.1.3/klu/model/constants.py
--rw-r--r--   0        0        0      454 2023-05-18 00:09:26.016842 klu-0.1.3/klu/model/errors.py
--rw-r--r--   0        0        0     1193 2023-05-17 00:20:41.308393 klu-0.1.3/klu/model/models.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/session/__init__.py
--rw-r--r--   0        0        0     1412 2023-05-16 01:10:51.006332 klu-0.1.3/klu/session/client.py
--rw-r--r--   0        0        0       31 2023-05-15 22:59:54.895982 klu-0.1.3/klu/session/constants.py
--rw-r--r--   0        0        0     1094 2023-05-16 00:57:12.477952 klu-0.1.3/klu/session/models.py
--rw-r--r--   0        0        0      111 2023-05-11 23:52:15.155255 klu-0.1.3/klu/utils/dict_helpers.py
--rw-r--r--   0        0        0      719 2023-05-01 22:31:07.149352 klu-0.1.3/klu/utils/file_upload.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/klu/workspace/__init__.py
--rw-r--r--   0        0        0     5379 2023-05-16 00:57:12.528580 klu-0.1.3/klu/workspace/client.py
--rw-r--r--   0        0        0      287 2023-05-08 01:20:03.988036 klu-0.1.3/klu/workspace/constants.py
--rw-r--r--   0        0        0      244 2023-05-18 00:09:26.033318 klu-0.1.3/klu/workspace/errors.py
--rw-r--r--   0        0        0      815 2023-05-15 22:31:50.548346 klu-0.1.3/klu/workspace/models.py
--rw-r--r--   0        0        0     2797 2023-05-22 17:59:47.479804 klu-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      103 2023-05-15 22:17:30.645200 klu-0.1.3/tests/integration/__init__.py
--rw-r--r--   0        0        0      128 2023-05-21 22:12:08.785805 klu-0.1.3/tests/integration/conftest.py
--rw-r--r--   0        0        0      252 2023-05-21 21:34:27.629928 klu-0.1.3/tests/integration/constants.py
--rw-r--r--   0        0        0        0 2023-05-17 01:53:20.259063 klu-0.1.3/tests/integration/files/__init__.py
--rw-r--r--   0        0        0   108574 2021-08-07 16:43:25.870000 klu-0.1.3/tests/integration/files/test-file-upload.pdf
--rw-r--r--   0        0        0     2298 2023-05-22 09:47:26.998235 klu-0.1.3/tests/integration/test_actions.py
--rw-r--r--   0        0        0     2269 2023-05-17 01:35:02.115114 klu-0.1.3/tests/integration/test_applications.py
--rw-r--r--   0        0        0     1148 2023-05-17 01:34:42.355919 klu-0.1.3/tests/integration/test_data.py
--rw-r--r--   0        0        0     2864 2023-05-21 21:55:43.590354 klu-0.1.3/tests/integration/test_data_index.py
--rw-r--r--   0        0        0      958 2023-05-17 01:35:15.023120 klu-0.1.3/tests/integration/test_models.py
--rw-r--r--   0        0        0     2263 2023-05-17 01:35:19.655390 klu-0.1.3/tests/integration/test_workspaces.py
--rw-r--r--   0        0        0     1417 2023-05-17 01:19:00.625257 klu-0.1.3/tests/integration/utils/actions.py
--rw-r--r--   0        0        0      752 2023-05-17 01:19:00.668605 klu-0.1.3/tests/integration/utils/applications.py
--rw-r--r--   0        0        0       68 2023-05-15 22:17:30.698602 klu-0.1.3/tests/integration/utils/common.py
--rw-r--r--   0        0        0     1555 2023-05-17 01:27:25.631403 klu-0.1.3/tests/integration/utils/data.py
--rw-r--r--   0        0        0      816 2023-05-17 01:27:25.638985 klu-0.1.3/tests/integration/utils/data_index.py
--rw-r--r--   0        0        0      830 2023-05-17 00:39:43.353577 klu-0.1.3/tests/integration/utils/models.py
--rw-r--r--   0        0        0      842 2023-05-17 01:19:00.583265 klu-0.1.3/tests/integration/utils/sessions.py
--rw-r--r--   0        0        0      658 2023-05-17 01:19:00.519346 klu-0.1.3/tests/integration/utils/workspace.py
--rw-r--r--   0        0        0        0 2023-05-08 13:03:00.679856 klu-0.1.3/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/tests/unit/action/__init__.py
--rw-r--r--   0        0        0     1702 2023-05-21 22:55:58.704587 klu-0.1.3/tests/unit/action/test_client.py
--rw-r--r--   0        0        0     1156 2023-05-15 21:48:29.904995 klu-0.1.3/tests/unit/action/utils.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/tests/unit/application/__init__.py
--rw-r--r--   0        0        0     1438 2023-05-21 22:39:04.530407 klu-0.1.3/tests/unit/application/test_client.py
--rw-r--r--   0        0        0     1170 2023-05-16 00:57:16.848585 klu-0.1.3/tests/unit/application/utils.py
--rw-r--r--   0        0        0      156 2023-05-21 22:55:55.517974 klu-0.1.3/tests/unit/conftest.py
--rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.3/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0      768 2023-05-01 22:56:20.546102 klu-0.1.3/tests/unit/utils/mock.py
--rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 klu-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-02 23:20:08.165888 klu-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2901 2023-05-17 21:55:04.290201 klu-0.1.4/README.md
+-rw-r--r--   0        0        0      156 2023-05-07 13:13:15.007463 klu-0.1.4/klu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/action/__init__.py
+-rw-r--r--   0        0        0    12135 2023-05-25 10:19:42.438116 klu-0.1.4/klu/action/client.py
+-rw-r--r--   0        0        0      272 2023-05-23 00:00:29.822238 klu-0.1.4/klu/action/constants.py
+-rw-r--r--   0        0        0      542 2023-05-01 22:54:25.386914 klu-0.1.4/klu/action/errors.py
+-rw-r--r--   0        0        0     1700 2023-05-24 12:53:09.893852 klu-0.1.4/klu/action/models.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:33:25.776741 klu-0.1.4/klu/api/__init__.py
+-rw-r--r--   0        0        0     3516 2023-05-24 00:48:31.834759 klu-0.1.4/klu/api/client.py
+-rw-r--r--   0        0        0      199 2023-05-16 02:22:01.505533 klu-0.1.4/klu/api/config.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648620 klu-0.1.4/klu/application/__init__.py
+-rw-r--r--   0        0        0     7677 2023-05-22 23:57:57.911029 klu-0.1.4/klu/application/client.py
+-rw-r--r--   0        0        0      259 2023-05-22 23:48:54.892441 klu-0.1.4/klu/application/constants.py
+-rw-r--r--   0        0        0      325 2023-05-18 00:09:26.025264 klu-0.1.4/klu/application/errors.py
+-rw-r--r--   0        0        0     1303 2023-05-16 01:32:56.622223 klu-0.1.4/klu/application/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/client/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-16 00:56:56.414877 klu-0.1.4/klu/client/klu.py
+-rw-r--r--   0        0        0        0 2023-04-17 20:44:45.994154 klu-0.1.4/klu/common/__init__.py
+-rw-r--r--   0        0        0     3103 2023-05-17 23:44:49.628180 klu-0.1.4/klu/common/client.py
+-rw-r--r--   0        0        0     2967 2023-05-18 00:09:26.039775 klu-0.1.4/klu/common/errors.py
+-rw-r--r--   0        0        0     2268 2023-05-07 22:15:35.049953 klu-0.1.4/klu/common/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/data/__init__.py
+-rw-r--r--   0        0        0     2240 2023-05-17 21:42:29.875608 klu-0.1.4/klu/data/client.py
+-rw-r--r--   0        0        0       24 2023-04-20 00:36:52.119366 klu-0.1.4/klu/data/constants.py
+-rw-r--r--   0        0        0      281 2023-05-18 00:09:26.054468 klu-0.1.4/klu/data/errors.py
+-rw-r--r--   0        0        0     2537 2023-05-16 00:57:12.476673 klu-0.1.4/klu/data/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/data_index/__init__.py
+-rw-r--r--   0        0        0     8445 2023-05-22 18:49:52.214610 klu-0.1.4/klu/data_index/client.py
+-rw-r--r--   0        0        0      289 2023-05-15 02:29:51.422572 klu-0.1.4/klu/data_index/constants.py
+-rw-r--r--   0        0        0      316 2023-05-18 00:09:26.046973 klu-0.1.4/klu/data_index/errors.py
+-rw-r--r--   0        0        0     3263 2023-05-21 21:41:28.245219 klu-0.1.4/klu/data_index/models.py
+-rw-r--r--   0        0        0       19 2023-04-02 23:20:08.167789 klu-0.1.4/klu/klu.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/model/__init__.py
+-rw-r--r--   0        0        0     3450 2023-05-22 18:50:10.373905 klu-0.1.4/klu/model/client.py
+-rw-r--r--   0        0        0       27 2023-04-22 00:45:10.009144 klu-0.1.4/klu/model/constants.py
+-rw-r--r--   0        0        0      454 2023-05-18 00:09:26.016842 klu-0.1.4/klu/model/errors.py
+-rw-r--r--   0        0        0     1193 2023-05-17 00:20:41.308393 klu-0.1.4/klu/model/models.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/session/__init__.py
+-rw-r--r--   0        0        0     1412 2023-05-16 01:10:51.006332 klu-0.1.4/klu/session/client.py
+-rw-r--r--   0        0        0       31 2023-05-15 22:59:54.895982 klu-0.1.4/klu/session/constants.py
+-rw-r--r--   0        0        0     1094 2023-05-16 00:57:12.477952 klu-0.1.4/klu/session/models.py
+-rw-r--r--   0        0        0      111 2023-05-11 23:52:15.155255 klu-0.1.4/klu/utils/dict_helpers.py
+-rw-r--r--   0        0        0      719 2023-05-01 22:31:07.149352 klu-0.1.4/klu/utils/file_upload.py
+-rw-r--r--   0        0        0     2308 2023-05-22 23:37:24.956177 klu-0.1.4/klu/utils/paginator.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/klu/workspace/__init__.py
+-rw-r--r--   0        0        0     7968 2023-05-23 00:00:29.836509 klu-0.1.4/klu/workspace/client.py
+-rw-r--r--   0        0        0      321 2023-05-22 23:57:57.890361 klu-0.1.4/klu/workspace/constants.py
+-rw-r--r--   0        0        0      244 2023-05-18 00:09:26.033318 klu-0.1.4/klu/workspace/errors.py
+-rw-r--r--   0        0        0      815 2023-05-15 22:31:50.548346 klu-0.1.4/klu/workspace/models.py
+-rw-r--r--   0        0        0     2797 2023-05-25 10:18:27.765075 klu-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-02 23:20:08.169124 klu-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-15 22:17:30.645200 klu-0.1.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0      128 2023-05-21 22:12:08.785805 klu-0.1.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0      252 2023-05-24 21:54:58.783798 klu-0.1.4/tests/integration/constants.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:53:20.259063 klu-0.1.4/tests/integration/files/__init__.py
+-rw-r--r--   0        0        0   108574 2021-08-07 16:43:25.870000 klu-0.1.4/tests/integration/files/test-file-upload.pdf
+-rw-r--r--   0        0        0     4782 2023-05-24 23:20:44.781905 klu-0.1.4/tests/integration/test_actions.py
+-rw-r--r--   0        0        0     3749 2023-05-22 23:33:40.123465 klu-0.1.4/tests/integration/test_applications.py
+-rw-r--r--   0        0        0     1148 2023-05-17 01:34:42.355919 klu-0.1.4/tests/integration/test_data.py
+-rw-r--r--   0        0        0     2864 2023-05-21 21:55:43.590354 klu-0.1.4/tests/integration/test_data_index.py
+-rw-r--r--   0        0        0      958 2023-05-17 01:35:15.023120 klu-0.1.4/tests/integration/test_models.py
+-rw-r--r--   0        0        0     2263 2023-05-17 01:35:19.655390 klu-0.1.4/tests/integration/test_workspaces.py
+-rw-r--r--   0        0        0     1435 2023-05-24 12:44:20.921698 klu-0.1.4/tests/integration/utils/actions.py
+-rw-r--r--   0        0        0      752 2023-05-17 01:19:00.668605 klu-0.1.4/tests/integration/utils/applications.py
+-rw-r--r--   0        0        0       68 2023-05-15 22:17:30.698602 klu-0.1.4/tests/integration/utils/common.py
+-rw-r--r--   0        0        0     1555 2023-05-17 01:27:25.631403 klu-0.1.4/tests/integration/utils/data.py
+-rw-r--r--   0        0        0      816 2023-05-17 01:27:25.638985 klu-0.1.4/tests/integration/utils/data_index.py
+-rw-r--r--   0        0        0      830 2023-05-24 23:19:18.771498 klu-0.1.4/tests/integration/utils/models.py
+-rw-r--r--   0        0        0      842 2023-05-17 01:19:00.583265 klu-0.1.4/tests/integration/utils/sessions.py
+-rw-r--r--   0        0        0      658 2023-05-17 01:19:00.519346 klu-0.1.4/tests/integration/utils/workspace.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:03:00.679856 klu-0.1.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/tests/unit/action/__init__.py
+-rw-r--r--   0        0        0     1692 2023-05-23 00:20:51.639436 klu-0.1.4/tests/unit/action/test_client.py
+-rw-r--r--   0        0        0     1156 2023-05-15 21:48:29.904995 klu-0.1.4/tests/unit/action/utils.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/tests/unit/application/__init__.py
+-rw-r--r--   0        0        0     1433 2023-05-23 00:20:51.607538 klu-0.1.4/tests/unit/application/test_client.py
+-rw-r--r--   0        0        0     1170 2023-05-16 00:57:16.848585 klu-0.1.4/tests/unit/application/utils.py
+-rw-r--r--   0        0        0      156 2023-05-21 22:55:55.517974 klu-0.1.4/tests/unit/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:47:20.648000 klu-0.1.4/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-01 22:56:20.546102 klu-0.1.4/tests/unit/utils/mock.py
+-rw-r--r--   0        0        0     4989 1970-01-01 00:00:00.000000 klu-0.1.4/PKG-INFO
```

### Comparing `klu-0.1.3/LICENSE` & `klu-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/README.md` & `klu-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/action/client.py` & `klu-0.1.4/klu/action/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, AsyncGenerator, List
+from typing import Optional, List
 
 import aiohttp
 from aiohttp import ClientResponseError
 from aiohttp.web_exceptions import HTTPNotFound
 
 from klu.common.errors import (
     UnknownKluError,
@@ -10,26 +10,29 @@
     InvalidUpdateParamsError,
 )
 from klu.action.constants import (
     ACTION_ENDPOINT,
     ACTION_DATA_ENDPOINT,
     CREATE_ACTION_ENDPOINT,
     PLAYGROUND_PROMPT_ENDPOINT,
+    DEFAULT_ACTIONS_PAGE_SIZE,
 )
 from klu.data.models import Data
+from klu.utils.paginator import Paginator
 from klu.common.client import KluClientBase
 from klu.utils.dict_helpers import dict_no_empty
 from klu.action.models import PromptResponse, Action
 from klu.workspace.errors import WorkspaceOrUserNotFoundError
 from klu.action.errors import ActionNotFoundError, InvalidActionPromptData
 
 
 class ActionsClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, ACTION_ENDPOINT, Action)
+        self._paginator = Paginator(ACTION_ENDPOINT)
 
     async def create(
         self,
         name: str,
         prompt: str,
         app_guid: str,
         model_guid: int,
@@ -41,15 +44,15 @@
         Creates new action instance
 
         Args:
             name (str): Action name
             prompt (str): Action prompt
             model_guid (int): Guid of a model used for action
             app_guid (str): GUID of the application for an action to be attached to
-            action_type (str): The type of the action
+            action_type (str): The type of the action. Can be one of [simple, complex, document-search, full-ai, custom]
             description (str): The description of the action
             model_config (str): Optional action model configuration dict
 
         Returns: Newly created Action object
         """
         return await super().create(
             name=name,
@@ -154,24 +157,23 @@
                         "filter": filter,
                         "action": action_guid,
                         "streaming": streaming,
                         "async_mode": async_mode,
                         "sessionGuid": session_guid,
                     },
                 )
+                return PromptResponse(**response)
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise ActionNotFoundError(action_guid)
 
                 raise UnknownKluAPIError(e.status, e.message)
             except Exception:
                 raise UnknownKluError()
 
-            return PromptResponse(**response)
-
     async def run_playground_prompt(
         self,
         prompt: str,
         model_id: int,
         tool_ids: Optional[list] = None,
         index_ids: Optional[list] = None,
         model_config: Optional[dict] = None,
@@ -201,42 +203,47 @@
                         "prompt": prompt,
                         "toolIds": tool_ids,
                         "modelId": model_id,
                         "indexIds": index_ids,
                         "modelConfig": model_config,
                     },
                 )
+                return PromptResponse(**response)
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise WorkspaceOrUserNotFoundError()
                 if e.status == 400:
                     raise InvalidActionPromptData(e.message)
 
-            return PromptResponse(**response)
-
-    async def get_action_streaming_data(self, streaming_url: str) -> AsyncGenerator[str, None]:
-        """
-        Get a streams of messages from an SQS queue for a specific channel.
-
-        Args:
-            streaming_url (str): The url you received from run_action_prompt with streaming param set to True.
-
-        Returns:
-            An asynchronous generator, which can be used to read chunks of data from the streaming url. Usage example:
-
-            async for chunk in get_streaming_data():
-                # Process the chunk of data here
-                print(chunk)
-        """
-        async with aiohttp.ClientSession() as session:
-            client = self._get_api_client(session)
+                raise UnknownKluAPIError(e.status, e.message)
+            except Exception:
+                raise UnknownKluError()
 
-            async with client.get(streaming_url) as response:
-                async for chunk in response.content.iter_chunked():
-                    yield chunk
+    # async def get_action_streaming_data(self, streaming_url: str) -> AsyncIterator[str]:
+    #     """
+    #     Get a streams of messages from an SQS queue for a specific channel.
+    #
+    #     Args:
+    #         streaming_url (str): The url you received from run_action_prompt with streaming param set to True.
+    #
+    #     Returns:
+    #         An asynchronous generator, which can be used to read chunks of data from the streaming url. Usage example:
+    #
+    #         async for chunk in get_streaming_data():
+    #             # Process the chunk of data here
+    #             print(chunk)
+    #     """
+    #     async with aiohttp.ClientSession() as session:
+    #         client = self._get_api_client(session)
+    #
+    #         async for data in client.get_streaming_data(streaming_url):
+    #             if data == "No messages to stream":
+    #                 client.get_streaming_data(streaming_url).aclose()
+    #
+    #             yield data
 
     async def get_action_data(self, id: str) -> List[Data]:
         """
         Retrieves data information for an action.
 
         Args:
             id (str): Guid of an action to fetch data for.
@@ -244,12 +251,75 @@
         Returns: An array of actions found by provided app id.
         """
         async with aiohttp.ClientSession() as session:
             client = self._get_api_client(session)
 
             try:
                 response = await client.get(ACTION_DATA_ENDPOINT.format(id=id))
+                return [Data._from_engine_format(data) for data in response]
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise ActionNotFoundError(id)
 
-            return [Data._from_engine_format(data) for data in response]
+                raise UnknownKluAPIError(e.status, e.message)
+            except Exception:
+                raise UnknownKluError()
+
+    async def list(self) -> List[Action]:
+        """
+        Retrieves all actions for a user represented by the used API_KEY.
+        Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
+
+        Returns: An array of all actions
+        """
+        async with aiohttp.ClientSession() as session:
+            client = self._get_api_client(session)
+            response = await self._paginator.fetch_all(client)
+
+            return [Action._from_engine_format(action) for action in response]
+
+    async def fetch_single_page(
+        self, page_number, limit: int = DEFAULT_ACTIONS_PAGE_SIZE
+    ) -> List[Action]:
+        """
+        Retrieves a single page of actions.
+        Can be used to fetch a specific page of actions provided a certain per_page config.
+        Does not rely on internal paginator state, so `reset_pagination` method call can be skipped
+
+        Args:
+            page_number (int): Number of the page to fetch
+            limit (int): Number of instances to fetch per page. Defaults to 50
+
+        Returns: An array of actions fetched for a queried page. Empty if queried page does not exist
+        """
+        async with aiohttp.ClientSession() as session:
+            client = self._get_api_client(session)
+            response = await self._paginator.fetch_single_page(
+                client, page_number, limit=limit
+            )
+
+            return [Action._from_engine_format(action) for action in response]
+
+    async def fetch_next_page(
+        self, limit: int = DEFAULT_ACTIONS_PAGE_SIZE, offset: int = None
+    ) -> List[Action]:
+        """
+        Retrieves the next page of actions. Can be used to fetch a flexible number of pages starting.
+        The place to start from can be controlled by the offset parameter.
+        After using this method, we suggest to call `reset_pagination` method to reset the page cursor.
+
+        Args:
+            limit (int): Number of instances to fetch per page. Defaults to 50
+            offset (int): The number of instances to skip. Can be used to query the pages of actions skipping certain number of instances.
+
+        Returns: An array of actions fetched for a queried page. Empty if the end was reached at the previous step.
+        """
+        async with aiohttp.ClientSession() as session:
+            client = self._get_api_client(session)
+            response = await self._paginator.fetch_next_page(
+                client, limit=limit, offset=offset
+            )
+
+            return [Action._from_engine_format(action) for action in response]
+
+    async def reset_pagination(self):
+        self._paginator = Paginator(ACTION_ENDPOINT)
```

### Comparing `klu-0.1.3/klu/action/errors.py` & `klu-0.1.4/klu/action/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/action/models.py` & `klu-0.1.4/klu/model/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,39 @@
 from typing import Optional
 from datetime import datetime
 from dataclasses import dataclass, asdict
 
-from klu.common.models import BaseEngineModel, BaseDataClass
+from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Action(BaseEngineModel):
+class Model(BaseEngineModel):
+    id: int
+    llm: str
     guid: str
-    name: str
-    prompt: str
-    app_id: int
-    model_id: int
-    description: Optional[str]
-    model_config: Optional[dict]
-    experiment_id: Optional[int] = None
+    model_name: str
+    created_by_id: str
+    workspace_model_provider_id: int
     updated_at: Optional[datetime] = None
     created_at: Optional[datetime] = None
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Action":
+    def _from_engine_format(cls, data: dict) -> "Model":
         return cls._create_instance(
             **{
-                "app_id": data.pop("appId", None),
-                "model_id": data.pop("modelId", None),
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
-                "experiment_id": data.pop("experimentId", None),
+                "created_by_id": data.pop("createdById", None),
+                "workspace_model_provider_id": data.pop("workspaceModelProviderId", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self)
+        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
-        return {
-            "appId": base_dict.pop("app_id", None),
-            "modelId": base_dict.pop("model_id", None),
-            "updatedAt": base_dict.pop("updated_at", None),
-            "createdAt": base_dict.pop("created_at", None),
-            "experimentId": base_dict.pop("experiment_id", None),
-            **base_dict,
-        }
+        base_dict.pop("updated_at", None)
+        base_dict.pop("created_at", None)
+        base_dict.pop("created_by_id", None)
+        base_dict.pop("workspace_model_provider_id", None)
 
-
-@dataclass
-class PromptResponse(BaseDataClass):
-    msg: str
-    streaming: bool
-    result_url: Optional[str] = None
-    feedback_url: Optional[str] = None
-    streaming_url: Optional[str] = None
+        return base_dict
```

### Comparing `klu-0.1.3/klu/api/client.py` & `klu-0.1.4/klu/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import wraps
 
 import aiohttp
 
-from typing import List, Union, Optional
+from typing import List, Union, Optional, AsyncIterator
 
 from aiohttp import ClientResponseError
 from aiohttp.web_exceptions import HTTPNotFound
 
 from klu.api.config import get_api_url
 from klu.common.errors import (
     UnknownKluError,
@@ -48,38 +48,57 @@
         self.session = session
         self.api_url = get_api_url()
         self.headers = {"Authorization": f"Bearer {api_key}"}
 
     @_handle_http_exception
     async def get(self, path: str, params: dict = None) -> Union[dict, List[dict]]:
         url = f"{self.api_url}{path}"
-        async with self.session.get(url, params=params, headers=self.headers) as response:
+        async with self.session.get(
+            url, params=params, headers=self.headers
+        ) as response:
             response.raise_for_status()
             return await response.json()
 
     @_handle_http_exception
     async def post(self, path: str, json_data: Optional[dict] = None) -> dict:
         url = f"{self.api_url}{path}"
-        async with self.session.post(url, json=json_data, headers=self.headers) as response:
+        async with self.session.post(
+            url, json=json_data, headers=self.headers
+        ) as response:
             if not response.ok and response.content_type == "application/json":
                 content = await response.json()
                 detail_message = content.get("detail") if content else None
 
                 if detail_message:
                     response.reason = detail_message
 
             response.raise_for_status()
             return await response.json()
 
     @_handle_http_exception
     async def put(self, path: str, json_data: dict) -> dict:
         url = f"{self.api_url}{path}"
-        async with self.session.put(url, json=json_data, headers=self.headers) as response:
+        async with self.session.put(
+            url, json=json_data, headers=self.headers
+        ) as response:
             response.raise_for_status()
             return await response.json()
 
     @_handle_http_exception
     async def delete(self, path: str) -> dict:
         url = f"{self.api_url}{path}"
         async with self.session.delete(url, headers=self.headers) as response:
             response.raise_for_status()
             return await response.json()
+
+    async def get_streaming_data(self, url: str) -> AsyncIterator[str]:
+        try:
+            async with self.session.get(url) as response:
+                response.raise_for_status()
+
+                async for data in response.content.iter_any():
+                    yield data.decode("utf-8")
+
+        except ClientResponseError as e:
+            raise UnknownKluAPIError(e.status, e.message)
+        except Exception:
+            raise UnknownKluError()
```

### Comparing `klu-0.1.3/klu/application/models.py` & `klu-0.1.4/klu/application/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/client/klu.py` & `klu-0.1.4/klu/client/klu.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/common/client.py` & `klu-0.1.4/klu/common/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/common/errors.py` & `klu-0.1.4/klu/common/errors.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/common/models.py` & `klu-0.1.4/klu/common/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/data/client.py` & `klu-0.1.4/klu/data/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/data/models.py` & `klu-0.1.4/klu/data/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/data_index/client.py` & `klu-0.1.4/klu/data_index/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,16 @@
             client = self._get_api_client(session)
             try:
                 response = await client.post(DATA_INDEX_STATUS_ENDPOINT.format(id=guid))
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise DataIndexNotFoundError(guid)
 
+                raise UnknownKluAPIError(e.status, e.message)
+
             return DataIndexStatusEnum.get(response.get("status"))
 
     async def process_data_index(self, data_index_guid: str, file_name: str, splitter: Optional[str] = None) -> dict:
         """
         Processes existing index identified by provided data_index id using provider column splitter
 
         Args:
```

### Comparing `klu-0.1.3/klu/data_index/models.py` & `klu-0.1.4/klu/data_index/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/model/client.py` & `klu-0.1.4/klu/model/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from klu.model.models import Model
 from klu.common.models import KluId
 from klu.common.client import KluClientBase
 from klu.model.constants import MODEL_ENDPOINT
 from klu.utils.dict_helpers import dict_no_empty
 from klu.model.errors import UnknownModelProviderError
-from klu.common.errors import InvalidUpdateParamsError
+from klu.common.errors import InvalidUpdateParamsError, UnknownKluAPIError
 
 
 class ModelsClient(KluClientBase):
     def __init__(self, api_key: str):
         super().__init__(api_key, MODEL_ENDPOINT, Model)
 
     async def create(self, llm: str, workspace_model_provider_id: int) -> Model:
@@ -25,42 +25,48 @@
         Args:
             llm (str): Model llm. Required
             workspace_model_provider_id (str): Unique identifier of model provider.
                 Can be retrieved from a model providers listing endpoint.
 
         Returns: A newly created Model object.
         """
-        return await super().create(llm=llm, workspaceModelProviderId=workspace_model_provider_id)
+        return await super().create(
+            llm=llm, workspaceModelProviderId=workspace_model_provider_id
+        )
 
     async def get(self, guid: str) -> Model:
         """
         Retrieves model  information based on the id.
 
         Args:
             guid (str): GUID of a model to fetch. The one that was used during the model creation
 
         Returns: Model object
         """
         return await super().get(guid)
 
-    async def update(self, id: str, llm: Optional[str] = None, key: Optional[str] = None) -> Model:
+    async def update(
+        self, id: str, llm: Optional[str] = None, key: Optional[str] = None
+    ) -> Model:
         """
         Update model data. At least one of the params has to be provided
 
         Args:
             id (str): ID of a data_index to update.
             llm: Optional[str]. New data_index name
             key: Optional[str]. New data_index description
 
         Returns: Updated application instance
         """
         if not llm and not key:
             raise InvalidUpdateParamsError()
 
-        return await super().update(**{"id": id, **dict_no_empty({"llm": llm, "key": key})})
+        return await super().update(
+            **{"id": id, **dict_no_empty({"llm": llm, "key": key})}
+        )
 
     async def delete(self, id: KluId) -> Model:
         """
         Delete model based on the id.
 
         Args:
             id (str): ID of a model to delete.
@@ -85,12 +91,13 @@
                 response = await client.post(
                     MODEL_ENDPOINT,
                     {
                         "api_key": api_key,
                         "provider": provider,
                     },
                 )
+                return bool(response.get("validated"))
             except (HTTPNotFound, ClientResponseError) as e:
                 if e.status == 404:
                     raise UnknownModelProviderError(provider)
 
-            return bool(response.get("validated"))
+                raise UnknownKluAPIError(e.status, e.message)
```

### Comparing `klu-0.1.3/klu/model/models.py` & `klu-0.1.4/klu/session/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 from datetime import datetime
 from dataclasses import dataclass, asdict
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Model(BaseEngineModel):
+class Session(BaseEngineModel):
     id: int
-    llm: str
     guid: str
-    model_name: str
+    action_id: int
     created_by_id: str
-    workspace_model_provider_id: int
-    updated_at: Optional[datetime] = None
     created_at: Optional[datetime] = None
+    updated_at: Optional[datetime] = None
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Model":
+    def _from_engine_format(cls, data: dict) -> "Session":
         return cls._create_instance(
             **{
+                "action_id": data.pop("actionId", None),
                 "updated_at": data.pop("updatedAt", None),
                 "created_at": data.pop("createdAt", None),
                 "created_by_id": data.pop("createdById", None),
-                "workspace_model_provider_id": data.pop("workspaceModelProviderId", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
         base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
 
+        base_dict.pop("action_id", None)
         base_dict.pop("updated_at", None)
         base_dict.pop("created_at", None)
         base_dict.pop("created_by_id", None)
-        base_dict.pop("workspace_model_provider_id", None)
 
         return base_dict
```

### Comparing `klu-0.1.3/klu/session/client.py` & `klu-0.1.4/klu/session/client.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/klu/session/models.py` & `klu-0.1.4/klu/workspace/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-from typing import Optional
-from datetime import datetime
+from uuid import UUID, uuid4
 from dataclasses import dataclass, asdict
 
 from klu.common.models import BaseEngineModel
 
 
 @dataclass
-class Session(BaseEngineModel):
-    id: int
-    guid: str
-    action_id: int
+class Workspace(BaseEngineModel):
+    id: str
+    name: str
+    slug: str
     created_by_id: str
-    created_at: Optional[datetime] = None
-    updated_at: Optional[datetime] = None
+    """
+        Workspace unique identifier. This is the id you can later use to query this object and create application.
+    """
+    project_guid: str
 
     @classmethod
-    def _from_engine_format(cls, data: dict) -> "Session":
+    def _from_engine_format(cls, data: dict) -> "Workspace":
         return cls._create_instance(
             **{
-                "action_id": data.pop("actionId", None),
-                "updated_at": data.pop("updatedAt", None),
-                "created_at": data.pop("createdAt", None),
                 "created_by_id": data.pop("createdById", None),
             },
             **data,
         )
 
     def _to_engine_format(self) -> dict:
-        base_dict = asdict(self, dict_factory=lambda x: {k: v for (k, v) in x if v is not None})
+        base_dict = asdict(self)
 
-        base_dict.pop("action_id", None)
-        base_dict.pop("updated_at", None)
-        base_dict.pop("created_at", None)
-        base_dict.pop("created_by_id", None)
-
-        return base_dict
+        return {
+            "createdById": base_dict.pop("created_by_id", None),
+            **base_dict,
+        }
```

### Comparing `klu-0.1.3/klu/utils/file_upload.py` & `klu-0.1.4/klu/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/pyproject.toml` & `klu-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "klu"
-version = "0.1.3"
+version = "0.1.4"
 homepage = "https://github.com/ssabev/klu"
 description = "SDK for building AI Enabled apps."
 authors = ["Stefan Sabev <stefan@launchpad.pm>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `klu-0.1.3/tests/integration/files/test-file-upload.pdf` & `klu-0.1.4/tests/integration/files/test-file-upload.pdf`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/test_applications.py` & `klu-0.1.4/tests/integration/test_applications.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+import math
 from uuid import uuid4
 
 import pytest
 
 from klu.client.klu import KluClient
 
 from tests.integration.constants import API_KEY
+from tests.integration.utils.applications import (
+    create_application,
+    get_unique_test_app_name,
+)
 from tests.integration.utils.data import create_data
 from tests.integration.utils.actions import create_action
 from tests.integration.utils.models import ModelSingleton
-from tests.integration.utils.applications import create_application
 
 client = KluClient(API_KEY)
 
 model_singleton = ModelSingleton()
 
 
-def get_test_app_name() -> str:
-    return f"test-app-name-{str(uuid4())}"
-
-
 @pytest.mark.asyncio
 async def test_list_app_data():
     default_model = await model_singleton.get_default_model()
 
     app = await create_application()
     action = await create_action(app_guid=app.guid, model_guid=default_model.guid)
 
@@ -42,16 +42,71 @@
     await create_action(app_guid=app.guid, model_guid=default_model.guid)
 
     actions = await client.applications.get_app_actions(app.guid)
     assert len(actions) == 2
 
 
 @pytest.mark.asyncio
+async def test_list_all_apps():
+    await create_application()
+    await create_application()
+
+    apps = await client.applications.list()
+    assert len(apps) >= 2
+
+
+@pytest.mark.asyncio
+async def test_get_app_page():
+    await create_application()
+    await create_application()
+    await create_application()
+    await create_application()
+
+    apps_page_1 = await client.applications.fetch_single_page(1, limit=2)
+    apps_page_2 = await client.applications.fetch_single_page(2, limit=2)
+
+    assert len(apps_page_1) == 2
+    assert len(apps_page_2) == 2
+
+    for index, page_2_app in enumerate(apps_page_2):
+        page_1_app = apps_page_1[index]
+        assert page_2_app.created_at > page_1_app.created_at
+
+
+@pytest.mark.asyncio
+async def test_apps_fetch_next_page_odd_total():
+    all_apps = await client.applications.list()
+
+    per_page = 2
+    initial_len = len(all_apps)
+
+    is_odd_total = initial_len % per_page != 0
+    if not is_odd_total:
+        await create_application()
+
+        is_odd_total = True
+        initial_len += 1
+
+    total_pages = math.ceil(initial_len / per_page)
+
+    all_pages = []
+    for page in range(1, total_pages + 1):
+        is_last_page = page == total_pages
+        apps_page = await client.applications.fetch_next_page(limit=2)
+        all_pages.extend(apps_page)
+
+        expected_page_len = 1 if is_last_page and is_odd_total else 2
+        assert len(apps_page) == expected_page_len
+
+    assert len(all_pages) == initial_len
+
+
+@pytest.mark.asyncio
 async def test_crud_applications():
-    test_app_name = get_test_app_name()
+    test_app_name = get_unique_test_app_name()
 
     create_response = await create_application(
         name=test_app_name,
         app_type="test-app-type",
         description="test-app-description",
     )
```

### Comparing `klu-0.1.3/tests/integration/test_data.py` & `klu-0.1.4/tests/integration/test_data.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/test_data_index.py` & `klu-0.1.4/tests/integration/test_data_index.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/test_models.py` & `klu-0.1.4/tests/integration/test_models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/test_workspaces.py` & `klu-0.1.4/tests/integration/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/utils/actions.py` & `klu-0.1.4/tests/integration/utils/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,24 +22,26 @@
         model_guid = model.guid
 
     return await client.actions.create(
         app_guid=app_guid,
         model_guid=model_guid,
         name=kwargs.get("name", "test-action-name"),
         model_config=kwargs.get("model_config", None),
-        prompt=kwargs.get("prompt", "test-action-prompt"),
-        action_type=kwargs.get("action_type", "test-action-type"),
+        action_type=kwargs.get("action_type", "simple"),
+        prompt=kwargs.get("prompt", "Tell me about it"),
         description=kwargs.get("description", "test-action-description"),
     )
 
 
 class ActionSingleton:
     _action = None
 
     async def get_default_action(self, **kwargs) -> Action:
         if not self._action:
             model = await create_model()
             app = await create_application()
 
-            self._action = await create_action(app_guid=app.guid, model_guid=model.guid, **kwargs)
+            self._action = await create_action(
+                app_guid=app.guid, model_guid=model.guid, **kwargs
+            )
 
         return self._action
```

### Comparing `klu-0.1.3/tests/integration/utils/applications.py` & `klu-0.1.4/tests/integration/utils/applications.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/utils/data.py` & `klu-0.1.4/tests/integration/utils/data.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/utils/data_index.py` & `klu-0.1.4/tests/integration/utils/data_index.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/utils/models.py` & `klu-0.1.4/tests/integration/utils/models.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/utils/sessions.py` & `klu-0.1.4/tests/integration/utils/sessions.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/integration/utils/workspace.py` & `klu-0.1.4/tests/integration/utils/workspace.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/unit/action/test_client.py` & `klu-0.1.4/tests/unit/action/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @pytest.mark.asyncio
 async def test_get_app_actions_converts_response_to_dataclass_provided_valid_response_dicts(
     klu_client: KluClient,
 ):
     with patch(
-        "klu.application.client.APIClient", new_callable=get_api_client_mock
+        "klu.common.client.APIClient", new_callable=get_api_client_mock
     ) as client_mock:
         action_1_guid = "test_action_1"
         action_2_guid = "test_action_2"
 
         test_action_1 = get_action_data(guid=action_1_guid)
         test_action_2 = get_action_data(guid=action_2_guid)
 
@@ -39,14 +39,14 @@
 
 
 @pytest.mark.asyncio
 async def test_get_app_actions_raises_klu_error_provided_404_response_from_api(
     klu_client: KluClient,
 ):
     with patch(
-        "klu.application.client.APIClient", new_callable=get_api_client_mock
+        "klu.common.client.APIClient", new_callable=get_api_client_mock
     ) as client_mock:
         client_mock.get = client_get_function_mock(web.HTTPNotFound())
         with pytest.raises(Exception) as exc_info:
             await klu_client.applications.get_app_actions("test")
 
         assert exc_info.type is ApplicationNotFoundError
```

### Comparing `klu-0.1.3/tests/unit/action/utils.py` & `klu-0.1.4/tests/unit/action/utils.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/unit/application/test_client.py` & `klu-0.1.4/tests/unit/application/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,14 @@
 
 
 @pytest.mark.asyncio
 async def test_get_app_raises_klu_error_provided_404_response_from_api(
     klu_client: KluClient,
 ):
     with patch(
-        "klu.application.client.APIClient", new_callable=get_api_client_mock
+        "klu.common.client.APIClient", new_callable=get_api_client_mock
     ) as client_mock:
         client_mock.get = client_get_function_mock(web.HTTPNotFound())
         with pytest.raises(Exception) as exc_info:
             await klu_client.applications.get_app_actions("test")
 
         assert exc_info.type is ApplicationNotFoundError
```

### Comparing `klu-0.1.3/tests/unit/application/utils.py` & `klu-0.1.4/tests/unit/application/utils.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/tests/unit/utils/mock.py` & `klu-0.1.4/tests/unit/utils/mock.py`

 * *Files identical despite different names*

### Comparing `klu-0.1.3/PKG-INFO` & `klu-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klu
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK for building AI Enabled apps.
 Home-page: https://github.com/ssabev/klu
 License: MIT
 Author: Stefan Sabev
 Author-email: stefan@launchpad.pm
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

