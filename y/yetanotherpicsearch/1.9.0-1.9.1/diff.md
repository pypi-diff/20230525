# Comparing `tmp/yetanotherpicsearch-1.9.0.tar.gz` & `tmp/yetanotherpicsearch-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetanotherpicsearch-1.9.0.tar", max compression
+gzip compressed data, was "yetanotherpicsearch-1.9.1.tar", max compression
```

## Comparing `yetanotherpicsearch-1.9.0.tar` & `yetanotherpicsearch-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-05-25 16:22:55.945484 yetanotherpicsearch-1.9.0/LICENSE
--rw-r--r--   0        0        0     2041 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/README.md
--rw-r--r--   0        0        0     9488 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ascii2d.py
--rw-r--r--   0        0        0      657 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/baidu.py
--rw-r--r--   0        0        0     2781 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/config.py
--rw-r--r--   0        0        0     5086 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ehentai.py
--rw-r--r--   0        0        0     1089 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/google.py
--rw-r--r--   0        0        0     1959 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/iqdb.py
--rw-r--r--   0        0        0     3132 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/nhentai.py
--rw-r--r--   0        0        0      924 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/nhentai_model.py
--rw-r--r--   0        0        0     6003 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/saucenao.py
--rw-r--r--   0        0        0     6656 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/utils.py
--rw-r--r--   0        0        0     1827 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/whatanime.py
--rw-r--r--   0        0        0      965 2023-05-25 16:22:55.949483 yetanotherpicsearch-1.9.0/YetAnotherPicSearch/yandex.py
--rw-r--r--   0        0        0     1432 2023-05-25 16:22:55.957484 yetanotherpicsearch-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/LICENSE
+-rw-r--r--   0        0        0     2041 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/README.md
+-rw-r--r--   0        0        0     9488 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ascii2d.py
+-rw-r--r--   0        0        0      657 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/baidu.py
+-rw-r--r--   0        0        0     2781 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/config.py
+-rw-r--r--   0        0        0     5086 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ehentai.py
+-rw-r--r--   0        0        0     1195 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/google.py
+-rw-r--r--   0        0        0     1959 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/iqdb.py
+-rw-r--r--   0        0        0     3132 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai.py
+-rw-r--r--   0        0        0      924 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai_model.py
+-rw-r--r--   0        0        0     6003 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/saucenao.py
+-rw-r--r--   0        0        0     6656 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/utils.py
+-rw-r--r--   0        0        0     1827 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/whatanime.py
+-rw-r--r--   0        0        0     1075 2023-05-25 16:43:59.139602 yetanotherpicsearch-1.9.1/YetAnotherPicSearch/yandex.py
+-rw-r--r--   0        0        0     1432 2023-05-25 16:43:59.147602 yetanotherpicsearch-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.1/PKG-INFO
```

### Comparing `yetanotherpicsearch-1.9.0/LICENSE` & `yetanotherpicsearch-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/README.md` & `yetanotherpicsearch-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/__init__.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/__init__.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ascii2d.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ascii2d.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/baidu.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/config.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/config.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/ehentai.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/google.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/google.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from typing import List
 
 from httpx import AsyncClient
 from PicImageSearch import Google
 from PicImageSearch.model import GoogleResponse
 
-from .utils import async_lock
+from .utils import async_lock, get_image_bytes_by_url, shorten_url
 
 
 @async_lock()
-async def google_search(file: bytes, client: AsyncClient) -> List[str]:
+async def google_search(url: str, client: AsyncClient) -> List[str]:
     google = Google(client=client)
-    if res := await google.search(file=file):
+    _file = await get_image_bytes_by_url(url)
+    if res := await google.search(file=_file):
         return await search_result_filter(res)
     return ["Google 暂时无法使用"]
 
 
 async def search_result_filter(
     res: GoogleResponse,
 ) -> List[str]:
+    url = await shorten_url(res.url)
     if not res.raw:
-        return [f"Google 搜索结果为空\n搜索页面：{res.url}"]
+        return [f"Google 搜索结果为空\n搜索页面：{url}"]
 
     selected_res = next((i for i in res.raw if i.thumbnail), res.raw[0])
     if not selected_res.thumbnail:
-        return [f"Google 搜索结果为空\n搜索页面：{res.url}"]
+        return [f"Google 搜索结果为空\n搜索页面：{url}"]
 
     thumbnail = f"[CQ:image,file=base64://{selected_res.thumbnail.split(',', 1)[1]}]"
     res_list = [
         "Google 搜索结果",
         thumbnail,
         selected_res.title,
         f"来源：{selected_res.url}",
-        f"搜索页面：{res.url}",
+        f"搜索页面：{url}",
     ]
     return ["\n".join([i for i in res_list if i])]
```

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/iqdb.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/iqdb.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/nhentai.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/nhentai_model.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/nhentai_model.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/saucenao.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/saucenao.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/utils.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/utils.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/whatanime.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/whatanime.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.0/YetAnotherPicSearch/yandex.py` & `yetanotherpicsearch-1.9.1/YetAnotherPicSearch/yandex.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from typing import List
 
 from httpx import AsyncClient
 from PicImageSearch import Yandex
 from PicImageSearch.model import YandexResponse
 
-from .utils import async_lock, handle_img
+from .utils import async_lock, get_image_bytes_by_url, handle_img, shorten_url
 
 
 @async_lock()
-async def yandex_search(file: bytes, client: AsyncClient) -> List[str]:
+async def yandex_search(url: str, client: AsyncClient) -> List[str]:
     yandex = Yandex(client=client)
-    if res := await yandex.search(file=file):
+    _file = await get_image_bytes_by_url(url)
+    if res := await yandex.search(file=_file):
         return await search_result_filter(res)
     return ["Yandex 暂时无法使用"]
 
 
 async def search_result_filter(
     res: YandexResponse,
 ) -> List[str]:
+    url = await shorten_url(res.url)
     if not res.raw:
-        return [f"Yandex 搜索结果为空\n搜索页面：{res.url}"]
+        return [f"Yandex 搜索结果为空\n搜索页面：{url}"]
 
     thumbnail = await handle_img(res.raw[0].thumbnail)
     res_list = [
         "Yandex 搜索结果",
         thumbnail,
         res.raw[0].size,
         res.raw[0].title,
         res.raw[0].source,
         res.raw[0].content,
         f"来源：{res.raw[0].url}",
-        f"搜索页面：{res.url}",
+        f"搜索页面：{url}",
     ]
     return ["\n".join([i for i in res_list if i])]
```

### Comparing `yetanotherpicsearch-1.9.0/pyproject.toml` & `yetanotherpicsearch-1.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YetAnotherPicSearch"
-version = "1.9.0"
+version = "1.9.1"
 description = "Yet Another Picture Search Nonebot Plugin"
 authors = ["NekoAria"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "YetAnotherPicSearch" },
 ]
```

### Comparing `yetanotherpicsearch-1.9.0/PKG-INFO` & `yetanotherpicsearch-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetanotherpicsearch
-Version: 1.9.0
+Version: 1.9.1
 Summary: Yet Another Picture Search Nonebot Plugin
 Home-page: https://github.com/NekoAria/YetAnotherPicSearch
 License: GPL-3.0-only
 Keywords: nonebot,ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex,anime,danbooru,doujin,pixiv
 Author: NekoAria
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

