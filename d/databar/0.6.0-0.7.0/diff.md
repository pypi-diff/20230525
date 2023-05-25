# Comparing `tmp/databar-0.6.0.tar.gz` & `tmp/databar-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databar-0.6.0.tar", last modified: Thu May 18 14:58:25 2023, max compression
+gzip compressed data, was "databar-0.7.0.tar", last modified: Thu May 25 17:31:17 2023, max compression
```

## Comparing `databar-0.6.0.tar` & `databar-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.771646 databar-0.6.0/
--rw-r--r--   0 sadilet    (502) staff       (20)     1069 2023-05-18 14:36:56.000000 databar-0.6.0/LICENSE
--rw-r--r--   0 sadilet    (502) staff       (20)       81 2023-05-18 14:36:56.000000 databar-0.6.0/MANIFEST.in
--rw-r--r--   0 sadilet    (502) staff       (20)     1421 2023-05-18 14:58:25.771705 databar-0.6.0/PKG-INFO
--rw-r--r--   0 sadilet    (502) staff       (20)     1089 2023-05-18 14:36:56.000000 databar-0.6.0/README.md
--rw-r--r--   0 sadilet    (502) staff       (20)     1670 2023-05-18 14:58:25.772181 databar-0.6.0/setup.cfg
--rw-r--r--   0 sadilet    (502) staff       (20)       86 2023-05-18 14:36:56.000000 databar-0.6.0/setup.py
-drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.769056 databar-0.6.0/src/
-drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.770582 databar-0.6.0/src/databar/
--rw-r--r--   0 sadilet    (502) staff       (20)       96 2023-05-18 14:36:56.000000 databar-0.6.0/src/databar/__init__.py
--rw-r--r--   0 sadilet    (502) staff       (20)    14089 2023-05-18 14:47:29.000000 databar-0.6.0/src/databar/connection.py
--rw-r--r--   0 sadilet    (502) staff       (20)     2800 2023-05-18 14:36:56.000000 databar-0.6.0/src/databar/helpers.py
--rw-r--r--   0 sadilet    (502) staff       (20)     9645 2023-05-18 14:36:56.000000 databar-0.6.0/src/databar/table.py
-drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.771165 databar-0.6.0/src/databar.egg-info/
--rw-r--r--   0 sadilet    (502) staff       (20)     1421 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/PKG-INFO
--rw-r--r--   0 sadilet    (502) staff       (20)      377 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/SOURCES.txt
--rw-r--r--   0 sadilet    (502) staff       (20)        1 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/dependency_links.txt
--rw-r--r--   0 sadilet    (502) staff       (20)      144 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/requires.txt
--rw-r--r--   0 sadilet    (502) staff       (20)        8 2023-05-18 14:58:25.000000 databar-0.6.0/src/databar.egg-info/top_level.txt
-drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-18 14:58:25.771523 databar-0.6.0/tests/
--rw-r--r--   0 sadilet    (502) staff       (20)        0 2023-05-18 14:36:56.000000 databar-0.6.0/tests/__init__.py
--rw-r--r--   0 sadilet    (502) staff       (20)      274 2023-05-18 14:36:56.000000 databar-0.6.0/tests/test_metadata.py
--rw-r--r--   0 sadilet    (502) staff       (20)     4770 2023-05-18 14:36:56.000000 databar-0.6.0/tests/test_table.py
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-25 17:31:17.932638 databar-0.7.0/
+-rw-r--r--   0 sadilet    (502) staff       (20)     1069 2023-05-18 14:36:56.000000 databar-0.7.0/LICENSE
+-rw-r--r--   0 sadilet    (502) staff       (20)       81 2023-05-18 14:36:56.000000 databar-0.7.0/MANIFEST.in
+-rw-r--r--   0 sadilet    (502) staff       (20)     1421 2023-05-25 17:31:17.932704 databar-0.7.0/PKG-INFO
+-rw-r--r--   0 sadilet    (502) staff       (20)     1089 2023-05-18 14:36:56.000000 databar-0.7.0/README.md
+-rw-r--r--   0 sadilet    (502) staff       (20)     1670 2023-05-25 17:31:17.933089 databar-0.7.0/setup.cfg
+-rw-r--r--   0 sadilet    (502) staff       (20)       86 2023-05-18 14:36:56.000000 databar-0.7.0/setup.py
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-25 17:31:17.929734 databar-0.7.0/src/
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-25 17:31:17.931271 databar-0.7.0/src/databar/
+-rw-r--r--   0 sadilet    (502) staff       (20)       96 2023-05-18 14:36:56.000000 databar-0.7.0/src/databar/__init__.py
+-rw-r--r--   0 sadilet    (502) staff       (20)    14258 2023-05-25 17:27:02.000000 databar-0.7.0/src/databar/connection.py
+-rw-r--r--   0 sadilet    (502) staff       (20)     2800 2023-05-18 14:36:56.000000 databar-0.7.0/src/databar/helpers.py
+-rw-r--r--   0 sadilet    (502) staff       (20)     9645 2023-05-18 14:36:56.000000 databar-0.7.0/src/databar/table.py
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-25 17:31:17.932027 databar-0.7.0/src/databar.egg-info/
+-rw-r--r--   0 sadilet    (502) staff       (20)     1421 2023-05-25 17:31:17.000000 databar-0.7.0/src/databar.egg-info/PKG-INFO
+-rw-r--r--   0 sadilet    (502) staff       (20)      377 2023-05-25 17:31:17.000000 databar-0.7.0/src/databar.egg-info/SOURCES.txt
+-rw-r--r--   0 sadilet    (502) staff       (20)        1 2023-05-25 17:31:17.000000 databar-0.7.0/src/databar.egg-info/dependency_links.txt
+-rw-r--r--   0 sadilet    (502) staff       (20)      144 2023-05-25 17:31:17.000000 databar-0.7.0/src/databar.egg-info/requires.txt
+-rw-r--r--   0 sadilet    (502) staff       (20)        8 2023-05-25 17:31:17.000000 databar-0.7.0/src/databar.egg-info/top_level.txt
+drwxr-xr-x   0 sadilet    (502) staff       (20)        0 2023-05-25 17:31:17.932488 databar-0.7.0/tests/
+-rw-r--r--   0 sadilet    (502) staff       (20)        0 2023-05-18 14:36:56.000000 databar-0.7.0/tests/__init__.py
+-rw-r--r--   0 sadilet    (502) staff       (20)      274 2023-05-18 14:36:56.000000 databar-0.7.0/tests/test_metadata.py
+-rw-r--r--   0 sadilet    (502) staff       (20)     4770 2023-05-18 14:36:56.000000 databar-0.7.0/tests/test_table.py
```

### Comparing `databar-0.6.0/LICENSE` & `databar-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databar-0.6.0/PKG-INFO` & `databar-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databar
-Version: 0.6.0
+Version: 0.7.0
 Summary: Official Databar.ai python package
 Home-page: https://github.com/databar-ai/databar-python
 Author: Databar.ai Team
 Author-email: founders@databar.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `databar-0.6.0/README.md` & `databar-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `databar-0.6.0/setup.cfg` & `databar-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 description = Official Databar.ai python package
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = databar
 url = https://github.com/databar-ai/databar-python
-version = 0.6.0
+version = 0.7.0
 
 [mypy]
 check_untyped_defs = True
 
 [mypy-aiohttp.*]
 ignore_missing_imports = True
```

### Comparing `databar-0.6.0/src/databar/connection.py` & `databar-0.7.0/src/databar/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         )
         raise_for_status(response)
         print(tabulate(response.json()["results"], headers="keys", tablefmt="pretty"))
 
     def make_request(
         self,
         endpoint: str,
-        params: Optional[Dict[str, Any]] = None,
+        params: Optional[Union[List[Dict[str, Any]], Dict[str, Any]]] = None,
         rows_or_pages: Optional[int] = None,
         api_key: Optional[int] = None,
         fmt: Literal["df", "json"] = "df",
     ) -> Union[pd.DataFrame, List[Dict[str, Any]], None]:
         if not params:
             params = {}
 
@@ -183,19 +183,24 @@
         response = self._session.post(
             urljoin(self._base_url, "v1/dataset/retrieve/"),
             json={"api": api, "dataset": endpoint},
         )
         raise_for_status(response)
         endpoint_id = response.json()["id"]
 
+        if isinstance(params, dict):
+            params = [params]
+
         response = self._session.post(
             urljoin(self._base_url, "v3/request/create-by-dataset/"),
             json={
                 "source_request": "python-sdk",
-                "rows_params": [{"__eid": "0", **params}],
+                "rows_params": [
+                    {"__eid": str(i), **params[i]} for i in range(len(params))
+                ],
                 "rows_or_pages": rows_or_pages,
                 "authorization": api_key,
                 "dataset": endpoint_id,
             },
         )
         raise_for_status(response)
```

### Comparing `databar-0.6.0/src/databar/helpers.py` & `databar-0.7.0/src/databar/helpers.py`

 * *Files identical despite different names*

### Comparing `databar-0.6.0/src/databar/table.py` & `databar-0.7.0/src/databar/table.py`

 * *Files identical despite different names*

### Comparing `databar-0.6.0/src/databar.egg-info/PKG-INFO` & `databar-0.7.0/src/databar.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databar
-Version: 0.6.0
+Version: 0.7.0
 Summary: Official Databar.ai python package
 Home-page: https://github.com/databar-ai/databar-python
 Author: Databar.ai Team
 Author-email: founders@databar.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `databar-0.6.0/tests/test_table.py` & `databar-0.7.0/tests/test_table.py`

 * *Files identical despite different names*

