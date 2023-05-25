# Comparing `tmp/picimagesearch-3.9.0.tar.gz` & `tmp/picimagesearch-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picimagesearch-3.9.0.tar", max compression
+gzip compressed data, was "picimagesearch-3.9.1.tar", max compression
```

## Comparing `picimagesearch-3.9.0.tar` & `picimagesearch-3.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1063 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/LICENSE
--rw-r--r--   0        0        0      251 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/__init__.py
--rw-r--r--   0        0        0     2145 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/ascii2d.py
--rw-r--r--   0        0        0     1384 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/baidu.py
--rw-r--r--   0        0        0     1433 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/ehentai.py
--rw-r--r--   0        0        0     2421 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/google.py
--rw-r--r--   0        0        0     1215 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/iqdb.py
--rw-r--r--   0        0        0      397 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/__init__.py
--rw-r--r--   0        0        0     2656 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/ascii2d.py
--rw-r--r--   0        0        0      749 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/baidu.py
--rw-r--r--   0        0        0     1895 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/ehentai.py
--rw-r--r--   0        0        0     2234 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/google.py
--rw-r--r--   0        0        0     3711 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/iqdb.py
--rw-r--r--   0        0        0     5170 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/saucenao.py
--rw-r--r--   0        0        0     2755 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/tracemoe.py
--rw-r--r--   0        0        0     1312 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/model/yandex.py
--rw-r--r--   0        0        0     4557 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/network.py
--rw-r--r--   0        0        0     4702 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/saucenao.py
--rw-r--r--   0        0        0     1518 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/sync.py
--rw-r--r--   0        0        0     4829 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/tracemoe.py
--rw-r--r--   0        0        0     1945 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/PicImageSearch/yandex.py
--rw-r--r--   0        0        0     3390 2023-03-30 11:14:05.723060 picimagesearch-3.9.0/README.md
--rw-r--r--   0        0        0     1148 2023-03-30 11:14:05.727060 picimagesearch-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     4433 1970-01-01 00:00:00.000000 picimagesearch-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/LICENSE
+-rw-r--r--   0        0        0      251 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/ascii2d.py
+-rw-r--r--   0        0        0     1384 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/baidu.py
+-rw-r--r--   0        0        0     1433 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/ehentai.py
+-rw-r--r--   0        0        0     2421 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/google.py
+-rw-r--r--   0        0        0     1215 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/iqdb.py
+-rw-r--r--   0        0        0      397 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/__init__.py
+-rw-r--r--   0        0        0     2656 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/ascii2d.py
+-rw-r--r--   0        0        0      749 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/baidu.py
+-rw-r--r--   0        0        0     1895 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/ehentai.py
+-rw-r--r--   0        0        0     2234 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/google.py
+-rw-r--r--   0        0        0     3711 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/iqdb.py
+-rw-r--r--   0        0        0     5170 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/saucenao.py
+-rw-r--r--   0        0        0     2755 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/tracemoe.py
+-rw-r--r--   0        0        0     1312 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/model/yandex.py
+-rw-r--r--   0        0        0     4526 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/network.py
+-rw-r--r--   0        0        0     4702 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/saucenao.py
+-rw-r--r--   0        0        0     1518 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/sync.py
+-rw-r--r--   0        0        0     4829 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/tracemoe.py
+-rw-r--r--   0        0        0     1945 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/PicImageSearch/yandex.py
+-rw-r--r--   0        0        0     3390 2023-05-24 19:52:35.705425 picimagesearch-3.9.1/README.md
+-rw-r--r--   0        0        0     1148 2023-05-24 19:52:35.709425 picimagesearch-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4433 1970-01-01 00:00:00.000000 picimagesearch-3.9.1/PKG-INFO
```

### Comparing `picimagesearch-3.9.0/LICENSE` & `picimagesearch-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/ascii2d.py` & `picimagesearch-3.9.1/PicImageSearch/ascii2d.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/baidu.py` & `picimagesearch-3.9.1/PicImageSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/ehentai.py` & `picimagesearch-3.9.1/PicImageSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/google.py` & `picimagesearch-3.9.1/PicImageSearch/google.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/iqdb.py` & `picimagesearch-3.9.1/PicImageSearch/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/ascii2d.py` & `picimagesearch-3.9.1/PicImageSearch/model/ascii2d.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/baidu.py` & `picimagesearch-3.9.1/PicImageSearch/model/baidu.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/ehentai.py` & `picimagesearch-3.9.1/PicImageSearch/model/ehentai.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/google.py` & `picimagesearch-3.9.1/PicImageSearch/model/google.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
             for i in data.find('a[aria-label~="Page"]').items()
         ]
         self.pages.insert(index - 1, resp_url)
         script_list = list(data.find("script").items())
         # 结果返回值
         thumbnail_dict: Dict[str, str] = self.create_thumbnail_dict(script_list)
         self.raw: List[GoogleItem] = [
-            GoogleItem(i, (thumbnail_dict.get(i("img").eq(1).attr("id"), None)))
-            for i in data.find(".g").items()
+            GoogleItem(i, thumbnail_dict.get(i("img").attr("id"), None))
+            for i in data.find("#search .g").items()
         ]
 
     @staticmethod
     def create_thumbnail_dict(script_list: List[PyQuery]) -> Dict[str, str]:
         thumbnail_dict = {}
         base_64_regex = compile(r"data:image/(?:jpeg|jpg|png|gif);base64,[^'\"]+")
         id_regex = compile(r"dimg_\d+")
```

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/iqdb.py` & `picimagesearch-3.9.1/PicImageSearch/model/iqdb.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/saucenao.py` & `picimagesearch-3.9.1/PicImageSearch/model/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/tracemoe.py` & `picimagesearch-3.9.1/PicImageSearch/model/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/model/yandex.py` & `picimagesearch-3.9.1/PicImageSearch/model/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/network.py` & `picimagesearch-3.9.1/PicImageSearch/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 key, value = line.strip().split("=", 1)
                 self.cookies[key] = value
 
         self.client: AsyncClient = AsyncClient(
             headers=headers,
             cookies=self.cookies,
             verify=verify_ssl,
-            proxies={"all://": proxies} if proxies else {},
+            proxies=proxies,
             timeout=timeout,
             follow_redirects=True,
         )
 
     def start(self) -> AsyncClient:
         return self.client
```

### Comparing `picimagesearch-3.9.0/PicImageSearch/saucenao.py` & `picimagesearch-3.9.1/PicImageSearch/saucenao.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/sync.py` & `picimagesearch-3.9.1/PicImageSearch/sync.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/tracemoe.py` & `picimagesearch-3.9.1/PicImageSearch/tracemoe.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/PicImageSearch/yandex.py` & `picimagesearch-3.9.1/PicImageSearch/yandex.py`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/README.md` & `picimagesearch-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `picimagesearch-3.9.0/pyproject.toml` & `picimagesearch-3.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "PicImageSearch"
-version = "3.9.0"
+version = "3.9.1"
 description = "PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "lleans", "chinoll", "NekoAria"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "PicImageSearch" }
 ]
 homepage = "https://github.com/kitUIN/PicImageSearch"
 repository = "https://github.com/kitUIN/PicImageSearch"
 keywords = ["google", "iqdb", "saucenao", "tracemoe", "ascii2d"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-httpx = "^0.23.3"
+httpx = "^0.24.1"
 lxml = "^4.9.2"
 pyquery = "^2.0.0"
 socksio = { version = "^1.0.0", optional = true }
 
 [tool.poetry.extras]
 socks = ["socksio"]
 
 [tool.poetry.dev-dependencies]
-loguru = "^0.6.0"
+loguru = "^0.7.0"
 
 [tool.mypy]
 python_version = "3.7"
 ignore_missing_imports = true
 implicit_reexport = true
 pretty = true
 show_error_codes = true
```

### Comparing `picimagesearch-3.9.0/PKG-INFO` & `picimagesearch-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picimagesearch
-Version: 3.9.0
+Version: 3.9.1
 Summary: PicImageSearch APIs for Python 3.x 适用于 Python 3 以图搜源整合API
 Home-page: https://github.com/kitUIN/PicImageSearch
 License: MIT
 Keywords: google,iqdb,saucenao,tracemoe,ascii2d
 Author: kitUIN
 Author-email: kulujun@gmail.com
 Maintainer: kitUIN
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: socks
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: pyquery (>=2.0.0,<3.0.0)
 Requires-Dist: socksio (>=1.0.0,<2.0.0) ; extra == "socks"
 Project-URL: Repository, https://github.com/kitUIN/PicImageSearch
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: picimagesearch Version: 3.9.0 Summary:
+Metadata-Version: 2.1 Name: picimagesearch Version: 3.9.1 Summary:
 PicImageSearch APIs for Python 3.x éç¨äº Python 3 ä»¥å¾ææºæ´åAPI
 Home-page: https://github.com/kitUIN/PicImageSearch License: MIT Keywords:
 google,iqdb,saucenao,tracemoe,ascii2d Author: kitUIN Author-email:
 kulujun@gmail.com Maintainer: kitUIN Maintainer-email: kulujun@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: socks Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist:
+Provides-Extra: socks Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist:
 lxml (>=4.9.2,<5.0.0) Requires-Dist: pyquery (>=2.0.0,<3.0.0) Requires-Dist:
 socksio (>=1.0.0,<2.0.0) ; extra == "socks" Project-URL: Repository, https://
 github.com/kitUIN/PicImageSearch Description-Content-Type: text/markdown
          # PicImageSearch â¨ èåè¯å¾å¼æ ç¨äºä»¥å¾ææºâ¨
                  [license] [pypi] [python] [release] [release]
                         ðææ¡£ Â· ðæäº¤å»ºè®®
 ## æ¯æ - [x] [SauceNAO](https://saucenao.com/) - [x] [TraceMoe](https://
```

