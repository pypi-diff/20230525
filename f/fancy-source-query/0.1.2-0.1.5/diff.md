# Comparing `tmp/fancy-source-query-0.1.2.tar.gz` & `tmp/fancy-source-query-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fancy-source-query-0.1.2.tar", last modified: Mon Mar 27 07:48:38 2023, max compression
+gzip compressed data, was "fancy-source-query-0.1.5.tar", last modified: Thu May 25 13:06:55 2023, max compression
```

## Comparing `fancy-source-query-0.1.2.tar` & `fancy-source-query-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-03-25 11:45:15.921299 fancy-source-query-0.1.2/fancy_source_query/__init__.py
--rw-r--r--   0        0        0     3503 2023-03-26 05:28:50.277058 fancy-source-query-0.1.2/fancy_source_query/config.py
--rw-r--r--   0        0        0      208 2023-03-25 15:44:59.982249 fancy-source-query-0.1.2/fancy_source_query/exceptions.py
--rw-r--r--   0        0        0     3206 2023-03-25 15:11:44.121688 fancy-source-query-0.1.2/fancy_source_query/fmt.py
--rw-r--r--   0        0        0      628 2023-03-26 13:39:42.469711 fancy-source-query-0.1.2/fancy_source_query/guess_map.py
--rw-r--r--   0        0        0    10123 2023-03-27 07:43:42.038839 fancy-source-query-0.1.2/fancy_source_query/interfaces/__init__.py
--rw-r--r--   0        0        0     1476 2023-03-26 03:06:53.522999 fancy-source-query-0.1.2/fancy_source_query/interfaces/cli.py
--rw-r--r--   0        0        0     3875 2023-03-27 07:47:18.563742 fancy-source-query-0.1.2/fancy_source_query/interfaces/nonebot.py
--rw-r--r--   0        0        0     4438 2023-03-26 02:12:30.809713 fancy-source-query-0.1.2/fancy_source_query/querypool/__init__.py
--rw-r--r--   0        0        0     2628 2023-03-26 05:20:19.688407 fancy-source-query-0.1.2/fancy_source_query/querypool/infos.py
--rw-r--r--   0        0        0     1988 2023-03-25 16:03:37.683810 fancy-source-query-0.1.2/fancy_source_query/server_group.py
--rw-r--r--   0        0        0      825 2023-03-27 07:47:49.069501 fancy-source-query-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5589 2023-03-26 07:04:45.277512 fancy-source-query-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-03-25 11:52:15.195394 fancy-source-query-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0      927 2023-03-25 15:12:08.712984 fancy-source-query-0.1.2/tests/test_guess_map.py
--rw-r--r--   0        0        0     5762 1970-01-01 00:00:00.000000 fancy-source-query-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5666 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/__init__.py
+-rw-r--r--   0        0        0     3790 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/config.py
+-rw-r--r--   0        0        0      313 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/exceptions.py
+-rw-r--r--   0        0        0     3685 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/fmt.py
+-rw-r--r--   0        0        0      628 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/guess_map.py
+-rw-r--r--   0        0        0    11749 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/interfaces/__init__.py
+-rw-r--r--   0        0        0     1323 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/interfaces/cli.py
+-rw-r--r--   0        0        0     6354 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/interfaces/nonebot.py
+-rw-r--r--   0        0        0     4794 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/querypool/__init__.py
+-rw-r--r--   0        0        0     2935 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/querypool/infos.py
+-rw-r--r--   0        0        0     1988 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/fancy_source_query/server_group.py
+-rw-r--r--   0        0        0      825 2023-05-25 13:05:35.437124 fancy-source-query-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0      892 2023-05-16 06:58:27.696402 fancy-source-query-0.1.5/tests/test_guess_map.py
+-rw-r--r--   0        0        0     5976 1970-01-01 00:00:00.000000 fancy-source-query-0.1.5/PKG-INFO
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/config.py` & `fancy-source-query-0.1.5/fancy_source_query/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pydantic import BaseModel, Extra
 from impaper.config import Config as ImPaperConfig
 
 NONEBOT_CONFIG_KEY = "fancy_source_query_config"
 CONFIG_PATH_PREFIX = "fancy_source_query"
 MAPNAMES_PATH_PREFIX = "mapnames"
 DEFAULT_CONFIG_PATH = "fancy_source_query.toml"
+DEFAULT_MAPNAMES_PATH_OFFICIAL = "officials.toml"
 DEFAULT_MAPNAMES_PATH = "mapnames.toml"
 
 
 class ServerConfig(BaseModel, extra=Extra.ignore):
     "服务器名称、地址"
     group: str
     name: str
@@ -29,30 +30,34 @@
 
 
 class FmtConfig(BaseModel, extra=Extra.ignore):
     "设置格式化模板"
     server_info: str = "{name}\n==({players:>2d}/{max_players:>2d})[{mapname}]"
     player_info: str = ">>[{score}]({minutes:.1f}min){name}"
     rule_info: str = "({key} = {value})"
+    players_count: str = "Players: {players}"
+    query_time: str = "----{time}"
     # strftime 格式符
     time: str = "%Y-%m-%d %H:%M:%S"
 
 
 class FancySourceQueryConfig(BaseModel, extra=Extra.ignore):
     """插件的主要配置"""
 
     # 默认超时等待 5s
     timeout: int = 5
     # 默认查询池缓存 20s
     cache_delay: int = 20
     # 默认限制文本输出 5 行，超过 5 行的转成图片输出
     output_max_lines: int = 5
+    # 一次性随机抽取三方图的最大数量
+    map_choices_max_counts: int = 15
     # Fancy Source Query 可以配置地图数据库，方便将地图代码转换成人类可读的地图名
     # 该路径相对于 nonebot 进程工作目录
-    mapnames_db: str = DEFAULT_MAPNAMES_PATH
+    mapnames_db: list[str] = [DEFAULT_MAPNAMES_PATH_OFFICIAL, DEFAULT_MAPNAMES_PATH]
     # 默认的服务器组，在不传入组名时使用此组
     default_server_group: str
     # 转图片时的字号
     fontsize = 16
 
     impaper: ImPaperConfig
     fmt: FmtConfig
@@ -99,10 +104,11 @@
 
     config = toml.load(config_path)
     config = FancySourceQueryConfig.parse_obj(config[CONFIG_PATH_PREFIX])
     return config
 
 
 class Mapname(BaseModel, extra=Extra.ignore):
+    official: bool = False
     name: str
     name_zh: str | None = None
     maps: list[str]
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/fmt.py` & `fancy-source-query-0.1.5/fancy_source_query/fmt.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 
 def fmt_time(t: float) -> str:
     return strftime("%Y-%m-%d %H:%M:%S", localtime(t))
 
 
 class InfoFormatter:
-    __fmt: FmtConfig
-    __rlookup: dict[str, Mapname]
+    _fmt: FmtConfig
+    _rlookup: dict[str, Mapname]
 
     def __init__(self) -> None:
-        self.__fmt = FmtConfig()
+        self._fmt = FmtConfig()
 
     def config(
         self, fmt: FmtConfig | None = None, rlookup: dict[str, Mapname] | None = None
     ):
         if fmt:
             logging.debug("updated InfoFormatter's config.")
-            self.__fmt = fmt
+            self._fmt = fmt
         if rlookup:
             logging.debug("updated InfoFormatter's map rlookup.")
-            self.__rlookup = rlookup
+            self._rlookup = rlookup
 
     def format(
         self, info: ServerInfo | PlayerInfo | RuleInfo | ServerPair | ServerTriple
     ) -> str:
         "通用的格式化方法，会判断传入类型并具体分配实际方法"
         if isinstance(info, ServerInfo):
             return self.fmt_server_info(info)
@@ -39,32 +39,38 @@
             return self.fmt_player_info(info)
         elif isinstance(info, RuleInfo):
             return self.fmt_rule_info(info)
         elif isinstance(info, ServerTriple):
             return self.fmt_server_triple(info)
 
     def fmt_server_info(self, info: ServerInfo) -> str:
-        fmt = self.__fmt.server_info.format(
+        code = info.map
+        name = self.guess_map(code)
+        if name:
+            mapname = f"{name}|{code}"
+        else:
+            mapname = code
+        fmt = self._fmt.server_info.format(
             name=info.name,
             players=info.players,
             max_players=info.max_players,
-            mapname=self.guess_map(info.map),
+            mapname=mapname,
         )
         return fmt
 
     def fmt_player_info(self, info: PlayerInfo) -> str:
-        fmt = self.__fmt.player_info.format(
+        fmt = self._fmt.player_info.format(
             name=info.name,
             minutes=info.duration / 60,
             score=info.score,
         )
         return fmt
 
     def fmt_rule_info(self, info: RuleInfo) -> str:
-        fmt = self.__fmt.rule_info.format(
+        fmt = self._fmt.rule_info.format(
             key=info.name,
             value=info.value,
         )
         return fmt
 
     def fmt_server_pair(self, info: ServerPair) -> str:
         sfmt = self.fmt_server_info(info.server)
@@ -76,17 +82,26 @@
         sfmt = self.fmt_server_info(info.server)
         sorted_p = sorted(info.players, key=lambda x: x.score, reverse=True)
         pfmt = [self.fmt_player_info(p) for p in sorted_p]
         sorted_r = sorted(info.rules, key=lambda x: x.name)
         rfmt = [self.fmt_rule_info(r) for r in sorted_r]
         return "{}\n{}\n{}".format(sfmt, "\n".join(pfmt), "\n".join(rfmt))
 
-    def guess_map(self, code: str) -> str:
-        "除了 guess map 之外还需要完成格式化任务 name|code"
-        name = guess_map(self.__rlookup, code)
+    def guess_map(self, code: str) -> str | None:
+        "如果能查询到则返回对应名称，否则返回 None"
+        name = guess_map(self._rlookup, code)
         if name:
-            return f"{name}|{code}"
+            return name
         else:
-            return code
+            return None
+
+    def fmt_players_count(self, p: int) -> str:
+        "格式化总人数统计"
+        return self._fmt.players_count.format(players=p)
 
     def fmt_time(self, t: float) -> str:
-        return strftime(self.__fmt.time, localtime(t))
+        return strftime(self._fmt.time, localtime(t))
+
+    def fmt_query_time(self, t: float) -> str:
+        "和 fmt_time 的区别在于，这个函数生成显示样式的时间"
+        ttime = self.fmt_time(t)
+        return self._fmt.query_time.format(time=ttime)
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/guess_map.py` & `fancy-source-query-0.1.5/fancy_source_query/guess_map.py`

 * *Files identical despite different names*

### Comparing `fancy-source-query-0.1.2/fancy_source_query/interfaces/__init__.py` & `fancy-source-query-0.1.5/fancy_source_query/interfaces/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,48 @@
 
 此接口导出一个 FancySourceQuery 对象，其成员函数提供了对应的功能。
 """
 import asyncio
 import logging
 import re
 import socket
+from typing import Literal
 
 import toml
+from pydantic import BaseModel
+
+from impaper.draw import TextDrawer
 
 from ..config import MAPNAMES_PATH_PREFIX, FancySourceQueryConfig, Mapname, load_config
 from ..exceptions import ObjectNotFound
 from ..fmt import InfoFormatter
 from ..guess_map import build_rlookup
 from ..querypool import QueryPool
 from ..querypool.infos import PlayerInfo, ServerInfo, ServerPair
 from ..server_group import Server, ServerGroup, build_server_group_graph
-from impaper.draw import TextDrawer
 
 WHITESPACE = re.compile("[ \u2002\u2003]")
 
 
+class QueryResult(BaseModel):
+    """查询结果
+
+    + tag : 查询类型，一共有一下几种：
+        + o : overview
+        + s : only server
+        + sp : server and players
+        + spm : server and players multi
+        + p : search player
+    """
+    tag: Literal["o", "s", "sp", "spm", "p"]
+    # query time
+    qtime: float
+    result: None | list[ServerPair] | list[ServerInfo] | ServerPair | ServerInfo
+
+
 class FancySourceQuery:
     """面向 Python 的 Fancy Source Query 接口，各方法返回 对象 而非文本。
     格式化为文本是 cli 或 nonebot 接口的工作。
 
     + `update_config` : 刷新配置项（本体配置、服务器组配置）
     + `update_mapnames` : 刷新地图名反查表
     + `find_server` : 在指定的服务器组中根据名称寻找服务器
@@ -75,16 +94,19 @@
         self.qstr_pat_server_name = re.compile(f"^(?:{all_server_names})$")
         socket.setdefaulttimeout(self.config.timeout)
         if self.t2g is not None:
             self.t2g.conf = self.config.impaper
             self.t2g.fontsize = self.config.fontsize
 
     def update_mapnames(self):
-        mapnames = toml.load(self.config.mapnames_db)
-        self.mapnames = [Mapname.parse_obj(x) for x in mapnames[MAPNAMES_PATH_PREFIX]]
+        mapnames_lists = [toml.load(i) for i in self.config.mapnames_db]
+        mapnames_list = []
+        for ml in mapnames_lists:
+            mapnames_list.extend(ml[MAPNAMES_PATH_PREFIX])
+        self.mapnames = [Mapname.parse_obj(x) for x in mapnames_list]
         self.map_rlookup = build_rlookup(self.mapnames)
         self.ifmt.config(rlookup=self.map_rlookup)
         logging.debug("mapnames refreshed")
 
     def find_server(self, sname: str, gname: str | None) -> Server:
         """在指定的服务器组中寻找服务器"""
         group = self.find_group(gname)
@@ -94,46 +116,48 @@
             raise ObjectNotFound("server in group not found", gname, sname)
         return server
 
     def find_group(self, gname: str | None) -> ServerGroup:
         """根据组名寻找服务器组"""
         if gname is None:
             gname = self.config.default_server_group
-            logging.info("use default server group {gname!r}.")
+            logging.info(f"use default server group {gname!r}.")
         group = self.server_group.get(gname, None)
         if group is None:
             logging.error(f"server group {gname!r} not found.")
             raise ObjectNotFound("server group not found", gname)
         return group
 
     async def query_server(
         self, sname: str, gname: str | None
-    ) -> tuple[float, ServerInfo]:
+    ) -> QueryResult:
         """根据服务器组和服务器的名称查询服务器信息，返回查询时间 和 Server Info"""
         server = self.find_server(sname, gname)
         host, port = server.host, server.port
         qtime, sinfo = await self.query_pool.server_info(host, port)
-        return qtime, sinfo
+        r = QueryResult(tag="s", qtime=qtime, result=sinfo)
+        return r
 
     async def query_server_and_players(
         self, sname: str, gname: str | None
-    ) -> tuple[float, ServerPair]:
+    ) -> QueryResult:
         """根据服务器组和服务器的名称查询服务器信息和玩家信息，
         返回查询时间 和 ServerPair"""
         server = self.find_server(sname, gname)
         host, port = server.host, server.port
         qtime1, sinfo = await self.query_pool.server_info(host, port)
         qtime2, pinfo = await self.query_pool.players_info(host, port)
         spair = ServerPair(server=sinfo, players=pinfo)
         qtime = max(qtime1, qtime2)
-        return qtime, spair
+        r = QueryResult(tag="sp", qtime=qtime, result=spair)
+        return r
 
     async def query_server_and_players_multi(
         self, snames: list[str], gname: str | None
-    ) -> tuple[float, list[ServerPair]]:
+    ) -> QueryResult:
         """查询多个服务器的信息和玩家信息，返回最晚查询时间和 list[ServerPair]"""
         servers = []
         for sname in snames:
             try:
                 servers.append(self.find_server(sname, gname))
             except ObjectNotFound:
                 logging.warning("object not found, but skiped.")
@@ -146,35 +170,37 @@
             *(self.query_pool.players_info(s.host, s.port) for s in servers)
         )
         qtime = max([r[0] for r in sinfos] + [r[0] for r in pinfos])
         pairs = sorted(
             [ServerPair(server=r[0][1], players=r[1][1]) for r in zip(sinfos, pinfos)],
             key=lambda pair: pair.server.name,
         )
-        return qtime, pairs
+        r = QueryResult(tag="spm", qtime=qtime, result=pairs)
+        return r
 
     async def query_servers_overview(
         self, gname: str | None
-    ) -> tuple[float, list[ServerInfo]]:
+    ) -> QueryResult:
         """查询某服务器组内的服务器信息，返回最晚查询时间和 `list[ServerInfo]`
 
         + `sgroup` 服务器组名
         """
         group = self.find_group(gname)
         servers = sorted(group.servers.values(), key=lambda s: s.name)
         results = await asyncio.gather(
             *[self.query_pool.server_info(s.host, s.port) for s in servers]
         )
         qtime = max(r[0] for r in results)
         sinfos = [r[1] for r in results]
-        return qtime, sinfos
+        r = QueryResult(tag="o", qtime=qtime, result=sinfos)
+        return r
 
     async def search_player(
         self, player_regex: str, gname: str | None
-    ) -> tuple[float, list[ServerPair] | None]:
+    ) -> QueryResult:
         """在某个组中查找某些玩家，只要玩家名中含有 `player` 的片段，
         便会认为是查找目标。
         返回最晚查询时间和相关的服务器与玩家信息。
         如果未找到则返回无意义的时间戳和None。
         """
         group = self.find_group(gname)
         servers = sorted(group.servers.values(), key=lambda s: s.name)
@@ -199,26 +225,25 @@
                 if pat.search(WHITESPACE.sub("", p.name)):
                     qtime = max(qtime, qt)
                     if i not in occursins:
                         occursins[i] = [p]
                     else:
                         occursins[i].append(p)
         if len(occursins) == 0:
-            return qtime, None
+            return QueryResult(tag="p", qtime=qtime, result=None)
         pairs = sorted(
             (ServerPair(server=total[i][1], players=p) for (i, p) in occursins.items()),
             key=lambda pair: pair.server.name,
         )
-        return (qtime, pairs)
+        r = QueryResult(tag="p", qtime=qtime, result=pairs)
+        return r
 
     async def query(
         self, gname: str | None, qstr: str
-    ) -> tuple[
-        float, None | list[ServerPair] | list[ServerInfo] | ServerPair | ServerInfo
-    ]:
+    ) -> QueryResult:
         """根据 qstr 内容进行查询：
 
         1. qstr 是空字符串或“人数” - 调用 `query_servers_overview`
         2. qstr 是已知的服务器名 - 调用 `query_server_and_players`
         3. qstr 是空格分隔的服务器名 - 调用 `query_server_and_players_multi`
         4. qstr 是其它情况 - 调用 `search_player`
         """
@@ -244,7 +269,35 @@
         return self.session_group.get(session, None)
 
     def lazy_load_t2g(self, t2g: TextDrawer):
         """需要时再加载"""
         self.t2g = t2g
         self.t2g.conf = self.config.impaper
         self.t2g.fontsize = self.config.fontsize
+
+
+async def fmt_qresult(fsq: FancySourceQuery, r: QueryResult, qstr: str) -> str:
+    if r.tag == "p" and r.result is None:
+        if r.result is None:
+            return f"【{qstr}】不在哦~😥"
+
+    body = []
+    if isinstance(r.result, list):
+        body.extend(fsq.ifmt.format(r) for r in r.result)
+    else:
+        body.append(fsq.ifmt.format(r.result))
+    body.append("\n")
+    if isinstance(r.result, list):
+        players = 0
+        for rr in r.result:
+            if r.tag == "p":
+                players += len(rr.players)
+            elif isinstance(rr, ServerPair):
+                players += rr.server.players
+            elif isinstance(rr, ServerInfo):
+                players += rr.players
+        tplayers = fsq.ifmt.fmt_players_count(players)
+        body.append(tplayers)
+    ttime = fsq.ifmt.fmt_query_time(r.qtime)
+    body.append(ttime)
+    text = "\n".join(body)
+    return text
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/interfaces/cli.py` & `fancy-source-query-0.1.5/fancy_source_query/interfaces/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 + interfaces: Python 接口
 """
 import asyncio
 import os
 from argparse import ArgumentParser
 from pathlib import Path
 
-from . import FancySourceQuery
+from . import FancySourceQuery, QueryResult, fmt_qresult
 
 
 def cli_parser():
     """命令行工具不提供刷新配置的功能"""
     p = ArgumentParser(
         prog="fsq",
         usage="query source server's info",
@@ -32,21 +32,18 @@
     # 是否修改工作目录
     if args.c:
         cwd = Path(args.c).absolute().as_posix()
         os.chdir(cwd)
     app = FancySourceQuery()
     gname = args.GROUP
     qstr = args.QSTR
-    qtime, result = await app.query(gname, qstr)
-    if result is None:
-        print("Error: 无查询结果")
-    if isinstance(result, list):
-        fmts = "\n".join(app.ifmt.format(r) for r in result)
-    else:
-        fmts = app.ifmt.format(result)
-    ttime = app.ifmt.fmt_time(qtime)
-    text = f"{fmts}\n\n----{ttime}"
+    qresult: QueryResult = await app.query(gname, qstr)
+    text = await fmt_qresult(app, qresult, qstr)
     print(text)
 
 
 def cli_main():
     asyncio.run(cli_main_async())
+
+
+if __name__ == "__main__":
+    cli_main()
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/querypool/__init__.py` & `fancy-source-query-0.1.5/fancy_source_query/querypool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """包装 Valve 的 A2S API"""
 import logging
 from time import time
 
 import fancy_source_query.fmt as fmt
 
-from ..exceptions import QueryTimeout
+from ..exceptions import QueryTimeout, ServerRestarting
 from .infos import PlayerInfo, ServerInfo, players_info, server_info
 
 
 class QueryPool:
     """缓存查询结果
 
     (host, port) => (timestamp, value)
@@ -71,14 +71,23 @@
                 name="超时",
                 players=0,
                 max_players=0,
                 map="unknown",
                 vac=False,
                 ping=0.0,
             )
+        except ServerRestarting:
+            return querytime, ServerInfo(
+                name="换图或重启",
+                players=0,
+                max_players=0,
+                map="unknown",
+                vac=False,
+                ping=0.0,
+            )
         logging.debug(f"new server query({fmt.fmt_time(querytime)}) {sinfo!r}")
         self.__server_cache[(host, port)] = (querytime, sinfo)
         return (querytime, sinfo)
 
     async def players_info(
         self, host: str, port: int
     ) -> tuple[float, list[PlayerInfo]]:
@@ -110,10 +119,13 @@
         如果超时，则返回超时信息，但不计入缓存。
         """
         querytime = time()
         try:
             pinfo = await players_info(host, port)
         except QueryTimeout:
             return querytime, []
+        except ServerRestarting:
+            return querytime, []
+
         logging.debug(f"new players query({fmt.fmt_time(querytime)}) {pinfo!r}")
         self.__players_cache[(host, port)] = (querytime, pinfo)
         return (querytime, pinfo)
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/querypool/infos.py` & `fancy-source-query-0.1.5/fancy_source_query/querypool/infos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import socket
 from typing import Any
 from pydantic import BaseModel
 
 from steam.game_servers import a2s_info, a2s_players, a2s_rules
 
-from ..exceptions import QueryTimeout
+from ..exceptions import QueryTimeout, ServerRestarting
 
 
 class PlayerInfo(BaseModel):
     name: str
     score: int
     duration: float
     index: int
@@ -57,14 +57,16 @@
     + vac: 是否开启 VAC
     + ping: 本机与服务器的延迟
     """
     try:
         info = a2s_info(server_addr=(host, port))
     except socket.timeout:
         raise QueryTimeout({"host": host, "port": port})
+    except ConnectionRefusedError:
+        raise ServerRestarting({"host": host, "port": port})
 
     info_ = {
         "name": info["name"],
         "players": info["players"],
         "max_players": info["max_players"],
         "map": info["map"],
         "vac": True if info["vac"] == 1 else False,
@@ -87,14 +89,16 @@
     + score: 分数
     + name: 名称
     """
     try:
         info = a2s_players(server_addr=(host, port))
     except socket.timeout:
         raise QueryTimeout({"host": host, "port": port})
+    except ConnectionRefusedError:
+        raise ServerRestarting({"host": host, "port": port})
 
     logging.debug(f"new players info query to {host}:{port}")
     return sorted([PlayerInfo(**i) for i in info], key=lambda o: -o.score)
 
 
 async def rules_info(host: str, port: int) -> list[RuleInfo]:
     """查询服务器的规则
@@ -102,8 +106,11 @@
     + name: 规则名称
     + value: 值
     """
     try:
         info = a2s_rules(server_addr=(host, port))
     except socket.timeout:
         raise QueryTimeout({"host": host, "port": port})
+    except ConnectionRefusedError:
+        raise ServerRestarting({"host": host, "port": port})
+
     return [RuleInfo(**i) for i in info]
```

### Comparing `fancy-source-query-0.1.2/fancy_source_query/server_group.py` & `fancy-source-query-0.1.5/fancy_source_query/server_group.py`

 * *Files identical despite different names*

### Comparing `fancy-source-query-0.1.2/pyproject.toml` & `fancy-source-query-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "fancy_source_query"
-version = "0.1.2"
+version = "0.1.5"
 description = "Intelligent tool to query source servers, with a cli interface and plugin integrates into nonebot."
 authors = [
     { name = "zombie110year", email = "zombie110year@outlook.com" },
 ]
 dependencies = [
     "nonebot2[fastapi]>=2.0.0rc3",
     "steam[client]>=1.4.4",
     "pydantic>=1.10.7",
-    "impaper>=0.1.3",
+    "impaper>=0.1.6",
     "exrex>=0.11.0",
     "toml>=0.10.2",
     "nonebot-adapter-onebot>=2.2.2",
 ]
 requires-python = ">=3.10,<4.0"
 readme = "README.md"
```

### Comparing `fancy-source-query-0.1.2/README.md` & `fancy-source-query-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,137 +1,144 @@
-# Nonebot plugin fancy source query
-
-这个插件的目的是将 Source Server Query 的功能集成进 Nonebot 框架中，
-以便使用者方便地实现查询 Valve Source 服务器状态的查询。
-并且默认实现了将较长的查询结果转换成图片输出的功能，以免刷屏
-（此功能仅在 QQ 上测试）。
-
-
-## 功能介绍
-
-FancySourceQuery(以下简称FSQ) 插件可以查询 Source 服务器的名称、人数、正在运行的地图和服务器内玩家的详细状态。
-提供以下指令：
-
-1. 查询：查询当前服务器组的概况（所有服务器名称、当前人数、最大玩家数、地图名称）并统计总人数
-2. 查询人数：同上
-3. 查询（服务器名）：当输入的参数不为空或“人数”时，机器人优先将其认作服务器的名称，将会从当前服务器中寻找对应的服务器，
-    查询服务器的状态和详细的玩家状态
-4. 查询（玩家名）：当输入的参数不为空或“人数”或已知的服务器名时，机器人会将其认作玩家的名称片段，将会从当前服务器组里的所有服务器中搜索玩家名匹配的玩家信息（输入参数被当作正则表达式处理，并且匹配标准是 `re.search`）
-5. 刷新配置：此功能仅 SUPERUSER 可用，可让机器人在不停机的情况下重新加载配置文件
-6. 刷新地图数据：此功能仅 SUPERUSER 可用，可让机器人在不停机的情况下重新加载地图数据
-
-该插件的所有功能都提供 Python 接口或命令行接口，可以在不启动 Nonebot 的情况下执行，以便调试。
-
-+ Python 接口为 `fancy_source_query.interfaces:FancySourceQuery` 此对象的所有方法都返回适合 Python 处理的对象
-+ Cli 接口在 `fancy_source_query.interfaces.cli:cli_main` 此方法提供了命令行的程序调用
-+ nonebot 接口在 `fancy_source_query.interfaces.nonebot` 此模块中定义了 Nonebot 响应函数，只支持 Onebot v11 程序
-
-## 相关文件
-
-运行时，你的项目文件夹下必须有这两个文件：
-
-1. `fancy_source_query.toml` ： 默认的配置文件
-2. `mapnames.toml` ： 默认的地图数据文件，其中储存了地图的原名、中文名、地图代码，以便插件生成对应的反查表
-
-文件内容可以查看仓库中的示例，其中 `mapnames.toml` 文件在另一地址有随时更新的版本 （TODO）
-
-## 安装
-
-将此插件添加到 Nonebot 项目的依赖中，可以使用 nb-cli 或者 pdm, poetry, pip 等
-包管理工具安装。
-
-例如：
-
-```sh
-pdm add fancy_source_query
-```
-
-然后在 `pyproject.toml` 中配置：
-
-```toml
-[tool.nonebot]
-plugins = [
-    # ...
-    "fancy_source_query.interfaces.nonebot",
-    # ...
-]
-```
-
-## 配置
-
-此插件的配置分为两个部分，一个是 NoneBot 的 Env 配置文件，另一个（主要的）是 toml 格式的配置。
-
-```env
-FANCY_SOURCE_QUERY_CONFIG="fancy_source_query.toml"
-```
-
-env 配置中只需要指定插件配置文件的路径，默认为 nonebot 进程工作目录下的 `fancy_source_query.toml` 文件。
-以下为默认的配置模板与解释：
-
-```toml
-[fancy_source_query]
-# 默认超时等待 5s
-timeout = 5
-# 默认查询池缓存 20s
-cache_delay = 20
-# 默认限制文本输出 5 行，超过 5 行的转成图片输出
-output_max_lines = 5
-# Fancy Source Query 可以配置地图数据库，方便将地图代码转换成人类可读的地图名
-# 该路径相对于 nonebot 进程工作目录
-mapnames_db = "mapnames.toml"
-# 默认的服务器组，在不传入组名时使用此组
-default_server_group = "A"
-# 转图片时的字号，px
-fontsize = 16
-
-[fancy_source_query.impaper]
-# 建议留空，加载默认的更纱黑体，
-# 或者指定一个 ttf 文件的路径。
-# font.path =
-[fancy_source_query.impaper.layout]
-# 外边距，按上右下左的顺序（和 CSS 里的习惯一致），px
-# 右边距建议拉大一点，防止手机上看时像素被遮住
-margin = [6, 6, 18, 6]
-# 内边距，按上右下左的顺序（和 CSS 里的习惯一致），px
-padding = [2, 2, 2, 2]
-# 行间距，px
-spacing = 2
-
-# 格式化查询数据的模板
-[fancy_source_query.fmt]
-server_info = "{name}\n==({players:>2d}/{max_players:>2d})[{mapname}]"
-player_info = ">>[{score}]({minutes:.1f}min){name}"
-rule_info = "({key} = {value})"
-# strftime 格式符
-time = "%Y-%m-%d %H:%M:%S"
-
-# Fancy Source Query 可以为不同的 QQ 群设置不同的服务器组
-# 为不同的群分别提供查询服务，例如为 A 群配置服务器组 AG, 其中包含服务器 A1, A2, A3；
-# 为 B 群配置服务器组 BG，其中包含服务器 B1, B2, B3；
-# 为 开发者测试群 配置服务器组 DEVG，其中包含所有服务器；
-# 那么机器人在 A 群中查询时只会考虑 A1, A2, A3 服务器，以此类推。
-[[fancy_source_query.server_groups]]
-name = "A"
-related_sessions = ["<QQ群号A>", "<开发者测试群>"]
-[[fancy_source_query.server_groups]]
-name = "B"
-related_sessions = ["<QQ群号B>", "<开发者测试群>"]
-
-[[fancy_source_query.servers]]
-# 此处的 A 需要与 server_group.name 相同
-group = "A"
-name = "A1"
-host = "127.0.0.1"
-port = 65501
-[[fancy_source_query.servers]]
-group = "A"
-name = "A2"
-host = "127.0.0.1"
-port = 65502
-[[fancy_source_query.servers]]
-group = "B"
-name = "B1"
-host = "127.0.0.1"
-port = 64501
-```
-
-在修改完配置文件后，可以通过 SUPERUSER 账号向机器人发送 "刷新" 指令，以热重载配置和数据。
+# Nonebot plugin fancy source query
+
+这个插件的目的是将 Source Server Query 的功能集成进 Nonebot 框架中，
+以便使用者方便地实现查询 Valve Source 服务器状态的查询。
+并且默认实现了将较长的查询结果转换成图片输出的功能，以免刷屏
+（此功能仅在 QQ 上测试）。
+
+
+## 功能介绍
+
+FancySourceQuery(以下简称FSQ) 插件可以查询 Source 服务器的名称、人数、正在运行的地图和服务器内玩家的详细状态。
+提供以下指令：
+
+1. 查询：查询当前服务器组的概况（所有服务器名称、当前人数、最大玩家数、地图名称）并统计总人数
+2. 查询人数：同上
+3. 查询（服务器名）：当输入的参数不为空或“人数”时，机器人优先将其认作服务器的名称，将会从当前服务器中寻找对应的服务器，
+    查询服务器的状态和详细的玩家状态
+4. 查询（玩家名）：当输入的参数不为空或“人数”或已知的服务器名时，机器人会将其认作玩家的名称片段，将会从当前服务器组里的所有服务器中搜索玩家名匹配的玩家信息（输入参数被当作正则表达式处理，并且匹配标准是 `re.search`）
+5. 刷新配置：此功能仅 SUPERUSER 可用，可让机器人在不停机的情况下重新加载配置文件
+6. 刷新地图数据：此功能仅 SUPERUSER 可用，可让机器人在不停机的情况下重新加载地图数据
+
+该插件的所有功能都提供 Python 接口或命令行接口，可以在不启动 Nonebot 的情况下执行，以便调试。
+
++ Python 接口为 `fancy_source_query.interfaces:FancySourceQuery` 此对象的所有方法都返回适合 Python 处理的对象
++ Cli 接口在 `fancy_source_query.interfaces.cli:cli_main` 此方法提供了命令行的程序调用
++ nonebot 接口在 `fancy_source_query.interfaces.nonebot` 此模块中定义了 Nonebot 响应函数，只支持 Onebot v11 程序
+
+## 相关文件
+
+运行时，你的项目文件夹下必须有这两个文件：
+
+1. `fancy_source_query.toml` ： 默认的配置文件
+2. `mapnames.toml` ： 默认的地图数据文件，其中储存了地图的原名、中文名、地图代码，以便插件生成对应的反查表
+
+文件内容可以查看仓库中的示例，其中 `mapnames.toml` 文件在另一地址有随时更新的版本 （TODO）
+
+## 安装
+
+将此插件添加到 Nonebot 项目的依赖中，可以使用 nb-cli 或者 pdm, poetry, pip 等
+包管理工具安装。
+
+例如：
+
+```sh
+pdm add fancy_source_query
+```
+
+然后在 `pyproject.toml` 中配置：
+
+```toml
+[tool.nonebot]
+plugins = [
+    # ...
+    "fancy_source_query.interfaces.nonebot",
+    # ...
+]
+```
+
+## 配置
+
+此插件的配置分为两个部分，一个是 NoneBot 的 Env 配置文件，另一个（主要的）是 toml 格式的配置。
+
+```env
+FANCY_SOURCE_QUERY_CONFIG="fancy_source_query.toml"
+```
+
+env 配置中只需要指定插件配置文件的路径，默认为 nonebot 进程工作目录下的 `fancy_source_query.toml` 文件。
+以下为默认的配置模板与解释：
+
+```toml
+[fancy_source_query]
+# 默认超时等待 5s
+timeout = 5
+# 默认查询池缓存 20s
+cache_delay = 20
+# 默认限制文本输出 5 行，超过 5 行的转成图片输出
+output_max_lines = 5
+# Fancy Source Query 可以配置地图数据库，方便将地图代码转换成人类可读的地图名
+# 该路径相对于 nonebot 进程工作目录
+mapnames_db = "mapnames.toml"
+# 默认的服务器组，在不传入组名时使用此组
+default_server_group = "A"
+# 转图片时的字号，px
+fontsize = 16
+
+[fancy_source_query.impaper]
+# 建议留空，加载默认的更纱黑体，
+# 或者指定一个 ttf 文件的路径。
+# font.path =
+[fancy_source_query.impaper.layout]
+# 外边距，按上右下左的顺序（和 CSS 里的习惯一致），px
+# 右边距建议拉大一点，防止手机上看时像素被遮住
+margin = [6, 6, 18, 6]
+# 内边距，按上右下左的顺序（和 CSS 里的习惯一致），px
+padding = [2, 2, 2, 2]
+# 行间距，px
+spacing = 2
+[fancy_source_query.impaper.typesetting]
+# 行宽，英文1，汉字2
+line_width = 52
+# 折行缩进
+indentation = "  "
+
+# 格式化查询数据的模板
+[fancy_source_query.fmt]
+server_info = "服务器：{name}\n概况：({players:>2d}/{max_players:>2d})[{mapname}]"
+player_info = "[{score}]({minutes:.1f}min){name}"
+rule_info = "({key} = {value})"
+players_count = "总人数：{players}"
+query_time = "查询时间：{time}"
+# strftime 格式符
+time = "%Y-%m-%d %H:%M:%S"
+
+# Fancy Source Query 可以为不同的 QQ 群设置不同的服务器组
+# 为不同的群分别提供查询服务，例如为 A 群配置服务器组 AG, 其中包含服务器 A1, A2, A3；
+# 为 B 群配置服务器组 BG，其中包含服务器 B1, B2, B3；
+# 为 开发者测试群 配置服务器组 DEVG，其中包含所有服务器；
+# 那么机器人在 A 群中查询时只会考虑 A1, A2, A3 服务器，以此类推。
+[[fancy_source_query.server_groups]]
+name = "A"
+related_sessions = ["<QQ群号A>", "<开发者测试群>"]
+[[fancy_source_query.server_groups]]
+name = "B"
+related_sessions = ["<QQ群号B>", "<开发者测试群>"]
+
+[[fancy_source_query.servers]]
+# 此处的 A 需要与 server_group.name 相同
+group = "A"
+name = "A1"
+host = "127.0.0.1"
+port = 65501
+[[fancy_source_query.servers]]
+group = "A"
+name = "A2"
+host = "127.0.0.1"
+port = 65502
+[[fancy_source_query.servers]]
+group = "B"
+name = "B1"
+host = "127.0.0.1"
+port = 64501
+```
+
+在修改完配置文件后，可以通过 SUPERUSER 账号向机器人发送 "刷新" 指令，以热重载配置和数据。
```

### Comparing `fancy-source-query-0.1.2/tests/test_guess_map.py` & `fancy-source-query-0.1.5/tests/test_guess_map.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import pytest
-import toml
-
-from fancy_source_query.config import (
-    DEFAULT_MAPNAMES_PATH,
-    MAPNAMES_PATH_PREFIX,
-    Mapname,
-)
-from fancy_source_query.guess_map import build_rlookup, guess_map
-from fancy_source_query.interfaces import FancySourceQuery
-
-
-@pytest.fixture(scope="session", autouse=True)
-def rlookup():
-    mapnames = toml.load(DEFAULT_MAPNAMES_PATH)
-    mapnames = [Mapname.parse_obj(x) for x in mapnames[MAPNAMES_PATH_PREFIX]]
-    return build_rlookup(mapnames)
-
-
-@pytest.fixture(scope="session", autouse=True)
-def fsquery():
-    x = FancySourceQuery()
-    return x
-
-
-def test_c1m1(rlookup: dict[str, Mapname]):
-    code = "c1m1_hotel"
-    name = guess_map(rlookup, code)
-    assert name == "死亡中心"
-
-
-def test_fsquery_guess_map(fsquery: FancySourceQuery):
-    code = "c1m1_hotel"
-    name = fsquery.ifmt.guess_map(code)
-    assert name == f"死亡中心|{code}"
+import pytest
+import toml
+
+from fancy_source_query.config import (
+    DEFAULT_MAPNAMES_PATH,
+    MAPNAMES_PATH_PREFIX,
+    Mapname,
+)
+from fancy_source_query.guess_map import build_rlookup, guess_map
+from fancy_source_query.interfaces import FancySourceQuery
+
+
+@pytest.fixture(scope="session", autouse=True)
+def rlookup():
+    mapnames = toml.load(DEFAULT_MAPNAMES_PATH)
+    mapnames = [Mapname.parse_obj(x) for x in mapnames[MAPNAMES_PATH_PREFIX]]
+    return build_rlookup(mapnames)
+
+
+@pytest.fixture(scope="session", autouse=True)
+def fsquery():
+    x = FancySourceQuery()
+    return x
+
+
+def test_c1m1(rlookup: dict[str, Mapname]):
+    code = "c1m1_hotel"
+    name = guess_map(rlookup, code)
+    assert name == "死亡中心"
+
+
+def test_fsquery_guess_map(fsquery: FancySourceQuery):
+    code = "c1m1_hotel"
+    name = fsquery.ifmt.guess_map(code)
+    assert name == f"死亡中心|{code}"
```

### Comparing `fancy-source-query-0.1.2/PKG-INFO` & `fancy-source-query-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fancy_source_query
-Version: 0.1.2
+Version: 0.1.5
 Summary: Intelligent tool to query source servers, with a cli interface and plugin integrates into nonebot.
 License: MIT
 Author-email: zombie110year <zombie110year@outlook.com>
 Requires-Python: >=3.10,<4.0
 Description-Content-Type: text/markdown
 
 # Nonebot plugin fancy source query
@@ -100,20 +100,27 @@
 # 外边距，按上右下左的顺序（和 CSS 里的习惯一致），px
 # 右边距建议拉大一点，防止手机上看时像素被遮住
 margin = [6, 6, 18, 6]
 # 内边距，按上右下左的顺序（和 CSS 里的习惯一致），px
 padding = [2, 2, 2, 2]
 # 行间距，px
 spacing = 2
+[fancy_source_query.impaper.typesetting]
+# 行宽，英文1，汉字2
+line_width = 52
+# 折行缩进
+indentation = "  "
 
 # 格式化查询数据的模板
 [fancy_source_query.fmt]
-server_info = "{name}\n==({players:>2d}/{max_players:>2d})[{mapname}]"
-player_info = ">>[{score}]({minutes:.1f}min){name}"
+server_info = "服务器：{name}\n概况：({players:>2d}/{max_players:>2d})[{mapname}]"
+player_info = "[{score}]({minutes:.1f}min){name}"
 rule_info = "({key} = {value})"
+players_count = "总人数：{players}"
+query_time = "查询时间：{time}"
 # strftime 格式符
 time = "%Y-%m-%d %H:%M:%S"
 
 # Fancy Source Query 可以为不同的 QQ 群设置不同的服务器组
 # 为不同的群分别提供查询服务，例如为 A 群配置服务器组 AG, 其中包含服务器 A1, A2, A3；
 # 为 B 群配置服务器组 BG，其中包含服务器 B1, B2, B3；
 # 为 开发者测试群 配置服务器组 DEVG，其中包含所有服务器；
```

