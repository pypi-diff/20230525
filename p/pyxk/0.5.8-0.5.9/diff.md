# Comparing `tmp/pyxk-0.5.8.tar.gz` & `tmp/pyxk-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.8.tar", last modified: Tue May 23 04:41:28 2023, max compression
+gzip compressed data, was "pyxk-0.5.9.tar", last modified: Thu May 25 09:12:20 2023, max compression
```

## Comparing `pyxk-0.5.8.tar` & `pyxk-0.5.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.8/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-23 04:41:28.367688 pyxk-0.5.8/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.8/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.357688 pyxk-0.5.8/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    18325 2023-05-22 03:35:48.000000 pyxk-0.5.8/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/m3u8downloader/
--rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/m3u8downloader/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3391 2023-05-23 04:31:51.000000 pyxk-0.5.8/pyxk/m3u8downloader/enter_point.py
--rw-rw----   0 root         (0) everybody  (9997)     4907 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/m3u8downloader/m3u8download.py
--rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/m3u8downloader/m3u8parse.py
--rw-rw----   0 root         (0) everybody  (9997)    11879 2023-05-23 04:35:40.000000 pyxk-0.5.8/pyxk/m3u8downloader/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.367688 pyxk-0.5.8/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3502 2023-05-23 04:20:34.000000 pyxk-0.5.8/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    15210 2023-05-23 04:29:24.000000 pyxk-0.5.8/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-14 14:04:32.000000 pyxk-0.5.8/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-23 04:41:28.357688 pyxk-0.5.8/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-23 04:41:28.000000 pyxk-0.5.8/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-23 04:41:28.367688 pyxk-0.5.8/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-23 04:41:14.000000 pyxk-0.5.8/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.693999 pyxk-0.5.9/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.9/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-25 09:12:20.693999 pyxk-0.5.9/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.9/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.673999 pyxk-0.5.9/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      491 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.683999 pyxk-0.5.9/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    19056 2023-05-25 04:45:25.000000 pyxk-0.5.9/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      615 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.683999 pyxk-0.5.9/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3633 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4695 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.683999 pyxk-0.5.9/pyxk/m3u8downloader/
+-rw-rw----   0 root         (0) everybody  (9997)       66 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3391 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/enter_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     4907 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/m3u8download.py
+-rw-rw----   0 root         (0) everybody  (9997)     2968 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/m3u8parse.py
+-rw-rw----   0 root         (0) everybody  (9997)    11879 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/m3u8downloader/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.693999 pyxk-0.5.9/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      247 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     7480 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3502 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    15235 2023-05-24 06:43:11.000000 pyxk-0.5.9/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    19033 2023-05-23 04:42:38.000000 pyxk-0.5.9/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-25 09:12:20.673999 pyxk-0.5.9/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      345 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      627 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       99 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-25 09:12:20.000000 pyxk-0.5.9/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-25 09:12:20.693999 pyxk-0.5.9/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      927 2023-05-25 09:11:55.000000 pyxk-0.5.9/setup.py
```

### Comparing `pyxk-0.5.8/LICENSE` & `pyxk-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/aclient/client.py` & `pyxk-0.5.9/pyxk/aclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 )
 from pyxk.utils import (
     chardet,
     LazyLoader,
     get_user_agent,
     default_headers,
 )
-
+_copy = LazyLoader("_copy", globals(), "copy")
 _yarl = LazyLoader("_yarl", globals(), "yarl")
 _selector = LazyLoader("_selector", globals(), "parsel.selector")
 aiohttp_client_exceptions = LazyLoader("aiohttp_client_exceptions", globals(), "aiohttp.client_exceptions")
 
 __all__ = ["Client"]
 
 
 
 class Client:
     """异步下载器 - 类变量
 
     :params: limit: aiohttp 并发控制
     :params: timeout: 请求超时时间
+    :params: req_kwargs: start_request请求参数
     :params: async_sleep: 异步休眠时间
     :params: maximum_retry: 异步请求最大重试次数
     :params: headers: 请求头
     :params: semaphore: asyncio 并发控制
     :params: verify: ssl验证
     :params: start_urls: 请求入口urls
     :params: user_agnet: User-Agent
@@ -60,14 +61,15 @@
 
     :params: base_url: base_url
     :params: **kwargs: 关键字 实例化参数
     """
 
     limit: Optional[int] = None
     timeout: Timeout = None
+    req_kwargs: Optional[dict] = None
     async_sleep: Optional[int] = None
     maximum_retry: Optional[int] = None
     headers: Optional[Union[dict, CIMDict]] = None
     semaphore: Union[Optional[int], asyncio.Semaphore] = None
     verify: Optional[bool] = None
     start_urls: Union[List[str], List[Tuple[str, dict]]] = []
     user_agent: Optional[str] = None
@@ -86,15 +88,15 @@
         ("maximum_retry", 20),
         ("user_agent", get_user_agent()),
         ("aiohttp_kwargs", {}),
         ("until_request_succeed", False),
     )
 
     def __init__(self, *, base_url: StrOrURL=None, **kwargs):
-        """Client init
+        """__init__
 
         :params: base_url: base_url
         :params: **kwargs: 关键字 实例化参数
         """
         for key, val in kwargs.items():
             setattr(self, key, val)
         # event loop
@@ -133,45 +135,57 @@
                 asyncio.set_event_loop(self._loop)
             # semaphore
             if not isinstance(self.semaphore, (int, float)) or self.semaphore < 0:
                 self.semaphore = dict(self.attr)["semaphore"]
             self.semaphore = asyncio.Semaphore(self.semaphore)
             # aiohttp kwargs
             aiohttp_kwargs = self.aiohttp_kwargs \
-                if isinstance(self.aiohttp_kwargs, dict) else dict(self.attr)["aiohttp_kwargs"]
-            aiohttp_kwargs = aiohttp_kwargs.copy()
+                if isinstance(self.aiohttp_kwargs, dict) \
+                else dict(self.attr)["aiohttp_kwargs"]
+            aiohttp_kwargs = _copy.deepcopy(aiohttp_kwargs)
             # timeout
             if not aiohttp_kwargs.__contains__("timeout"):
                 if not isinstance(self.timeout, aiohttp.ClientTimeout):
                     timeout = aiohttp.ClientTimeout(
                         total = self.timeout \
-                            if isinstance(self.timeout, (int, float)) and self.timeout > 0 else dict(self.attr)["timeout"]
+                            if isinstance(self.timeout, (int, float)) and self.timeout > 0 \
+                            else dict(self.attr)["timeout"]
                     )
                 else:
                     timeout = self.timeout
                 aiohttp_kwargs["timeout"] = timeout
             # connector
             if not aiohttp_kwargs.__contains__("connector"):
                 aiohttp_kwargs["connector"] = aiohttp.TCPConnector(
                     loop = self._loop,
                     limit = self.limit \
-                        if isinstance(self.limit, int) and self.limit > 0 else dict(self.attr)["limit"],
-                    ssl = bool(self.verify) if self.verify is not None else dict(self.attr)["verify"],
+                        if isinstance(self.limit, int) and self.limit > 0 \
+                        else dict(self.attr)["limit"],
+                    ssl = bool(self.verify) \
+                        if self.verify is not None \
+                        else dict(self.attr)["verify"],
                 )
             # headers
-            if not aiohttp_kwargs.__contains__("headers"):
-                headers = CIMultiDict(self.headers) \
-                    if isinstance(self.headers, (dict, CIMultiDict)) else dict(self.attr)["headers"]
-                headers = headers.copy()
-                # User Agent
-                if self.user_agent and isinstance(self.user_agent, str):
-                    headers["User-Agent"] = self.user_agent
-                if not headers.__contains__("User-Agent"):
-                    headers["User-Agent"] = dict(self.attr)["user_agent"]
-                aiohttp_kwargs["headers"] = headers
+            if aiohttp_kwargs.__contains__("headers"):
+                headers = self.headers \
+                    if self.headers \
+                    else aiohttp_kwargs.pop("headers")
+                if not isinstance(headers, (dict, CIMultiDict)):
+                    headers = {}
+            else:
+                headers = self.headers \
+                    if isinstance(self.headers, (dict, CIMultiDict)) \
+                    else dict(self.attr)["headers"]
+            headers = CIMultiDict(_copy.deepcopy(headers))
+            # User Agent
+            if self.user_agent and isinstance(self.user_agent, str):
+                headers["User-Agent"] = self.user_agent
+            else:
+                headers.setdefault("User-Agent", dict(self.attr)["user_agent"])
+            aiohttp_kwargs["headers"] = headers
             # 创建 aiohttp client_session
             self._session = aiohttp.ClientSession(loop=self._loop, **aiohttp_kwargs)
             # 开始运行
             await self.start()
             result = await self.start_request()
             await self.completed(result)
         finally:
@@ -184,23 +198,32 @@
         if isinstance(self._session, aiohttp.ClientSession) and self._session.closed is False:
             await self._session.close()
 
     async def start_request(self) -> list:
         """start_urls 默认运行方法"""
         if not self.start_urls or not isinstance(self.start_urls, (list, tuple)):
             raise NotImplementedError(f"{self.__class__.__name__}.start_urls is not available!")
+        # req_kwargs
+        req_kwargs = self.req_kwargs
+        if not req_kwargs or not isinstance(req_kwargs, dict):
+            req_kwargs = {}
         tasks = []
         for item in self.start_urls:
             url, cb_kwargs = item, None
             if isinstance(item, (list, tuple)) and len(item) >= 2:
                 url, cb_kwargs = item[0], dict(item[1])
             # base_url
             if not self._base_url:
                 self.base_url = url
-            task = self.request(url=url, callback=self.parse, cb_kwargs=cb_kwargs)
+            task = self.request(
+                url=url,
+                callback=self.parse,
+                cb_kwargs=cb_kwargs,
+                **req_kwargs
+            )
             tasks.append(task)
         result = await asyncio.gather(*tasks)
         return result
 
     async def request(
         self,
         url: StrOrURL,
@@ -217,15 +240,16 @@
         :params: *
         :params: method: 请求方法(default: GET)
         :params: cb_kwargs: 回调函数 关键字参数
         :params: **req_kwargs: 异步请求 request参数
         """
         retry, exc_count, ret, response = 0, 0, None, None
         maximum_retry = self.maximum_retry \
-            if isinstance(self.maximum_retry, int) and self.maximum_retry > 0 else dict(self.attr)["maximum_retry"]
+            if isinstance(self.maximum_retry, int) and self.maximum_retry > 0 \
+            else dict(self.attr)["maximum_retry"]
         async with self.semaphore:
             url = self.build_url(url)
             while True:
                 try:
                     response = await self._session.request(method=method, url=url, **req_kwargs)
                     # 抛出 error status_code
                     if isinstance(self.error_status_code, (list, tuple)) and response.status in self.error_status_code:
@@ -346,15 +370,16 @@
         result = await asyncio.gather(*tasks, return_exceptions=return_exceptions)
         return result
 
     async def sleep(self, delay: Optional[Union[int, float]]=None, result: Any=None):
         """异步休眠"""
         if not isinstance(delay, (int, float)) or delay < 0:
             delay = self.async_sleep \
-                if isinstance(self.async_sleep, (int, float)) and self.async_sleep > 0 else dict(self.attr)["async_sleep"]
+                if isinstance(self.async_sleep, (int, float)) and self.async_sleep >= 0 \
+                else dict(self.attr)["async_sleep"]
         return await asyncio.sleep(delay, result=result)
 
     def build_url(self, _url) -> StrOrURL:
         """构造完整url地址"""
         if not isinstance(_url, (str, _yarl.URL)):
             return _url
         _url = _yarl.URL(_url)
@@ -382,28 +407,28 @@
 
     @property
     def base_url(self) -> StrOrURL:
         """base_url"""
         return self._base_url
 
     @base_url.setter
-    def base_url(self, _url: StrOrURL) -> None:
+    def base_url(self, _url: StrOrURL):
         self._base_url = self.set_base_url(_url)
 
     async def parse(self, response: Response, **kwargs):
         """默认解析函数"""
         raise NotImplementedError(f"'{self.__class__.__name__}.parse' not implemented!")
 
-    async def completed(self, result: list) -> None:
+    async def completed(self, result: list):
         """运行完成结果回调函数"""
 
-    async def start(self) -> None:
+    async def start(self):
         """创建 aiohttp session 后调用"""
 
-    async def close(self) -> None:
+    async def close(self):
         """关闭 aiohttp session 前调用"""
 
 async def xpath(
     self,
     query: str,
     namespaces: Optional[Mapping[str, str]] = None,
     encoding: Optional[str] = None,
```

### Comparing `pyxk-0.5.8/pyxk/aclient/typedef.py` & `pyxk-0.5.9/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/aes/_fmtdata.py` & `pyxk-0.5.9/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/aes/cryptor.py` & `pyxk-0.5.9/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/m3u8downloader/enter_point.py` & `pyxk-0.5.9/pyxk/m3u8downloader/enter_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/m3u8downloader/m3u8download.py` & `pyxk-0.5.9/pyxk/m3u8downloader/m3u8download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/m3u8downloader/m3u8parse.py` & `pyxk-0.5.9/pyxk/m3u8downloader/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/m3u8downloader/main.py` & `pyxk-0.5.9/pyxk/m3u8downloader/main.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/requests/api.py` & `pyxk-0.5.9/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/requests/entry_point.py` & `pyxk-0.5.9/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk/requests/sessions.py` & `pyxk-0.5.9/pyxk/requests/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,17 @@
         *,
         headers: Optional[Union[CIDict, dict]] = None,
         base_url: Optional[str] = None,
         user_agent: Optional[str] = None
     ):
         super().__init__()
         headers = CIDict(headers)
-        if user_agent and isinstance(user_agent, str):
-            headers.__setitem__("User-Agent", user_agent or get_user_agent())
+        if not user_agent or not isinstance(user_agent, str):
+            user_agent = get_user_agent()
+        headers.__setitem__("User-Agent", user_agent)
         self.headers.update(headers)
         self._base_url = self.set_base_url(base_url)
         self._console = _rich_console.Console()
 
     def request(
         self, method, url, *, show_status=True, params=None, data=None, headers=None, cookies=None, files=None, auth=None, timeout=5, allow_redirects=True, proxies=None, hooks=None, stream=None, verify=None, cert=None, json=None
     ) -> Response:
```

### Comparing `pyxk-0.5.8/pyxk/utils.py` & `pyxk-0.5.9/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.9/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.8/setup.py` & `pyxk-0.5.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.8",
+    version="0.5.9",
     author="pengke",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

