# Comparing `tmp/toolforge-weld-0.2.1.tar.gz` & `tmp/toolforge-weld-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-0.2.1.tar", last modified: Sun May 21 12:26:23 2023, max compression
+gzip compressed data, was "toolforge-weld-1.0.0.tar", last modified: Thu May 25 08:33:19 2023, max compression
```

## Comparing `toolforge-weld-0.2.1.tar` & `toolforge-weld-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    34524 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      968 2023-05-21 12:25:09.000000 toolforge-weld-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.161054 toolforge-weld-0.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_kubernetes_config.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.161054 toolforge-weld-0.2.1/toolforge_weld/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-05-21 12:25:09.000000 toolforge-weld-0.2.1/toolforge_weld/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3021 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/kubernetes_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/toolforge_weld/logs/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/logs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/logs/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/logs/source.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.161054 toolforge-weld-0.2.1/toolforge_weld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:33:19.274733 toolforge-weld-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-25 08:33:19.274733 toolforge-weld-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 08:33:19.274733 toolforge-weld-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      968 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:33:19.270733 toolforge-weld-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/tests/test_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:33:19.270733 toolforge-weld-1.0.0/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3021 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:33:19.274733 toolforge-weld-1.0.0/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-25 08:33:08.000000 toolforge-weld-1.0.0/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:33:19.274733 toolforge-weld-1.0.0/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-25 08:33:19.000000 toolforge-weld-1.0.0/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-25 08:33:19.000000 toolforge-weld-1.0.0/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:33:19.000000 toolforge-weld-1.0.0/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-25 08:33:19.000000 toolforge-weld-1.0.0/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-25 08:33:19.000000 toolforge-weld-1.0.0/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-0.2.1/LICENSE` & `toolforge-weld-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/PKG-INFO` & `toolforge-weld-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 0.2.1
+Version: 1.0.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-0.2.1/setup.py` & `toolforge-weld-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 
 setup(
     name="toolforge-weld",
-    version="0.2.1",
+    version="1.0.0",
     author="Taavi Väänänen",
     author_email="hi@taavi.wtf",
     license="AGPL-3.0-or-later",
     packages=find_packages(),
     package_data={"toolforge_weld": ["py.typed"]},
     description="Shared Python code for Toolforge infrastructure components",
     long_description=(this_directory / 'README.md').read_text(),
```

### Comparing `toolforge-weld-0.2.1/tests/test_api_client.py` & `toolforge-weld-1.0.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/tests/test_kubernetes_config.py` & `toolforge-weld-1.0.0/tests/test_kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld/api_client.py` & `toolforge-weld-1.0.0/toolforge_weld/api_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 import requests
 import urllib3
 
 import toolforge_weld
 from toolforge_weld.kubernetes_config import Kubeconfig
 
 
+# TODO: these are available natively starting with python 3.9
+# but toolforge bastions run python 3.7 as of this writing
+def _removesuffix(input_string: str, suffix: str) -> str:
+    if suffix and input_string.endswith(suffix):
+        return input_string[: -len(suffix)]  # noqa: E203
+    return input_string
+
+
+def _removeprefix(input_string: str, prefix: str) -> str:
+    if prefix and input_string.startswith(prefix):
+        return input_string[len(prefix) :]  # noqa: E203
+    return input_string
+
+
 class ToolforgeClient:
     """Toolforge API client."""
 
     def __init__(
         self,
         *,
         server: str,
@@ -48,34 +62,30 @@
             if self.exception_handler:
                 raise self.exception_handler(e)
             raise e
 
     def make_kwargs(self, url: str, **kwargs) -> Dict[str, Any]:
         """Setup kwargs for a Requests request."""
         kwargs["url"] = "{}/{}".format(
-            self.server.removesuffix("/"), url.removeprefix("/")
+            _removesuffix(self.server, "/"), _removeprefix(url, "/")
         )
 
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
 
         return kwargs
 
-    def get(self, url, **kwargs) -> Dict[str, Any]:
+    def get(self, url, **kwargs) -> dict[str, Any]:
         """GET request."""
-        r = self._make_request("GET", url, **kwargs)
-        return r.json()
+        return self._make_request("GET", url, **kwargs).json()
 
-    def post(self, url, **kwargs) -> int:
+    def post(self, url, **kwargs) -> dict[str, Any]:
         """POST request."""
-        r = self._make_request("POST", url, **kwargs)
-        return r.status_code
+        return self._make_request("POST", url, **kwargs).json()
 
-    def put(self, url, **kwargs) -> int:
+    def put(self, url, **kwargs) -> dict[str, Any]:
         """PUT request."""
-        r = self._make_request("PUT", url, **kwargs)
-        return r.status_code
+        return self._make_request("PUT", url, **kwargs).json()
 
-    def delete(self, url, **kwargs) -> int:
+    def delete(self, url, **kwargs) -> dict[str, Any]:
         """DELETE request."""
-        r = self._make_request("DELETE", url, **kwargs)
-        return r.status_code
+        return self._make_request("DELETE", url, **kwargs).json()
```

### Comparing `toolforge-weld-0.2.1/toolforge_weld/errors.py` & `toolforge-weld-1.0.0/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld/kubernetes.py` & `toolforge-weld-1.0.0/toolforge_weld/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld/kubernetes_config.py` & `toolforge-weld-1.0.0/toolforge_weld/kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld/logs/__init__.py` & `toolforge-weld-1.0.0/toolforge_weld/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-1.0.0/toolforge_weld/logs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld/logs/source.py` & `toolforge-weld-1.0.0/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.1/toolforge_weld.egg-info/PKG-INFO` & `toolforge-weld-1.0.0/toolforge_weld.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 0.2.1
+Version: 1.0.0
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-0.2.1/toolforge_weld.egg-info/SOURCES.txt` & `toolforge-weld-1.0.0/toolforge_weld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

