# Comparing `tmp/nonebot_plugin_majsoul-0.1.6.tar.gz` & `tmp/nonebot_plugin_majsoul-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_majsoul-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_majsoul-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_majsoul-0.1.6.tar` & `nonebot_plugin_majsoul-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.1.6/LICENSE
--rw-r--r--   0        0        0      623 2023-05-10 04:23:05.048672 nonebot_plugin_majsoul-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2449 2022-12-17 10:37:40.516448 nonebot_plugin_majsoul-0.1.6/README.md
--rw-r--r--   0        0        0     1321 2023-03-23 15:20:27.440710 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/__init__.py
--rw-r--r--   0        0        0      237 2023-03-01 06:00:00.226716 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/config.py
--rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/errors.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/interceptors/__init__.py
--rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/interceptors/handle_error.py
--rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/__init__.py
--rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/auto_retry.py
--rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/host_prober.py
--rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
--rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/api.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
--rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
--rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
--rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
--rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
--rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
--rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
--rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
--rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
--rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
--rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
--rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
--rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
--rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
--rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
--rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
--rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
--rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
--rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
--rw-r--r--   0        0        0     9420 2023-03-28 05:00:03.699457 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
--rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
--rw-r--r--   0        0        0        0 2022-12-05 07:11:39.109850 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/res/__init__.py
--rw-r--r--   0        0        0  9765052 2022-12-05 07:11:39.108850 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/res/LXGWWenKaiMonoLite-Regular.ttf
--rw-r--r--   0        0        0        0 2022-12-04 13:54:54.946684 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/__init__.py
--rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/decode_integer.py
--rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/my_executor.py
--rw-r--r--   0        0        0      101 2022-10-29 00:19:22.302000 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/nonebot.py
--rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/percentile.py
--rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/rank.py
--rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.2.0/LICENSE
+-rw-r--r--   0        0        0      719 2023-05-25 08:02:43.629565 nonebot_plugin_majsoul-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3619 2023-05-25 09:12:53.469977 nonebot_plugin_majsoul-0.2.0/README.md
+-rw-r--r--   0        0        0     1062 2023-05-25 08:43:24.660366 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-25 08:45:02.584548 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/config.py
+-rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/errors.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/interceptors/__init__.py
+-rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/interceptors/handle_error.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/network/__init__.py
+-rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/network/auto_retry.py
+-rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/network/host_prober.py
+-rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
+-rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/api.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
+-rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
+-rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
+-rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
+-rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
+-rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
+-rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
+-rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
+-rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
+-rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
+-rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
+-rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
+-rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
+-rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
+-rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
+-rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
+-rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
+-rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
+-rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
+-rw-r--r--   0        0        0     9731 2023-05-25 08:57:58.318285 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
+-rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
+-rw-r--r--   0        0        0       67 2023-05-25 08:11:04.925321 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paipu/__init__.py
+-rw-r--r--   0        0        0      887 2023-05-25 08:12:40.329877 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paipu/downloader.py
+-rw-r--r--   0        0        0     2631 2023-05-25 09:01:41.946504 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paipu/query_paipu.py
+-rw-r--r--   0        0        0        0 2023-05-25 08:00:39.014941 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/__init__.py
+-rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/decode_integer.py
+-rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/my_executor.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247572 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/nonebot.py
+-rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/percentile.py
+-rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/rank.py
+-rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_majsoul-0.1.6/LICENSE` & `nonebot_plugin_majsoul-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/pyproject.toml` & `nonebot_plugin_majsoul-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "nonebot-plugin-majsoul"
-version = "0.1.6"
+version = "0.2.0"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_majsoul", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 nonebot2 = "^2.0.0rc3"
 tzlocal = "^4.2"
 httpx = "^0.23.0"
 pydantic = "^1.10.2"
 monthdelta = "^0.9.1"
 icmplib = "^3.0.3"
 matplotlib = "^3.6.2"
 typing-extensions = "^4.4.0"
 nonebot-plugin-send-anything-anywhere = "^0.2.1"
+nonebot-adapter-onebot = "^2.2.3"
+nonebot-plugin-gocqhttp-cross-machine-upload-file = "^0.1.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/__init__.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,16 @@
 @License        : AGPLv3
 @GitHub         : https://github.com/ssttkkl/nonebot-plugin-majsoul
 """
 from nonebot import require
 
 require("nonebot_plugin_saa")
 
-from importlib import resources
-from matplotlib import font_manager, pyplot as plt
-
-from . import res
 from .utils.nonebot import default_cmd_start
 
-with resources.path(res, "LXGWWenKaiMonoLite-Regular.ttf") as path:
-    font_manager.fontManager.addfont(path)
-plt.rcParams['font.sans-serif'] = 'LXGW WenKai Mono Lite'
-
 help_text = f"""
 牌谱屋：
 - {default_cmd_start}雀魂(三麻)信息 <雀魂账号> [<房间类型>] [最近<数量>场] [最近<数量>{{天|周|个月|年}}]
 - {default_cmd_start}雀魂(三麻)对局 <雀魂账号> [<房间类型>]
 - {default_cmd_start}雀魂(三麻)PT图 <雀魂账号> [最近<数量>场] [最近<数量>{{天|周|个月|年}}]
 
 以上命令格式中，以<>包裹的表示一个参数，以[]包裹的表示一个可选项。
@@ -35,7 +27,8 @@
 __plugin_meta__ = PluginMetadata(
     name='雀魂查询',
     description='根据牌谱屋的数据查询雀魂账号信息',
     usage=help_text
 )
 
 from . import paifuya
+from . import paipu
```

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/interceptors/handle_error.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/auto_retry.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/network/auto_retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/host_prober.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/network/host_prober.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/api.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import sys
 from asyncio import wait_for
 from datetime import datetime, timezone
 from io import BytesIO
 from typing import Sequence, Optional, Text
 
 import matplotlib.pyplot as plt
 from httpx import HTTPStatusError
+from matplotlib import font_manager
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from nonebot import on_command
 from nonebot.internal.adapter import Event
 from nonebot_plugin_saa import MessageFactory, Image
 
 from nonebot_plugin_majsoul.config import conf
@@ -22,14 +24,22 @@
 from .data.models.room_rank import all_four_player_room_rank, all_three_player_room_rank, RoomRank
 from .mappers.player_num import map_player_num
 from .mappers.player_rank import map_player_rank
 from .parsers.limit_of_games import try_parse_limit_of_games
 from .parsers.time_span import try_parse_time_span
 from ..utils.my_executor import run_in_my_executor
 
+if conf.majsoul_font:
+    plt.rcParams['font.sans-serif'] = conf.majsoul_font
+elif sys.platform == 'win32':
+    plt.rcParams['font.sans-serif'] = "Microsoft YaHei"
+
+if conf.majsoul_font_path:
+    font_manager.fontManager.addfont(conf.majsoul_font_path)
+
 
 def make_handler(player_num: PlayerNum):
     async def majsoul_pt_plot(event: Event):
         args = event.get_message().extract_plain_text().split()
         cmd, args = args[0], args[1:]
 
         if len(args) == 0:
```

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/decode_integer.py` & `nonebot_plugin_majsoul-0.2.0/src/nonebot_plugin_majsoul/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.6/PKG-INFO` & `nonebot_plugin_majsoul-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-majsoul
-Version: 0.1.6
+Version: 0.2.0
 Summary: 
 License: AGPL-3.0
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: icmplib (>=3.0.3,<4.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: monthdelta (>=0.9.1,<0.10.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file (>=0.1.4,<0.2.0)
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: tzlocal (>=4.2,<5.0)
 Description-Content-Type: text/markdown
 
@@ -69,20 +72,64 @@
 
 ![最近对局](img/records.png)
 
 ![最近对局（消息）](img/records_forward.png)
 
 #### 绘制个人PT推移图
 
+**若绘图出现乱码或是需要更换绘图字体，请参考下文进行字体配置**
+
 指令：`/雀魂(三麻)PT图 <雀魂账号> [最近<数量>场] [最近<数量>{天|周|个月|年}]`
 
 ![雀魂PT推移图](img/pt_plot.png)
 
 ![雀魂PT推移图（图）](img/pt_plot_img.png)
 
+#### 下载雀魂牌谱
+
+将雀魂牌谱保存为天凤JSON格式。**必须配置雀魂账号与密码。**
+
+指令：`/下载雀魂牌谱 <牌谱链接或UUID>`
+
+## 配置字体
+
+### 更换为系统已安装字体
+
+修改配置项`majsoul_font`为字体名。
+
+例如：配置`majsoul_font=Microsoft YaHei`将使用微软雅黑字体
+
+### 更换为外部字体
+
+修改配置项`majsoul_font_path`为字体路径，并修改配置项`majsoul_font`为字体名。
+
+例如：在 https://github.com/lxgw/LxgwWenKai-Lite/releases 下载LXGWWenKaiMonoLite-Regular.ttf并放置于bot根目录，配置`majsoul_font_path=LXGWWenKaiMonoLite-Regular.ttf`，配置`majsoul_font=LXGW WenKai Mono Lite`
+
+## 配置项
+
+### majsoul_query_timeout
+
+指令超时（单位：秒）
+
+### majsoul_font
+
+绘图用的字体名称
+
+### majsoul_font_path
+
+绘图用的字体文件路径
+
+### majsoul_username
+
+下载牌谱用的雀魂账号邮箱。推荐使用小号。
+
+### majsoul_password
+
+下载牌谱用的雀魂账号密码。推荐使用小号。
+
 ## See Also
 
 - [nonebot-plugin-mahjong-utils](https://github.com/ssttkkl/nonebot-plugin-mahjong-utils)：日麻小工具插件。支持手牌分析、番符点数查询。
 - [nonebot-plugin-mahjong-scoreboard](https://github.com/ssttkkl/nonebot-plugin-mahjong-scoreboard)
   ：日麻计分器。为面麻群友提供日麻对局分数记录。根据马点进行PT精算，统计PT增减，支持对局与榜单查询与导出。
 
 ## 在线乞讨
```

#### html2text {}

```diff
@@ -1,37 +1,56 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.2.0 Summary:
 License: AGPL-3.0 Author: ssttkkl Author-email: huang.wen.long@hotmail.com
-Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero
+Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-
-Dist: icmplib (>=3.0.3,<4.0.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: monthdelta (>=0.9.1,<0.10.0) Requires-Dist: nonebot-plugin-send-
-anything-anywhere (>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist: typing-extensions
-(>=4.4.0,<5.0.0) Requires-Dist: tzlocal (>=4.2,<5.0) Description-Content-Type:
-text/markdown
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-Dist: icmplib (>=3.0.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0) Requires-Dist: monthdelta
+(>=0.9.1,<0.10.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-gocqhttp-cross-machine-upload-file
+(>=0.1.4,<0.2.0) Requires-Dist: nonebot-plugin-send-anything-anywhere
+(>=0.2.1,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0) Requires-Dist:
+pydantic (>=1.10.2,<2.0.0) Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Requires-Dist: tzlocal (>=4.2,<5.0) Description-Content-Type: text/markdown
                                    [nonebot]
     nonebot-plugin-majsoul ============ _â¨ éé­ä¿¡æ¯æ¥è¯¢æä»¶ â¨_
                            [license] [pypi] [python]
 å[DaiShengSheng/Majsoul_bot](https://github.com/DaiShengSheng/
 Majsoul_bot)å¯åèåçéé­ä¿¡æ¯æ¥è¯¢ Bot æä»¶ã
 æ¯æééå¨ï¼Onebot V11 ## åè½ ### éé­çè°±å± ####
 æ¥è¯¢ä¸ªäººæ°æ®ï¼å¯æç§æ¶é´ãæç§åºæ°ãæç§æ¿é´ç±»åæ¥è¯¢ï¼
 æä»¤ï¼`/éé­(ä¸éº»)ä¿¡æ¯ <éé­è´¦å·> [<æ¿é´ç±»å>]
 [æè¿<æ°é>åº] [æè¿<æ°é>{å¤©|å¨|ä¸ªæ|å¹´}]` ![éé­ä¿¡æ¯](img/
 majsoul_info.png) ![éé­ä¿¡æ¯2](img/majsoul_info_2.png) ####
 æ¥è¯¢ä¸ªäººæè¿å¯¹å±ï¼å¯æç§æ¿é´ç±»åæ¥è¯¢ï¼ æä»¤ï¼`/éé­
 (ä¸éº»)å¯¹å± <éé­è´¦å·> [<æ¿é´ç±»å>]` ![æè¿å¯¹å±](img/
 records.png) ![æè¿å¯¹å±ï¼æ¶æ¯ï¼](img/records_forward.png) ####
-ç»å¶ä¸ªäººPTæ¨ç§»å¾ æä»¤ï¼`/éé­(ä¸éº»)PTå¾ <éé­è´¦å·>
-[æè¿<æ°é>åº] [æè¿<æ°é>{å¤©|å¨|ä¸ªæ|å¹´}]` ![éé­PTæ¨ç§»å¾]
-(img/pt_plot.png) ![éé­PTæ¨ç§»å¾ï¼å¾ï¼](img/pt_plot_img.png) ## See
-Also - [nonebot-plugin-mahjong-utils](https://github.com/ssttkkl/nonebot-
-plugin-mahjong-
+ç»å¶ä¸ªäººPTæ¨ç§»å¾
+**è¥ç»å¾åºç°ä¹±ç ææ¯éè¦æ´æ¢ç»å¾å­ä½ï¼è¯·åèä¸æè¿è¡å­ä½éç½®**
+æä»¤ï¼`/éé­(ä¸éº»)PTå¾ <éé­è´¦å·> [æè¿<æ°é>åº]
+[æè¿<æ°é>{å¤©|å¨|ä¸ªæ|å¹´}]` ![éé­PTæ¨ç§»å¾](img/pt_plot.png) !
+[éé­PTæ¨ç§»å¾ï¼å¾ï¼](img/pt_plot_img.png) #### ä¸è½½éé­çè°±
+å°éé­çè°±ä¿å­ä¸ºå¤©å¤JSONæ ¼å¼ã**å¿é¡»éç½®éé­è´¦å·ä¸å¯ç ã**
+æä»¤ï¼`/ä¸è½½éé­çè°± <çè°±é¾æ¥æUUID>` ## éç½®å­ä½ ###
+æ´æ¢ä¸ºç³»ç»å·²å®è£å­ä½ ä¿®æ¹éç½®é¡¹`majsoul_font`ä¸ºå­ä½åã
+ä¾å¦ï¼éç½®`majsoul_font=Microsoft YaHei`å°ä½¿ç¨å¾®è½¯éé»å­ä½ ###
+æ´æ¢ä¸ºå¤é¨å­ä½
+ä¿®æ¹éç½®é¡¹`majsoul_font_path`ä¸ºå­ä½è·¯å¾ï¼å¹¶ä¿®æ¹éç½®é¡¹`majsoul_font`ä¸ºå­ä½åã
+ä¾å¦ï¼å¨ https://github.com/lxgw/LxgwWenKai-Lite/releases
+ä¸è½½LXGWWenKaiMonoLite-
+Regular.ttfå¹¶æ¾ç½®äºbotæ ¹ç®å½ï¼éç½®`majsoul_font_path=LXGWWenKaiMonoLite-
+Regular.ttf`ï¼éç½®`majsoul_font=LXGW WenKai Mono Lite` ## éç½®é¡¹ ###
+majsoul_query_timeout æä»¤è¶æ¶ï¼åä½ï¼ç§ï¼ ### majsoul_font
+ç»å¾ç¨çå­ä½åç§° ### majsoul_font_path ç»å¾ç¨çå­ä½æä»¶è·¯å¾
+### majsoul_username
+ä¸è½½çè°±ç¨çéé­è´¦å·é®ç®±ãæ¨èä½¿ç¨å°å·ã ###
+majsoul_password ä¸è½½çè°±ç¨çéé­è´¦å·å¯ç ãæ¨èä½¿ç¨å°å·ã
+## See Also - [nonebot-plugin-mahjong-utils](https://github.com/ssttkkl/
+nonebot-plugin-mahjong-
 utils)ï¼æ¥éº»å°å·¥å·æä»¶ãæ¯ææçåæãçªç¬¦ç¹æ°æ¥è¯¢ã -
 [nonebot-plugin-mahjong-scoreboard](https://github.com/ssttkkl/nonebot-plugin-
 mahjong-scoreboard)
 ï¼æ¥éº»è®¡åå¨ãä¸ºé¢éº»ç¾¤åæä¾æ¥éº»å¯¹å±åæ°è®°å½ãæ ¹æ®é©¬ç¹è¿è¡PTç²¾ç®ï¼ç»è®¡PTå¢åï¼æ¯æå¯¹å±ä¸æ¦åæ¥è¯¢ä¸å¯¼åºã
 ## å¨çº¿ä¹è®¨ ç¹å»è¯·ææä¸¤æmaimai ![](https://github.com/ssttkkl/
 ssttkkl/blob/main/afdian-ssttkkl.jfif)  ## LICENSE [AGPLv3](https://
 raw.githubusercontent.com/ssttkkl/nonebot-plugin-majsoul/master/LICENSE)
```

