# Comparing `tmp/duckduckgo_search-3.2.0.tar.gz` & `tmp/duckduckgo_search-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.2.0.tar", last modified: Tue May 23 12:18:40 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.3.0.tar", last modified: Thu May 25 05:26:24 2023, max compression
```

## Comparing `duckduckgo_search-3.2.0.tar` & `duckduckgo_search-3.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 12:18:40.000000 duckduckgo_search-3.2.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:18:40.041953 duckduckgo_search-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-23 12:18:23.000000 duckduckgo_search-3.2.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.466904 duckduckgo_search-3.3.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.466904 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 05:26:24.000000 duckduckgo_search-3.3.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 05:26:24.470904 duckduckgo_search-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-25 05:26:08.000000 duckduckgo_search-3.3.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.2.0/LICENSE.md` & `duckduckgo_search-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.2.0/PKG-INFO` & `duckduckgo_search-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.2.0
+Version: 3.3.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.2.0/README.md` & `duckduckgo_search-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.2.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.3.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.2.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.3.0/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.2.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.3.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.2.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.3.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from decimal import Decimal
 from html import unescape
 from time import sleep
 from typing import Deque, Dict, Iterator, Optional
 from urllib.parse import unquote
 
 import requests
-from requests.exceptions import HTTPError, JSONDecodeError, Timeout
 from requests.models import Response
 
 logger = logging.getLogger(__name__)
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
     "Referer": "https://duckduckgo.com/",
@@ -55,23 +54,24 @@
 
     def _get_url(self, method: str, url: str, **kwargs) -> Optional[Response]:
         for i in range(3):
             try:
                 resp = self._session.request(
                     method, url, timeout=self._timeout, **kwargs
                 )
-                if self._is_500_in_url(resp.url):
+                if self._is_500_in_url(resp.url) or resp.status_code == 202:
                     raise requests.HTTPError
                 resp.raise_for_status()
-                return resp
+                if resp.status_code == 200:
+                    return resp
             except Exception as ex:
                 logger.warning(f"_get_url() {url} {type(ex).__name__} {ex}")
                 if i >= 2 or "418" in str(ex):
                     raise ex
-                sleep(2**i)
+            sleep(3)
         return None
 
     def _get_vqd(self, keywords: str) -> Optional[str]:
         """Get vqd value for a search query."""
         resp = self._get_url("POST", "https://duckduckgo.com", data={"q": keywords})
         if resp:
             for c1, c2 in (
@@ -117,61 +117,71 @@
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         assert vqd, "error in getting vqd"
 
-        safesearch_base = {"on": 1, "moderate": -1, "off": -2}
         payload = {
-            "q": keywords,
+            "q": keywords,  #
+            "kl": region,
             "l": region,
-            "p": safesearch_base[safesearch.lower()],
             "s": 0,
             "df": timelimit,
-            "o": "json",
             "vqd": vqd,
+            "o": "json",
         }
+        if safesearch == "off":
+            # payload["p"] = '-2'
+            payload["ex"] = "-2"
+        elif safesearch == "moderate":
+            payload["p"] = ""
+            payload["sp"] = "0"
+            payload["ex"] = "-1"
+        elif safesearch == "on":  # strict
+            payload["sp"] = "0"
+            payload["p"] = "1"
 
         cache = set()
         for _ in range(10):
             resp = self._get_url(
                 "GET", "https://links.duckduckgo.com/d.js", params=payload
             )
             if resp is None:
                 break
             try:
                 page_data = resp.json().get("results", None)
-            except (AttributeError, JSONDecodeError):
+            except Exception:
+                break
+            if page_data is None:
                 break
 
-            if page_data:
-                result_exists = False
-                for row in page_data:
-                    if "n" in row:
-                        payload["s"] = row["n"].split("s=")[-1].split("&")[0]
-                    href = row.get("u", None)
-                    if (
-                        href
-                        and href not in cache
-                        and href != f"http://www.google.com/search?q={keywords}"
-                    ):
-                        cache.add(href)
-                        body = self._normalize(row["a"])
-                        if body:
-                            result_exists = True
-                            yield {
-                                "title": self._normalize(row["t"]),
-                                "href": href,
-                                "body": body,
-                            }
-                    elif result_exists is False:
-                        break
-                if result_exists is False:
+            result_exists = False
+            for row in page_data:
+                if "n" in row:
+                    payload["s"] = row["n"].split("s=")[-1].split("&")[0]
+                href = row.get("u", None)
+                if (
+                    href
+                    and href not in cache
+                    and href != f"http://www.google.com/search?q={keywords}"
+                ):
+                    cache.add(href)
+                    body = self._normalize(row["a"])
+                    if body:
+                        result_exists = True
+                        yield {
+                            "title": self._normalize(row["t"]),
+                            "href": href,
+                            "body": body,
+                        }
+                elif result_exists is False:
                     break
+            if result_exists is False:
+                break
 
     def images(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -228,39 +238,40 @@
         cache = set()
         for _ in range(10):
             resp = self._get_url("GET", "https://duckduckgo.com/i.js", params=payload)
             if resp is None:
                 break
             try:
                 resp_json = resp.json()
-            except (AttributeError, JSONDecodeError):
+            except Exception:
                 break
-
             page_data = resp_json.get("results", None)
-            if page_data:
-                result_exists = False
-                for row in page_data:
-                    image_url = row.get("image", None)
-                    if image_url and image_url not in cache:
-                        cache.add(image_url)
-                        result_exists = True
-                        yield {
-                            "title": row["title"],
-                            "image": image_url,
-                            "thumbnail": row["thumbnail"],
-                            "url": row["url"],
-                            "height": row["height"],
-                            "width": row["width"],
-                            "source": row["source"],
-                        }
-                next = resp_json.get("next", None)
-                if next:
-                    payload["s"] = next.split("s=")[-1].split("&")[0]
-                if next is None or result_exists is False:
-                    break
+            if page_data is None:
+                break
+
+            result_exists = False
+            for row in page_data:
+                image_url = row.get("image", None)
+                if image_url and image_url not in cache:
+                    cache.add(image_url)
+                    result_exists = True
+                    yield {
+                        "title": row["title"],
+                        "image": image_url,
+                        "thumbnail": row["thumbnail"],
+                        "url": row["url"],
+                        "height": row["height"],
+                        "width": row["width"],
+                        "source": row["source"],
+                    }
+            next = resp_json.get("next", None)
+            if next:
+                payload["s"] = next.split("s=")[-1].split("&")[0]
+            if next is None or result_exists is False:
+                break
 
     def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -306,30 +317,31 @@
         cache = set()
         for _ in range(10):
             resp = self._get_url("GET", "https://duckduckgo.com/v.js", params=payload)
             if resp is None:
                 break
             try:
                 resp_json = resp.json()
-            except (AttributeError, JSONDecodeError):
+            except Exception:
                 break
-
             page_data = resp_json.get("results", None)
-            if page_data:
-                result_exists = False
-                for row in page_data:
-                    if row["content"] not in cache:
-                        cache.add(row["content"])
-                        result_exists = True
-                        yield row
-                next = resp_json.get("next", None)
-                if next:
-                    payload["s"] = next.split("s=")[-1].split("&")[0]
-                if not result_exists or not next:
-                    break
+            if page_data is None:
+                break
+
+            result_exists = False
+            for row in page_data:
+                if row["content"] not in cache:
+                    cache.add(row["content"])
+                    result_exists = True
+                    yield row
+            next = resp_json.get("next", None)
+            if next:
+                payload["s"] = next.split("s=")[-1].split("&")[0]
+            if not result_exists or not next:
+                break
 
     def news(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
@@ -368,37 +380,38 @@
             resp = self._get_url(
                 "GET", "https://duckduckgo.com/news.js", params=payload
             )
             if resp is None:
                 break
             try:
                 resp_json = resp.json()
-            except (AttributeError, JSONDecodeError):
+            except Exception:
                 break
-
             page_data = resp_json.get("results", None)
-            if page_data:
-                result_exists = False
-                for row in page_data:
-                    if row["url"] not in cache:
-                        cache.add(row["url"])
-                        result_exists = True
-                        yield {
-                            "date": datetime.utcfromtimestamp(row["date"]).isoformat(),
-                            "title": row["title"],
-                            "body": self._normalize(row["excerpt"]),
-                            "url": row["url"],
-                            "image": row.get("image", None),
-                            "source": row["source"],
-                        }
-                next = resp_json.get("next", None)
-                if next:
-                    payload["s"] = next.split("s=")[-1].split("&")[0]
-                if not result_exists or not next:
-                    break
+            if page_data is None:
+                break
+
+            result_exists = False
+            for row in page_data:
+                if row["url"] not in cache:
+                    cache.add(row["url"])
+                    result_exists = True
+                    yield {
+                        "date": datetime.utcfromtimestamp(row["date"]).isoformat(),
+                        "title": row["title"],
+                        "body": self._normalize(row["excerpt"]),
+                        "url": row["url"],
+                        "image": row.get("image", None),
+                        "source": row["source"],
+                    }
+            next = resp_json.get("next", None)
+            if next:
+                payload["s"] = next.split("s=")[-1].split("&")[0]
+            if not result_exists or not next:
+                break
 
     def answers(
         self,
         keywords: str,
     ) -> Iterator[dict]:
         """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params
 
@@ -417,15 +430,15 @@
         }
 
         resp = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
         if resp is None:
             return None
         try:
             page_data = resp.json()
-        except (AttributeError, JSONDecodeError):
+        except Exception:
             page_data = None
 
         if page_data:
             answer = page_data.get("AbstractText", None)
             url = page_data.get("AbstractURL", None)
             if answer:
                 yield {
@@ -441,15 +454,15 @@
             "format": "json",
         }
         resp = self._get_url("GET", "https://api.duckduckgo.com/", params=payload)
         if resp is None:
             return None
         try:
             page_data = resp.json().get("RelatedTopics", None)
-        except (AttributeError, JSONDecodeError):
+        except Exception:
             page_data = None
 
         if page_data:
             for i, row in enumerate(page_data):
                 topic = row.get("Name", None)
                 if not topic:
                     icon = row["Icon"].get("URL", None)
@@ -493,15 +506,15 @@
         resp = self._get_url("GET", "https://duckduckgo.com/ac", params=payload)
         if resp is None:
             return None
         try:
             page_data = resp.json()
             for r in page_data:
                 yield r
-        except (AttributeError, JSONDecodeError):
+        except Exception:
             pass
 
     def maps(
         self,
         keywords: str,
         place: Optional[str] = None,
         street: Optional[str] = None,
@@ -613,48 +626,49 @@
             resp = self._get_url(
                 "GET", "https://duckduckgo.com/local.js", params=params
             )
             if resp is None:
                 break
             try:
                 page_data = resp.json().get("results", [])
-            except (AttributeError, JSONDecodeError):
+            except Exception:
+                break
+            if page_data is None:
                 break
 
-            if page_data:
-                for res in page_data:
-                    result = MapsResult()
-                    result.title = res["name"]
-                    result.address = res["address"]
-                    if f"{result.title} {result.address}" in cache:
-                        continue
-                    else:
-                        cache.add(f"{result.title} {result.address}")
-                        result.country_code = res["country_code"]
-                        result.url = res["website"]
-                        result.phone = res["phone"]
-                        result.latitude = res["coordinates"]["latitude"]
-                        result.longitude = res["coordinates"]["longitude"]
-                        result.source = unquote(res["url"])
-                        if res["embed"]:
-                            result.image = res["embed"].get("image", "")
-                            result.links = res["embed"].get("third_party_links", "")
-                            result.desc = res["embed"].get("description", "")
-                        result.hours = res["hours"]
-                        yield result.__dict__
-
-                # divide the square into 4 parts and add to the queue
-                if len(page_data) >= 15:
-                    lat_middle = (lat_t + lat_b) / 2
-                    lon_middle = (lon_l + lon_r) / 2
-                    bbox1 = (lat_t, lon_l, lat_middle, lon_middle)
-                    bbox2 = (lat_t, lon_middle, lat_middle, lon_r)
-                    bbox3 = (lat_middle, lon_l, lat_b, lon_middle)
-                    bbox4 = (lat_middle, lon_middle, lat_b, lon_r)
-                    work_bboxes.extendleft([bbox1, bbox2, bbox3, bbox4])
+            for res in page_data:
+                result = MapsResult()
+                result.title = res["name"]
+                result.address = res["address"]
+                if f"{result.title} {result.address}" in cache:
+                    continue
+                else:
+                    cache.add(f"{result.title} {result.address}")
+                    result.country_code = res["country_code"]
+                    result.url = res["website"]
+                    result.phone = res["phone"]
+                    result.latitude = res["coordinates"]["latitude"]
+                    result.longitude = res["coordinates"]["longitude"]
+                    result.source = unquote(res["url"])
+                    if res["embed"]:
+                        result.image = res["embed"].get("image", "")
+                        result.links = res["embed"].get("third_party_links", "")
+                        result.desc = res["embed"].get("description", "")
+                    result.hours = res["hours"]
+                    yield result.__dict__
+
+            # divide the square into 4 parts and add to the queue
+            if len(page_data) >= 15:
+                lat_middle = (lat_t + lat_b) / 2
+                lon_middle = (lon_l + lon_r) / 2
+                bbox1 = (lat_t, lon_l, lat_middle, lon_middle)
+                bbox2 = (lat_t, lon_middle, lat_middle, lon_r)
+                bbox3 = (lat_middle, lon_l, lat_b, lon_middle)
+                bbox4 = (lat_middle, lon_middle, lat_b, lon_r)
+                work_bboxes.extendleft([bbox1, bbox2, bbox3, bbox4])
 
     def translate(
         self,
         keywords: str,
         from_: Optional[str] = None,
         to: str = "en",
     ) -> Optional[dict]:
@@ -688,10 +702,10 @@
             data=keywords.encode(),
         )
         if resp is None:
             return None
         try:
             page_data = resp.json()
             page_data["original"] = keywords
-        except (AttributeError, JSONDecodeError):
+        except Exception:
             page_data = None
         return page_data
```

### Comparing `duckduckgo_search-3.2.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.3.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.2.0
+Version: 3.3.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.2.0/pyproject.toml` & `duckduckgo_search-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.2.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.3.0/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

