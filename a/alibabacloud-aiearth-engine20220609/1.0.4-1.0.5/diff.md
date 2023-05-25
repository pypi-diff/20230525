# Comparing `tmp/alibabacloud_aiearth-engine20220609-1.0.4.tar.gz` & `tmp/alibabacloud_aiearth-engine20220609-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiearth-engine20220609-1.0.4.tar", last modified: Thu Mar 23 08:35:11 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiearth-engine20220609-1.0.5.tar", last modified: Thu May 25 11:51:15 2023, max compression
```

## Comparing `alibabacloud_aiearth-engine20220609-1.0.4.tar` & `alibabacloud_aiearth-engine20220609-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      239 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42313 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609/client.py
--rw-r--r--   0 root         (0) root         (0)    79679 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-03-23 08:35:11.000000 alibabacloud_aiearth-engine20220609-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45127 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/client.py
+-rw-r--r--   0 root         (0) root         (0)    82980 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-05-25 11:51:15.000000 alibabacloud_aiearth-engine20220609-1.0.5/setup.py
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/LICENSE` & `alibabacloud_aiearth-engine20220609-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/PKG-INFO` & `alibabacloud_aiearth-engine20220609-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiearth-engine20220609
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud AIEarth-Engine (20220609) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/README-CN.md` & `alibabacloud_aiearth-engine20220609-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/README.md` & `alibabacloud_aiearth-engine20220609-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609/client.py` & `alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,16 @@
         request: aiearth__engine_20220609_models.DownloadDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> aiearth__engine_20220609_models.DownloadDataResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.band_no):
             body['BandNo'] = request.band_no
+        if not UtilClient.is_unset(request.compress):
+            body['Compress'] = request.compress
         if not UtilClient.is_unset(request.data_id):
             body['DataId'] = request.data_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DownloadData',
@@ -268,14 +270,16 @@
         request: aiearth__engine_20220609_models.DownloadDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> aiearth__engine_20220609_models.DownloadDataResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.band_no):
             body['BandNo'] = request.band_no
+        if not UtilClient.is_unset(request.compress):
+            body['Compress'] = request.compress
         if not UtilClient.is_unset(request.data_id):
             body['DataId'] = request.data_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='DownloadData',
@@ -381,14 +385,84 @@
     async def get_jobs_async(
         self,
         request: aiearth__engine_20220609_models.GetJobsRequest,
     ) -> aiearth__engine_20220609_models.GetJobsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_jobs_with_options_async(request, runtime)
 
+    def get_user_token_with_options(
+        self,
+        request: aiearth__engine_20220609_models.GetUserTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> aiearth__engine_20220609_models.GetUserTokenResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.force_create):
+            body['ForceCreate'] = request.force_create
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetUserToken',
+            version='2022-06-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiearth__engine_20220609_models.GetUserTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_user_token_with_options_async(
+        self,
+        request: aiearth__engine_20220609_models.GetUserTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> aiearth__engine_20220609_models.GetUserTokenResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.force_create):
+            body['ForceCreate'] = request.force_create
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetUserToken',
+            version='2022-06-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiearth__engine_20220609_models.GetUserTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_user_token(
+        self,
+        request: aiearth__engine_20220609_models.GetUserTokenRequest,
+    ) -> aiearth__engine_20220609_models.GetUserTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_user_token_with_options(request, runtime)
+
+    async def get_user_token_async(
+        self,
+        request: aiearth__engine_20220609_models.GetUserTokenRequest,
+    ) -> aiearth__engine_20220609_models.GetUserTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_user_token_with_options_async(request, runtime)
+
     def list_datas_with_options(
         self,
         tmp_req: aiearth__engine_20220609_models.ListDatasRequest,
         runtime: util_models.RuntimeOptions,
     ) -> aiearth__engine_20220609_models.ListDatasResponse:
         UtilClient.validate_model(tmp_req)
         request = aiearth__engine_20220609_models.ListDatasShrinkRequest()
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609/models.py` & `alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -575,38 +575,44 @@
         return self
 
 
 class DownloadDataRequest(TeaModel):
     def __init__(
         self,
         band_no: str = None,
+        compress: bool = None,
         data_id: str = None,
     ):
         self.band_no = band_no
+        self.compress = compress
         self.data_id = data_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.band_no is not None:
             result['BandNo'] = self.band_no
+        if self.compress is not None:
+            result['Compress'] = self.compress
         if self.data_id is not None:
             result['DataId'] = self.data_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('BandNo') is not None:
             self.band_no = m.get('BandNo')
+        if m.get('Compress') is not None:
+            self.compress = m.get('Compress')
         if m.get('DataId') is not None:
             self.data_id = m.get('DataId')
         return self
 
 
 class DownloadDataResponseBody(TeaModel):
     def __init__(
@@ -931,14 +937,124 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetJobsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetUserTokenRequest(TeaModel):
+    def __init__(
+        self,
+        force_create: bool = None,
+    ):
+        self.force_create = force_create
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.force_create is not None:
+            result['ForceCreate'] = self.force_create
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ForceCreate') is not None:
+            self.force_create = m.get('ForceCreate')
+        return self
+
+
+class GetUserTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        expired_at: int = None,
+        request_id: str = None,
+        token: str = None,
+    ):
+        self.expired_at = expired_at
+        self.request_id = request_id
+        self.token = token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.expired_at is not None:
+            result['ExpiredAt'] = self.expired_at
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.token is not None:
+            result['Token'] = self.token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExpiredAt') is not None:
+            self.expired_at = m.get('ExpiredAt')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Token') is not None:
+            self.token = m.get('Token')
+        return self
+
+
+class GetUserTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetUserTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetUserTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListDatasRequest(TeaModel):
     def __init__(
         self,
         cloudage_max: int = None,
         cloudage_min: int = None,
         date_end: str = None,
         date_start: str = None,
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO` & `alibabacloud_aiearth-engine20220609-1.0.5/alibabacloud_aiearth_engine20220609.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiearth-engine20220609
-Version: 1.0.4
+Version: 1.0.5
 Summary: Alibaba Cloud AIEarth-Engine (20220609) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiearth-engine20220609-1.0.4/setup.py` & `alibabacloud_aiearth-engine20220609-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiearth-engine20220609.
 
-Created on 23/03/2023
+Created on 25/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiearth_engine20220609"
 NAME = "alibabacloud_aiearth-engine20220609" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIEarth-Engine (20220609) SDK Library for Python"
```

