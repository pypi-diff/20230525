# Comparing `tmp/duckduckgo_search-3.4.0.tar.gz` & `tmp/duckduckgo_search-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.4.0.tar", last modified: Thu May 25 20:49:23 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.4.1.tar", last modified: Thu May 25 21:11:40 2023, max compression
```

## Comparing `duckduckgo_search-3.4.0.tar` & `duckduckgo_search-3.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    27342 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 20:49:23.000000 duckduckgo_search-3.4.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:23.687882 duckduckgo_search-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-25 20:49:07.000000 duckduckgo_search-3.4.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13561 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 21:11:40.000000 duckduckgo_search-3.4.1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:11:40.197756 duckduckgo_search-3.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-25 21:11:23.000000 duckduckgo_search-3.4.1/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.4.0/LICENSE.md` & `duckduckgo_search-3.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.0/PKG-INFO` & `duckduckgo_search-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.4.0
+Version: 3.4.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.4.0/README.md` & `duckduckgo_search-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.4.1/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.4.1/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.4.1/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.4.1/duckduckgo_search/duckduckgo_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,19 @@
                         "href": href,
                         "body": self._normalize("".join(body)) if body else None,
                     }
 
             if result_exists is False:
                 break
 
-            next_page = tree.xpath('.//div[@class="nav-link"]')[-1]
+            next_page = tree.xpath('.//div[@class="nav-link"]')
+            next_page = next_page[-1] if next_page else None
+            if next_page is None:
+                return
+
             names = next_page.xpath('.//input[@type="hidden"]/@name')
             values = next_page.xpath('.//input[@type="hidden"]/@value')
             payload = {n: v for n, v in zip(names, values)}
             sleep(1)
 
     def images(
         self,
```

### Comparing `duckduckgo_search-3.4.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.4.1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.4.0
+Version: 3.4.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.4.0/pyproject.toml` & `duckduckgo_search-3.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.4.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.4.1/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

