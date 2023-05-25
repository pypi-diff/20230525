# Comparing `tmp/blaster-server-0.0.432.tar.gz` & `tmp/blaster-server-0.0.432b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.432.tar", last modified: Mon May 22 22:34:58 2023, max compression
+gzip compressed data, was "blaster-server-0.0.432b0.tar", last modified: Thu May 25 14:27:08 2023, max compression
```

## Comparing `blaster-server-0.0.432.tar` & `blaster-server-0.0.432b0.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.432/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.432/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-05-22 22:34:58.216565 blaster-server-0.0.432/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.432/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.432/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.432/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.432/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.432/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.432/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.432/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-19 10:42:50.000000 blaster-server-0.0.432/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3828 2023-05-15 14:10:32.000000 blaster-server-0.0.432/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.432/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.432/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.432/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.432/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15728 2023-05-17 08:23:45.000000 blaster-server-0.0.432/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38823 2023-05-22 20:14:53.000000 blaster-server-0.0.432/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46589 2023-05-22 20:12:00.000000 blaster-server-0.0.432/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.432/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.432/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.432/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.432/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.432/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.432/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.432/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.432/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.432/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.432/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.212565 blaster-server-0.0.432/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.432/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      206 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-22 22:34:58.000000 blaster-server-0.0.432/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.432/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.432/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.432/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.432/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.432/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.432/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.432/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.432/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-22 22:34:58.216565 blaster-server-0.0.432/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1539 2023-05-17 20:32:09.000000 blaster-server-0.0.432/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-22 22:34:58.216565 blaster-server-0.0.432/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.432/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.432/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-17 08:26:43.000000 blaster-server-0.0.432/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.432/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.432/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.432/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.750486 blaster-server-0.0.432b0/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.432b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-05-25 14:27:08.750486 blaster-server-0.0.432b0/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.432b0/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.432b0/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.432b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.432b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.432b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.432b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.432b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-19 10:42:50.000000 blaster-server-0.0.432b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3988 2023-05-25 14:24:02.000000 blaster-server-0.0.432b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.432b0/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.432b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.432b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62746 2023-05-25 13:44:57.000000 blaster-server-0.0.432b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15728 2023-05-17 08:23:45.000000 blaster-server-0.0.432b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38827 2023-05-25 14:26:32.000000 blaster-server-0.0.432b0/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46589 2023-05-22 20:12:00.000000 blaster-server-0.0.432b0/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.432b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.432b0/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.432b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.432b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.432b0/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.432b0/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-25 14:08:42.000000 blaster-server-0.0.432b0/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.432b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.432b0/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.432b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.746486 blaster-server-0.0.432b0/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.750486 blaster-server-0.0.432b0/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-05-25 14:27:08.000000 blaster-server-0.0.432b0/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1714 2023-05-25 14:27:08.000000 blaster-server-0.0.432b0/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-25 14:27:08.000000 blaster-server-0.0.432b0/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      206 2023-05-25 14:27:08.000000 blaster-server-0.0.432b0/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-25 14:27:08.000000 blaster-server-0.0.432b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.750486 blaster-server-0.0.432b0/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.432b0/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.432b0/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.432b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.432b0/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.432b0/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.432b0/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.432b0/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-25 14:27:08.750486 blaster-server-0.0.432b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1540 2023-05-25 13:48:01.000000 blaster-server-0.0.432b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-25 14:27:08.750486 blaster-server-0.0.432b0/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.432b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.432b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-25 13:50:32.000000 blaster-server-0.0.432b0/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-17 08:26:43.000000 blaster-server-0.0.432b0/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.432b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.432b0/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.432b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.432/LICENSE.txt` & `blaster-server-0.0.432b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/PKG-INFO` & `blaster-server-0.0.432b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.432
+Version: 0.0.432b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.432/README.md` & `blaster-server-0.0.432b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/__init__.py` & `blaster-server-0.0.432b0/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/cloud/analytics.py` & `blaster-server-0.0.432b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.432b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/cloud/push_tasks.py` & `blaster-server-0.0.432b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/cloud/storage.py` & `blaster-server-0.0.432b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/config.py` & `blaster-server-0.0.432b0/blaster/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # they may depend on config and won't load correctly.
 # keep it isolated as much as possible
 
 # default env variables
 IS_PROD = environ.get("IS_PROD") == "1"
 IS_STAGING = IS_PROD and environ.get("IS_STAGING") == "1"
 IS_DEV = 1 if not (IS_PROD or IS_STAGING) else 0
+IS_TEST = IS_DEV and environ.get("IS_TEST") == "1"
 
 # CRITICAL-50 ERROR-40  WARNING-30  INFO-20  DEBUG-10  NOTSET-0
 APP_NAME = ""
 APP_VERSION = "0"
 LOG_LEVEL = logging.DEBUG if IS_DEV else (logging.INFO if IS_STAGING else logging.WARN)
 DEBUG_PRINT_LEVEL = IS_DEV and int(environ.get("DEBUG_PRINT_LEVEL") or 0)
 
@@ -39,20 +40,22 @@
                 path
             )
             config_files = []
             if(os.path.isfile(path)):
                 config_files = [path]
             else:
                 config_files.append(os.path.join(path, "app.yaml"))
-                if(config.IS_DEV):
+                if(self.IS_DEV):
                     config_files.append(os.path.join(path, "dev.yaml"))
-                elif(config.IS_PROD):
+                    if(self.IS_TEST):
+                        config_files.append(os.path.join(path, "test.yaml"))
+                elif(self.IS_PROD):
                     config_files.append(os.path.join(path, "prod.yaml"))
                     config_files.append(os.path.join(path, "prod.secrets.yaml"))
-                    if(config.IS_STAGING):
+                    if(self.IS_STAGING):
                         config_files.append(os.path.join(path, "staging.yaml"))
                         config_files.append(os.path.join(path, "staging.secrets.yaml"))
             for f in config_files:
                 if(not os.path.isfile(f)):
                     continue
                 print("Loading config file: ", f)
                 for k, v in yaml.safe_load(open(f).read()).items():
```

### Comparing `blaster-server-0.0.432/blaster/connection_pool.py` & `blaster-server-0.0.432b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/logging.py` & `blaster-server-0.0.432b0/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/mongo_orm.py` & `blaster-server-0.0.432b0/blaster/mongo_orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 from pymongo.errors import DuplicateKeyError, OperationFailure
 from pymongo import ReturnDocument, ReadPreference
 from .tools import ExpiringCache, all_subclasses,\
 	cur_ms, list_diff2, batched_iter, set_by_key_list, _OBJ_END_
 from .config import IS_DEV, MONGO_WARN_MAX_RESULTS_RATE,\
 	MONGO_MAX_RESULTS_AT_HIGH_SCAN_RATE,\
 	MONGO_WARN_MAX_QUERY_RESPONSE_TIME_SECONDS,\
-	DEBUG_PRINT_LEVEL
+	DEBUG_PRINT_LEVEL, IS_TEST
 from gevent.threading import Thread
 from gevent import time
 from .logging import LOG_WARN, LOG_SERVER, LOG_ERROR
 
 _loading_errors = {}
 
-MONGO_RUNNING_IN_TEST_MODE = IS_DEV and int(environ.get("BLASTER_MONGO_RUNNING_IN_TEST_MODE") or 0)
 
 EVENT_BEFORE_DELETE = -2
 EVENT_AFTER_DELETE = -1
 EVENT_BEFORE_UPDATE = 1
 EVENT_AFTER_UPDATE = 2
 EVENT_BEFORE_CREATE = 3
 EVENT_AFTER_CREATE = 4
@@ -1870,25 +1869,25 @@
 			"mongo_indexes",
 			desc=(
 				f"index {_index_keys} not declared in orm, delete it on db? "
 				f'db.{_Model._collection_name_with_shard_}.dropIndex("{existing_indexes[_index_keys][0]}")'
 			)
 		)
 
-	if(MONGO_RUNNING_IN_TEST_MODE):
+	if(IS_TEST):
 		# create indexes in test mode automatically
 		for pymongo_index, mongo_index_args in _pymongo_indexes_to_create.items():
 			print(
 				"\n\n#MONGO: creating_indexes automatically in test mode", _Model, pymongo_index, mongo_index_args
 			)
 			# in each node create indexes
 			for db_node in _Model._db_nodes_:
 				db_node.get_collection(_Model).create_index(pymongo_index, **mongo_index_args)
 
-	if(_new_indexes and not MONGO_RUNNING_IN_TEST_MODE):
+	if(_new_indexes and not IS_TEST):
 		for _index in _new_indexes:
 			missing_index_creation_string = (
 				f"db.{_Model._collection_name_with_shard_}"
 				f".createIndex({json.dumps({x:y for x,y in _index})}, "
 				f"{json.dumps(_pymongo_indexes_to_create[_index])})"
 			)
 			LOG_ERROR("missing_mongo_indexes", desc=missing_index_creation_string)
@@ -1917,15 +1916,15 @@
 				)
 				LOG_ERROR("index_options_changed", desc=index_options_changed)
 				if("index_options_changed" not in _loading_errors):
 					_loading_errors["index_options_changed"] = []
 				_loading_errors["index_options_changed"].append(index_options_changed)
 
 	# create secondary shards
-	for _secondary_shard_key in list(_Model._secondary_shards_.keys()): # iterate on copy
+	for _secondary_shard_key in list(_Model._secondary_shards_.keys()):  # iterate on copy
 		_secondary_shard = _Model._secondary_shards_[_secondary_shard_key]
 		if(not _secondary_shard.attrs):
 			_Model._secondary_shards_.pop(_secondary_shard_key)
 			LOG_ERROR(
 				"MONGO", description="not creating secondary shards without any related index",
 				model=_Model.__name__,
 				secondary_shard_key=_secondary_shard_key
@@ -1969,29 +1968,29 @@
 	# initialize control db
 	if(isinstance(db_nodes, dict)):
 		db_nodes = [DatabaseNode(**db_nodes)]
 	elif(isinstance(db_nodes, list)):
 		db_nodes = [DatabaseNode(**db_node) for db_node in db_nodes]
 	else:
 		raise Exception(
-			"argument must be a list of dicts, or a single dict, not %s"%(type(db_nodes))
+			f"argument must be a list of dicts, or a single dict, not {type(db_nodes)}"
 		)
 	# check connection to mongodb
 	[db_node.mongo_client.server_info() for db_node in db_nodes]
 
 	# initialize control db
 	CollectionTracker._db_nodes_ = db_nodes
 	initialize_model([CollectionTracker])
 
 	# set default db name for each class
 	for cls in all_subclasses(Model):
 		if(not getattr(cls, "_db_name_", None)):
 			cls._db_name_ = default_db_name
 		initialize_model(cls)
-	
+
 	if(_loading_errors):
 		raise Exception("initialize_mongo has errors: Check error logs: " + str(_loading_errors))
 
 
 # Initially intended to be < 500 line and more for educating
 # about sharding
 # How this works:
```

### Comparing `blaster-server-0.0.432/blaster/schema.py` & `blaster-server-0.0.432b0/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/server.py` & `blaster-server-0.0.432b0/blaster/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1249,15 +1249,15 @@
 
 
 Request.set_arg_type_hook(WebSocketServerHandler, _get_web_socket_handler)
 
 
 # Utils
 
-MOILE_USER_AGENT_REGEX = re.compile(r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows ce|xda|xiino", re.I|re.M)
+MOBILE_USER_AGENT_REGEX = re.compile(r"(android|bb\\d+|meego).+mobile|avantgo|bada\\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\\.(browser|link)|vodafone|wap|windows ce|xda|xiino", re.I|re.M)
 
-MOILE_USER_AGENT_REGEX2 = re.compile(r"1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\\-(n|u)|c55\\/|capi|ccwa|cdm\\-|cell|chtm|cldc|cmd\\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\\-s|devi|dica|dmob|do(c|p)o|ds(12|\\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\\-|_)|g1 u|g560|gene|gf\\-5|g\\-mo|go(\\.w|od)|gr(ad|un)|haie|hcit|hd\\-(m|p|t)|hei\\-|hi(pt|ta)|hp( i|ip)|hs\\-c|ht(c(\\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\\-(20|go|ma)|i230|iac( |\\-|\\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\\/)|klon|kpt |kwc\\-|kyo(c|k)|le(no|xi)|lg( g|\\/(k|l|u)|50|54|\\-[a-w])|libw|lynx|m1\\-w|m3ga|m50\\/|ma(te|ui|xo)|mc(01|21|ca)|m\\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\\-2|po(ck|rt|se)|prox|psio|pt\\-g|qa\\-a|qc(07|12|21|32|60|\\-[2-7]|i\\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\\-|oo|p\\-)|sdk\\/|se(c(\\-|0|1)|47|mc|nd|ri)|sgh\\-|shar|sie(\\-|m)|sk\\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\\-|v\\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\\-|tdg\\-|tel(i|m)|tim\\-|t\\-mo|to(pl|sh)|ts(70|m\\-|m3|m5)|tx\\-9|up(\\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\\-|your|zeto|zte\\-", re.I | re.M)
+MOBILE_USER_AGENT_REGEX2 = re.compile(r"1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\\-(n|u)|c55\\/|capi|ccwa|cdm\\-|cell|chtm|cldc|cmd\\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\\-s|devi|dica|dmob|do(c|p)o|ds(12|\\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\\-|_)|g1 u|g560|gene|gf\\-5|g\\-mo|go(\\.w|od)|gr(ad|un)|haie|hcit|hd\\-(m|p|t)|hei\\-|hi(pt|ta)|hp( i|ip)|hs\\-c|ht(c(\\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\\-(20|go|ma)|i230|iac( |\\-|\\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\\/)|klon|kpt |kwc\\-|kyo(c|k)|le(no|xi)|lg( g|\\/(k|l|u)|50|54|\\-[a-w])|libw|lynx|m1\\-w|m3ga|m50\\/|ma(te|ui|xo)|mc(01|21|ca)|m\\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\\-2|po(ck|rt|se)|prox|psio|pt\\-g|qa\\-a|qc(07|12|21|32|60|\\-[2-7]|i\\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\\-|oo|p\\-)|sdk\\/|se(c(\\-|0|1)|47|mc|nd|ri)|sgh\\-|shar|sie(\\-|m)|sk\\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\\-|v\\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\\-|tdg\\-|tel(i|m)|tim\\-|t\\-mo|to(pl|sh)|ts(70|m\\-|m3|m5)|tx\\-9|up(\\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\\-|your|zeto|zte\\-", re.I | re.M)
 
 
 def is_mobile_user_agent(user_agent):
-	return MOILE_USER_AGENT_REGEX.search(user_agent) \
-		or MOILE_USER_AGENT_REGEX2.search(user_agent[0:4])
+	return MOBILE_USER_AGENT_REGEX.search(user_agent) \
+		or MOBILE_USER_AGENT_REGEX2.search(user_agent[0:4])
```

### Comparing `blaster-server-0.0.432/blaster/tools.py` & `blaster-server-0.0.432b0/blaster/tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/data/countries.json` & `blaster-server-0.0.432b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/data/mime_types.json` & `blaster-server-0.0.432b0/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/data_utils.py` & `blaster-server-0.0.432b0/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/events.py` & `blaster-server-0.0.432b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/fork.py` & `blaster-server-0.0.432b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.432b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.432b0/blaster/utils/phone_number_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from .data_utils import COUNTRY_DATA
 from ..tools import ltrim
 
-PHONE_NUMBER_REGEX = re.compile(r"^\+?[0-9]+")
-
+NON_DIGITS = re.compile(r"[^0-9]")
 
 country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "255": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [7, 8], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
 
 
 class SimpleTrie(dict):
 	end_obj = None
 
@@ -31,110 +30,64 @@
 
 	def __init__(self, country_phone_code, national_number, phone_number):
 		self.phone_number = phone_number
 		self.national_number = national_number
 		if(country_phone_code):
 			self.country_phone_code = country_phone_code.lstrip("+")
 
-	# mobile numbers only
 	@classmethod
-	def parse_phone_number(
-		cls, phone_number,
-		country_phone_code=None, iso2_country_code=None
-	):
-		# assume phone number without country code
-		# assume phone number with country code without +
-		# assume + by mistake
-		if(not phone_number):
-			return None
-
-		phone_number = phone_number.replace(" ", "")
-
-		if(not PHONE_NUMBER_REGEX.match(phone_number)):
-			return None
-
-		if(country_phone_code):
-			country_phone_code = country_phone_code.lstrip("+")
-
+	def validate(cls, phone_number):  # with country code
 		phone_number = phone_number.lstrip("+0")
-
 		_root = country_code_num_digits_trie
 		for i in range(0, len(phone_number)):
 			_d = phone_number[i]
 			if(_root.end_obj):
 				_remaining_len = len(phone_number) - i
 				for _r in _root.end_obj:
 					if(_r == _remaining_len):
 						return PhoneNumberObj(phone_number[: i], phone_number[i:], phone_number)
 
 			if(_d not in _root):
 				break
 			_root = _root[_d]
+		return None
 
+	# mobile numbers only
+	@classmethod
+	def parse_phone_number(
+		cls, phone_number,
+		country_phone_code=None, iso2_country_code=None
+	):
+		given_phone_number = NON_DIGITS.sub("", phone_number or "")
+		phone_number = given_phone_number.lstrip("0")
+		# Assume it's with country code
+
+		# Add given country code
 		if(not country_phone_code and iso2_country_code):
 			if(_country_data := COUNTRY_DATA.get(iso2_country_code)):
 				country_phone_code = _country_data["phone_code"]
 
-		if(not country_phone_code):
-			country_phone_code = "31"  # try netherlands by default
-
-		if len(phone_number) in country_code_num_digits_map[country_phone_code]:
-			return PhoneNumberObj(
-				country_phone_code, phone_number,
-				country_phone_code + phone_number
-			)
-
-		phone_number_strip = ltrim(phone_number, country_phone_code)
-		if len(phone_number_strip) in country_code_num_digits_map[country_phone_code]:
-			return PhoneNumberObj(
-				country_phone_code, phone_number_strip,
-				country_phone_code + phone_number_strip
-			)
-
-		if(phone_number.startswith(country_phone_code)):
-			# strip and parse again
-			return PhoneNumberObj.parse_phone_number(
-				phone_number_strip,
-				country_phone_code=country_phone_code, iso2_country_code=iso2_country_code
-			)
-
-		return None
+		# try with given country code
+		if(country_phone_code):
+			if(ret := PhoneNumberObj.validate(country_phone_code + phone_number)):
+				return ret
+			if(len(given_phone_number) != len(phone_number)):  # 0 strippe
+				if(ret := PhoneNumberObj.validate(country_phone_code + given_phone_number)):
+					return ret
+		# Assuming full number is given
+		return PhoneNumberObj.validate(phone_number)
 
 
 def sanitize_phone_number(
 	phone_number, country_phone_code=None,
 	iso2_country_code=None
 ):
-	if(not phone_number):
-		return None
-	phone_number = phone_number.replace(" ", "").strip().lower()
-	if(not PHONE_NUMBER_REGEX.match(phone_number)):
-		return None
-
 	try:
 		phone_number = PhoneNumberObj.parse_phone_number(
 			phone_number,
 			country_phone_code=country_phone_code,
 			iso2_country_code=iso2_country_code
 		).phone_number
 	except Exception:
 		return None
 
 	return phone_number
-
-
-# Test
-def test():
-	def assert_equals(a, b):
-		if(a == b):
-			print("yes")
-		else:
-			print("no")
-	print(PhoneNumberObj.parse_phone_number('+917680971071').__dict__)
-	print(PhoneNumberObj.parse_phone_number('+917680971071').__dict__)
-	print(PhoneNumberObj.parse_phone_number("229270555", country_phone_code="31").__dict__)
-	assert_equals(PhoneNumberObj.parse_phone_number('+917680971071', '+91').phone_number, "917680971071")
-	assert_equals(PhoneNumberObj.parse_phone_number('917680971071', '+91').phone_number, "917680971071")
-	assert_equals(PhoneNumberObj.parse_phone_number('07680971071', '+91').phone_number, "917680971071")
-	assert_equals(PhoneNumberObj.parse_phone_number('7680971071', '+91').phone_number, "917680971071")
-	assert_equals(PhoneNumberObj.parse_phone_number('7680971071', '+64').phone_number, "647680971071")
-	assert_equals(PhoneNumberObj.parse_phone_number('76809710', '+64').phone_number, "6476809710")
```

### Comparing `blaster-server-0.0.432/blaster/utils/xss_html.py` & `blaster-server-0.0.432b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/__init__.py` & `blaster-server-0.0.432b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_abnf.py` & `blaster-server-0.0.432b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_app.py` & `blaster-server-0.0.432b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_core.py` & `blaster-server-0.0.432b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_exceptions.py` & `blaster-server-0.0.432b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_handshake.py` & `blaster-server-0.0.432b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_http.py` & `blaster-server-0.0.432b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_logging.py` & `blaster-server-0.0.432b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_socket.py` & `blaster-server-0.0.432b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.432b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_url.py` & `blaster-server-0.0.432b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/_utils.py` & `blaster-server-0.0.432b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/server.py` & `blaster-server-0.0.432b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.432b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.432b0/blaster_server.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.432
+Version: 0.0.432b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.432/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.432b0/blaster_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,11 +55,12 @@
 examples/mongo_ormexample.py
 examples/simple_examples.py
 examples/test_chat_room.py
 examples/tornado_hello_world.py
 examples/wheezy_hello.py
 test/__init__.py
 test/test_mongo_orm.py
+test/test_phone_number_utils.py
 test/test_schema.py
 test/test_tools.py
 test/test_utils.py
 test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.432/examples/gevent_wsgi_test.py` & `blaster-server-0.0.432b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/examples/mongo_ormexample.py` & `blaster-server-0.0.432b0/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/examples/simple_examples.py` & `blaster-server-0.0.432b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/examples/test_chat_room.py` & `blaster-server-0.0.432b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/examples/tornado_hello_world.py` & `blaster-server-0.0.432b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/examples/wheezy_hello.py` & `blaster-server-0.0.432b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/setup.py` & `blaster-server-0.0.432b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.432',
+	version='0.0.432b',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.432/test/test_mongo_orm.py` & `blaster-server-0.0.432b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/test/test_schema.py` & `blaster-server-0.0.432b0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/test/test_tools.py` & `blaster-server-0.0.432b0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/test/test_utils.py` & `blaster-server-0.0.432b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.432/test/timeit_snippets.py` & `blaster-server-0.0.432b0/test/timeit_snippets.py`

 * *Files identical despite different names*

