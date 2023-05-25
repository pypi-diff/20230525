# Comparing `tmp/eia-0.2.1.tar.gz` & `tmp/eia-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eia-0.2.1.tar", last modified: Thu May 25 03:53:10 2023, max compression
+gzip compressed data, was "eia-0.3.0.tar", last modified: Thu May 25 19:43:48 2023, max compression
```

## Comparing `eia-0.2.1.tar` & `eia-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.144040 eia-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 03:52:33.000000 eia-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 03:53:10.144040 eia-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 03:52:33.000000 eia-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.140040 eia-0.2.1/eia/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 03:52:33.000000 eia-0.2.1/eia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 03:52:33.000000 eia-0.2.1/eia/api_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-05-25 03:52:33.000000 eia-0.2.1/eia/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.140040 eia-0.2.1/eia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 03:53:10.000000 eia-0.2.1/eia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 03:52:33.000000 eia-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:53:10.144040 eia-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:53:10.144040 eia-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-25 03:52:33.000000 eia-0.2.1/tests/test_api_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-25 03:52:33.000000 eia-0.2.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:43:48.757564 eia-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 19:43:15.000000 eia-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 19:43:48.757564 eia-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 19:43:15.000000 eia-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:43:48.757564 eia-0.3.0/eia/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 19:43:15.000000 eia-0.3.0/eia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 19:43:15.000000 eia-0.3.0/eia/api_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-25 19:43:15.000000 eia-0.3.0/eia/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:43:48.757564 eia-0.3.0/eia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 19:43:48.000000 eia-0.3.0/eia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 19:43:48.000000 eia-0.3.0/eia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:43:48.000000 eia-0.3.0/eia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 19:43:48.000000 eia-0.3.0/eia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 19:43:48.000000 eia-0.3.0/eia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 19:43:15.000000 eia-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:43:48.757564 eia-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:43:48.757564 eia-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-25 19:43:15.000000 eia-0.3.0/tests/test_api_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-25 19:43:15.000000 eia-0.3.0/tests/test_client.py
```

### Comparing `eia-0.2.1/LICENSE` & `eia-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eia-0.2.1/PKG-INFO` & `eia-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia
-Version: 0.2.1
+Version: 0.3.0
 Summary: Client for interacting with the EIA API
 Author: James Campbell
 License: MIT License
         
         Copyright (c) 2023 James Campbell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eia-0.2.1/README.md` & `eia-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `eia-0.2.1/eia/api_models.py` & `eia-0.3.0/eia/api_models.py`

 * *Files identical despite different names*

### Comparing `eia-0.2.1/eia/client.py` & `eia-0.3.0/eia/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict, Literal, Union
 import logging
 from pydantic import BaseModel, ValidationError
 import os
 
 import pandas
+from ratelimit import sleep_and_retry, limits
 import requests
 
 from eia.api_models import DatasetInfo, FacetOption, FrequencyType, SeriesInfo
 
 logger = logging.getLogger(__name__)
 
 
@@ -69,51 +70,57 @@
             params_str += f"&{data_str}"
 
         if len(sort_str) > 0:
             params_str += f"&{sort_str}"
 
         return params_str
 
+
 class SessionManager:
     def __init__(self):
         self._init_session()
-    
+
     def _init_session(self):
         self._session = requests.Session()
         self._session.headers.update({"Content-Type": "application/json"})
 
-    def get(self, *args, **kwargs):
-        # TODO: add rate limiting
+    @sleep_and_retry
+    @limits(calls=20, period=60)
+    @limits(calls=900, period=900)
+    def get(self, *args, **kwargs) -> requests.Response:
         retries = 0
         while retries < 3:
             try:
                 return self._session.get(*args, **kwargs)
-            except ConnectionError:
+            except requests.exceptions.ConnectionError:
                 self._init_session()
                 retries += 1
-        raise ConnectionError("Could not connect to EIA API after 3 retries")        
+        raise requests.exceptions.ConnectionError(
+            "Could not connect to EIA API after 3 retries"
+        )
+
 
 class Client:
     """Client for the EIA API.
 
-    Simplifies the process of fetching data from the EIA API by adding typed 
+    Simplifies the process of fetching data from the EIA API by adding typed
     parameters and returning a pandas DataFrame.
     """
 
     def __init__(self, api_key: Union[str, None] = None):
         """Initialize the client with an API key.
 
         Args:
-            api_key (str, optional): API key to use for requests. If no API key is 
-                provided, the client will attempt to use the EIA_API_KEY 
+            api_key (str, optional): API key to use for requests. If no API key is
+                provided, the client will attempt to use the EIA_API_KEY
                 environment variable.
 
 
         Raises:
-            ValueError: If no API key is provided and the EIA_API_KEY environment 
+            ValueError: If no API key is provided and the EIA_API_KEY environment
                 variable is not set.
         """
         if api_key is None:
             api_key = os.getenv("EIA_API_KEY")
         if not api_key:
             raise ValueError("api_key is required to use the EIA API")
         self._api_key = api_key
@@ -158,19 +165,19 @@
         except requests.exceptions.HTTPError:
             raise requests.exceptions.HTTPError(
                 f"Error fetching data from EIA API: {res.json()['error']}"
             )
         return data
 
     def dataset_info(self, dataset: Union[str, None] = None) -> DatasetInfo:
-        """Get information about a dataset, including available series 
+        """Get information about a dataset, including available series
         or child datasets.
 
         Args:
-            dataset (str, optional): The dataset to get information about. If 
+            dataset (str, optional): The dataset to get information about. If
                 no dataset is provided, the root dataset will be returned.
 
         Returns:
             DatasetInfo: Information about the dataset.
         """
         if dataset is None:
             dataset_key = "__root__"
@@ -201,15 +208,15 @@
         return info
 
     def series_info(self, series: str, get_facet_info: bool = True) -> SeriesInfo:
         """Get information about a series, including available facets and facet options.
 
         Args:
             series (str): The series to get information about.
-            get_facet_info (bool, optional): Whether to fetch facet 
+            get_facet_info (bool, optional): Whether to fetch facet
                 information. Defaults to True.
 
         Returns:
             SeriesInfo: Information about the series.
         """
         if series in self._info:
             info = self._info[series]
@@ -292,15 +299,15 @@
                     )
         if offset < 0:
             errors.append(ValueError("Offset must be non-negative"))
 
         if length < 0 or length > 5000:
             errors.append(ValueError("Length must be between 0 and 5000"))
 
-        # Note: we cannot validate sort using the info object, because the 
+        # Note: we cannot validate sort using the info object, because the
         # API does not return sort information
         # TODO: Validate start and end dates
         if len(errors) > 0:
             raise ValueError("\n".join([str(error) for error in errors]))
         return APIParams(
             frequency=frequency,
             data=data,
@@ -325,23 +332,23 @@
         end: Union[str, None] = None,
     ) -> pandas.DataFrame:
         """Get data from the EIA API for a named data series.
 
         Args:
             series (str): The name of the series to fetch data for.
             data (list[str]): The data elements to fetch.
-            frequency (FrequencyType, optional): The frequency of the data to fetch. 
+            frequency (FrequencyType, optional): The frequency of the data to fetch.
                 If not specified, uses the default frequency.
-            facets (list[FacetDefinition], optional): The facets to fetch. If not 
+            facets (list[FacetDefinition], optional): The facets to fetch. If not
                 specified, fetches all facets.
-            sort (list[SortDirective], optional): The sort directives to use. If not 
+            sort (list[SortDirective], optional): The sort directives to use. If not
                 specified, uses the default sort order.
-            offset (int, optional): The offset to use when fetching data. 
+            offset (int, optional): The offset to use when fetching data.
                 Defaults to 0.
-            length (int, optional): The number of data points to fetch. 
+            length (int, optional): The number of data points to fetch.
                 Defaults to None, which will fetch all available data.
             start (str, optional): The start date to fetch data for. Defaults to None.
             end (str, optional): The end date to fetch data for. Defaults to None.
 
         Returns:
             pandas.DataFrame: A dataframe containing the requested data.
 
@@ -376,23 +383,23 @@
         if length is None:
             length = 5000
         check_for_more_results = True
         dfs = []
         while check_for_more_results:
             logger.info(f"Fetching data for {series} with offset {offset}")
             params = self._build_api_params(
-                info, 
-                frequency, 
-                data, 
-                facets, 
-                sort, # type: ignore
-                offset, 
-                length, 
-                start, 
-                end
+                info,
+                frequency,
+                data,
+                facets,
+                sort,  # type: ignore
+                offset,
+                length,
+                start,
+                end,
             )
             df = self._get_data(series, params=params, show_warnings=False)
             if len(df) < length:
                 check_for_more_results = False
             else:
                 offset += len(df)
             dfs.append(df)
```

### Comparing `eia-0.2.1/eia.egg-info/PKG-INFO` & `eia-0.3.0/eia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eia
-Version: 0.2.1
+Version: 0.3.0
 Summary: Client for interacting with the EIA API
 Author: James Campbell
 License: MIT License
         
         Copyright (c) 2023 James Campbell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `eia-0.2.1/pyproject.toml` & `eia-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eia"
-version = "0.2.1"
+version = "0.3.0"
 description = "Client for interacting with the EIA API"
 authors = [
   { name = "James Campbell" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
@@ -16,15 +16,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "requests >= 2.26.0",
     "pandas >= 1.0",
-    "pydantic >= 1.7"
+    "pydantic >= 1.7",
+    "ratelimit >= 2.2.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jcampbell/eia"
 "Bug Tracker" = "https://github.com/jcampbell/eia/issues"
 
 [options]
```

### Comparing `eia-0.2.1/tests/test_api_params.py` & `eia-0.3.0/tests/test_api_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,12 @@
         offset=10,
         length=100,
         start="2020-01-01",
         end="2020-01-31",
     )
     assert (
         params.query_str
-        == (
-            "frequency=weekly&offset=10&length=100&start=2020-01-01&end=2020-01-31"
-            "&facets[stateid][0]=AK&facets[stateid][1]=AL&data[0]=price&data[1]=volume"
-            "&sort[0][column]=date&sort[0][direction]=desc&sort[1][column]=stateid&"
-            "sort[1][direction]=asc"
-        )
+        == "frequency=weekly&offset=10&length=100&start=2020-01-01&end=2020-01-31"
+        "&facets[stateid][0]=AK&facets[stateid][1]=AL&data[0]=price&data[1]=volume"
+        "&sort[0][column]=date&sort[0][direction]=desc&sort[1][column]=stateid&"
+        "sort[1][direction]=asc"
     )
```

### Comparing `eia-0.2.1/tests/test_client.py` & `eia-0.3.0/tests/test_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,124 @@
 from typing import List, Dict
 import pytest
-from unittest.mock import MagicMock, patch
+from unittest.mock import MagicMock
 
 import urllib.parse
 
 import requests
 
 from eia import Client
 from eia.api_models import DataInfo, DatasetInfo, FacetInfo, FrequencyInfo, SeriesInfo
 
+
 def mock_get(*args, **kwargs):
     class MockResponse:
         def __init__(self, json_data: Dict, status_code: int):
             self.json_data = json_data
             self.status_code = status_code
 
         def raise_for_status(self):
             if self.status_code != 200:
                 raise requests.HTTPError("failed raise for status")
 
         def json(self):
             return self.json_data
 
     parsed = urllib.parse.urlparse(args[0])
-    path = parsed.path 
+    path = parsed.path
     if path == "/v2/test_series":
-        return MockResponse({"response": SeriesInfo(
-            id="test_series", 
-            description="Test Series", 
-            frequency=[FrequencyInfo(id="weekly", description="Weekly", query="W", format="YYYY-MM-DD")], 
-            facets=[FacetInfo(id="facetid", description="basic_facet")],
-            facet_options=None,
-            data={"value": DataInfo(alias=None, units=None)},
-            startPeriod="2023-05-24",
-            endPeriod="2023-05-24",
-            defaultDateFormat="YYYY-MM-DD",
-            defaultFrequency="weekly"
-        ).dict()}, 200)
+        return MockResponse(
+            {
+                "response": SeriesInfo(
+                    id="test_series",
+                    description="Test Series",
+                    frequency=[
+                        FrequencyInfo(
+                            id="weekly",
+                            description="Weekly",
+                            query="W",
+                            format="YYYY-MM-DD",
+                        )
+                    ],
+                    facets=[FacetInfo(id="facetid", description="basic_facet")],
+                    facet_options=None,
+                    data={"value": DataInfo(alias=None, units=None)},
+                    startPeriod="2023-05-24",
+                    endPeriod="2023-05-24",
+                    defaultDateFormat="YYYY-MM-DD",
+                    defaultFrequency="weekly",
+                ).dict()
+            },
+            200,
+        )
 
     elif path == "/v2/test_series/facet/facetid":
         return MockResponse(
-            {"response": {
-                "facets": [
-                    {"id": "facetid", "name": "test_facet"}
-                ]
-            }}, 200
+            {"response": {"facets": [{"id": "facetid", "name": "test_facet"}]}}, 200
         )
 
     elif path == "/v2/test_series/data/":
+        return MockResponse({"response": {"data": []}}, 200)
+
+    elif path == "/v2/test_dataset":
         return MockResponse(
-            {"response": {"data": []}}, 200
+            {
+                "response": DatasetInfo(
+                    id="test_dataset",
+                    name="test_dataset",
+                    description="test_dataset",
+                    routes=[],
+                ).dict()
+            },
+            200,
         )
-    
-    elif path == "/v2/test_dataset":
-        return MockResponse({"response": DatasetInfo(id="test_dataset", name="test_dataset", description="test_dataset", routes=[]).dict()}, 200)
 
     else:
         return MockResponse({"response": [], "error": "unrecognized path"}, 404)
 
 
-
-
 @pytest.fixture
 def mock_client():
     client = Client()
     client._session.get = MagicMock(side_effect=mock_get)
     return client
 
+
 def _get_request_path(*, args: List[str], kwargs: Dict[str, str]) -> str:
     if "url" in kwargs:
         url = kwargs["url"]
     else:
         url = args[0]
     parsed = urllib.parse.urlparse(url)
     return parsed.path
 
+
 def test_get_data_no_fetch_facets(mock_client):
     client = mock_client
     client.get("test_series", frequency="weekly", data=["value"])
-    paths_requested = [_get_request_path(args=call_info[0], kwargs=call_info[1]) for call_info in client._session.get.call_args_list]
+    paths_requested = [
+        _get_request_path(args=call_info[0], kwargs=call_info[1])
+        for call_info in client._session.get.call_args_list
+    ]
     assert len(paths_requested) == 2
     assert "/v2/test_series" in paths_requested
     assert "/v2/test_series/facets/facetid" not in paths_requested
     assert "/v2/test_series/data/" in paths_requested
 
+
 def test_get_series_info_fetch_facets(mock_client):
     client = mock_client
     client.series_info("test_series")
-    paths_requested = [_get_request_path(args=call_info[0], kwargs=call_info[1]) for call_info in client._session.get.call_args_list]
+    paths_requested = [
+        _get_request_path(args=call_info[0], kwargs=call_info[1])
+        for call_info in client._session.get.call_args_list
+    ]
     assert len(paths_requested) == 2
     assert "/v2/test_series" in paths_requested
     assert "/v2/test_series/facet/facetid" in paths_requested
 
+
 def test_invalid_path(mock_client):
     client = mock_client
     with pytest.raises(requests.HTTPError) as e:
         client.get("invalid_path", frequency="weekly", data=["value"])
     assert "unrecognized path" in str(e.value)
```

