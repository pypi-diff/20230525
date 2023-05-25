# Comparing `tmp/nonebot_plugin_xiuxian_2-2.9.2.1.tar.gz` & `tmp/nonebot_plugin_xiuxian_2-2.9.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_xiuxian_2-2.9.2.1.tar", last modified: Mon May  1 09:00:46 2023, max compression
+gzip compressed data, was "nonebot_plugin_xiuxian_2-2.9.2.2.tar", last modified: Fri May  5 13:42:31 2023, max compression
```

## Comparing `nonebot_plugin_xiuxian_2-2.9.2.1.tar` & `nonebot_plugin_xiuxian_2-2.9.2.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.309723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.313723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/item_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/lay_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    54783 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/player_fight.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/read_buff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49555 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.313723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/
--rw-r--r--   0 runner    (1001) docker     (123)    72789 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/
--rw-r--r--   0 runner    (1001) docker     (123)    72776 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/back_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/
--rw-r--r--   0 runner    (1001) docker     (123)    60905 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/
--rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/
--rw-r--r--   0 runner    (1001) docker     (123)    45638 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/
--rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mix_elixir_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/
--rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/
--rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.309723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.818426 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.818426 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/item_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/lay_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54783 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/player_fight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/read_buff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49567 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/
+-rw-r--r--   0 runner    (1001) docker     (123)    72789 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/
+-rw-r--r--   0 runner    (1001) docker     (123)    72776 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/back_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/
+-rw-r--r--   0 runner    (1001) docker     (123)    60905 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/
+-rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/
+-rw-r--r--   0 runner    (1001) docker     (123)    45638 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/
+-rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mix_elixir_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/
+-rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.822425 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/
+-rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:42:31.818426 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-05 13:42:31.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-05 13:42:31.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:42:31.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 13:42:31.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 13:42:31.000000 nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:42:31.826426 nonebot_plugin_xiuxian_2-2.9.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 13:42:20.000000 nonebot_plugin_xiuxian_2-2.9.2.2/setup.py
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/PKG-INFO` & `nonebot_plugin_xiuxian_2-2.9.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_xiuxian_2
-Version: 2.9.2.1
+Version: 2.9.2.2
 Summary: 修仙插件
 Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat
 Author-email: 1242550160@qq.com
 Keywords: pip,nonebot2,文游,修仙
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_xiuxian_2 Version: 2.9.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_xiuxian_2 Version: 2.9.2.2 Summary:
 ä¿®ä»æä»¶ Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat Author-email: 1242550160@qq.com Keywords:
 pip,nonebot2,ææ¸¸,ä¿®ä» Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified) Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/README.md` & `nonebot_plugin_xiuxian_2-2.9.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/data_source.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/item_json.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/item_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/lay_out.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/lay_out.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/player_fight.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/player_fight.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/read_buff.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/read_buff.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/utils.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 UserCd = namedtuple("UserCd", ["user_id", "type", "create_time", "scheduled_time"])
 SectInfo = namedtuple("SectInfo",
                       ["sect_id", "sect_name", "sect_owner", "sect_scale", "sect_used_stone", "sect_fairyland",
                        "sect_materials", "mainbuff", "secbuff", "elixir_room_level"])
 BuffInfo = namedtuple("BuffInfo",
                       ["id", "user_id", "main_buff", "sec_buff", "faqi_buff", "fabao_weapon", "armor_buff", "atk_buff",
-                       "blessed_spot"])
+                       "blessed_spot", "sub_buff"])
 back = namedtuple("back", ["user_id", "goods_id", "goods_name", "goods_type", "goods_num", "create_time", "update_time",
                            "remake", "day_num", "all_num", "action_time", "state", "bind_num"])
 
 num = '578043031'
 
 
 class XiuxianDateManage:
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/back_util.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/back_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-xiuxian-2
-Version: 2.9.2.1
+Version: 2.9.2.2
 Summary: 修仙插件
 Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat
 Author-email: 1242550160@qq.com
 Keywords: pip,nonebot2,文游,修仙
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-xiuxian-2 Version: 2.9.2.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-xiuxian-2 Version: 2.9.2.2 Summary:
 ä¿®ä»æä»¶ Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat Author-email: 1242550160@qq.com Keywords:
 pip,nonebot2,ææ¸¸,ä¿®ä» Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified) Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt` & `nonebot_plugin_xiuxian_2-2.9.2.2/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.2.1/setup.py` & `nonebot_plugin_xiuxian_2-2.9.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
     setuptools.setup(
     name='nonebot_plugin_xiuxian_2',
-    version='2.9.2.1',
+    version='2.9.2.2',
     author='QingmuCat',
     author_email='1242550160@qq.com',
     keywords=["pip", "nonebot2", "文游", "修仙"],
     url='https://github.com/QingMuCat/nonebot_plugin_xiuxian_2',
     description='''修仙插件''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

