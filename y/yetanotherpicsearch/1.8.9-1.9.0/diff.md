# Comparing `tmp/yetanotherpicsearch-1.8.9.tar.gz` & `tmp/yetanotherpicsearch-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetanotherpicsearch-1.8.9.tar", max compression
+gzip compressed data, was "yetanotherpicsearch-1.9.0.tar", max compression
```

## Comparing `yetanotherpicsearch-1.8.9.tar` & `yetanotherpicsearch-1.9.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/LICENSE
--rw-r--r--   0        0        0     1915 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/README.md
--rw-r--r--   0        0        0    10163 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/__init__.py
--rw-r--r--   0        0        0     2069 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/ascii2d.py
--rw-r--r--   0        0        0      678 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/baidu.py
--rw-r--r--   0        0        0     2775 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/config.py
--rw-r--r--   0        0        0     5557 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/ehentai.py
--rw-r--r--   0        0        0     1955 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/iqdb.py
--rw-r--r--   0        0        0     3544 2023-03-22 08:40:09.244647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/nhentai.py
--rw-r--r--   0        0        0     5967 2023-03-22 08:40:09.248647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/saucenao.py
--rw-r--r--   0        0        0     5008 2023-03-22 08:40:09.248647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/utils.py
--rw-r--r--   0        0        0     1807 2023-03-22 08:40:09.248647 yetanotherpicsearch-1.8.9/YetAnotherPicSearch/whatanime.py
--rw-r--r--   0        0        0     1358 2023-03-22 08:40:09.256647 yetanotherpicsearch-1.8.9/pyproject.toml
--rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.8.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-25 16:22:55.945484 yetanotherpicsearch-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2041 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/README.md
+-rw-r--r--   0        0        0     9488 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ascii2d.py
+-rw-r--r--   0        0        0      657 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/baidu.py
+-rw-r--r--   0        0        0     2781 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/config.py
+-rw-r--r--   0        0        0     5086 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ehentai.py
+-rw-r--r--   0        0        0     1089 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/google.py
+-rw-r--r--   0        0        0     1959 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/iqdb.py
+-rw-r--r--   0        0        0     3132 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/nhentai.py
+-rw-r--r--   0        0        0      924 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/nhentai_model.py
+-rw-r--r--   0        0        0     6003 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/saucenao.py
+-rw-r--r--   0        0        0     6656 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/utils.py
+-rw-r--r--   0        0        0     1827 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/whatanime.py
+-rw-r--r--   0        0        0      965 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/yandex.py
+-rw-r--r--   0        0        0     1432 2023-05-25 16:22:55.957484 yetanotherpicsearch-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.0/PKG-INFO
```

### Comparing `yetanotherpicsearch-1.8.9/LICENSE` & `yetanotherpicsearch-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.8.9/README.md` & `yetanotherpicsearch-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 
 ## 项目简介
 
 主要受到 [cq-picsearcher-bot](https://github.com/Tsuk1ko/cq-picsearcher-bot) 的启发。我只需要基础的搜图功能，于是忍不住自己也写了一个，用来搜图、搜番、搜本子。
 
 目前支持的搜图服务：
 
-- [SauceNAO](https://saucenao.com)
-- [Ascii2D](https://ascii2d.net)
-- [Iqdb](https://iqdb.org)
-- [E-Hentai](https://e-hentai.org)
-- [WhatAnime](https://trace.moe)
+- [Ascii2D](https://ascii2d.net/)
 - [Baidu](https://graph.baidu.com/)
+- [E-Hentai](https://e-hentai.org/)
+- [ExHentai](https://exhentai.org/)
+- [Google](https://www.google.com/imghp)
+- [Iqdb](https://iqdb.org/)
+- [SauceNAO](https://saucenao.com/)
+- [TraceMoe](https://trace.moe/)
+- [Yandex](https://yandex.com/images/search)
 
 目前适配的是 `OneBot V11` ，没适配 QQ 频道。
 
 此外，还有使用体验更好的 Telegram 移植版： [YetAnotherPicSearch4Telegram](https://github.com/NekoAria/YetAnotherPicSearch4Telegram)
 
 ## 文档目录
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/__init__.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import asyncio
 import re
-from collections import defaultdict
 from contextlib import suppress
-from typing import Any, DefaultDict, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple
 
-import arrow
-from aiohttp import ClientSession
 from cachetools import TTLCache
+from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import (
     ActionFailed,
     Bot,
     GroupMessageEvent,
     LifecycleMetaEvent,
     Message,
     MessageEvent,
@@ -24,26 +21,25 @@
 from shelved_cache import PersistentCache
 from tenacity import retry, stop_after_attempt, stop_after_delay
 
 from .ascii2d import ascii2d_search
 from .baidu import baidu_search
 from .config import config
 from .ehentai import ehentai_search
+from .google import google_search
 from .iqdb import iqdb_search
 from .saucenao import saucenao_search
 from .utils import (
     DEFAULT_HEADERS,
     SEARCH_FUNCTION_TYPE,
     get_bot_friend_list,
     handle_reply_msg,
 )
+from .yandex import yandex_search
 
-sending_lock: DefaultDict[Tuple[Union[int, str], str], asyncio.Lock] = defaultdict(
-    asyncio.Lock
-)
 pic_search_cache = PersistentCache(
     TTLCache,
     filename="pic_search_cache",
     maxsize=config.cache_expire * 100,
     ttl=config.cache_expire * 24 * 60 * 60,
 )
 
@@ -92,15 +88,15 @@
 async def image_search(
     bot: Bot,
     event: MessageEvent,
     url: str,
     md5: str,
     mode: str,
     purge: bool,
-    client: ClientSession,
+    client: AsyncClient,
     index: Optional[int] = None,
 ) -> None:
     url = await get_universal_img_url(url)
     cache_key = f"{md5}_{mode}"
     try:
         if not purge and cache_key in pic_search_cache:
             result, extra_handle = pic_search_cache[cache_key]
@@ -120,26 +116,30 @@
     except Exception as e:
         logger.exception(f"该图 [{url}] 搜图失败")
         await send_result_message(bot, event, [f"该图搜图失败\nE: {repr(e)}"], index)
 
 
 @retry(stop=(stop_after_attempt(3) | stop_after_delay(30)), reraise=True)
 async def handle_search_mode(
-    url: str, md5: str, mode: str, client: ClientSession
+    url: str, md5: str, mode: str, client: AsyncClient
 ) -> Tuple[List[str], Optional[SEARCH_FUNCTION_TYPE]]:
     extra_handle = None
 
     if mode == "a2d":
         result = await ascii2d_search(url, client)
+    elif mode == "baidu":
+        result = await baidu_search(url, client)
     elif mode == "ex":
         result, extra_handle = await ehentai_search(url, client)
+    elif mode == "google":
+        result = await google_search(url, client)
     elif mode == "iqdb":
         result, extra_handle = await iqdb_search(url, client)
-    elif mode == "baidu":
-        result = await baidu_search(url, client)
+    elif mode == "yandex":
+        result = await yandex_search(url, client)
     else:
         result, extra_handle = await saucenao_search(url, client, mode)
 
     pic_search_cache[f"{md5}_{mode}"] = result, extra_handle
 
     return result, extra_handle
 
@@ -147,18 +147,18 @@
 async def get_universal_img_url(url: str) -> str:
     if re.match("^https?://(c2cpicdw|gchat).qpic.cn/(offpic|gchatpic)_new/", url):
         final_url = url.replace(
             "/c2cpicdw.qpic.cn/offpic_new/", "/gchat.qpic.cn/gchatpic_new/"
         )
         final_url = re.sub(r"/\d+/+\d+-\d+-", "/0/0-0-", final_url)
         final_url = re.sub(r"\?.*$", "", final_url)
-        async with ClientSession(headers=DEFAULT_HEADERS) as session:
-            async with session.get(final_url) as resp:
-                if resp.status < 400:
-                    return final_url
+        async with AsyncClient(headers=DEFAULT_HEADERS) as session:
+            resp = await session.get(final_url)
+            if resp.status_code < 400:
+                return final_url
     return url
 
 
 def get_image_urls_with_md5(event: MessageEvent) -> List[Tuple[str, str]]:
     message = event.reply.message if event.reply else event.message
     return [
         (i.data["url"], str(i.data["file"]).rstrip(".image").upper())
@@ -166,15 +166,26 @@
         if i.type == "image" and i.data.get("url")
     ]
 
 
 def get_args(msg: Message) -> Tuple[str, bool]:
     mode = "all"
     plain_text = msg.extract_plain_text().strip()
-    args = ["pixiv", "danbooru", "doujin", "anime", "a2d", "ex", "iqdb", "baidu"]
+    args = [
+        "a2d",
+        "anime",
+        "baidu",
+        "danbooru",
+        "doujin",
+        "ex",
+        "google",
+        "iqdb",
+        "pixiv",
+        "yandex",
+    ]
     if plain_text:
         for i in args:
             if f"--{i}" in plain_text:
                 mode = i
                 break
     purge = "--purge" in plain_text
     return mode, purge
@@ -187,45 +198,22 @@
         isinstance(event, PrivateMessageEvent)
         and event.user_id == int(list(config.superusers)[0])
     ):
         msg_list = [
             msg.replace("❤️ 已收藏\n", "") if "已收藏" in msg else msg for msg in msg_list
         ]
 
-    if isinstance(event, GroupMessageEvent):
-        current_sending_lock = sending_lock[(event.group_id, "group")]
-    else:
-        current_sending_lock = sending_lock[(event.user_id, "private")]
-
     if flag := (config.forward_search_result and len(msg_list) > 1):
         try:
-            await send_message_with_lock(
-                bot, event, msg_list, current_sending_lock, index
-            )
+            await send_forward_msg(bot, event, msg_list, index)
         except ActionFailed:
             flag = False
     if not flag:
         for msg in msg_list:
-            await send_message_with_lock(bot, event, [msg], current_sending_lock, index)
-
-
-async def send_message_with_lock(
-    bot: Bot,
-    event: MessageEvent,
-    msg_list: List[str],
-    current_sending_lock: asyncio.Lock,
-    index: Optional[int] = None,
-) -> None:
-    start_time = arrow.now()
-    async with current_sending_lock:
-        if len(msg_list) == 1:
-            await send_msg(bot, event, msg_list[0], index)
-        else:
-            await send_forward_msg(bot, event, msg_list, index)
-        await asyncio.sleep(max(1 - (arrow.now() - start_time).total_seconds(), 0))
+            await send_msg(bot, event, msg, index)
 
 
 async def send_msg(
     bot: Bot, event: MessageEvent, message: str, index: Optional[int] = None
 ) -> None:
     if index is not None:
         message = f"第 {index + 1} 张图片的搜索结果：\n{message}"
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/ascii2d.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ascii2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import List
 
-from aiohttp import ClientSession
+from httpx import AsyncClient
 from PicImageSearch import Ascii2D
 from PicImageSearch.model import Ascii2DResponse
 
 from .config import config
-from .utils import get_image_bytes_by_url, handle_img, shorten_url
+from .utils import async_lock, get_image_bytes_by_url, handle_img, shorten_url
 
 
-async def ascii2d_search(url: str, client: ClientSession) -> List[str]:
+@async_lock()
+async def ascii2d_search(url: str, client: AsyncClient) -> List[str]:
     ascii2d_color = Ascii2D(client=client)
     _file = await get_image_bytes_by_url(url)
     color_res = await ascii2d_color.search(file=_file)
     if not color_res.raw:
         return ["Ascii2D 暂时无法使用"]
 
     resp_text, resp_url, _ = await ascii2d_color.get(
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/baidu.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/baidu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import List
 
-from aiohttp import ClientSession
+from httpx import AsyncClient
 from PicImageSearch import BaiDu
 
-from .utils import handle_img, shorten_url
+from .utils import async_lock, handle_img, shorten_url
 
 
-async def baidu_search(url: str, client: ClientSession) -> List[str]:
+@async_lock()
+async def baidu_search(url: str, client: AsyncClient) -> List[str]:
     baidu = BaiDu(client=client)
     res = await baidu.search(url)
     _url = await shorten_url(res.url)
     if not res.raw:
         return [f"Baidu 搜索结果为空\n搜索页面：{_url}"]
     thumbnail = await handle_img(res.raw[0].thumbnail)
     res_list = [
-        f"Baidu ({res.raw[0].similarity}%)",
+        "Baidu 搜索结果",
         thumbnail,
-        res.raw[0].title,
         res.raw[0].url,
         f"搜索页面：{_url}",
     ]
     return ["\n".join([i for i in res_list if i])]
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/config.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     saucenao_nsfw_hide_level: int = 0
     # saucenao 相似度低于这个百分比将被认定为相似度过低
     saucenao_low_acc: int = 60
     # 是否在 saucenao 或 iqdb 相似度过低时 / ehentai 无结果时 自动使用 ascii2d
     auto_use_ascii2d: bool = True
     # 若结果消息有多条，采用合并转发方式发送搜图结果
     forward_search_result: bool = True
-    # 大部分请求所使用的代理: http / socks4 / socks5
+    # 大部分请求所使用的代理: http / socks4(a) / socks5(h)
     proxy: Optional[str] = None
     # saucenao 搜图结果缓存过期时间 (天)
     cache_expire: int = 3
     # saucenao APIKEY，必填，否则无法使用 saucenao 搜图
     saucenao_api_key: str
     # exhentai cookies，选填，没有的情况下自动改用 e-hentai 搜图
     exhentai_cookies: Optional[str] = None
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/ehentai.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ehentai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,76 @@
 import itertools
 import re
-from asyncio import sleep
 from collections import defaultdict
-from difflib import SequenceMatcher
 from typing import Any, Dict, List, Optional, Tuple
 
 import arrow
-from aiohttp import ClientSession
+from httpx import AsyncClient
 from PicImageSearch import EHentai
 from PicImageSearch.model import EHentaiResponse
 from pyquery import PyQuery
 
 from .ascii2d import ascii2d_search
 from .config import config
 from .utils import (
     DEFAULT_HEADERS,
     SEARCH_FUNCTION_TYPE,
-    get_session_with_proxy,
+    async_lock,
+    filter_results_with_ratio,
     handle_img,
+    parse_cookies,
+    preprocess_search_query,
     shorten_url,
 )
 
-EHENTAI_HEADERS = (
-    {"Cookie": config.exhentai_cookies, **DEFAULT_HEADERS}
-    if config.exhentai_cookies
-    else DEFAULT_HEADERS
-)
-
 
+@async_lock(freq=8)
 async def ehentai_search(
-    url: str, client: ClientSession
+    url: str, client: AsyncClient
 ) -> Tuple[List[str], Optional[SEARCH_FUNCTION_TYPE]]:
     ex = bool(config.exhentai_cookies)
     ehentai = EHentai(client=client)
 
     if res := await ehentai.search(url, ex=ex):
         if "Please wait a bit longer between each file search" in res.origin:
-            await sleep(30 / 4)
             return await ehentai_search(url, client)
 
-        if not res.raw:
-            # 如果第一次没找到，使搜索结果包含被删除的部分，并重新搜索
-            resp_text, resp_url, _ = await ehentai.get(f"{res.url}&fs_exp=on")
-            res = EHentaiResponse(resp_text, resp_url)
         final_res: List[str] = await search_result_filter(res)
-
         if not res.raw and config.auto_use_ascii2d:
             final_res.append("自动使用 Ascii2D 进行搜索")
             return final_res, ascii2d_search
 
         return final_res, None
 
     return ["EHentai 暂时无法使用"], None
 
 
 async def ehentai_title_search(title: str) -> List[str]:
-    title = re.sub(r"●|~| ::: |[中国翻訳]", " ", title).strip()
+    query = preprocess_search_query(title)
     url = "https://exhentai.org" if config.exhentai_cookies else "https://e-hentai.org"
-    params: Dict[str, Any] = {"f_search": title}
+    params: Dict[str, Any] = {"f_search": query}
 
-    async with get_session_with_proxy(headers=EHENTAI_HEADERS) as session:
+    async with AsyncClient(
+        headers=DEFAULT_HEADERS,
+        cookies=parse_cookies(config.exhentai_cookies),
+        proxies=config.proxy,
+    ) as session:
         resp = await session.get(url, params=params)
-        if res := EHentaiResponse(await resp.text(), str(resp.url)):
+        if res := EHentaiResponse(resp.text, str(resp.url)):
             if not res.raw:
                 # 如果第一次没找到，使搜索结果包含被删除的部分，并重新搜索
                 params["advsearch"] = 1
                 params["f_sname"] = "on"
                 params["f_sh"] = "on"
                 resp = await session.get(url, params=params)
-                res = EHentaiResponse(await resp.text(), str(resp.url))
+                res = EHentaiResponse(resp.text, str(resp.url))
 
             # 只保留标题和搜索关键词相关度较高的结果，并排序，以此来提高准确度
             if res.raw:
-                raw_with_ratio = [
-                    (i, SequenceMatcher(lambda x: x == " ", title, i.title).ratio())
-                    for i in res.raw
-                ]
-                raw_with_ratio.sort(key=lambda x: x[1], reverse=True)
-                if filtered := [i[0] for i in raw_with_ratio if i[1] > 0.65]:
-                    res.raw = filtered
-                else:
-                    res.raw = [i[0] for i in raw_with_ratio]
+                res.raw = filter_results_with_ratio(res, title)
             return await search_result_filter(res)
 
         return ["EHentai 暂时无法使用"]
 
 
 async def search_result_filter(
     res: EHentaiResponse,
@@ -99,19 +85,21 @@
     ]:
         res.raw = not_expunged_res
 
     # 尝试过滤无主题的杂图图集
     if not_themeless_res := [i for i in res.raw if "themeless" not in " ".join(i.tags)]:
         res.raw = not_themeless_res
 
-    # 尝试过滤评分只有 1 星的
-    if not_1_star_res := [
-        i for i in res.raw if ("-64px" not in PyQuery(i.origin)("div.ir").attr("style"))
+    # 尝试过滤评分低于 3 星的
+    if above_3_star_res := [
+        i
+        for i in res.raw
+        if get_star_rating(PyQuery(i.origin)("div.ir").attr("style")) >= 3
     ]:
-        res.raw = not_1_star_res
+        res.raw = above_3_star_res
 
     # 尽可能过滤掉非预期结果(大概
     priority = defaultdict(lambda: 0)
     priority["Image Set"] = 1
     priority["Non-H"] = 2
     priority["Western"] = 3
     priority["Misc"] = 4
@@ -150,7 +138,15 @@
         "❤️ 已收藏" if favorited else "",
         f"类型：{selected_res.type}",
         f"日期：{date}",
         f"来源：{selected_res.url}",
         f"搜索页面：{url}",
     ]
     return ["\n".join([i for i in res_list if i])]
+
+
+def get_star_rating(css_style: str) -> float:
+    x, y = re.search(r"(-?\d+)px (-\d+)px", css_style).groups()  # type: ignore
+    star_rating = 5 - int(x.rstrip("px")) / -16
+    if y == "-21px":
+        star_rating -= 0.5
+    return star_rating
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/iqdb.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/iqdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Optional, Tuple
 
-from aiohttp import ClientSession
+from httpx import URL, AsyncClient
 from PicImageSearch import Iqdb
-from yarl import URL
 
 from .ascii2d import ascii2d_search
 from .config import config
-from .utils import SEARCH_FUNCTION_TYPE, get_source, handle_img, shorten_url
+from .utils import SEARCH_FUNCTION_TYPE, async_lock, get_source, handle_img, shorten_url
 
 
+@async_lock()
 async def iqdb_search(
-    url: str, client: ClientSession
+    url: str, client: AsyncClient
 ) -> Tuple[List[str], Optional[SEARCH_FUNCTION_TYPE]]:
     iqdb = Iqdb(client=client)
     res = await iqdb.search(url)
     if not res.raw:
         return ["Iqdb 暂时无法使用，自动使用 Ascii2D 进行搜索"], ascii2d_search
 
     final_res: List[str] = []
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/saucenao.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/saucenao.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import re
-from asyncio import sleep
 from typing import List, Optional, Tuple
 
-from aiohttp import ClientSession
+from httpx import URL, AsyncClient
 from PicImageSearch import SauceNAO
 from PicImageSearch.model import SauceNAOItem, SauceNAOResponse
-from yarl import URL
 
 from .ascii2d import ascii2d_search
 from .config import config
 from .ehentai import ehentai_title_search
 from .nhentai import nhentai_title_search
-from .utils import SEARCH_FUNCTION_TYPE, get_source, handle_img, shorten_url
+from .utils import SEARCH_FUNCTION_TYPE, async_lock, get_source, handle_img, shorten_url
 from .whatanime import whatanime_search
 
 SAUCENAO_DB = {
     "all": 999,
     "pixiv": 5,
     "danbooru": 9,
     "anime": [21, 22],
     "doujin": [18, 38],
     "fakku": 16,
 }
 
 
+@async_lock(freq=8)
 async def saucenao_search(
-    url: str, client: ClientSession, mode: str
+    url: str, client: AsyncClient, mode: str
 ) -> Tuple[List[str], Optional[SEARCH_FUNCTION_TYPE]]:
     db = SAUCENAO_DB[mode]
     if isinstance(db, list):
         saucenao = SauceNAO(
             client=client,
             api_key=config.saucenao_api_key,
             hide=config.saucenao_nsfw_hide_level,
@@ -45,15 +44,14 @@
     res = await saucenao.search(url)
 
     if (
         res
         and res.status == 429
         and "4 searches every 30 seconds" in res.origin["header"]["message"]
     ):
-        await sleep(30 / 4)
         return await saucenao_search(url, client, mode)
 
     if not res or not res.raw:
         final_res = ["SauceNAO 暂时无法使用，自动使用 Ascii2D 进行搜索"]
         return final_res, ascii2d_search
 
     selected_res = get_best_result(res, res.raw[0])
@@ -152,16 +150,17 @@
     title_search_result = await ehentai_title_search(title)
 
     if (
         title_search_result[0].startswith("EHentai 搜索结果为空")
         and config.nhentai_useragent
         and config.nhentai_cookies
     ):
-        title_search_result.append("自动使用 NHentai 进行搜索")
-        title_search_result.extend(await nhentai_title_search(title))
+        nhentai_title_search_result = await nhentai_title_search(title)
+        if not nhentai_title_search_result[0].startswith("NHentai 搜索结果为空"):
+            title_search_result = nhentai_title_search_result
 
     return title_search_result
 
 
 async def handle_saucenao_low_acc(
     mode: str, selected_res: SauceNAOItem
 ) -> Tuple[List[str], Optional[SEARCH_FUNCTION_TYPE]]:
```

### Comparing `yetanotherpicsearch-1.8.9/YetAnotherPicSearch/whatanime.py` & `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/whatanime.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import math
 from typing import Any, Dict, List
 
-from aiohttp import ClientSession
+from httpx import AsyncClient
 from PicImageSearch import TraceMoe
 
 from .config import config
-from .utils import handle_img
+from .utils import async_lock, handle_img
 
 
-async def whatanime_search(url: str, client: ClientSession) -> List[str]:
+@async_lock()
+async def whatanime_search(url: str, client: AsyncClient) -> List[str]:
     whatanime = TraceMoe(client=client)
     res = await whatanime.search(url)
     if res and res.raw:
         time = res.raw[0].From
         minutes = math.floor(time / 60)
         seconds = math.floor(time % 60)
         time_str = f"{minutes:02d}:{seconds:02d}"
```

### Comparing `yetanotherpicsearch-1.8.9/pyproject.toml` & `yetanotherpicsearch-1.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "YetAnotherPicSearch"
-version = "1.8.9"
+version = "1.9.0"
 description = "Yet Another Picture Search Nonebot Plugin"
 authors = ["NekoAria"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "YetAnotherPicSearch" },
 ]
 homepage = "https://github.com/NekoAria/YetAnotherPicSearch"
 repository = "https://github.com/NekoAria/YetAnotherPicSearch"
-keywords = ["nonebot", "saucenao", "pixiv", "danbooru", "doujin", "anime", "ascii2d", "iqdb", "exhentai"]
+keywords = ["nonebot", "ascii2d", "baidu", "e-hentai", "google", "iqdb", "saucenao", "tracemoe", "yandex", "anime", "danbooru", "doujin", "pixiv"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-aiohttp = {extras = ["speedups"], version = "^3.8.4"}
-aiohttp_socks = { version = "^0.8.0", optional = true }
 arrow = "^1.2.3"
 cachetools = "^5.3.0"
+httpx = "^0.24.1"
 lxml = "^4.9.2"
-nonebot-adapter-onebot = "^2.2.2"
-nonebot2 = "^2.0.0-rc.3"
-PicImageSearch = "^3.7.8"
-pydantic = "^1.10.6"
+nonebot-adapter-onebot = "^2.2.3"
+nonebot2 = "^2.0.0-rc.4"
+PicImageSearch = "^3.9.2"
+pydantic = "^1.10.7"
 pyquery = "^2.0.0"
+python-socks = {extras = ["asyncio"], version = "^2.2.0", optional = true}
+socksio = { version = "^1.0.0", optional = true }
 shelved-cache = "^0.3.1"
 tenacity = "^8.2.2"
-yarl = "^1.8.2"
 
 [tool.poetry.extras]
-socks = ["aiohttp_socks"]
+socks = ["python-socks", "socksio"]
 
 [tool.poetry.dev-dependencies]
 
 [tool.mypy]
 python_version = "3.8"
 plugins = [
     "pydantic.mypy"
@@ -41,15 +41,15 @@
 ignore_missing_imports = true
 implicit_reexport = true
 pretty = true
 show_error_codes = true
 strict = true
 
 [tool.ruff]
-select = ["F", "E", "W", "I"]
+select = ["F", "E", "W", "I", "UP"]
 target-version = "py38"
 line-length = 120
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [build-system]
```

### Comparing `yetanotherpicsearch-1.8.9/PKG-INFO` & `yetanotherpicsearch-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: yetanotherpicsearch
-Version: 1.8.9
+Version: 1.9.0
 Summary: Yet Another Picture Search Nonebot Plugin
 Home-page: https://github.com/NekoAria/YetAnotherPicSearch
 License: GPL-3.0-only
-Keywords: nonebot,saucenao,pixiv,danbooru,doujin,anime,ascii2d,iqdb,exhentai
+Keywords: nonebot,ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex,anime,danbooru,doujin,pixiv
 Author: NekoAria
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: socks
-Requires-Dist: PicImageSearch (>=3.7.8,<4.0.0)
-Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
-Requires-Dist: aiohttp_socks (>=0.8.0,<0.9.0) ; extra == "socks"
+Requires-Dist: PicImageSearch (>=3.9.2,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-rc.3,<3.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0-rc.4,<3.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyquery (>=2.0.0,<3.0.0)
+Requires-Dist: python-socks[asyncio] (>=2.2.0,<3.0.0) ; extra == "socks"
 Requires-Dist: shelved-cache (>=0.3.1,<0.4.0)
+Requires-Dist: socksio (>=1.0.0,<2.0.0) ; extra == "socks"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
-Requires-Dist: yarl (>=1.8.2,<2.0.0)
 Project-URL: Repository, https://github.com/NekoAria/YetAnotherPicSearch
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # YetAnotherPicSearch
 
@@ -44,20 +44,23 @@
 
 ## 项目简介
 
 主要受到 [cq-picsearcher-bot](https://github.com/Tsuk1ko/cq-picsearcher-bot) 的启发。我只需要基础的搜图功能，于是忍不住自己也写了一个，用来搜图、搜番、搜本子。
 
 目前支持的搜图服务：
 
-- [SauceNAO](https://saucenao.com)
-- [Ascii2D](https://ascii2d.net)
-- [Iqdb](https://iqdb.org)
-- [E-Hentai](https://e-hentai.org)
-- [WhatAnime](https://trace.moe)
+- [Ascii2D](https://ascii2d.net/)
 - [Baidu](https://graph.baidu.com/)
+- [E-Hentai](https://e-hentai.org/)
+- [ExHentai](https://exhentai.org/)
+- [Google](https://www.google.com/imghp)
+- [Iqdb](https://iqdb.org/)
+- [SauceNAO](https://saucenao.com/)
+- [TraceMoe](https://trace.moe/)
+- [Yandex](https://yandex.com/images/search)
 
 目前适配的是 `OneBot V11` ，没适配 QQ 频道。
 
 此外，还有使用体验更好的 Telegram 移植版： [YetAnotherPicSearch4Telegram](https://github.com/NekoAria/YetAnotherPicSearch4Telegram)
 
 ## 文档目录
```

