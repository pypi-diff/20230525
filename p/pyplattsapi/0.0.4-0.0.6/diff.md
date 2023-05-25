# Comparing `tmp/pyplattsapi-0.0.4.tar.gz` & `tmp/pyplattsapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplattsapi-0.0.4.tar", last modified: Thu Nov 10 15:19:48 2022, max compression
+gzip compressed data, was "pyplattsapi-0.0.6.tar", last modified: Thu Nov 24 16:20:59 2022, max compression
```

## Comparing `pyplattsapi-0.0.4.tar` & `pyplattsapi-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 15:19:48.027161 pyplattsapi-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-10 15:19:48.027161 pyplattsapi-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 15:19:48.023162 pyplattsapi-0.0.4/pyplattsapi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/global_oil_demand.py
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/locationmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/oil_inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/plattsapicore.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/price_forecast.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/refining_margins_crude_arbitrage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/world_oil_supply.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/pyplattsapi/world_refinery_database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 15:19:48.027161 pyplattsapi-0.0.4/pyplattsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-11-10 15:19:47.000000 pyplattsapi-0.0.4/pyplattsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-10 15:19:47.000000 pyplattsapi-0.0.4/pyplattsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 15:19:47.000000 pyplattsapi-0.0.4/pyplattsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-10 15:19:47.000000 pyplattsapi-0.0.4/pyplattsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-10 15:19:47.000000 pyplattsapi-0.0.4/pyplattsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 15:19:48.027161 pyplattsapi-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 15:19:48.027161 pyplattsapi-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/tests/test_global_oil_demand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/tests/test_plattsapicore.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/tests/test_refining_margins_crude_arbitrage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/tests/test_world_oil_supply.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-11-10 15:19:32.000000 pyplattsapi-0.0.4/tests/test_world_refinery_database.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 16:20:59.020058 pyplattsapi-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2022-11-24 16:20:59.020058 pyplattsapi-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 16:20:59.016059 pyplattsapi-0.0.6/pyplattsapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/global_oil_demand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/locationmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/oil_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/plattsapicore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/price_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/refining_margins_crude_arbitrage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/world_oil_supply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7315 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/pyplattsapi/world_refinery_database.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 16:20:59.016059 pyplattsapi-0.0.6/pyplattsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2022-11-24 16:20:58.000000 pyplattsapi-0.0.6/pyplattsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2022-11-24 16:20:58.000000 pyplattsapi-0.0.6/pyplattsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 16:20:58.000000 pyplattsapi-0.0.6/pyplattsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2022-11-24 16:20:58.000000 pyplattsapi-0.0.6/pyplattsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-24 16:20:58.000000 pyplattsapi-0.0.6/pyplattsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 16:20:59.020058 pyplattsapi-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 16:20:59.020058 pyplattsapi-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/tests/test_global_oil_demand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/tests/test_plattsapicore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/tests/test_refining_margins_crude_arbitrage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/tests/test_world_oil_supply.py
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2022-11-24 16:20:51.000000 pyplattsapi-0.0.6/tests/test_world_refinery_database.py
```

### Comparing `pyplattsapi-0.0.4/pyplattsapi/global_oil_demand.py` & `pyplattsapi-0.0.6/pyplattsapi/global_oil_demand.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/pyplattsapi/locationmap.py` & `pyplattsapi-0.0.6/pyplattsapi/locationmap.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/pyplattsapi/oil_inventory.py` & `pyplattsapi-0.0.6/pyplattsapi/oil_inventory.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/pyplattsapi/plattsapicore.py` & `pyplattsapi-0.0.6/pyplattsapi/plattsapicore.py`

 * *Files 21% similar despite different names*

```diff
@@ -83,8 +83,42 @@
     while nextPage:
         r = generic_api_call_helper(r['@odata.nextLink'], api_name=api_name, params=None)
         d = pd.concat([pd.Series(x) for x in r["value"]], axis=1)
         res = pd.concat([d, res], axis=1)
         nextPage = r['@odata.nextLink'] if '@odata.nextLink' in r else None
 
     res = res.T
-    return res
+    return res
+
+def no_token_api_call(api: str, api_name: str, params: dict):
+    # make call for page 1
+    r = no_token_api_call_helper(api, api_name, params, page=1)
+    max_page = int(r["metadata"]["count"] / 1000)
+    res = pd.concat([pd.Series(x) for x in r["results"]], axis=1)
+    # make call for pages 2 -> n (if needed as determined by max_page)
+    for page in range(2, max_page + 2):
+        time.sleep(0.55) # 2 calls per second allowed
+        r = no_token_api_call_helper(api, api_name, params, page=page)
+        d = pd.concat([pd.Series(x) for x in r["results"]], axis=1)
+        res = pd.concat([d, res], axis=1)
+
+    res = res.T
+    return res
+
+def no_token_api_call_helper(api: str, api_name: str, params: dict, page: int = None):
+    if page is not None:
+        params['page'] = page
+    response = requests.get(
+        url=api, headers=no_token_build_header(api_name), params=params
+    )
+    if response.status_code == 200:
+        return response.json()
+    else:
+        raise HTTPError(url=api, code=response.status_code, msg=response.json()['cause'], hdrs=None, fp=None)
+
+@ttl_cache(ttl=10 * 60)
+def no_token_build_header(api_dataset):
+    header = {
+        "accept": "application/json",
+        "appkey": extract_credential(api_dataset),
+    }
+    return header
```

### Comparing `pyplattsapi-0.0.4/pyplattsapi/price_forecast.py` & `pyplattsapi-0.0.6/pyplattsapi/price_forecast.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/pyplattsapi/refining_margins_crude_arbitrage.py` & `pyplattsapi-0.0.6/pyplattsapi/refining_margins_crude_arbitrage.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/pyplattsapi/world_oil_supply.py` & `pyplattsapi-0.0.6/pyplattsapi/world_oil_supply.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/pyplattsapi.egg-info/SOURCES.txt` & `pyplattsapi-0.0.6/pyplattsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/setup.py` & `pyplattsapi-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="pyplattsapi",
-    version="0.0.4",
+    version="0.0.6",
     author="aeorxc",
     description="Wrapper around Platts API",
     url="https://github.com/aeorxc/pyplattsapi",
     project_urls={
         "Source": "https://github.com/aeorxc/pyplattsapi",
     },
     packages=setuptools.find_packages(),
```

### Comparing `pyplattsapi-0.0.4/tests/test_global_oil_demand.py` & `pyplattsapi-0.0.6/tests/test_global_oil_demand.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/tests/test_plattsapicore.py` & `pyplattsapi-0.0.6/tests/test_plattsapicore.py`

 * *Files identical despite different names*

### Comparing `pyplattsapi-0.0.4/tests/test_world_oil_supply.py` & `pyplattsapi-0.0.6/tests/test_world_oil_supply.py`

 * *Files identical despite different names*

