# Comparing `tmp/deebot-client-2.0.0b1.tar.gz` & `tmp/deebot-client-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-2.0.0b1.tar", last modified: Sun Apr 16 10:11:05 2023, max compression
+gzip compressed data, was "deebot-client-2.0.0b2.tar", last modified: Thu May 25 20:02:24 2023, max compression
```

## Comparing `deebot-client-2.0.0b1.tar` & `deebot-client-2.0.0b2.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 10:11:05.823820 deebot-client-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.815820 deebot-client-2.0.0b1/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/messages/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/messages/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/vacuum_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.815820 deebot-client-2.0.0b1/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-16 10:11:05.823820 deebot-client-2.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-16 10:11:01.000000 deebot-client-2.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.815820 deebot-client-2.0.0b1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.085160 deebot-client-2.0.0b2/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.089160 deebot-client-2.0.0b2/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.089160 deebot-client-2.0.0b2/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.089160 deebot-client-2.0.0b2/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/messages/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/messages/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/vacuum_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.085160 deebot-client-2.0.0b2/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.081160 deebot-client-2.0.0b2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/events/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_stats.py
```

### Comparing `deebot-client-2.0.0b1/LICENSE.txt` & `deebot-client-2.0.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/PKG-INFO` & `deebot-client-2.0.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
@@ -70,16 +70,15 @@
 
     devices_ = await api_client.get_devices()
 
     bot = VacuumBot(devices_[0], authenticator)
 
     mqtt_config = MqttConfiguration(config=config)
     mqtt = MqttClient(mqtt_config, authenticator)
-    await mqtt.connect()
-    await mqtt.subscribe(bot)
+    await bot.initialize(mqtt)
 
     async def on_battery(event: BatteryEvent):
       # Do stuff on battery event
       if event.value == 100:
         # Battery full
         pass
```

### Comparing `deebot-client-2.0.0b1/README.md` & `deebot-client-2.0.0b2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 
     devices_ = await api_client.get_devices()
 
     bot = VacuumBot(devices_[0], authenticator)
 
     mqtt_config = MqttConfiguration(config=config)
     mqtt = MqttClient(mqtt_config, authenticator)
-    await mqtt.connect()
-    await mqtt.subscribe(bot)
+    await bot.initialize(mqtt)
 
     async def on_battery(event: BatteryEvent):
       # Do stuff on battery event
       if event.value == 100:
         # Battery full
         pass
```

### Comparing `deebot-client-2.0.0b1/deebot_client/api_client.py` & `deebot-client-2.0.0b2/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/authentication.py` & `deebot-client-2.0.0b2/deebot_client/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Authentication module."""
 import asyncio
 import time
-from collections.abc import Callable, Mapping
+from collections.abc import Awaitable, Callable, Mapping
 from typing import Any
 from urllib.parse import urljoin
 
 from aiohttp import ClientResponseError, hdrs
 
 from .const import REALM
 from .exceptions import ApiError, AuthenticationError, InvalidAuthenticationError
@@ -305,73 +305,52 @@
         self._auth_client = _AuthClient(
             config,
             account_id,
             password_hash,
         )
 
         self._lock = asyncio.Lock()
-        self._on_credentials_changed: set[Callable[[Credentials], None]] = set()
+        self._on_credentials_changed: set[
+            Callable[[Credentials], Awaitable[None]]
+        ] = set()
         self._credentials: Credentials | None = None
-        self._refresh_task: asyncio.TimerHandle | None = None
+        self._refresh_handle: asyncio.TimerHandle | None = None
 
     async def authenticate(self, force: bool = False) -> Credentials:
         """Authenticate on ecovacs servers."""
         async with self._lock:
             should_login = False
             if self._credentials is None or force:
                 _LOGGER.debug("No cached credentials, performing login")
                 should_login = True
             elif self._credentials.expires_at < time.time():
                 _LOGGER.debug("Credentials have expired, performing login")
                 should_login = True
 
             if should_login:
                 self._credentials = await self._auth_client.login()
-                if self._refresh_task:
-                    self._refresh_task.cancel()
-
+                self._cancel_refresh_task()
                 self._create_refresh_task()
 
                 for on_changed in self._on_credentials_changed:
-                    on_changed(self._credentials)
+                    await on_changed(self._credentials)
 
             assert self._credentials is not None
             return self._credentials
 
-    def subscribe(self, callback: Callable[[Credentials], None]) -> None:
-        """Add callback on new credentials."""
-        self._on_credentials_changed.add(callback)
+    def subscribe(
+        self, callback: Callable[[Credentials], Awaitable[None]]
+    ) -> Callable[[], None]:
+        """Add callback on new credentials and return subscribe callback."""
 
-    def unsubscribe(self, callback: Callable[[Credentials], None]) -> None:
-        """Remove callback on new credentials."""
-        if callback in self._on_credentials_changed:
+        def unsubscribe() -> None:
             self._on_credentials_changed.remove(callback)
 
-    def _create_refresh_task(self) -> None:
-        # refresh at 99% of validity
-        assert self._credentials is not None
-        validity = (self._credentials.expires_at - time.time()) * 0.99
-
-        self._refresh_task = asyncio.get_event_loop().call_later(
-            validity, self._auto_refresh_task
-        )
-
-    def _auto_refresh_task(self) -> None:
-        _LOGGER.debug("Refresh token")
-
-        async def refresh() -> None:
-            try:
-                self._refresh_task = None
-                await self.authenticate(True)
-            except Exception:  # pylint: disable=broad-except
-                _LOGGER.error(
-                    "An exception occurred during refreshing token", exc_info=True
-                )
-
-        asyncio.create_task(refresh())
+        self._on_credentials_changed.add(callback)
+        return unsubscribe
 
     async def post_authenticated(
         self,
         path: str,
         json: dict[str, Any],
         *,
         query_params: dict[str, Any] | None = None,
@@ -381,7 +360,36 @@
         return await self._auth_client.post(
             path,
             json,
             query_params=query_params,
             headers=headers,
             credentials=await self.authenticate(),
         )
+
+    async def teardown(self) -> None:
+        """Teardown authenticator."""
+        self._cancel_refresh_task()
+
+    def _cancel_refresh_task(self) -> None:
+        if self._refresh_handle and not self._refresh_handle.cancelled():
+            self._refresh_handle.cancel()
+
+    def _create_refresh_task(self) -> None:
+        # refresh at 99% of validity
+        def refresh() -> None:
+            _LOGGER.debug("Refresh token")
+
+            async def async_refresh() -> None:
+                try:
+                    await self.authenticate(True)
+                except Exception:  # pylint: disable=broad-except
+                    _LOGGER.error(
+                        "An exception occurred during refreshing token", exc_info=True
+                    )
+
+            asyncio.create_task(async_refresh())
+            self._refresh_handle = None
+
+        assert self._credentials is not None
+        validity = (self._credentials.expires_at - time.time()) * 0.99
+
+        self._refresh_handle = asyncio.get_event_loop().call_later(validity, refresh)
```

### Comparing `deebot-client-2.0.0b1/deebot_client/command.py` & `deebot-client-2.0.0b2/deebot_client/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base command."""
 import asyncio
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Any, final
 
 from .authentication import Authenticator
 from .const import PATH_API_IOT_DEVMANAGER, REQUEST_HEADERS
 from .events.event_bus import EventBus
 from .logging_filter import get_logger
@@ -15,15 +15,15 @@
 _LOGGER = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class CommandResult(HandlingResult):
     """Command result object."""
 
-    requested_commands: list["Command"] | None = None
+    requested_commands: list["Command"] = field(default_factory=lambda: [])
 
     @classmethod
     def success(cls) -> "CommandResult":
         """Create result with handling success."""
         return CommandResult(HandlingState.SUCCESS)
 
     @classmethod
@@ -31,51 +31,61 @@
         """Create result with handling analyse."""
         return CommandResult(HandlingState.ANALYSE)
 
 
 class Command(ABC):
     """Abstract command object."""
 
+    _targets_bot: bool = True
+
     def __init__(self, args: dict | list | None = None) -> None:
         if args is None:
             args = {}
         self._args = args
 
     @property  # type: ignore[misc]
     @classmethod
     @abstractmethod
     def name(cls) -> str:
         """Command name."""
 
     @final
     async def execute(
         self, authenticator: Authenticator, device_info: DeviceInfo, event_bus: EventBus
-    ) -> None:
-        """Execute command."""
+    ) -> bool:
+        """Execute command.
+
+        Returns:
+            bot_reached (bool): True if the command was targeting the bot and it responded in time. False otherwise.
+                                This value is not indicating if the command was executed successfully.
+        """
         try:
             result = await self._execute(authenticator, device_info, event_bus)
-            if result.state == HandlingState.SUCCESS and result.requested_commands:
+            if result.state == HandlingState.SUCCESS:
                 # Execute command which are requested by the handler
                 tasks = []
                 for requested_command in result.requested_commands:
                     tasks.append(
                         asyncio.create_task(
                             requested_command.execute(
                                 authenticator, device_info, event_bus
                             )
                         )
                     )
 
                 await asyncio.gather(*tasks)
+
+                return self._targets_bot
         except Exception:  # pylint: disable=broad-except
             _LOGGER.warning(
                 "Could not execute command %s",
                 self.name,
                 exc_info=True,
             )
+        return False
 
     async def _execute(
         self, authenticator: Authenticator, device_info: DeviceInfo, event_bus: EventBus
     ) -> CommandResult:
         """Execute command."""
         response = await self._execute_api_request(authenticator, device_info)
```

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/__init__.py` & `deebot-client-2.0.0b2/deebot_client/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Commands module."""
-from typing import Dict, Type
-
 from ..command import Command
 from .advanced_mode import GetAdvancedMode, SetAdvancedMode
 from .battery import GetBattery
 from .carpet import GetCarpetAutoFanBoost, SetCarpetAutoFanBoost
 from .charge import Charge
 from .charge_state import GetChargeState
 from .clean import Clean, CleanArea, GetCleanInfo
@@ -97,16 +95,16 @@
     SetVolume,
 
     GetWaterInfo,
     SetWaterInfo,
 ]
 # fmt: on
 
-COMMANDS_WITH_HANDLING: dict[str, type[Command]] = {
+COMMANDS: dict[str, type[Command]] = {
     cmd.name: cmd for cmd in _COMMANDS  # type: ignore[misc]
 }
 
 COMMANDS_WITH_MQTT_P2P_HANDLING: dict[str, type[CommandHandlingMqttP2P]] = {
     cmd_name: cmd
-    for (cmd_name, cmd) in COMMANDS_WITH_HANDLING.items()
+    for (cmd_name, cmd) in COMMANDS.items()
     if issubclass(cmd, CommandHandlingMqttP2P)
 }
```

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/charge.py` & `deebot-client-2.0.0b2/deebot_client/commands/charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/charge_state.py` & `deebot-client-2.0.0b2/deebot_client/commands/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/clean.py` & `deebot-client-2.0.0b2/deebot_client/commands/clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/clean_count.py` & `deebot-client-2.0.0b2/deebot_client/commands/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/clean_logs.py` & `deebot-client-2.0.0b2/deebot_client/commands/clean_logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 _LOGGER = get_logger(__name__)
 
 
 class GetCleanLogs(Command):
     """Get clean logs command."""
 
+    _targets_bot: bool = False
     name = "GetCleanLogs"
 
     def __init__(self, count: int = 0) -> None:
         super().__init__({"count": count})
 
     async def _execute_api_request(
         self, authenticator: Authenticator, device_info: DeviceInfo
```

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/common.py` & `deebot-client-2.0.0b2/deebot_client/commands/common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/custom.py` & `deebot-client-2.0.0b2/deebot_client/commands/custom.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 
 _LOGGER = get_logger(__name__)
 
 
 class CustomCommand(Command):
     """Custom command, used when user wants to execute a command, which is not part of this library."""
 
-    name = "CustomCommand"
+    name: str = "CustomCommand"
 
     def __init__(self, name: str, args: dict | list | None = None) -> None:
-        self._name = name
+        self.name = name
         super().__init__(args)
 
     def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
         """Handle response from a command.
 
         :return: A message response
         """
         if response.get("ret") == "ok":
             data = response.get("resp", response)
-            event_bus.notify(CustomCommandEvent(self._name, data))
+            event_bus.notify(CustomCommandEvent(self.name, data))
             return CommandResult.success()
 
-        _LOGGER.warning('Command "%s" was not successfully: %s', self._name, response)
+        _LOGGER.warning('Command "%s" was not successfully: %s', self.name, response)
         return CommandResult(HandlingState.FAILED)
 
     def __eq__(self, obj: object) -> bool:
         if super().__eq__(obj) and isinstance(obj, CustomCommand):
-            return self._name == obj._name
+            return self.name == obj.name
 
         return False
 
     def __hash__(self) -> int:
-        return super().__hash__() + hash(self._name)
+        return super().__hash__() + hash(self.name)
 
 
 class CustomPayloadCommand(CustomCommand):
     """Custom command, where args is the raw payload."""
 
     def _get_payload(self) -> dict[str, Any] | list:
         return self._args
```

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/error.py` & `deebot-client-2.0.0b2/deebot_client/commands/error.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/fan_speed.py` & `deebot-client-2.0.0b2/deebot_client/commands/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/life_span.py` & `deebot-client-2.0.0b2/deebot_client/commands/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/map.py` & `deebot-client-2.0.0b2/deebot_client/commands/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/pos.py` & `deebot-client-2.0.0b2/deebot_client/commands/pos.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/stats.py` & `deebot-client-2.0.0b2/deebot_client/commands/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/volume.py` & `deebot-client-2.0.0b2/deebot_client/commands/volume.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/commands/water_info.py` & `deebot-client-2.0.0b2/deebot_client/commands/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/events/__init__.py` & `deebot-client-2.0.0b2/deebot_client/events/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/events/const.py` & `deebot-client-2.0.0b2/deebot_client/events/const.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/events/event_bus.py` & `deebot-client-2.0.0b2/deebot_client/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/events/map.py` & `deebot-client-2.0.0b2/deebot_client/events/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/logging_filter.py` & `deebot-client-2.0.0b2/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/map.py` & `deebot-client-2.0.0b2/deebot_client/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/message.py` & `deebot-client-2.0.0b2/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/messages/battery.py` & `deebot-client-2.0.0b2/deebot_client/messages/battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/messages/stats.py` & `deebot-client-2.0.0b2/deebot_client/messages/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/models.py` & `deebot-client-2.0.0b2/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client/util.py` & `deebot-client-2.0.0b2/deebot_client/util.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/deebot_client.egg-info/PKG-INFO` & `deebot-client-2.0.0b2/deebot_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
@@ -70,16 +70,15 @@
 
     devices_ = await api_client.get_devices()
 
     bot = VacuumBot(devices_[0], authenticator)
 
     mqtt_config = MqttConfiguration(config=config)
     mqtt = MqttClient(mqtt_config, authenticator)
-    await mqtt.connect()
-    await mqtt.subscribe(bot)
+    await bot.initialize(mqtt)
 
     async def on_battery(event: BatteryEvent):
       # Do stuff on battery event
       if event.value == 100:
         # Battery full
         pass
```

### Comparing `deebot-client-2.0.0b1/deebot_client.egg-info/SOURCES.txt` & `deebot-client-2.0.0b2/deebot_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,9 +76,10 @@
 tests/commands/test_true_detect.py
 tests/commands/test_water_info.py
 tests/events/__init__.py
 tests/events/test_events.py
 tests/events/test_water_info.py
 tests/messages/__init__.py
 tests/messages/test_battery.py
+tests/messages/test_get_messages.py
 tests/messages/test_messages.py
 tests/messages/test_stats.py
```

### Comparing `deebot-client-2.0.0b1/setup.py` & `deebot-client-2.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = list(val.strip() for val in file)
 
 setup(
     name="deebot-client",
-    version="2.0.0b1",
+    version="2.0.0b2",
     url="https://github.com/DeebotUniverse/client.py",
     description="a library for controlling certain deebot vacuums",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DeebotUniverse",
     author_email="deebotuniverse@knatschig-as-hell.info",
     license="GPL-3.0",
```

### Comparing `deebot-client-2.0.0b1/tests/commands/__init__.py` & `deebot-client-2.0.0b2/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_advanced_mode.py` & `deebot-client-2.0.0b2/tests/commands/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_carpet.py` & `deebot-client-2.0.0b2/tests/commands/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_charge.py` & `deebot-client-2.0.0b2/tests/commands/test_charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_clean.py` & `deebot-client-2.0.0b2/tests/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_clean_count.py` & `deebot-client-2.0.0b2/tests/commands/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_clean_log.py` & `deebot-client-2.0.0b2/tests/commands/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_clean_preference.py` & `deebot-client-2.0.0b2/tests/commands/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_continuous_cleaning.py` & `deebot-client-2.0.0b2/tests/commands/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_custom.py` & `deebot-client-2.0.0b2/tests/commands/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_fan_speed.py` & `deebot-client-2.0.0b2/tests/commands/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_life_span.py` & `deebot-client-2.0.0b2/tests/commands/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_map.py` & `deebot-client-2.0.0b2/tests/commands/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_mulitmap_state.py` & `deebot-client-2.0.0b2/tests/commands/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_true_detect.py` & `deebot-client-2.0.0b2/tests/commands/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/commands/test_water_info.py` & `deebot-client-2.0.0b2/tests/commands/test_water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/messages/test_battery.py` & `deebot-client-2.0.0b2/tests/messages/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b1/tests/messages/test_stats.py` & `deebot-client-2.0.0b2/tests/messages/test_stats.py`

 * *Files identical despite different names*

