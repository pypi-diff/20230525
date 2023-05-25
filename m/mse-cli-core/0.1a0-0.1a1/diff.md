# Comparing `tmp/mse_cli_core-0.1a0.tar.gz` & `tmp/mse_cli_core-0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a0.tar", last modified: Wed May 24 12:46:22 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a1.tar", last modified: Wed May 24 16:22:47 2023, max compression
```

## Comparing `mse_cli_core-0.1a0.tar` & `mse_cli_core-0.1a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:46:22.502671 mse_cli_core-0.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 12:46:22.502671 mse_cli_core-0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 12:46:22.502671 mse_cli_core-0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:46:22.494670 mse_cli_core-0.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:46:22.498671 mse_cli_core-0.1a0/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:46:22.498671 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 12:46:22.000000 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 12:46:22.000000 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:46:22.000000 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 12:46:22.000000 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 12:46:22.000000 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:46:22.000000 mse_cli_core-0.1a0/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:46:22.502671 mse_cli_core-0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-24 12:45:50.000000 mse_cli_core-0.1a0/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:47.545114 mse_cli_core-0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 16:22:47.545114 mse_cli_core-0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 16:22:47.549114 mse_cli_core-0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:47.541113 mse_cli_core-0.1a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:47.545114 mse_cli_core-0.1a1/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:47.545114 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 16:22:47.000000 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-24 16:22:47.000000 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:22:47.000000 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 16:22:47.000000 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 16:22:47.000000 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:22:47.000000 mse_cli_core-0.1a1/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:47.545114 mse_cli_core-0.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-24 16:22:08.000000 mse_cli_core-0.1a1/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a0/PKG-INFO` & `mse_cli_core-0.1a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli_core
-Version: 0.1a0
+Version: 0.1a1
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a0/setup.cfg` & `mse_cli_core-0.1a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/setup.py` & `mse_cli_core-0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a1/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a1/src/mse_cli_core/bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """mse_cli_core.bootstrap module."""
 
-import time
 from typing import Any, Dict, Optional, Union
 from uuid import UUID
 
 import requests
 from pydantic import BaseModel
 
 from mse_cli_core.base64 import base64url_encode
+from mse_cli_core.clock_tick import ClockTick
 
 
 class ConfigurationPayload(BaseModel):
     """Definition of the bootstrap server payload."""
 
     app_id: UUID
     secrets: Optional[Any]
@@ -32,57 +32,63 @@
 
         if self.code_secret_key:
             data["code_secret_key"] = self.code_secret_key.hex()
 
         return data
 
 
-def send_secrets(url: str, data: Dict[str, Any], verify: Union[bool, str] = True):
+def configure_app(url: str, data: Dict[str, Any], verify: Union[bool, str] = True):
     """Send the secrets to the configuration server."""
     r = requests.post(
         url=url,
         json=data,
         headers={"Content-Type": "application/json"},
         verify=verify,
         timeout=60,
     )
 
     if not r.ok:
         raise Exception(
-            f"Fail to send secrets data (Response {r.status_code} {r.text})"
+            "Fail to send data to the configuration server "
+            f"(Response {r.status_code} {r.text})"
         )
 
 
-def wait_for_conf_server(url: str, verify: Union[bool, str] = True):
+def wait_for_conf_server(clock: ClockTick, url: str, verify: Union[bool, str] = True):
     """Hold on until the configuration server is up and listing."""
-    while not is_waiting_for_secrets(url, verify):
-        time.sleep(5)
+    while clock.tick():
+        if is_waiting_for_secrets(url, verify):
+            break
 
 
 def is_waiting_for_secrets(url: str, verify: Union[bool, str] = True) -> bool:
     """Check whether the configuration server is up."""
     try:
         response = requests.get(url=url, verify=verify, timeout=5)
 
         if response.status_code == 200 and "Mse-Status" in response.headers:
             return True
     except requests.exceptions.SSLError:
         return False
+    except requests.exceptions.ConnectionError:
+        return False
 
     return False
 
 
 def wait_for_app_server(
+    clock: ClockTick,
     url: str,
     healthcheck_endpoint: str,
     verify: Union[bool, str] = True,
 ):
     """Hold on until the configuration server is stopped and the app starts."""
-    while not is_ready(url, healthcheck_endpoint, verify):
-        time.sleep(5)
+    while clock.tick():
+        if is_ready(url, healthcheck_endpoint, verify):
+            break
 
 
 def is_ready(
     url: str, healthcheck_endpoint: str, verify: Union[bool, str] = True
 ) -> bool:
     """Check whether the app server is up."""
     try:
```

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a1/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a1/src/mse_cli_core/enclave.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a1/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a1/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a1/src/mse_cli_core/no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a1/src/mse_cli_core/sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a1/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a1/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli-core
-Version: 0.1a0
+Version: 0.1a1
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a0/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a1/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/tests/test_base64.py` & `mse_cli_core-0.1a1/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/tests/test_boostrap.py` & `mse_cli_core-0.1a1/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/tests/test_ignore_file.py` & `mse_cli_core-0.1a1/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/tests/test_no_sgx_docker.py` & `mse_cli_core-0.1a1/tests/test_no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/tests/test_sgx_docker.py` & `mse_cli_core-0.1a1/tests/test_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a0/tests/test_test_docker.py` & `mse_cli_core-0.1a1/tests/test_test_docker.py`

 * *Files identical despite different names*

