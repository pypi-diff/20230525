# Comparing `tmp/duckduckgo_search-3.3.0.tar.gz` & `tmp/duckduckgo_search-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.3.0.tar", last modified: Thu May 25 05:26:24 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.4.0.tar", last modified: Thu May 25 20:49:23 2023, max compression
```

## Comparing `duckduckgo_search-3.3.0.tar` & `duckduckgo_search-3.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.466904 duckduckgo_search-3.3.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.466904 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.3.0/LICENSE.md` & `duckduckgo_search-3.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.3.0/PKG-INFO` & `duckduckgo_search-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.3.0
+Version: 3.4.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.3.0/README.md` & `duckduckgo_search-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.3.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.4.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.3.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.4.0/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.3.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.4.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.3.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.4.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import re
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from html import unescape
 from time import sleep
-from typing import Deque, Dict, Iterator, Optional
+from typing import Deque, Dict, Iterator, Optional, Set
 from urllib.parse import unquote
 
 import requests
+from lxml import html
 from requests.models import Response
 
 logger = logging.getLogger(__name__)
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
     "Referer": "https://duckduckgo.com/",
@@ -93,14 +94,15 @@
 
     def _normalize(self, raw_html: str) -> str:
         """strip HTML tags"""
         if raw_html:
             return unescape(re.sub(REGEX_STRIP_TAGS, "", raw_html))
         return ""
 
+    '''
     def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
     ) -> Iterator[dict]:
@@ -174,14 +176,81 @@
                             "href": href,
                             "body": body,
                         }
                 elif result_exists is False:
                     break
             if result_exists is False:
                 break
+    '''
+
+    def text(
+        self,
+        keywords: str,
+        region: str = "wt-wt",
+        safesearch: str = "moderate",
+        timelimit: Optional[str] = None,
+    ) -> Iterator[dict]:
+        """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
+
+        Args:
+            keywords: keywords for query.
+            region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
+            safesearch: on, moderate, off. Defaults to "moderate".
+            timelimit: d, w, m, y. Defaults to None.
+
+        Yields:
+            dict with search results.
+
+        """
+        assert keywords, "keywords is mandatory"
+
+        safesearch_base = {"on": 1, "moderate": -1, "off": -2}
+        payload = {
+            "q": keywords,
+            "l": region,
+            "p": safesearch_base[safesearch.lower()],
+            "df": timelimit,
+        }
+        cache: Set[str] = set()
+        for _ in range(10):
+            resp = self._get_url(
+                "POST", "https://html.duckduckgo.com/html", data=payload
+            )
+            if resp is None:
+                break
+            tree = html.fromstring(resp.content)
+            if tree.xpath('//div[@class="no-results"]/text()'):
+                return
+            result_exists = False
+            for e in tree.xpath('//div[contains(@class, "results_links")]'):
+                href = e.xpath('.//a[contains(@class, "result__a")]/@href')
+                href = href[0] if href else None
+                if (
+                    href
+                    and href not in cache
+                    and href != f"http://www.google.com/search?q={keywords}"
+                ):
+                    cache.add(href)
+                    title = e.xpath('.//a[contains(@class, "result__a")]/text()')
+                    body = e.xpath('.//a[contains(@class, "result__snippet")]//text()')
+                    result_exists = True
+                    yield {
+                        "title": self._normalize(title[0]) if title else None,
+                        "href": href,
+                        "body": self._normalize("".join(body)) if body else None,
+                    }
+
+            if result_exists is False:
+                break
+
+            next_page = tree.xpath('.//div[@class="nav-link"]')[-1]
+            names = next_page.xpath('.//input[@type="hidden"]/@name')
+            values = next_page.xpath('.//input[@type="hidden"]/@value')
+            payload = {n: v for n, v in zip(names, values)}
+            sleep(1)
 
     def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
```

### Comparing `duckduckgo_search-3.3.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.4.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.3.0
+Version: 3.4.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.3.0/pyproject.toml` & `duckduckgo_search-3.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
+    "lxml>=4.9.2",
     "requests>=2.31.0",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
```

### Comparing `duckduckgo_search-3.3.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.4.0/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

