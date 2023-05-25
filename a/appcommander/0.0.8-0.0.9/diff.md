# Comparing `tmp/appcommander-0.0.8.tar.gz` & `tmp/appcommander-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appcommander-0.0.8.tar", last modified: Fri Jan 13 23:24:42 2023, max compression
+gzip compressed data, was "appcommander-0.0.9.tar", last modified: Sun Feb  5 12:39:45 2023, max compression
```

## Comparing `appcommander-0.0.8.tar` & `appcommander-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,70 @@
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/
--rw-rw-r--   0 name      (1000) name      (1000)     4678 2023-01-13 23:24:42.779012 appcommander-0.0.8/PKG-INFO
--rw-------   0 name      (1000) name      (1000)     3826 2023-01-13 23:23:10.000000 appcommander-0.0.8/README.md
--rw-rw-r--   0 name      (1000) name      (1000)    34523 2023-01-13 23:17:46.000000 appcommander-0.0.8/licence
--rw-rw-r--   0 name      (1000) name      (1000)     1395 2023-01-13 23:17:46.000000 appcommander-0.0.8/pyproject.toml
--rw-rw-r--   0 name      (1000) name      (1000)     1378 2023-01-13 23:24:42.783012 appcommander-0.0.8/setup.cfg
--rw-rw-r--   0 name      (1000) name      (1000)      235 2023-01-13 23:18:44.000000 appcommander-0.0.8/setup.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.775012 appcommander-0.0.8/src/
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/src/appcommander/
--rw-rw-r--   0 name      (1000) name      (1000)     3307 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/Screen.py
--rw-rw-r--   0 name      (1000) name      (1000)      141 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)      436 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/__main__.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/src/appcommander/arg_parser/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/arg_parser/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     2073 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/arg_parser/arg_parser.py
--rw-rw-r--   0 name      (1000) name      (1000)     2344 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/arg_parser/process_args.py
--rw-rw-r--   0 name      (1000) name      (1000)     1704 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/create_screens.py
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/file_input_output.py
--rw-rw-r--   0 name      (1000) name      (1000)      361 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/hardcoded.py
--rw-rw-r--   0 name      (1000) name      (1000)    11096 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/helper.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/src/appcommander/org_torproject_android/
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/
--rw-rw-r--   0 name      (1000) name      (1000)     2050 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/Script.py
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     4339 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/app_specific_helper.py
--rw-rw-r--   0 name      (1000) name      (1000)     2554 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_0.py
--rw-rw-r--   0 name      (1000) name      (1000)     2568 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_1.py
--rw-rw-r--   0 name      (1000) name      (1000)     2611 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_2.py
--rw-rw-r--   0 name      (1000) name      (1000)     2592 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_3.py
--rw-rw-r--   0 name      (1000) name      (1000)     2746 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_4.py
--rw-rw-r--   0 name      (1000) name      (1000)     3910 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_5.py
--rw-rw-r--   0 name      (1000) name      (1000)     4531 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_6.py
--rw-rw-r--   0 name      (1000) name      (1000)     3312 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_7.py
--rw-rw-r--   0 name      (1000) name      (1000)     1073 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_flow.py
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/org_torproject_android/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     3135 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/plot_script_flow.py
--rw-rw-r--   0 name      (1000) name      (1000)     3249 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/run_script.py
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/screen_reading.py
--rw-rw-r--   0 name      (1000) name      (1000)     1620 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/script_orientation.py
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/text_parsing.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/src/appcommander/verification/
--rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.8/src/appcommander/verification/__init__.py
--rw-rw-r--   0 name      (1000) name      (1000)     4501 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/verification/arg_verification.py
--rw-rw-r--   0 name      (1000) name      (1000)     2882 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/verification/status_verification.py
--rw-rw-r--   0 name      (1000) name      (1000)     1937 2023-01-13 23:18:44.000000 appcommander-0.0.8/src/appcommander/verification/verify_phone_connection.py
-drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-01-13 23:24:42.779012 appcommander-0.0.8/src/appcommander.egg-info/
--rw-rw-r--   0 name      (1000) name      (1000)     4678 2023-01-13 23:24:42.000000 appcommander-0.0.8/src/appcommander.egg-info/PKG-INFO
--rw-rw-r--   0 name      (1000) name      (1000)     1855 2023-01-13 23:24:42.000000 appcommander-0.0.8/src/appcommander.egg-info/SOURCES.txt
--rw-rw-r--   0 name      (1000) name      (1000)        1 2023-01-13 23:24:42.000000 appcommander-0.0.8/src/appcommander.egg-info/dependency_links.txt
--rw-rw-r--   0 name      (1000) name      (1000)       51 2023-01-13 23:24:42.000000 appcommander-0.0.8/src/appcommander.egg-info/entry_points.txt
--rw-rw-r--   0 name      (1000) name      (1000)       67 2023-01-13 23:24:42.000000 appcommander-0.0.8/src/appcommander.egg-info/requires.txt
--rw-rw-r--   0 name      (1000) name      (1000)       13 2023-01-13 23:24:42.000000 appcommander-0.0.8/src/appcommander.egg-info/top_level.txt
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.126842 appcommander-0.0.9/
+-rw-rw-r--   0 name      (1000) name      (1000)     5434 2023-02-05 12:39:45.126842 appcommander-0.0.9/PKG-INFO
+-rw-------   0 name      (1000) name      (1000)     4582 2023-02-05 12:15:56.000000 appcommander-0.0.9/README.md
+-rw-rw-r--   0 name      (1000) name      (1000)    34523 2023-01-13 23:17:46.000000 appcommander-0.0.9/licence
+-rw-rw-r--   0 name      (1000) name      (1000)     1395 2023-01-13 23:17:46.000000 appcommander-0.0.9/pyproject.toml
+-rw-rw-r--   0 name      (1000) name      (1000)     1378 2023-02-05 12:39:45.130842 appcommander-0.0.9/setup.cfg
+-rw-rw-r--   0 name      (1000) name      (1000)      235 2023-01-13 23:18:44.000000 appcommander-0.0.9/setup.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.114842 appcommander-0.0.9/src/
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.118842 appcommander-0.0.9/src/appcommander/
+-rw-rw-r--   0 name      (1000) name      (1000)     3482 2023-01-14 00:40:39.000000 appcommander-0.0.9/src/appcommander/Screen.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2809 2023-01-14 18:24:30.000000 appcommander-0.0.9/src/appcommander/Script.py
+-rw-rw-r--   0 name      (1000) name      (1000)      141 2023-02-05 12:38:44.000000 appcommander-0.0.9/src/appcommander/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)      436 2023-02-05 12:14:50.000000 appcommander-0.0.9/src/appcommander/__main__.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.122842 appcommander-0.0.9/src/appcommander/arg_parser/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/arg_parser/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2857 2023-01-14 18:18:33.000000 appcommander-0.0.9/src/appcommander/arg_parser/arg_parser.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2727 2023-02-04 22:05:07.000000 appcommander-0.0.9/src/appcommander/arg_parser/process_args.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.122842 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.122842 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/
+-rw-rw-r--   0 name      (1000) name      (1000)     1441 2023-01-15 01:53:40.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/App_input_data.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2269 2023-01-15 20:03:48.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/Screen_flow.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1694 2023-01-15 19:52:49.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/helper.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2589 2023-01-14 18:06:21.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_0.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2551 2023-01-15 15:44:33.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_1.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2311 2023-01-15 15:50:15.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_2.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3262 2023-01-15 21:32:46.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_3.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3304 2023-01-15 03:03:10.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_4.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3178 2023-01-15 03:03:16.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_5.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3146 2023-01-15 15:44:14.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_6.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3546 2023-01-15 21:29:21.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_7.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3533 2023-01-15 19:52:52.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/V4_2_6/screen_8.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/at_bitfire_davdroid/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2940 2023-01-14 17:10:19.000000 appcommander-0.0.9/src/appcommander/create_screens.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/file_input_output.py
+-rw-rw-r--   0 name      (1000) name      (1000)      361 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/hardcoded.py
+-rw-rw-r--   0 name      (1000) name      (1000)    10310 2023-02-04 20:04:18.000000 appcommander-0.0.9/src/appcommander/helper.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.122842 appcommander-0.0.9/src/appcommander/org_torproject_android/
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.126842 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/
+-rw-rw-r--   0 name      (1000) name      (1000)      967 2023-01-15 01:53:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/App_input_data.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1073 2023-01-14 16:31:50.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/Screen_flow.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     4286 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/helper.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2523 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_0.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2538 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_1.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2581 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_2.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2562 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_3.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2716 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_4.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3879 2023-02-04 19:59:30.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_5.py
+-rw-rw-r--   0 name      (1000) name      (1000)     4647 2023-01-14 18:21:14.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_6.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3282 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_7.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/org_torproject_android/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     6816 2023-02-05 00:33:03.000000 appcommander-0.0.9/src/appcommander/plot_script_flow.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1041 2023-01-14 15:27:06.000000 appcommander-0.0.9/src/appcommander/run_bash_code.py
+-rw-rw-r--   0 name      (1000) name      (1000)     3644 2023-02-04 20:06:10.000000 appcommander-0.0.9/src/appcommander/run_script.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/screen_reading.py
+-rw-rw-r--   0 name      (1000) name      (1000)     1200 2023-01-14 00:30:52.000000 appcommander-0.0.9/src/appcommander/script_orientation.py
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/text_parsing.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.126842 appcommander-0.0.9/src/appcommander/verification/
+-rw-rw-r--   0 name      (1000) name      (1000)        0 2023-01-13 23:17:46.000000 appcommander-0.0.9/src/appcommander/verification/__init__.py
+-rw-rw-r--   0 name      (1000) name      (1000)     4459 2023-01-15 15:49:47.000000 appcommander-0.0.9/src/appcommander/verification/arg_verification.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2829 2023-02-04 19:47:55.000000 appcommander-0.0.9/src/appcommander/verification/status_verification.py
+-rw-rw-r--   0 name      (1000) name      (1000)     2154 2023-01-15 21:43:18.000000 appcommander-0.0.9/src/appcommander/verification/verify_phone_connection.py
+drwxrwxr-x   0 name      (1000) name      (1000)        0 2023-02-05 12:39:45.118842 appcommander-0.0.9/src/appcommander.egg-info/
+-rw-rw-r--   0 name      (1000) name      (1000)     5434 2023-02-05 12:39:45.000000 appcommander-0.0.9/src/appcommander.egg-info/PKG-INFO
+-rw-rw-r--   0 name      (1000) name      (1000)     2695 2023-02-05 12:39:45.000000 appcommander-0.0.9/src/appcommander.egg-info/SOURCES.txt
+-rw-rw-r--   0 name      (1000) name      (1000)        1 2023-02-05 12:39:45.000000 appcommander-0.0.9/src/appcommander.egg-info/dependency_links.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       51 2023-02-05 12:39:45.000000 appcommander-0.0.9/src/appcommander.egg-info/entry_points.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       67 2023-02-05 12:39:45.000000 appcommander-0.0.9/src/appcommander.egg-info/requires.txt
+-rw-rw-r--   0 name      (1000) name      (1000)       13 2023-02-05 12:39:45.000000 appcommander-0.0.9/src/appcommander.egg-info/top_level.txt
```

### Comparing `appcommander-0.0.8/PKG-INFO` & `appcommander-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appcommander
-Version: 0.0.8
+Version: 0.0.9
 Summary: Performs controlled Android app automation through UI.
 Home-page: https://github.com/Hiveminds/appcommander
 Author: a-t-0
 Author-email: no-email@no-email.org
 Maintainer: a-t-0
 Maintainer-email: no-email@no-email.org
 License: AGPLv3
@@ -49,15 +49,15 @@
 
 Also, each phone manufacturer has a different rooting process, this repo can
 become a library to safely- and automatically root all (rootable) Android
 phones automatically (except the user must enable `ADB` themselves).
 
 ## Example
 
-![image](https://user-images.githubusercontent.com/34750068/212434675-65839344-0dbd-43c1-a7c2-3717cdd40d31.png)
+![image](https://github.com/HiveMinds/app-commander/blob/main/src/appcommander/org_torproject_android/V16_6_3_RC_1/flow.png?raw=true)
 
 ## Usage
 
 First satisfy the prerequisites:
 
 ```bash
 pip install appcommander
@@ -72,14 +72,21 @@
 which is the same as:
 
 ```bash
 python -m src.appcommander --app-name org.torproject.android \
 --version "16.6.3 RC 1" -torify "DAVx5"
 ```
 
+Or, to configure DAVx5:
+
+```bash
+python -m src.appcommander -a at.bitfire.davdroid -v "4.2.6" -nu \
+<your_nextcloud_username> -np <your_nextcloud_password> -o <your_onion_url>
+```
+
 For more info, run:
 
 ```bash
 python -m src.appcommander --help
 ```
 
 ## Testing
@@ -166,7 +173,28 @@
 pip install -e .
 ```
 
 that installs the latest changes into the pip package locally (into your conda
 environment).
 
 <!-- Un-wrapped URL's (Badges and Hyperlinks) -->
+
+### Show your app-flow
+
+To show how your script works, run (along with any additional input args
+required for that script):
+
+```sh
+python -m src.appcommander -a <package_name> -v <app_version> -f \
+<additional arguments>
+```
+
+For example:
+
+```sh
+python -m src.appcommander -a "at.bitfire.davdroid" -v "4.2.6" -f  -nu \
+<some_filler> -np <some_filler> -o <some_filler>
+python -m src.appcommander -a "at.bitfire.davdroid" -v "4.2.6" -f -nu \
+asdf -np asdf -o asdf
+python -m src.appcommander -a org.torproject.android -v "16.6.3 RC 1" \
+-f -t "DAVx5"
+```
```

### Comparing `appcommander-0.0.8/README.md` & `appcommander-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 Also, each phone manufacturer has a different rooting process, this repo can
 become a library to safely- and automatically root all (rootable) Android
 phones automatically (except the user must enable `ADB` themselves).
 
 ## Example
 
-![image](https://user-images.githubusercontent.com/34750068/212434675-65839344-0dbd-43c1-a7c2-3717cdd40d31.png)
+![image](https://github.com/HiveMinds/app-commander/blob/main/src/appcommander/org_torproject_android/V16_6_3_RC_1/flow.png?raw=true)
 
 ## Usage
 
 First satisfy the prerequisites:
 
 ```bash
 pip install appcommander
@@ -49,14 +49,21 @@
 which is the same as:
 
 ```bash
 python -m src.appcommander --app-name org.torproject.android \
 --version "16.6.3 RC 1" -torify "DAVx5"
 ```
 
+Or, to configure DAVx5:
+
+```bash
+python -m src.appcommander -a at.bitfire.davdroid -v "4.2.6" -nu \
+<your_nextcloud_username> -np <your_nextcloud_password> -o <your_onion_url>
+```
+
 For more info, run:
 
 ```bash
 python -m src.appcommander --help
 ```
 
 ## Testing
@@ -143,7 +150,28 @@
 pip install -e .
 ```
 
 that installs the latest changes into the pip package locally (into your conda
 environment).
 
 <!-- Un-wrapped URL's (Badges and Hyperlinks) -->
+
+### Show your app-flow
+
+To show how your script works, run (along with any additional input args
+required for that script):
+
+```sh
+python -m src.appcommander -a <package_name> -v <app_version> -f \
+<additional arguments>
+```
+
+For example:
+
+```sh
+python -m src.appcommander -a "at.bitfire.davdroid" -v "4.2.6" -f  -nu \
+<some_filler> -np <some_filler> -o <some_filler>
+python -m src.appcommander -a "at.bitfire.davdroid" -v "4.2.6" -f -nu \
+asdf -np asdf -o asdf
+python -m src.appcommander -a org.torproject.android -v "16.6.3 RC 1" \
+-f -t "DAVx5"
+```
```

### Comparing `appcommander-0.0.8/licence` & `appcommander-0.0.9/licence`

 * *Files identical despite different names*

### Comparing `appcommander-0.0.8/pyproject.toml` & `appcommander-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appcommander-0.0.8/setup.cfg` & `appcommander-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `appcommander-0.0.8/src/appcommander/Screen.py` & `appcommander-0.0.9/src/appcommander/Screen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 """Starts a script to control an app."""
 
-from typing import Callable, Dict, List, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Union
 
 import networkx as nx
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
+if TYPE_CHECKING:
+    # pylint: disable=W0406
+    # from src.appcommander.Screen import Screen
+    from src.appcommander.Script import Script
+else:
+    Script = object
+    # Screen = object
 
+
+# pylint: disable=E0102
 # pylint: disable=R0902
 # pylint: disable=R0903
 class Screen:
     """Represents an Android app screen."""
 
     # pylint: disable=R0913
     # pylint: disable=W0102
     @typechecked
     def __init__(
         self,
-        max_retries: int,
-        screen_nr: int,
-        wait_time_sec: float,
+        is_start: bool,
         get_next_actions: Callable[
             [Dict[str, str], Dict[str, str], Dict[str, str]],
-            Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None],
+            Union[Callable, None],
         ],
+        max_retries: int,
         required_objects: List[Dict[str, str]],
+        screen_nr: int,
+        wait_time_sec: float,
         optional_objects: List[Dict[str, str]] = [],
     ) -> None:
         self.get_next_actions: Callable[
             [Dict[str, str], Dict[str, str], Dict[str, str]],
-            Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None],
+            Union[Callable, None],
         ] = get_next_actions
 
-        # eloping typed dict.
+        self.is_start = is_start
         self.max_retries: int = max_retries
 
         """Sets the required objects for this screen.
 
         (If these objects are not found within the screen information
         returned by the dev, the screen will not be recogniszed. If
         it is, the screen is recognised by the: is_expected_screen function.
@@ -60,15 +70,15 @@
         self.screen_dict: Dict = {}
 
 
 @typechecked
 def get_next_screen(
     current_screen_nr: str,
     script_graph: nx.DiGraph,
-    actions: Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None],
+    actions: Union[Callable[[AutomatorDevice, Screen, Script], Dict], None],
 ) -> bool:
     """Gets the next expected screen."""
 
     neighbour_edges = []
     neighbour_names = []
     edge_actions = []
```

### Comparing `appcommander-0.0.8/src/appcommander/arg_parser/arg_parser.py` & `appcommander-0.0.9/src/appcommander/arg_parser/arg_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -54,14 +54,44 @@
         type=str,
         help=(
             "The names (csv) of the Android apps that you want Orbot to torify"
             + ". You can choose from (left or right):'."
         ),
     )
 
+    # Create argument to allow user to specify its nextcloud username.
+    parser.add_argument(
+        "-nu",
+        "--nextcloud-username",
+        action="store",
+        type=str,
+        help=("Your Nextcloud username."),
+    )
+
+    # Create argument to allow user to specify its nextcloud username.
+    parser.add_argument(
+        "-np",
+        "--nextcloud-password",
+        action="store",
+        type=str,
+        help=(
+            "Your Nextcloud password. "
+            + "TODO: build support for local safe passing."
+        ),
+    )
+
+    # Create argument to allow user to specify your onion url.
+    parser.add_argument(
+        "-o",
+        "--onion-url",
+        action="store",
+        type=str,
+        help=("Your url like: lakjdsf2340usdffa.onion"),
+    )
+
     # Run experiment on a particular experiment_settings json file.
     parser.add_argument(
         "-v",
         "--version",
         action="store",
         type=str,
         help=("Give the version of the Android app."),
```

### Comparing `appcommander-0.0.8/src/appcommander/arg_parser/process_args.py` & `appcommander-0.0.9/src/appcommander/arg_parser/process_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Dict
 
 from typeguard import typechecked
 from uiautomator import device
 
 from src.appcommander.hardcoded import app_name_mappings
 from src.appcommander.helper import export_screen_data, get_screen_as_dict
-from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import Script
 from src.appcommander.plot_script_flow import visualise_script_flow
 from src.appcommander.run_script import run_script
+from src.appcommander.Script import Script
 from src.appcommander.verification.arg_verification import (
     get_verified_apps_to_torify,
     sort_out_app_name_and_package_name,
 )
 from src.appcommander.verification.verify_phone_connection import (
     assert_app_is_installed,
     assert_app_version_is_correct,
@@ -23,32 +23,32 @@
 @typechecked
 def process_args(args: argparse.Namespace) -> None:
     """Processes the arguments and ensures the accompanying tasks are
     executed."""
     app_name, package_name = sort_out_app_name_and_package_name(
         args.app_name, app_name_mappings=app_name_mappings
     )
-
+    input_data: Dict = {}
     if args.torify:
-        torifying_apps: Dict[str, str] = get_verified_apps_to_torify(
+        input_data["torifying_apps"] = get_verified_apps_to_torify(
             app_name_mappings, args.torify
         )
-
-    # Also verifies phone is connected.
-    assert_app_is_installed(package_name=package_name)
-    assert_app_version_is_correct(
-        package_name=package_name,
-        app_version=args.version,
-    )
+    if args.nextcloud_username:
+        input_data["nextcloud_username"] = args.nextcloud_username
+        input_data["nextcloud_password"] = args.nextcloud_password
+        # TODO: prompt user for pwd. or safely communicate from
+        # Collabora Online.
+    if args.onion_url:
+        input_data["onion_url"] = args.onion_url
 
     apk_script = Script(
         app_name=app_name,
         overwrite=False,
         package_name=package_name,
-        torifying_apps=torifying_apps,
+        cli_input_data=input_data,
         version=args.version,
     )
     if args.export_screen:
         unpacked_screen_dict: Dict = get_screen_as_dict(
             dev=device,
             unpack=True,
             screen_dict={},
@@ -61,13 +61,21 @@
             script=apk_script,
             overwrite=True,
             subdir="unverified",
         )
     elif args.export_script_flow:
         visualise_script_flow(
             G=apk_script.script_graph,
-            app_name=apk_script.app_name.replace(".", "_"),
+            package_name=apk_script.package_name.replace(".", "_"),
             app_version=apk_script.version.replace(".", "_").replace(" ", "_"),
         )
     else:
         print("")
+        # pprint(apk_script.__dict__)
+        # Also verifies phone is connected.
+        assert_app_is_installed(package_name=package_name)
+        assert_app_version_is_correct(
+            package_name=package_name,
+            app_version=args.version,
+        )
+
         run_script(apk_script, device)
```

### Comparing `appcommander-0.0.8/src/appcommander/create_screens.py` & `appcommander-0.0.9/src/appcommander/create_screens.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 """Functions to assist a script file for an arbitrary app."""
 import importlib
-from typing import TYPE_CHECKING, List
+from types import ModuleType
+from typing import TYPE_CHECKING, Any, List, Optional, Tuple
 
 import networkx as nx
 from typeguard import typechecked
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
     from src.appcommander.Screen import Screen
+    from src.appcommander.Script import Script
 else:
     Script = object
     Screen = object
 
-screen_path: str = "src.appcommander.org_torproject_android.V16_6_3_RC_1."
-moduleNames = []
-screen_func_names = []
-modules = []
-for screen_index in range(0, 8):
-    module_name = f"{screen_path}screen_{screen_index}"
-    moduleNames.append(module_name)
-    screen_func_names.append(f"screen_{screen_index}")
-    my_module = importlib.import_module(module_name)
-    modules.append(my_module)
-
 
 @typechecked
-def create_screens(script_graph: nx.DiGraph) -> List[Screen]:
+def create_screens(script: Script) -> List[Screen]:
     """Creates the screens as networkx nodes."""
+
+    modules, screen_func_names = load_screen_files_per_app_version(
+        script.app_version_mod_path, script.script_graph
+    )
     screens: List[Screen] = []
 
     # Create the Screen objects programmatically.
     for i, module in enumerate(modules):
         # Create the function (reference) programmatically.
         # module represents the file that contains the screen function.
         # screen_func_name[i] is the name of the screen_i function in that
@@ -41,9 +33,56 @@
         # like writing: screen_3 if i==3.
         screen_function = getattr(module, screen_func_names[i])
         # execute the screen function, which returns a Screen object.
         screens.append(screen_function())
 
     # Add the screen objects to the script graph.
     for screen in screens:
-        script_graph.nodes[screen.screen_nr]["Screen"] = screen
+        script.script_graph.nodes[screen.screen_nr]["Screen"] = screen
     return screens
+
+
+@typechecked
+def load_screen_files_per_app_version(
+    app_version_mod_path: str, graph: nx.DiGraph
+) -> Tuple[List[ModuleType], List[str]]:
+    """A module is a python file (in this case).
+
+    So this script loads the Python files from which the screen object
+    data is loaded. Each app and version has its own screen_x files.
+    """
+
+    # Specify path to screen_files
+    moduleNames = []
+    screen_func_names = []
+    modules = []
+    for screen_index in range(0, len(graph)):
+        module_name = f"{app_version_mod_path}screen_{screen_index}"
+        moduleNames.append(module_name)
+        screen_func_names.append(f"screen_{screen_index}")
+        my_module = importlib.import_module(module_name)
+        modules.append(my_module)
+    return modules, screen_func_names
+
+
+@typechecked
+def load_script_attribute(  # type:ignore[misc]
+    app_version_mod_path: str,
+    filename: str,
+    obj_name: str,
+    attribute_name: Optional[str] = None,
+) -> Any:
+    """Loads an attribute for the script object.
+
+    If attribute_name is empty, it will load the object named <filename>
+    inside the <filename>, otherwise it will load the attribute
+    <attribute_name> of that object.
+    """
+
+    file_path = f"{app_version_mod_path}{filename}"
+    imported_file = importlib.import_module(file_path)
+
+    the_object = getattr(imported_file, obj_name)
+    if attribute_name is not None:
+        attribute = getattr(the_object(), attribute_name)
+        return attribute
+    return the_object
```

### Comparing `appcommander-0.0.8/src/appcommander/helper.py` & `appcommander-0.0.9/src/appcommander/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Contains helper functions that are used throughout this repository."""
 import json
 import os
-import subprocess  # nosec
 import time
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 import xmltodict
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
+from src.appcommander.run_bash_code import run_bash_command
+
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
     from src.appcommander.Screen import Screen
+    from src.appcommander.Script import Script
 else:
     Screen = object
     Script = object
 
 
 @typechecked
 def output_json(output_dir: str, filename: str, screen_dict: Dict) -> None:
@@ -93,49 +92,18 @@
                     script=script,
                     overwrite=overwrite,
                     subdir="verified",
                 )
 
 
 @typechecked
-def run_bash_command(
-    await_compilation: bool, bash_command: str, verbose: bool
-) -> Union[None, str]:
-    """Runs a bash command."""
-    if await_compilation:
-        if verbose:
-            subprocess.call(bash_command, shell=True)  # nosec
-        else:
-            output = subprocess.check_output(  # nosec
-                bash_command,
-                shell=True,
-                # stderr=subprocess.DEVNULL,
-                # stdout=subprocess.DEVNULL,
-            )
-            return output.decode("utf-8")
-    else:
-        if verbose:
-            # pylint: disable=R1732
-            subprocess.Popen(bash_command, shell=True)  # nosec
-        else:
-            # pylint: disable=R1732
-            subprocess.Popen(  # nosec
-                bash_command,
-                shell=True,
-                stderr=subprocess.DEVNULL,
-                stdout=subprocess.DEVNULL,
-            )
-    return None
-
-
-@typechecked
 def launch_app(app_name: str) -> None:
     """Launches app on phone."""
 
-    # Launc the app on phone.
+    # Launch the app on phone.
     command = f'adb shell monkey -p "{app_name}" 1 &>/dev/null'
     run_bash_command(
         await_compilation=True, bash_command=command, verbose=False
     )
 
 
 # pylint: disable=R0913
@@ -156,16 +124,16 @@
     data is placed in a subfolder named: subdir, to reduce the
     probability of the developer basing script actions on data belonging
     to the wrong screen.
     """
     output_dir = (
         (
             "src/appcommander/"
-            + f"{script.app_name}"
-            + f"/V{script.version}/{subdir}"
+            + f"{script.package_name}"
+            + f"/V{script.version}/{subdir}/"
         )
         .replace(".", "_")
         .replace(" ", "_")
     )
     output_name = f"{screen_nr}"
 
     for extension in [".json", ".png"]:
@@ -226,14 +194,15 @@
     verbose: Optional[bool] = False,
 ) -> bool:
     """Custom verification per screen based on the optional and required
     objects in screen.
 
     Raise error if verification fails.
     """
+
     # Preliminary check to see if the required objects are in.
     if not required_objects_in_screen(
         expected_screen.required_objects, unpacked_screen_dict
     ):
         if not retry:
             return False
         # Retry and return True if the required objects were found.
@@ -242,15 +211,18 @@
             # Reload the screen data again.
             unpacked_screen_dict = get_screen_as_dict(
                 dev=dev,
                 unpack=True,
                 screen_dict={},
                 reload=True,
             )
-
+            print(
+                f"Wait: {expected_screen.wait_time_sec} [s] on screen: "
+                + f"{expected_screen.screen_nr}"
+            )
             time.sleep(expected_screen.wait_time_sec)
             if required_objects_in_screen(
                 required_objects=expected_screen.required_objects,
                 unpacked_screen_dict=unpacked_screen_dict,
             ):
                 return True
             if verbose:
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/app_specific_helper.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 
 from typeguard import typechecked
 
 from src.appcommander.helper import dict_contains_other_dict
 
 # pylint: disable=R0801
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
     from src.appcommander.Screen import Screen
+    from src.appcommander.Script import Script
 else:
     Screen = object
     Script = object
 
 
 @typechecked
 def get_torified_item_index_dict(
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_0.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_0.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,23 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
 def screen_0() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
     started."""
-
     max_retries = 5
     screen_nr = 0
     wait_time_sec = 1
     required_objects: List[Dict[str, str]] = [
         {
             "@text": "Connection request",
         },
@@ -37,15 +34,15 @@
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -53,14 +50,15 @@
         amount, and optionally retries a pre-determined amount of attempts.
         """
         # In the start screen just press ok.
         return actions_0
 
     return Screen(
         get_next_actions=get_next_actions,
+        is_start=True,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
     )
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_1.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_4.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,45 +8,48 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
-def screen_1() -> Screen:
+def screen_4() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
     started."""
 
     max_retries = 1
-    screen_nr = 1
+    screen_nr = 4
     wait_time_sec = 0.1
     required_objects: List[Dict[str, str]] = [
         {
-            "@text": "Hello",
+            "@text": "You can enable any app to go through Tor using our"
+            + " built-in VPN.",
+        },
+        {
+            "@text": "This won't make you anonymous, but it will help get"
+            " through firewalls.",
         },
         {
-            "@text": "Welcome to Tor on mobile.",
+            "@text": "CHOOSE APPS",
         },
     ]
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -54,30 +57,30 @@
         amount, and optionally retries a pre-determined amount of attempts.
         """
 
         return actions_0
 
     return Screen(
         get_next_actions=get_next_actions,
+        is_start=True,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
     )
 
 
 # pylint: disable=W0613
 @typechecked
 def actions_0(dev: AutomatorDevice, screen: Screen, script: Script) -> Dict:
     """Performs the actions in option 0 in this screen.
 
-    For this screen, it clicks the "Next" button (icon=">") in the
-    bottom right.
+    For this screen, it clicks the "DONE" button in the bottom right.
     """
-    dev(resourceId="org.torproject.android:id/next").click()
+    dev(resourceId="org.torproject.android:id/done").click()
 
     # Return the expected screens, using get_expected_screen_nrs.
     action_nr: int = int(inspect.stack()[0][3][8:])
     screen_nr: int = screen.screen_nr
     script_flow: nx.DiGraph = script.script_graph
     return {
         "expected_screens": get_expected_screen_nrs(
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_2.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_1.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,45 +8,43 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
-def screen_2() -> Screen:
+def screen_1() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
     started."""
 
     max_retries = 1
-    screen_nr = 2
+    screen_nr = 1
     wait_time_sec = 0.1
     required_objects: List[Dict[str, str]] = [
         {
-            "@text": "Browse the internet how you expect you should.",
+            "@text": "Hello",
         },
         {
-            "@text": "No tracking. No censorship.",
+            "@text": "Welcome to Tor on mobile.",
         },
     ]
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -54,14 +52,15 @@
         amount, and optionally retries a pre-determined amount of attempts.
         """
 
         return actions_0
 
     return Screen(
         get_next_actions=get_next_actions,
+        is_start=True,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
     )
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_3.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,45 +8,43 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
-def screen_3() -> Screen:
+def screen_2() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
     started."""
 
     max_retries = 1
-    screen_nr = 3
+    screen_nr = 2
     wait_time_sec = 0.1
     required_objects: List[Dict[str, str]] = [
         {
-            "@text": "Sometimes you need a bridge to get to Tor.",
+            "@text": "Browse the internet how you expect you should.",
         },
         {
-            "@text": "TELL ME MORE",
+            "@text": "No tracking. No censorship.",
         },
     ]
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -54,14 +52,15 @@
         amount, and optionally retries a pre-determined amount of attempts.
         """
 
         return actions_0
 
     return Screen(
         get_next_actions=get_next_actions,
+        is_start=True,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
     )
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_4.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_3.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,50 +8,43 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
-def screen_4() -> Screen:
+def screen_3() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
     started."""
 
     max_retries = 1
-    screen_nr = 4
+    screen_nr = 3
     wait_time_sec = 0.1
     required_objects: List[Dict[str, str]] = [
         {
-            "@text": "You can enable any app to go through Tor using our"
-            + " built-in VPN.",
-        },
-        {
-            "@text": "This won't make you anonymous, but it will help get"
-            " through firewalls.",
+            "@text": "Sometimes you need a bridge to get to Tor.",
         },
         {
-            "@text": "CHOOSE APPS",
+            "@text": "TELL ME MORE",
         },
     ]
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -59,29 +52,31 @@
         amount, and optionally retries a pre-determined amount of attempts.
         """
 
         return actions_0
 
     return Screen(
         get_next_actions=get_next_actions,
+        is_start=True,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
     )
 
 
 # pylint: disable=W0613
 @typechecked
 def actions_0(dev: AutomatorDevice, screen: Screen, script: Script) -> Dict:
     """Performs the actions in option 0 in this screen.
 
-    For this screen, it clicks the "DONE" button in the bottom right.
+    For this screen, it clicks the "Next" button (icon=">") in the
+    bottom right.
     """
-    dev(resourceId="org.torproject.android:id/done").click()
+    dev(resourceId="org.torproject.android:id/next").click()
 
     # Return the expected screens, using get_expected_screen_nrs.
     action_nr: int = int(inspect.stack()[0][3][8:])
     screen_nr: int = screen.screen_nr
     script_flow: nx.DiGraph = script.script_graph
     return {
         "expected_screens": get_expected_screen_nrs(
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_5.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_5.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
 def screen_5() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
@@ -34,15 +32,15 @@
         {
             "@text": "Global " "(Auto)",
         },
         {
             "@text": "Trouble " "connecting?",
         },
         {
-            "@text": "Use Bridges ",
+            "@text": "Use Bridges",
         },
         {
             "@text": "Orbot",
         },
         {
             "@resource-id": "org.torproject.android:id/btnStart",
         },
@@ -58,15 +56,15 @@
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -77,14 +75,15 @@
             # run start.
             return actions_1
         # Else:
         # Go to settings, and enable the required apps.
         return actions_0
 
     return Screen(
+        is_start=True,
         get_next_actions=get_next_actions,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
         optional_objects=optional_objects,
     )
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_6.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_6.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Union
 
 import networkx as nx
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.helper import get_screen_as_dict
-from src.appcommander.org_torproject_android.V16_6_3_RC_1.app_specific_helper import (
+from src.appcommander.org_torproject_android.V16_6_3_RC_1.helper import (
     get_torified_item_index_dict,
     orbot_torifying_app_is_checked,
 )
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
 def screen_6() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
@@ -50,29 +48,30 @@
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,  # pylint: disable=W0613
         script_description: Optional[Dict] = {},
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
         Then the app goes to the next screen and waits a pre-determined
         amount, and optionally retries a pre-determined amount of attempts.
         """
 
         return actions_0
 
     return Screen(
+        is_start=True,
         get_next_actions=get_next_actions,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
         optional_objects=optional_objects,
     )
@@ -80,16 +79,20 @@
 
 # pylint: disable=W0613
 @typechecked
 def actions_0(dev: AutomatorDevice, screen: Screen, script: Script) -> Dict:
     """Performs the actions in option 2 in this screen."""
 
     # Get the dictionary with apps that need to be torified.
-    torifying_apps = script.torifying_apps
+    torifying_apps = script.input_data.torifying_apps
 
+    if not isinstance(torifying_apps, Dict):
+        raise TypeError(
+            f"Error, torifying_apps not specified:{torifying_apps}"
+        )
     for app_name, _ in torifying_apps.items():
 
         # Refresh the Orbot settings screen.
         dev(descriptionMatches="Refresh Apps").click()
 
         # Reload the screen data.
         unpacked_screen_dict: Dict = get_screen_as_dict(
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_7.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_7.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
 from src.appcommander.Screen import Screen
 from src.appcommander.script_orientation import get_expected_screen_nrs
 
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
+    from src.appcommander.Script import Script
 else:
     Script = object
 
 
 @typechecked
 def screen_7() -> Screen:
     """Creates the settings for a starting screen where Orbot is not yet
@@ -59,15 +57,15 @@
 
     # pylint: disable=W0613
     @typechecked
     def get_next_actions(
         required_objects: List[Dict[str, str]],
         optional_objects: List[Dict[str, str]],
         script: Script,  # pylint: disable=W0613
-    ) -> Union[Callable[[AutomatorDevice, Dict[str, str]], Dict], None]:
+    ) -> Union[Callable[[AutomatorDevice, Screen, Script], Dict], None]:
         """Looks at the required objects and optional objects and determines
         which actions to take next.
         An example of the next actions could be the following List:
         0. Select a textbox.
         1. Send some data to a textbox.
         2. Click on the/a "Next" button.
 
@@ -79,14 +77,15 @@
             # run start.
             return None
         # Else:
         # Go to settings, and enable the required apps.
         return actions_0
 
     return Screen(
+        is_start=True,
         get_next_actions=get_next_actions,
         max_retries=max_retries,
         screen_nr=screen_nr,
         wait_time_sec=wait_time_sec,
         required_objects=required_objects,
         optional_objects=optional_objects,
     )
```

### Comparing `appcommander-0.0.8/src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_flow.py` & `appcommander-0.0.9/src/appcommander/org_torproject_android/V16_6_3_RC_1/Screen_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Stores the flow logic of the script in a networkx graph."""
 
 import networkx as nx
 from typeguard import typechecked
 
 
-class Script_flow:
+class Screen_flow:
     """Contains a map from screen number and action number to next expected
     screens."""
 
     # pylint: disable=R0903
     @typechecked
     def __init__(
         self,
```

### Comparing `appcommander-0.0.8/src/appcommander/run_script.py` & `appcommander-0.0.9/src/appcommander/run_script.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 
 from typing import Callable, Dict, List
 
 from typeguard import typechecked
 from uiautomator import AutomatorDevice
 
-from src.appcommander.helper import export_screen_data_if_valid, launch_app
-from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import Script
+from src.appcommander.helper import export_screen_data_if_valid
 from src.appcommander.Screen import Screen
-from src.appcommander.script_orientation import get_start_nodes
+from src.appcommander.Script import Script
 from src.appcommander.verification.status_verification import can_proceed
 
 
 @typechecked
 def run_script(script: Script, dev: AutomatorDevice) -> None:
     """Runs the incoming script on the phone.
 
@@ -21,31 +20,44 @@
     app_name is something like: com_whatsapp_android (not: Whatsapp). It
     is derived from how your android dev calls the app, with the dots
     replaced by underscores. E.g. com.whatsapp.android or something like
     that.
     """
 
     # Open the app.
-    app_name = script.app_name
-    launch_app(app_name)
+    # script.input_data.launch_app(app_name=script.app_name)
+    script.input_data.launch_app(package_name=script.package_name)
 
-    expected_screens: List[int] = get_start_nodes(script.script_graph)
+    expected_screens: List[int] = list(
+        map(lambda x: x.screen_nr, script.screens)
+    )
 
-    _, screen_nr = can_proceed(
+    # First perorm a quick scope, without retry to find the desired screen.
+    is_expected, screen_nr = can_proceed(
         dev=dev,
         expected_screennames=expected_screens,
-        retry=True,
+        retry=False,
         script=script,
     )
+
+    # If quickscope did not find desired screen, try again with retries and
+    # waiting times per retry.
+    if not is_expected:
+        _, screen_nr = can_proceed(
+            dev=dev,
+            expected_screennames=expected_screens,
+            retry=True,
+            script=script,
+        )
     script.past_screens.append(screen_nr)
 
     next_actions = "filler"
     retry: bool = False  # For the first screen, do a quick scope because it is
     # known already.
-    while next_actions is not None:
+    while next_actions is not None and expected_screens:
         _, screen_nr = can_proceed(
             dev=dev,
             expected_screennames=expected_screens,
             retry=retry,
             script=script,
         )
         retry = True
```

### Comparing `appcommander-0.0.8/src/appcommander/script_orientation.py` & `appcommander-0.0.9/src/appcommander/script_orientation.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from typing import TYPE_CHECKING, List
 
 import networkx as nx
 from typeguard import typechecked
 
 # pylint: disable=R0801
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
     from src.appcommander.Screen import Screen
+    from src.appcommander.Script import Script
 else:
     Screen = object
     Script = object
 
 
 def get_expected_screen_nrs(
     G: nx.DiGraph, screen_nr: int, action_nr: int
@@ -35,18 +33,7 @@
     """Determines whether the current screen is one of the expected screens."""
     expected_screens: List[Screen] = []
     for nodename in script_graph.nodes:
         if nodename in expected_screennames:
             expected_screens.append(script_graph.nodes[nodename]["Screen"])
 
     return expected_screens
-
-
-@typechecked
-def get_start_nodes(script_graph: nx.DiGraph) -> List[int]:
-    """Sets the start_nodes attributes to True in the nodes that are start
-    screens."""
-    start_nodenames: List[int] = []
-    for nodename in script_graph.nodes:
-        if script_graph.nodes[nodename]["is_start"]:
-            start_nodenames.append(nodename)
-    return start_nodenames
```

### Comparing `appcommander-0.0.8/src/appcommander/verification/arg_verification.py` & `appcommander-0.0.9/src/appcommander/verification/arg_verification.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 
 @typechecked
 def sort_out_app_name_and_package_name(
     some_apk_name: str, app_name_mappings: Dict[str, str]
 ) -> Tuple[str, str]:
     """Returns app name and package name based on user input and supported apk
     packages."""
+
     if some_apk_name in app_name_mappings.keys():
         app_name = some_apk_name
         package_name = app_name_mappings[app_name]
     elif some_apk_name in app_name_mappings.values():
-        app_name = str(
-            {
-                i
-                for i in app_name_mappings
-                if app_name_mappings[i] == some_apk_name
-            }
-        )
+        for key in app_name_mappings.keys():
+            if app_name_mappings[key] == some_apk_name:
+                app_name = key
         package_name = some_apk_name
     return app_name, package_name
 
 
 @typechecked
 def verify_args(args: argparse.Namespace) -> None:
     """Performs the checks to verify the parser."""
@@ -82,15 +79,15 @@
         make_path_if_not_exists(version_path)
     else:  # User tries to use app name even though app name may not exist.
         if not os.path.exists(version_path):
             raise NotADirectoryError(
                 f"Error, path:{version_path} does not exist. "
                 + " Please create it and add an accompanying script."
             )
-        script_path = f"{version_path}/Script.py"
+        script_path = f"{version_path}/Screen_flow.py"
         if not os.path.exists(script_path):
             raise NotADirectoryError(
                 f"Error, path:{script_path} does not exist. "
                 + " Please create it and make it work."
             )
```

### Comparing `appcommander-0.0.8/src/appcommander/verification/status_verification.py` & `appcommander-0.0.9/src/appcommander/verification/status_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,16 @@
     get_screen_as_dict,
     is_expected_screen,
 )
 from src.appcommander.script_orientation import get_expected_screens
 
 # pylint: disable=R0801
 if TYPE_CHECKING:
-    from src.appcommander.org_torproject_android.V16_6_3_RC_1.Script import (
-        Script,
-    )
     from src.appcommander.Screen import Screen
+    from src.appcommander.Script import Script
 else:
     Screen = object
     Script = object
 
 
 @typechecked
 def can_proceed(
```

### Comparing `appcommander-0.0.8/src/appcommander/verification/verify_phone_connection.py` & `appcommander-0.0.9/src/appcommander/verification/verify_phone_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,25 @@
     """Throws error if phone is not connected via ADB."""
     # Launc the app on phone.
     command = "adb devices"
     output = run_bash_command(
         await_compilation=True, bash_command=command, verbose=False
     )
     lines = output.split("\n")
+
+    found_device: bool = False
     # TODO: make more robust check, e.g. eat "List of devs attached" and see
     # whether any a-Z 0-9 characters exist in output.
-    if len(lines) <= 3:
+    for line in lines:
+        if "List of devices attached" not in line:
+            for letter in line:
+                if letter.isalnum():
+                    found_device = True
+
+    if not found_device:
         raise Exception("Error, no adb dev is found.")
 
     # TODO: check if more than one devs are connected, and if yes, raise
     # exception if user did not specify the desired dev name.
 
 
 @typechecked
```

### Comparing `appcommander-0.0.8/src/appcommander.egg-info/PKG-INFO` & `appcommander-0.0.9/src/appcommander.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appcommander
-Version: 0.0.8
+Version: 0.0.9
 Summary: Performs controlled Android app automation through UI.
 Home-page: https://github.com/Hiveminds/appcommander
 Author: a-t-0
 Author-email: no-email@no-email.org
 Maintainer: a-t-0
 Maintainer-email: no-email@no-email.org
 License: AGPLv3
@@ -49,15 +49,15 @@
 
 Also, each phone manufacturer has a different rooting process, this repo can
 become a library to safely- and automatically root all (rootable) Android
 phones automatically (except the user must enable `ADB` themselves).
 
 ## Example
 
-![image](https://user-images.githubusercontent.com/34750068/212434675-65839344-0dbd-43c1-a7c2-3717cdd40d31.png)
+![image](https://github.com/HiveMinds/app-commander/blob/main/src/appcommander/org_torproject_android/V16_6_3_RC_1/flow.png?raw=true)
 
 ## Usage
 
 First satisfy the prerequisites:
 
 ```bash
 pip install appcommander
@@ -72,14 +72,21 @@
 which is the same as:
 
 ```bash
 python -m src.appcommander --app-name org.torproject.android \
 --version "16.6.3 RC 1" -torify "DAVx5"
 ```
 
+Or, to configure DAVx5:
+
+```bash
+python -m src.appcommander -a at.bitfire.davdroid -v "4.2.6" -nu \
+<your_nextcloud_username> -np <your_nextcloud_password> -o <your_onion_url>
+```
+
 For more info, run:
 
 ```bash
 python -m src.appcommander --help
 ```
 
 ## Testing
@@ -166,7 +173,28 @@
 pip install -e .
 ```
 
 that installs the latest changes into the pip package locally (into your conda
 environment).
 
 <!-- Un-wrapped URL's (Badges and Hyperlinks) -->
+
+### Show your app-flow
+
+To show how your script works, run (along with any additional input args
+required for that script):
+
+```sh
+python -m src.appcommander -a <package_name> -v <app_version> -f \
+<additional arguments>
+```
+
+For example:
+
+```sh
+python -m src.appcommander -a "at.bitfire.davdroid" -v "4.2.6" -f  -nu \
+<some_filler> -np <some_filler> -o <some_filler>
+python -m src.appcommander -a "at.bitfire.davdroid" -v "4.2.6" -f -nu \
+asdf -np asdf -o asdf
+python -m src.appcommander -a org.torproject.android -v "16.6.3 RC 1" \
+-f -t "DAVx5"
+```
```

### Comparing `appcommander-0.0.8/src/appcommander.egg-info/SOURCES.txt` & `appcommander-0.0.9/src/appcommander.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 README.md
 licence
 pyproject.toml
 setup.cfg
 setup.py
 src/appcommander/Screen.py
+src/appcommander/Script.py
 src/appcommander/__init__.py
 src/appcommander/__main__.py
 src/appcommander/create_screens.py
 src/appcommander/file_input_output.py
 src/appcommander/hardcoded.py
 src/appcommander/helper.py
 src/appcommander/plot_script_flow.py
+src/appcommander/run_bash_code.py
 src/appcommander/run_script.py
 src/appcommander/screen_reading.py
 src/appcommander/script_orientation.py
 src/appcommander/text_parsing.py
 src/appcommander.egg-info/PKG-INFO
 src/appcommander.egg-info/SOURCES.txt
 src/appcommander.egg-info/dependency_links.txt
 src/appcommander.egg-info/entry_points.txt
 src/appcommander.egg-info/requires.txt
 src/appcommander.egg-info/top_level.txt
 src/appcommander/arg_parser/__init__.py
 src/appcommander/arg_parser/arg_parser.py
 src/appcommander/arg_parser/process_args.py
+src/appcommander/at_bitfire_davdroid/__init__.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/App_input_data.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/Screen_flow.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/__init__.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/helper.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_0.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_1.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_2.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_3.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_4.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_5.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_6.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_7.py
+src/appcommander/at_bitfire_davdroid/V4_2_6/screen_8.py
 src/appcommander/org_torproject_android/__init__.py
-src/appcommander/org_torproject_android/V16_6_3_RC_1/Script.py
+src/appcommander/org_torproject_android/V16_6_3_RC_1/App_input_data.py
+src/appcommander/org_torproject_android/V16_6_3_RC_1/Screen_flow.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/__init__.py
-src/appcommander/org_torproject_android/V16_6_3_RC_1/app_specific_helper.py
+src/appcommander/org_torproject_android/V16_6_3_RC_1/helper.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_0.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_1.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_2.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_3.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_4.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_5.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_6.py
 src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_7.py
-src/appcommander/org_torproject_android/V16_6_3_RC_1/screen_flow.py
 src/appcommander/verification/__init__.py
 src/appcommander/verification/arg_verification.py
 src/appcommander/verification/status_verification.py
 src/appcommander/verification/verify_phone_connection.py
```

