# Comparing `tmp/dartrig-0.0.8.tar.gz` & `tmp/dartrig-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.0.8.tar", last modified: Tue Apr 11 08:27:35 2023, max compression
+gzip compressed data, was "dist/dartrig-0.0.9.tar", last modified: Tue Apr 25 17:11:16 2023, max compression
```

## Comparing `dartrig-0.0.8.tar` & `dartrig-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:27:35.000000 dartrig-0.0.8/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-04-11 08:27:35.000000 dartrig-0.0.8/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.0.8/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.0.8/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      600 2023-04-11 08:26:59.000000 dartrig-0.0.8/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    11505 2023-04-11 01:58:31.000000 dartrig-0.0.8/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.0.8/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      193 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-11 08:27:35.000000 dartrig-0.0.8/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-11 08:27:35.000000 dartrig-0.0.8/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-25 17:11:16.000000 dartrig-0.0.9/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-04-25 17:11:16.000000 dartrig-0.0.9/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.0.9/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.0.9/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      600 2023-04-25 17:11:14.000000 dartrig-0.0.9/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-25 17:11:16.000000 dartrig-0.0.9/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    11455 2023-04-25 17:11:14.000000 dartrig-0.0.9/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.0.9/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-25 17:11:16.000000 dartrig-0.0.9/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-04-25 17:11:16.000000 dartrig-0.0.9/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      193 2023-04-25 17:11:16.000000 dartrig-0.0.9/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-04-25 17:11:16.000000 dartrig-0.0.9/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-25 17:11:16.000000 dartrig-0.0.9/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-25 17:11:16.000000 dartrig-0.0.9/setup.cfg
```

### Comparing `dartrig-0.0.8/PKG-INFO` & `dartrig-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.0.8
+Version: 0.0.9
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.0.8/LICENSE` & `dartrig-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.0.8/README.md` & `dartrig-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.0.8/setup.py` & `dartrig-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.0.8",
+    version="0.0.9",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="dartrig api wrapper",
     long_description_content_type="text/markdown",
     long_description=open('README.md', "r").read(),
     url="https://github.com/cheddars/dart_rigger",
```

### Comparing `dartrig-0.0.8/dartrig/__init__.py` & `dartrig-0.0.9/dartrig/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 import traceback
 import time
 from typing import List
 from datetime import datetime
 from bs4 import BeautifulSoup
 from cache import AdtCache
-from dartrig.annotations import memoize
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.103 Safari/537.36"}
 
 URLS = {
     "DART_BASE": "https://dart.fss.or.kr",
     "DART_LIST": "https://dart.fss.or.kr/dsab007/detailSearch.ax",
@@ -22,15 +21,14 @@
 
 
 class DartWeb:
     def __init__(self):
         self.session = requests.Session()
         self.session.get(URLS["DART_BASE"], headers=HEADERS)
 
-    @memoize
     def request_detail(self, rcp_no: str, dtd: str, ele_id: int = 0, offset: int = 0) -> str:
         """
         :param rcp_no:
         :param dtd: html | dart3.xsd
         :param ele_id:
         :param offset:
         :return:
@@ -38,26 +36,23 @@
         dcm_no = self.get_dcm_no_by_rcp_no(rcp_no)
         url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
         logger.info(f"request_detail url : {url}")
         response = self.session.get(url, headers=HEADERS)
         # response.encoding = "UTF-8"
         return response.text
 
-    @memoize
     def request_detail_with_dcm(self, rcp_no, dtd, dcm_no, ele_id=0, offset=0):
         url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
         logger.info(f"request_detail_with_dcm url : {url}")
         return self.session.get(url, headers=HEADERS).text
 
-    @memoize
     def dsaf001_report(self, rcp_no):
         logger.debug(f"dsaf001_report for rcp_no {rcp_no}")
         return self.session.get(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", headers=HEADERS).text
 
-    @memoize
     def get_dcm_no_by_rcp_no(self, rcp_no):
         try:
             html_text = self.dsaf001_report(rcp_no)
             numbers = re.findall("\d{7}", html_text)
             dcm_no = numbers[2]
         except Exception as ex:
             logger.exception(ex)
@@ -200,22 +195,22 @@
             else:
                 results.extend(response_items)
 
             if total_page == page_no:
                 logger.info(f"total page reached {total_page}")
                 break
 
-            if max_page >= page_no:
+            if max_page <= page_no:
                 logger.info(f"max page reached {max_page}")
                 break
 
         list_items = []
 
         for item in results:
-
+            logger.debug(f"item : {item}")
             # 각 항목별로 데이터 추출
             data = {
                 "company": item.get('corp_name', ''),
                 "market": item.get('corp_cls', ''),
                 "title": item.get('report_nm', ''),
                 "code": item.get('stock_code', ''),
                 "rcp_no": item.get('rcept_no', ''),
```

### Comparing `dartrig-0.0.8/dartrig/annotations.py` & `dartrig-0.0.9/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.0.8/dartrig.egg-info/PKG-INFO` & `dartrig-0.0.9/dartrig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.0.8
+Version: 0.0.9
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

