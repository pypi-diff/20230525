# Comparing `tmp/alibabacloud_das20200116-2.0.6.tar.gz` & `tmp/alibabacloud_das20200116-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_das20200116-2.0.6.tar", last modified: Tue Dec 28 10:04:08 2021, max compression
+gzip compressed data, was "dist/alibabacloud_das20200116-2.0.7.tar", last modified: Thu Jan 27 07:44:20 2022, max compression
```

## Comparing `alibabacloud_das20200116-2.0.6.tar` & `alibabacloud_das20200116-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/
--rw-r--r--   0 root         (0) root         (0)      443 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116/
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150920 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116/client.py
--rw-r--r--   0 root         (0) root         (0)   293903 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-12-28 10:04:08.000000 alibabacloud_das20200116-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2021-12-28 10:04:07.000000 alibabacloud_das20200116-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 07:44:20.000000 alibabacloud_das20200116-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      497 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-01-27 07:44:20.000000 alibabacloud_das20200116-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 07:44:20.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185246 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116/client.py
+-rw-r--r--   0 root         (0) root         (0)   372230 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 07:44:20.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-01-27 07:44:20.000000 alibabacloud_das20200116-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-01-27 07:44:19.000000 alibabacloud_das20200116-2.0.7/setup.py
```

### Comparing `alibabacloud_das20200116-2.0.6/LICENSE` & `alibabacloud_das20200116-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_das20200116-2.0.6/PKG-INFO` & `alibabacloud_das20200116-2.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_das20200116
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud DAS (20200116) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_das20200116-2.0.6/README-CN.md` & `alibabacloud_das20200116-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_das20200116-2.0.6/README.md` & `alibabacloud_das20200116-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_das20200116-2.0.6/alibabacloud_das20200116/client.py` & `alibabacloud_das20200116-2.0.7/alibabacloud_das20200116/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1796,14 +1796,296 @@
     async def enable_sql_concurrency_control_async(
         self,
         request: das20200116_models.EnableSqlConcurrencyControlRequest,
     ) -> das20200116_models.EnableSqlConcurrencyControlResponse:
         runtime = util_models.RuntimeOptions()
         return await self.enable_sql_concurrency_control_with_options_async(request, runtime)
 
+    def get_async_error_request_list_by_code_with_options(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.error_code):
+            query['ErrorCode'] = request.error_code
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncErrorRequestListByCode',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetAsyncErrorRequestListByCodeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_async_error_request_list_by_code_with_options_async(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.error_code):
+            query['ErrorCode'] = request.error_code
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncErrorRequestListByCode',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetAsyncErrorRequestListByCodeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_async_error_request_list_by_code(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
+    ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_async_error_request_list_by_code_with_options(request, runtime)
+
+    async def get_async_error_request_list_by_code_async(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestListByCodeRequest,
+    ) -> das20200116_models.GetAsyncErrorRequestListByCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_async_error_request_list_by_code_with_options_async(request, runtime)
+
+    def get_async_error_request_stat_by_code_with_options(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncErrorRequestStatByCode',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetAsyncErrorRequestStatByCodeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_async_error_request_stat_by_code_with_options_async(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncErrorRequestStatByCode',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetAsyncErrorRequestStatByCodeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_async_error_request_stat_by_code(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
+    ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_async_error_request_stat_by_code_with_options(request, runtime)
+
+    async def get_async_error_request_stat_by_code_async(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatByCodeRequest,
+    ) -> das20200116_models.GetAsyncErrorRequestStatByCodeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_async_error_request_stat_by_code_with_options_async(request, runtime)
+
+    def get_async_error_request_stat_result_with_options(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        if not UtilClient.is_unset(request.sql_id_list):
+            query['SqlIdList'] = request.sql_id_list
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncErrorRequestStatResult',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetAsyncErrorRequestStatResultResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_async_error_request_stat_result_with_options_async(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        if not UtilClient.is_unset(request.sql_id_list):
+            query['SqlIdList'] = request.sql_id_list
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAsyncErrorRequestStatResult',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetAsyncErrorRequestStatResultResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_async_error_request_stat_result(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
+    ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_async_error_request_stat_result_with_options(request, runtime)
+
+    async def get_async_error_request_stat_result_async(
+        self,
+        request: das20200116_models.GetAsyncErrorRequestStatResultRequest,
+    ) -> das20200116_models.GetAsyncErrorRequestStatResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_async_error_request_stat_result_with_options_async(request, runtime)
+
     def get_auto_resource_optimize_config_with_options(
         self,
         request: das20200116_models.GetAutoResourceOptimizeConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetAutoResourceOptimizeConfigResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2168,14 +2450,112 @@
     async def get_endpoint_switch_task_async(
         self,
         request: das20200116_models.GetEndpointSwitchTaskRequest,
     ) -> das20200116_models.GetEndpointSwitchTaskResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_endpoint_switch_task_with_options_async(request, runtime)
 
+    def get_error_request_sample_with_options(
+        self,
+        request: das20200116_models.GetErrorRequestSampleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetErrorRequestSampleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        if not UtilClient.is_unset(request.sql_id):
+            query['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetErrorRequestSample',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetErrorRequestSampleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_error_request_sample_with_options_async(
+        self,
+        request: das20200116_models.GetErrorRequestSampleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetErrorRequestSampleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.console_context):
+            query['ConsoleContext'] = request.console_context
+        if not UtilClient.is_unset(request.db_name):
+            query['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end):
+            query['End'] = request.end
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_id):
+            query['NodeId'] = request.node_id
+        if not UtilClient.is_unset(request.role):
+            query['Role'] = request.role
+        if not UtilClient.is_unset(request.sql_id):
+            query['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start):
+            query['Start'] = request.start
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetErrorRequestSample',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetErrorRequestSampleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_error_request_sample(
+        self,
+        request: das20200116_models.GetErrorRequestSampleRequest,
+    ) -> das20200116_models.GetErrorRequestSampleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_error_request_sample_with_options(request, runtime)
+
+    async def get_error_request_sample_async(
+        self,
+        request: das20200116_models.GetErrorRequestSampleRequest,
+    ) -> das20200116_models.GetErrorRequestSampleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_error_request_sample_with_options_async(request, runtime)
+
     def get_hdmaliyun_resource_sync_result_with_options(
         self,
         request: das20200116_models.GetHDMAliyunResourceSyncResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetHDMAliyunResourceSyncResultResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2454,14 +2834,476 @@
     async def get_instance_inspections_async(
         self,
         request: das20200116_models.GetInstanceInspectionsRequest,
     ) -> das20200116_models.GetInstanceInspectionsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_instance_inspections_with_options_async(request, runtime)
 
+    def get_query_optimize_data_stats_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataStatsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeDataStatsResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeDataStats',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeDataStatsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_data_stats_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataStatsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeDataStatsResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeDataStats',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeDataStatsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_data_stats(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataStatsRequest,
+    ) -> das20200116_models.GetQueryOptimizeDataStatsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_data_stats_with_options(request, runtime)
+
+    async def get_query_optimize_data_stats_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataStatsRequest,
+    ) -> das20200116_models.GetQueryOptimizeDataStatsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_data_stats_with_options_async(request, runtime)
+
+    def get_query_optimize_data_top_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTopRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeDataTopResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeDataTop',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeDataTopResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_data_top_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTopRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeDataTopResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeDataTop',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeDataTopResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_data_top(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTopRequest,
+    ) -> das20200116_models.GetQueryOptimizeDataTopResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_data_top_with_options(request, runtime)
+
+    async def get_query_optimize_data_top_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTopRequest,
+    ) -> das20200116_models.GetQueryOptimizeDataTopResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_data_top_with_options_async(request, runtime)
+
+    def get_query_optimize_data_trend_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTrendRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeDataTrendResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeDataTrend',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeDataTrendResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_data_trend_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTrendRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeDataTrendResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeDataTrend',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeDataTrendResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_data_trend(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTrendRequest,
+    ) -> das20200116_models.GetQueryOptimizeDataTrendResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_data_trend_with_options(request, runtime)
+
+    async def get_query_optimize_data_trend_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeDataTrendRequest,
+    ) -> das20200116_models.GetQueryOptimizeDataTrendResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_data_trend_with_options_async(request, runtime)
+
+    def get_query_optimize_exec_error_sample_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorSampleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorSampleResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeExecErrorSample',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeExecErrorSampleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_exec_error_sample_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorSampleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorSampleResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeExecErrorSample',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeExecErrorSampleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_exec_error_sample(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorSampleRequest,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorSampleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_exec_error_sample_with_options(request, runtime)
+
+    async def get_query_optimize_exec_error_sample_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorSampleRequest,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorSampleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_exec_error_sample_with_options_async(request, runtime)
+
+    def get_query_optimize_exec_error_stats_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorStatsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorStatsResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeExecErrorStats',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeExecErrorStatsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_exec_error_stats_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorStatsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorStatsResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeExecErrorStats',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeExecErrorStatsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_exec_error_stats(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorStatsRequest,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorStatsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_exec_error_stats_with_options(request, runtime)
+
+    async def get_query_optimize_exec_error_stats_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeExecErrorStatsRequest,
+    ) -> das20200116_models.GetQueryOptimizeExecErrorStatsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_exec_error_stats_with_options_async(request, runtime)
+
+    def get_query_optimize_rule_list_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeRuleListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeRuleListResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeRuleList',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeRuleListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_rule_list_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeRuleListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeRuleListResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeRuleList',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeRuleListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_rule_list(
+        self,
+        request: das20200116_models.GetQueryOptimizeRuleListRequest,
+    ) -> das20200116_models.GetQueryOptimizeRuleListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_rule_list_with_options(request, runtime)
+
+    async def get_query_optimize_rule_list_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeRuleListRequest,
+    ) -> das20200116_models.GetQueryOptimizeRuleListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_rule_list_with_options_async(request, runtime)
+
+    def get_query_optimize_solution_with_options(
+        self,
+        request: das20200116_models.GetQueryOptimizeSolutionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeSolutionResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeSolution',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeSolutionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_query_optimize_solution_with_options_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeSolutionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> das20200116_models.GetQueryOptimizeSolutionResponse:
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQueryOptimizeSolution',
+            version='2020-01-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            das20200116_models.GetQueryOptimizeSolutionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_query_optimize_solution(
+        self,
+        request: das20200116_models.GetQueryOptimizeSolutionRequest,
+    ) -> das20200116_models.GetQueryOptimizeSolutionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_query_optimize_solution_with_options(request, runtime)
+
+    async def get_query_optimize_solution_async(
+        self,
+        request: das20200116_models.GetQueryOptimizeSolutionRequest,
+    ) -> das20200116_models.GetQueryOptimizeSolutionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_query_optimize_solution_with_options_async(request, runtime)
+
     def get_request_diagnosis_page_with_options(
         self,
         request: das20200116_models.GetRequestDiagnosisPageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> das20200116_models.GetRequestDiagnosisPageResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_das20200116-2.0.6/alibabacloud_das20200116/models.py` & `alibabacloud_das20200116-2.0.7/alibabacloud_das20200116/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List
+from typing import Dict, List, Any
 
 
 class AddHDMInstanceRequest(TeaModel):
     def __init__(
         self,
         engine: str = None,
         flush_account: str = None,
@@ -4899,14 +4899,467 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = EnableSqlConcurrencyControlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetAsyncErrorRequestListByCodeRequest(TeaModel):
+    def __init__(
+        self,
+        console_context: str = None,
+        end: str = None,
+        error_code: str = None,
+        instance_id: str = None,
+        node_id: str = None,
+        start: str = None,
+    ):
+        self.console_context = console_context
+        self.end = end
+        self.error_code = error_code
+        self.instance_id = instance_id
+        self.node_id = node_id
+        self.start = start
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
+        if self.console_context is not None:
+            result['ConsoleContext'] = self.console_context
+        if self.end is not None:
+            result['End'] = self.end
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.start is not None:
+            result['Start'] = self.start
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConsoleContext') is not None:
+            self.console_context = m.get('ConsoleContext')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        return self
+
+
+class GetAsyncErrorRequestListByCodeResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAsyncErrorRequestListByCodeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetAsyncErrorRequestListByCodeResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetAsyncErrorRequestListByCodeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetAsyncErrorRequestStatByCodeRequest(TeaModel):
+    def __init__(
+        self,
+        console_context: str = None,
+        db_name: str = None,
+        end: str = None,
+        instance_id: str = None,
+        node_id: str = None,
+        role: str = None,
+        start: str = None,
+    ):
+        self.console_context = console_context
+        self.db_name = db_name
+        self.end = end
+        self.instance_id = instance_id
+        self.node_id = node_id
+        self.role = role
+        self.start = start
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
+        if self.console_context is not None:
+            result['ConsoleContext'] = self.console_context
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end is not None:
+            result['End'] = self.end
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.role is not None:
+            result['Role'] = self.role
+        if self.start is not None:
+            result['Start'] = self.start
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConsoleContext') is not None:
+            self.console_context = m.get('ConsoleContext')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('Role') is not None:
+            self.role = m.get('Role')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        return self
+
+
+class GetAsyncErrorRequestStatByCodeResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAsyncErrorRequestStatByCodeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetAsyncErrorRequestStatByCodeResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetAsyncErrorRequestStatByCodeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetAsyncErrorRequestStatResultRequest(TeaModel):
+    def __init__(
+        self,
+        console_context: str = None,
+        db_name: str = None,
+        end: str = None,
+        instance_id: str = None,
+        node_id: str = None,
+        role: str = None,
+        sql_id_list: str = None,
+        start: str = None,
+    ):
+        self.console_context = console_context
+        self.db_name = db_name
+        self.end = end
+        self.instance_id = instance_id
+        self.node_id = node_id
+        self.role = role
+        self.sql_id_list = sql_id_list
+        self.start = start
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
+        if self.console_context is not None:
+            result['ConsoleContext'] = self.console_context
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end is not None:
+            result['End'] = self.end
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.role is not None:
+            result['Role'] = self.role
+        if self.sql_id_list is not None:
+            result['SqlIdList'] = self.sql_id_list
+        if self.start is not None:
+            result['Start'] = self.start
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConsoleContext') is not None:
+            self.console_context = m.get('ConsoleContext')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('Role') is not None:
+            self.role = m.get('Role')
+        if m.get('SqlIdList') is not None:
+            self.sql_id_list = m.get('SqlIdList')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        return self
+
+
+class GetAsyncErrorRequestStatResultResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAsyncErrorRequestStatResultResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetAsyncErrorRequestStatResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetAsyncErrorRequestStatResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetAutoResourceOptimizeConfigRequest(TeaModel):
     def __init__(
         self,
         access_key: str = None,
         instance_id: str = None,
         signature: str = None,
         uid: str = None,
@@ -5656,14 +6109,171 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = GetEndpointSwitchTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetErrorRequestSampleRequest(TeaModel):
+    def __init__(
+        self,
+        console_context: str = None,
+        db_name: str = None,
+        end: str = None,
+        instance_id: str = None,
+        node_id: str = None,
+        role: str = None,
+        sql_id: str = None,
+        start: str = None,
+    ):
+        self.console_context = console_context
+        self.db_name = db_name
+        self.end = end
+        self.instance_id = instance_id
+        self.node_id = node_id
+        self.role = role
+        self.sql_id = sql_id
+        self.start = start
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
+        if self.console_context is not None:
+            result['ConsoleContext'] = self.console_context
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end is not None:
+            result['End'] = self.end
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_id is not None:
+            result['NodeId'] = self.node_id
+        if self.role is not None:
+            result['Role'] = self.role
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.start is not None:
+            result['Start'] = self.start
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ConsoleContext') is not None:
+            self.console_context = m.get('ConsoleContext')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeId') is not None:
+            self.node_id = m.get('NodeId')
+        if m.get('Role') is not None:
+            self.role = m.get('Role')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        return self
+
+
+class GetErrorRequestSampleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: str = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
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
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetErrorRequestSampleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetErrorRequestSampleResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetErrorRequestSampleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetHDMAliyunResourceSyncResultRequest(TeaModel):
     def __init__(
         self,
         task_id: str = None,
         uid: str = None,
         user_id: str = None,
         context: str = None,
@@ -6387,20 +6997,20 @@
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class GetInstanceInspectionsResponseBodyDataListBaseInspection(TeaModel):
     def __init__(
         self,
-        data: str = None,
+        data: Dict[str, Any] = None,
         end_time: int = None,
         gmt_create: int = None,
         instance: GetInstanceInspectionsResponseBodyDataListBaseInspectionInstance = None,
         score: int = None,
-        score_map: str = None,
+        score_map: Dict[str, Any] = None,
         start_time: int = None,
     ):
         self.data = data
         self.end_time = end_time
         self.gmt_create = gmt_create
         self.instance = instance
         self.score = score
@@ -6621,14 +7231,1926 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = GetInstanceInspectionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetQueryOptimizeDataStatsRequest(TeaModel):
+    def __init__(
+        self,
+        asc: str = None,
+        db_names: str = None,
+        engine: str = None,
+        instance_ids: str = None,
+        keywords: str = None,
+        logical_operator: str = None,
+        only_optimized_sql: str = None,
+        order_by: str = None,
+        page_no: str = None,
+        page_size: str = None,
+        rules: str = None,
+        sql_ids: str = None,
+        tag_names: str = None,
+        time: str = None,
+    ):
+        self.asc = asc
+        self.db_names = db_names
+        self.engine = engine
+        self.instance_ids = instance_ids
+        self.keywords = keywords
+        self.logical_operator = logical_operator
+        self.only_optimized_sql = only_optimized_sql
+        self.order_by = order_by
+        self.page_no = page_no
+        self.page_size = page_size
+        self.rules = rules
+        self.sql_ids = sql_ids
+        self.tag_names = tag_names
+        self.time = time
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
+        if self.asc is not None:
+            result['Asc'] = self.asc
+        if self.db_names is not None:
+            result['DbNames'] = self.db_names
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.instance_ids is not None:
+            result['InstanceIds'] = self.instance_ids
+        if self.keywords is not None:
+            result['Keywords'] = self.keywords
+        if self.logical_operator is not None:
+            result['LogicalOperator'] = self.logical_operator
+        if self.only_optimized_sql is not None:
+            result['OnlyOptimizedSql'] = self.only_optimized_sql
+        if self.order_by is not None:
+            result['OrderBy'] = self.order_by
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.rules is not None:
+            result['Rules'] = self.rules
+        if self.sql_ids is not None:
+            result['SqlIds'] = self.sql_ids
+        if self.tag_names is not None:
+            result['TagNames'] = self.tag_names
+        if self.time is not None:
+            result['Time'] = self.time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Asc') is not None:
+            self.asc = m.get('Asc')
+        if m.get('DbNames') is not None:
+            self.db_names = m.get('DbNames')
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('InstanceIds') is not None:
+            self.instance_ids = m.get('InstanceIds')
+        if m.get('Keywords') is not None:
+            self.keywords = m.get('Keywords')
+        if m.get('LogicalOperator') is not None:
+            self.logical_operator = m.get('LogicalOperator')
+        if m.get('OnlyOptimizedSql') is not None:
+            self.only_optimized_sql = m.get('OnlyOptimizedSql')
+        if m.get('OrderBy') is not None:
+            self.order_by = m.get('OrderBy')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Rules') is not None:
+            self.rules = m.get('Rules')
+        if m.get('SqlIds') is not None:
+            self.sql_ids = m.get('SqlIds')
+        if m.get('TagNames') is not None:
+            self.tag_names = m.get('TagNames')
+        if m.get('Time') is not None:
+            self.time = m.get('Time')
+        return self
+
+
+class GetQueryOptimizeDataStatsResponseBodyDataListRuleList(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        type: str = None,
+    ):
+        self.name = name
+        self.type = type
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetQueryOptimizeDataStatsResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        avg_lock_time: float = None,
+        avg_query_time: float = None,
+        avg_rows_affected: float = None,
+        avg_rows_examined: float = None,
+        avg_rows_sent: float = None,
+        count: int = None,
+        dbname: str = None,
+        instance_id: str = None,
+        max_lock_time: float = None,
+        max_query_time: float = None,
+        max_rows_affected: int = None,
+        max_rows_examined: int = None,
+        max_rows_sent: int = None,
+        psql: str = None,
+        rule_list: List[GetQueryOptimizeDataStatsResponseBodyDataListRuleList] = None,
+        sql_id: str = None,
+        sql_sample: str = None,
+        sql_type: str = None,
+    ):
+        self.avg_lock_time = avg_lock_time
+        self.avg_query_time = avg_query_time
+        self.avg_rows_affected = avg_rows_affected
+        self.avg_rows_examined = avg_rows_examined
+        self.avg_rows_sent = avg_rows_sent
+        self.count = count
+        self.dbname = dbname
+        self.instance_id = instance_id
+        self.max_lock_time = max_lock_time
+        self.max_query_time = max_query_time
+        self.max_rows_affected = max_rows_affected
+        self.max_rows_examined = max_rows_examined
+        self.max_rows_sent = max_rows_sent
+        self.psql = psql
+        self.rule_list = rule_list
+        self.sql_id = sql_id
+        self.sql_sample = sql_sample
+        self.sql_type = sql_type
+
+    def validate(self):
+        if self.rule_list:
+            for k in self.rule_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_lock_time is not None:
+            result['AvgLockTime'] = self.avg_lock_time
+        if self.avg_query_time is not None:
+            result['AvgQueryTime'] = self.avg_query_time
+        if self.avg_rows_affected is not None:
+            result['AvgRowsAffected'] = self.avg_rows_affected
+        if self.avg_rows_examined is not None:
+            result['AvgRowsExamined'] = self.avg_rows_examined
+        if self.avg_rows_sent is not None:
+            result['AvgRowsSent'] = self.avg_rows_sent
+        if self.count is not None:
+            result['Count'] = self.count
+        if self.dbname is not None:
+            result['Dbname'] = self.dbname
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.max_lock_time is not None:
+            result['MaxLockTime'] = self.max_lock_time
+        if self.max_query_time is not None:
+            result['MaxQueryTime'] = self.max_query_time
+        if self.max_rows_affected is not None:
+            result['MaxRowsAffected'] = self.max_rows_affected
+        if self.max_rows_examined is not None:
+            result['MaxRowsExamined'] = self.max_rows_examined
+        if self.max_rows_sent is not None:
+            result['MaxRowsSent'] = self.max_rows_sent
+        if self.psql is not None:
+            result['Psql'] = self.psql
+        result['RuleList'] = []
+        if self.rule_list is not None:
+            for k in self.rule_list:
+                result['RuleList'].append(k.to_map() if k else None)
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_sample is not None:
+            result['SqlSample'] = self.sql_sample
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgLockTime') is not None:
+            self.avg_lock_time = m.get('AvgLockTime')
+        if m.get('AvgQueryTime') is not None:
+            self.avg_query_time = m.get('AvgQueryTime')
+        if m.get('AvgRowsAffected') is not None:
+            self.avg_rows_affected = m.get('AvgRowsAffected')
+        if m.get('AvgRowsExamined') is not None:
+            self.avg_rows_examined = m.get('AvgRowsExamined')
+        if m.get('AvgRowsSent') is not None:
+            self.avg_rows_sent = m.get('AvgRowsSent')
+        if m.get('Count') is not None:
+            self.count = m.get('Count')
+        if m.get('Dbname') is not None:
+            self.dbname = m.get('Dbname')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('MaxLockTime') is not None:
+            self.max_lock_time = m.get('MaxLockTime')
+        if m.get('MaxQueryTime') is not None:
+            self.max_query_time = m.get('MaxQueryTime')
+        if m.get('MaxRowsAffected') is not None:
+            self.max_rows_affected = m.get('MaxRowsAffected')
+        if m.get('MaxRowsExamined') is not None:
+            self.max_rows_examined = m.get('MaxRowsExamined')
+        if m.get('MaxRowsSent') is not None:
+            self.max_rows_sent = m.get('MaxRowsSent')
+        if m.get('Psql') is not None:
+            self.psql = m.get('Psql')
+        self.rule_list = []
+        if m.get('RuleList') is not None:
+            for k in m.get('RuleList'):
+                temp_model = GetQueryOptimizeDataStatsResponseBodyDataListRuleList()
+                self.rule_list.append(temp_model.from_map(k))
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlSample') is not None:
+            self.sql_sample = m.get('SqlSample')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        return self
+
+
+class GetQueryOptimizeDataStatsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeDataStatsResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeDataStatsResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeDataStatsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeDataStatsResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeDataStatsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeDataStatsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeDataStatsResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeDataStatsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetQueryOptimizeDataTopRequest(TeaModel):
+    def __init__(
+        self,
+        engine: str = None,
+        instance_ids: str = None,
+        tag_names: str = None,
+        time: str = None,
+        type: str = None,
+    ):
+        self.engine = engine
+        self.instance_ids = instance_ids
+        self.tag_names = tag_names
+        self.time = time
+        self.type = type
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
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.instance_ids is not None:
+            result['InstanceIds'] = self.instance_ids
+        if self.tag_names is not None:
+            result['TagNames'] = self.tag_names
+        if self.time is not None:
+            result['Time'] = self.time
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('InstanceIds') is not None:
+            self.instance_ids = m.get('InstanceIds')
+        if m.get('TagNames') is not None:
+            self.tag_names = m.get('TagNames')
+        if m.get('Time') is not None:
+            self.time = m.get('Time')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetQueryOptimizeDataTopResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        type: str = None,
+        value: float = None,
+    ):
+        self.instance_id = instance_id
+        self.type = type
+        self.value = value
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
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.type is not None:
+            result['Type'] = self.type
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class GetQueryOptimizeDataTopResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeDataTopResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeDataTopResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeDataTopResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeDataTopResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeDataTopResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeDataTopResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeDataTopResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeDataTopResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetQueryOptimizeDataTrendRequest(TeaModel):
+    def __init__(
+        self,
+        end: str = None,
+        engine: str = None,
+        instance_ids: str = None,
+        start: str = None,
+        tag_names: str = None,
+    ):
+        self.end = end
+        self.engine = engine
+        self.instance_ids = instance_ids
+        self.start = start
+        self.tag_names = tag_names
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
+        if self.end is not None:
+            result['End'] = self.end
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.instance_ids is not None:
+            result['InstanceIds'] = self.instance_ids
+        if self.start is not None:
+            result['Start'] = self.start
+        if self.tag_names is not None:
+            result['TagNames'] = self.tag_names
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('End') is not None:
+            self.end = m.get('End')
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('InstanceIds') is not None:
+            self.instance_ids = m.get('InstanceIds')
+        if m.get('Start') is not None:
+            self.start = m.get('Start')
+        if m.get('TagNames') is not None:
+            self.tag_names = m.get('TagNames')
+        return self
+
+
+class GetQueryOptimizeDataTrendResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        kpi: str = None,
+        timestamp: int = None,
+        value: float = None,
+    ):
+        self.kpi = kpi
+        self.timestamp = timestamp
+        self.value = value
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
+        if self.kpi is not None:
+            result['Kpi'] = self.kpi
+        if self.timestamp is not None:
+            result['Timestamp'] = self.timestamp
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Kpi') is not None:
+            self.kpi = m.get('Kpi')
+        if m.get('Timestamp') is not None:
+            self.timestamp = m.get('Timestamp')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class GetQueryOptimizeDataTrendResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeDataTrendResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeDataTrendResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeDataTrendResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeDataTrendResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeDataTrendResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeDataTrendResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeDataTrendResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeDataTrendResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetQueryOptimizeExecErrorSampleRequest(TeaModel):
+    def __init__(
+        self,
+        engine: str = None,
+        instance_id: str = None,
+        sql_id: str = None,
+        time: str = None,
+    ):
+        self.engine = engine
+        self.instance_id = instance_id
+        self.sql_id = sql_id
+        self.time = time
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
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.time is not None:
+            result['Time'] = self.time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('Time') is not None:
+            self.time = m.get('Time')
+        return self
+
+
+class GetQueryOptimizeExecErrorSampleResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        dbname: str = None,
+        error_code: str = None,
+        orig_host: str = None,
+        sql_id: str = None,
+        sql_text: str = None,
+        timestamp: int = None,
+        user: str = None,
+    ):
+        self.dbname = dbname
+        self.error_code = error_code
+        self.orig_host = orig_host
+        self.sql_id = sql_id
+        self.sql_text = sql_text
+        self.timestamp = timestamp
+        self.user = user
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
+        if self.dbname is not None:
+            result['Dbname'] = self.dbname
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.orig_host is not None:
+            result['OrigHost'] = self.orig_host
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text is not None:
+            result['SqlText'] = self.sql_text
+        if self.timestamp is not None:
+            result['Timestamp'] = self.timestamp
+        if self.user is not None:
+            result['User'] = self.user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Dbname') is not None:
+            self.dbname = m.get('Dbname')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('OrigHost') is not None:
+            self.orig_host = m.get('OrigHost')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlText') is not None:
+            self.sql_text = m.get('SqlText')
+        if m.get('Timestamp') is not None:
+            self.timestamp = m.get('Timestamp')
+        if m.get('User') is not None:
+            self.user = m.get('User')
+        return self
+
+
+class GetQueryOptimizeExecErrorSampleResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeExecErrorSampleResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeExecErrorSampleResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeExecErrorSampleResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeExecErrorSampleResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeExecErrorSampleResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeExecErrorSampleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeExecErrorSampleResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeExecErrorSampleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetQueryOptimizeExecErrorStatsRequest(TeaModel):
+    def __init__(
+        self,
+        asc: str = None,
+        db_names: str = None,
+        engine: str = None,
+        instance_ids: str = None,
+        keywords: str = None,
+        logical_operator: str = None,
+        order_by: str = None,
+        page_no: str = None,
+        page_size: str = None,
+        time: str = None,
+    ):
+        self.asc = asc
+        self.db_names = db_names
+        self.engine = engine
+        self.instance_ids = instance_ids
+        self.keywords = keywords
+        self.logical_operator = logical_operator
+        self.order_by = order_by
+        self.page_no = page_no
+        self.page_size = page_size
+        self.time = time
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
+        if self.asc is not None:
+            result['Asc'] = self.asc
+        if self.db_names is not None:
+            result['DbNames'] = self.db_names
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.instance_ids is not None:
+            result['InstanceIds'] = self.instance_ids
+        if self.keywords is not None:
+            result['Keywords'] = self.keywords
+        if self.logical_operator is not None:
+            result['LogicalOperator'] = self.logical_operator
+        if self.order_by is not None:
+            result['OrderBy'] = self.order_by
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.time is not None:
+            result['Time'] = self.time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Asc') is not None:
+            self.asc = m.get('Asc')
+        if m.get('DbNames') is not None:
+            self.db_names = m.get('DbNames')
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('InstanceIds') is not None:
+            self.instance_ids = m.get('InstanceIds')
+        if m.get('Keywords') is not None:
+            self.keywords = m.get('Keywords')
+        if m.get('LogicalOperator') is not None:
+            self.logical_operator = m.get('LogicalOperator')
+        if m.get('OrderBy') is not None:
+            self.order_by = m.get('OrderBy')
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Time') is not None:
+            self.time = m.get('Time')
+        return self
+
+
+class GetQueryOptimizeExecErrorStatsResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        dbname: str = None,
+        error_code: str = None,
+        error_count: int = None,
+        instance_id: str = None,
+        instance_name: str = None,
+        sql_id: str = None,
+        sql_text: str = None,
+    ):
+        self.dbname = dbname
+        self.error_code = error_code
+        self.error_count = error_count
+        self.instance_id = instance_id
+        self.instance_name = instance_name
+        self.sql_id = sql_id
+        self.sql_text = sql_text
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
+        if self.dbname is not None:
+            result['Dbname'] = self.dbname
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_count is not None:
+            result['ErrorCount'] = self.error_count
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.instance_name is not None:
+            result['InstanceName'] = self.instance_name
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text is not None:
+            result['SqlText'] = self.sql_text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Dbname') is not None:
+            self.dbname = m.get('Dbname')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorCount') is not None:
+            self.error_count = m.get('ErrorCount')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('InstanceName') is not None:
+            self.instance_name = m.get('InstanceName')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlText') is not None:
+            self.sql_text = m.get('SqlText')
+        return self
+
+
+class GetQueryOptimizeExecErrorStatsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeExecErrorStatsResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeExecErrorStatsResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeExecErrorStatsResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeExecErrorStatsResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeExecErrorStatsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeExecErrorStatsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeExecErrorStatsResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeExecErrorStatsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetQueryOptimizeRuleListRequest(TeaModel):
+    def __init__(
+        self,
+        engine: str = None,
+        instance_ids: str = None,
+        tag_names: str = None,
+    ):
+        self.engine = engine
+        self.instance_ids = instance_ids
+        self.tag_names = tag_names
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
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.instance_ids is not None:
+            result['InstanceIds'] = self.instance_ids
+        if self.tag_names is not None:
+            result['TagNames'] = self.tag_names
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('InstanceIds') is not None:
+            self.instance_ids = m.get('InstanceIds')
+        if m.get('TagNames') is not None:
+            self.tag_names = m.get('TagNames')
+        return self
+
+
+class GetQueryOptimizeRuleListResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        rule_id: str = None,
+        type: str = None,
+    ):
+        self.name = name
+        self.rule_id = rule_id
+        self.type = type
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
+class GetQueryOptimizeRuleListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeRuleListResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeRuleListResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeRuleListResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeRuleListResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeRuleListResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeRuleListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeRuleListResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeRuleListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetQueryOptimizeSolutionRequest(TeaModel):
+    def __init__(
+        self,
+        engine: str = None,
+        rule_ids: str = None,
+        sql_id: str = None,
+    ):
+        self.engine = engine
+        self.rule_ids = rule_ids
+        self.sql_id = sql_id
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
+        if self.engine is not None:
+            result['Engine'] = self.engine
+        if self.rule_ids is not None:
+            result['RuleIds'] = self.rule_ids
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Engine') is not None:
+            self.engine = m.get('Engine')
+        if m.get('RuleIds') is not None:
+            self.rule_ids = m.get('RuleIds')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        return self
+
+
+class GetQueryOptimizeSolutionResponseBodyDataList(TeaModel):
+    def __init__(
+        self,
+        level: str = None,
+        rule_id: str = None,
+        solution: str = None,
+        solution_ext: str = None,
+    ):
+        self.level = level
+        self.rule_id = rule_id
+        self.solution = solution
+        self.solution_ext = solution_ext
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
+        if self.level is not None:
+            result['Level'] = self.level
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.solution is not None:
+            result['Solution'] = self.solution
+        if self.solution_ext is not None:
+            result['SolutionExt'] = self.solution_ext
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Level') is not None:
+            self.level = m.get('Level')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('Solution') is not None:
+            self.solution = m.get('Solution')
+        if m.get('SolutionExt') is not None:
+            self.solution_ext = m.get('SolutionExt')
+        return self
+
+
+class GetQueryOptimizeSolutionResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        extra: str = None,
+        list: List[GetQueryOptimizeSolutionResponseBodyDataList] = None,
+        page_no: int = None,
+        page_size: int = None,
+        total: int = None,
+    ):
+        self.extra = extra
+        self.list = list
+        self.page_no = page_no
+        self.page_size = page_size
+        self.total = total
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.extra is not None:
+            result['Extra'] = self.extra
+        result['List'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['List'].append(k.to_map() if k else None)
+        if self.page_no is not None:
+            result['PageNo'] = self.page_no
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Extra') is not None:
+            self.extra = m.get('Extra')
+        self.list = []
+        if m.get('List') is not None:
+            for k in m.get('List'):
+                temp_model = GetQueryOptimizeSolutionResponseBodyDataList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('PageNo') is not None:
+            self.page_no = m.get('PageNo')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class GetQueryOptimizeSolutionResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: GetQueryOptimizeSolutionResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetQueryOptimizeSolutionResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQueryOptimizeSolutionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: GetQueryOptimizeSolutionResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
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
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = GetQueryOptimizeSolutionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetRequestDiagnosisPageRequest(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         instance_id: str = None,
         node_id: str = None,
         page_no: str = None,
```

### Comparing `alibabacloud_das20200116-2.0.6/alibabacloud_das20200116.egg-info/PKG-INFO` & `alibabacloud_das20200116-2.0.7/alibabacloud_das20200116.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-das20200116
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud DAS (20200116) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_das20200116-2.0.6/setup.py` & `alibabacloud_das20200116-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_das20200116.
 
-Created on 28/12/2021
+Created on 27/01/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_das20200116"
 NAME = "alibabacloud_das20200116" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DAS (20200116) SDK Library for Python"
```

