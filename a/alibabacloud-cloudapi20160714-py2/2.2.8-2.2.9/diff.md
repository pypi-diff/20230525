# Comparing `tmp/alibabacloud_cloudapi20160714_py2-2.2.8.tar.gz` & `tmp/alibabacloud_cloudapi20160714_py2-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cloudapi20160714_py2-2.2.8.tar", last modified: Fri Sep  9 02:29:10 2022, max compression
+gzip compressed data, was "dist/alibabacloud_cloudapi20160714_py2-2.2.9.tar", last modified: Thu Oct 13 02:23:29 2022, max compression
```

## Comparing `alibabacloud_cloudapi20160714_py2-2.2.8.tar` & `alibabacloud_cloudapi20160714_py2-2.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/
--rw-r--r--   0 root         (0) root         (0)     1431 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714/__init__.py
--rw-r--r--   0 root         (0) root         (0)   228409 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714/client.py
--rw-r--r--   0 root         (0) root         (0)  1111016 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-09 02:29:10.000000 alibabacloud_cloudapi20160714_py2-2.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2022-09-09 02:29:09.000000 alibabacloud_cloudapi20160714_py2-2.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1493 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   241326 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/client.py
+-rw-r--r--   0 root         (0) root         (0)  1160625 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2022-10-13 02:23:29.000000 alibabacloud_cloudapi20160714_py2-2.2.9/setup.py
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/ChangeLog.md` & `alibabacloud_cloudapi20160714_py2-2.2.9/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-09-09 Version: 2.2.8
+- Update SetDomainWebSocketStatus.
+
 2022-09-02 Version: 2.2.7
 - Add input parameters of DescribeApps and DescribeDeployedApis.
 
 2022-08-29 Version: 2.2.6
 - Modify  Api Ram-Meta.
 
 2022-08-01 Version: 2.2.5
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/LICENSE` & `alibabacloud_cloudapi20160714_py2-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/PKG-INFO` & `alibabacloud_cloudapi20160714_py2-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cloudapi20160714_py2
-Version: 2.2.8
+Version: 2.2.9
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/README-CN.md` & `alibabacloud_cloudapi20160714_py2-2.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/README.md` & `alibabacloud_cloudapi20160714_py2-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714/client.py` & `alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,14 +594,82 @@
             self.call_api(params, req, runtime)
         )
 
     def create_backend_model(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_backend_model_with_options(request, runtime)
 
+    def create_dataset_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_name):
+            query['DatasetName'] = request.dataset_name
+        if not UtilClient.is_unset(request.dataset_type):
+            query['DatasetType'] = request.dataset_type
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataset',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.CreateDatasetResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_dataset(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_dataset_with_options(request, runtime)
+
+    def create_dataset_item_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.expired_time):
+            query['ExpiredTime'] = request.expired_time
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.value):
+            query['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatasetItem',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.CreateDatasetItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_dataset_item(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_dataset_item_with_options(request, runtime)
+
     def create_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
@@ -1172,14 +1240,76 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_backend_model(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_backend_model_with_options(request, runtime)
 
+    def delete_dataset_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDataset',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DeleteDatasetResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_dataset(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_dataset_with_options(request, runtime)
+
+    def delete_dataset_item_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.dataset_item_id):
+            query['DatasetItemId'] = request.dataset_item_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDatasetItem',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DeleteDatasetItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_dataset_item(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_dataset_item_with_options(request, runtime)
+
     def delete_domain_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
@@ -2676,14 +2806,148 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_backend_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_backend_list_with_options(request, runtime)
 
+    def describe_dataset_info_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDatasetInfo',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeDatasetInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_dataset_info(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_dataset_info_with_options(request, runtime)
+
+    def describe_dataset_item_info_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.dataset_item_id):
+            query['DatasetItemId'] = request.dataset_item_id
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        if not UtilClient.is_unset(request.value):
+            query['Value'] = request.value
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDatasetItemInfo',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeDatasetItemInfoResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_dataset_item_info(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_dataset_item_info_with_options(request, runtime)
+
+    def describe_dataset_item_list_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.dataset_item_ids):
+            query['DatasetItemIds'] = request.dataset_item_ids
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDatasetItemList',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeDatasetItemListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_dataset_item_list(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_dataset_item_list_with_options(request, runtime)
+
+    def describe_dataset_list_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_ids):
+            query['DatasetIds'] = request.dataset_ids
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDatasetList',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.DescribeDatasetListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_dataset_list(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_dataset_list_with_options(request, runtime)
+
     def describe_deploy_api_task_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.operation_uid):
             query['OperationUid'] = request.operation_uid
         if not UtilClient.is_unset(request.security_token):
             query['SecurityToken'] = request.security_token
@@ -4244,14 +4508,82 @@
             self.call_api(params, req, runtime)
         )
 
     def modify_backend_model(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_backend_model_with_options(request, runtime)
 
+    def modify_dataset_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.dataset_name):
+            query['DatasetName'] = request.dataset_name
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDataset',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.ModifyDatasetResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def modify_dataset(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_dataset_with_options(request, runtime)
+
+    def modify_dataset_item_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.dataset_id):
+            query['DatasetId'] = request.dataset_id
+        if not UtilClient.is_unset(request.dataset_item_id):
+            query['DatasetItemId'] = request.dataset_item_id
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.expired_time):
+            query['ExpiredTime'] = request.expired_time
+        if not UtilClient.is_unset(request.security_token):
+            query['SecurityToken'] = request.security_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDatasetItem',
+            version='2016-07-14',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            cloud_api20160714_models.ModifyDatasetItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def modify_dataset_item(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_dataset_item_with_options(request, runtime)
+
     def modify_instance_spec_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_pay):
             query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714/models.py` & `alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1843,14 +1843,228 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateBackendModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateDatasetRequest(TeaModel):
+    def __init__(self, dataset_name=None, dataset_type=None, security_token=None):
+        self.dataset_name = dataset_name  # type: str
+        self.dataset_type = dataset_type  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatasetRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_name is not None:
+            result['DatasetName'] = self.dataset_name
+        if self.dataset_type is not None:
+            result['DatasetType'] = self.dataset_type
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetName') is not None:
+            self.dataset_name = m.get('DatasetName')
+        if m.get('DatasetType') is not None:
+            self.dataset_type = m.get('DatasetType')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class CreateDatasetResponseBody(TeaModel):
+    def __init__(self, dataset_id=None, request_id=None):
+        self.dataset_id = dataset_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatasetResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateDatasetResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateDatasetResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateDatasetResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDatasetResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateDatasetItemRequest(TeaModel):
+    def __init__(self, dataset_id=None, description=None, expired_time=None, security_token=None, value=None):
+        self.dataset_id = dataset_id  # type: str
+        self.description = description  # type: str
+        self.expired_time = expired_time  # type: str
+        self.security_token = security_token  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatasetItemRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.expired_time is not None:
+            result['ExpiredTime'] = self.expired_time
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ExpiredTime') is not None:
+            self.expired_time = m.get('ExpiredTime')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateDatasetItemResponseBody(TeaModel):
+    def __init__(self, dataset_item_id=None, request_id=None):
+        self.dataset_item_id = dataset_item_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatasetItemResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_item_id is not None:
+            result['DatasetItemId'] = self.dataset_item_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetItemId') is not None:
+            self.dataset_item_id = m.get('DatasetItemId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateDatasetItemResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateDatasetItemResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateDatasetItemResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDatasetItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateInstanceRequest(TeaModel):
     def __init__(self, auto_pay=None, charge_type=None, duration=None, https_policy=None, instance_name=None,
                  instance_spec=None, pricing_cycle=None, token=None, zone_id=None):
         self.auto_pay = auto_pay  # type: bool
         self.charge_type = charge_type  # type: str
         self.duration = duration  # type: int
         self.https_policy = https_policy  # type: str
@@ -3825,14 +4039,203 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteBackendModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteDatasetRequest(TeaModel):
+    def __init__(self, dataset_id=None, security_token=None):
+        self.dataset_id = dataset_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatasetRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DeleteDatasetResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatasetResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteDatasetResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteDatasetResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteDatasetResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteDatasetResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteDatasetItemRequest(TeaModel):
+    def __init__(self, dataset_id=None, dataset_item_id=None, security_token=None):
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_item_id = dataset_item_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatasetItemRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_item_id is not None:
+            result['DatasetItemId'] = self.dataset_item_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetItemId') is not None:
+            self.dataset_item_id = m.get('DatasetItemId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DeleteDatasetItemResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatasetItemResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteDatasetItemResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteDatasetItemResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteDatasetItemResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteDatasetItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteDomainRequest(TeaModel):
     def __init__(self, domain_name=None, group_id=None, security_token=None):
         self.domain_name = domain_name  # type: str
         self.group_id = group_id  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
@@ -7786,27 +8189,28 @@
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class DescribeApiGroupResponseBodyCustomDomainsDomainItem(TeaModel):
     def __init__(self, bind_stage_name=None, certificate_id=None, certificate_name=None, custom_domain_type=None,
                  domain_binding_status=None, domain_cnamestatus=None, domain_legal_status=None, domain_name=None, domain_remark=None,
-                 domain_web_socket_status=None, is_http_redirect_to_https=None, wildcard_domain_patterns=None):
+                 domain_web_socket_status=None, is_http_redirect_to_https=None, wildcard_domain_patterns=None, wss_enable=None):
         self.bind_stage_name = bind_stage_name  # type: str
         self.certificate_id = certificate_id  # type: str
         self.certificate_name = certificate_name  # type: str
         self.custom_domain_type = custom_domain_type  # type: str
         self.domain_binding_status = domain_binding_status  # type: str
         self.domain_cnamestatus = domain_cnamestatus  # type: str
         self.domain_legal_status = domain_legal_status  # type: str
         self.domain_name = domain_name  # type: str
         self.domain_remark = domain_remark  # type: str
         self.domain_web_socket_status = domain_web_socket_status  # type: str
         self.is_http_redirect_to_https = is_http_redirect_to_https  # type: bool
         self.wildcard_domain_patterns = wildcard_domain_patterns  # type: str
+        self.wss_enable = wss_enable  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeApiGroupResponseBodyCustomDomainsDomainItem, self).to_map()
         if _map is not None:
@@ -7833,14 +8237,16 @@
             result['DomainRemark'] = self.domain_remark
         if self.domain_web_socket_status is not None:
             result['DomainWebSocketStatus'] = self.domain_web_socket_status
         if self.is_http_redirect_to_https is not None:
             result['IsHttpRedirectToHttps'] = self.is_http_redirect_to_https
         if self.wildcard_domain_patterns is not None:
             result['WildcardDomainPatterns'] = self.wildcard_domain_patterns
+        if self.wss_enable is not None:
+            result['WssEnable'] = self.wss_enable
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('BindStageName') is not None:
             self.bind_stage_name = m.get('BindStageName')
         if m.get('CertificateId') is not None:
@@ -7861,14 +8267,16 @@
             self.domain_remark = m.get('DomainRemark')
         if m.get('DomainWebSocketStatus') is not None:
             self.domain_web_socket_status = m.get('DomainWebSocketStatus')
         if m.get('IsHttpRedirectToHttps') is not None:
             self.is_http_redirect_to_https = m.get('IsHttpRedirectToHttps')
         if m.get('WildcardDomainPatterns') is not None:
             self.wildcard_domain_patterns = m.get('WildcardDomainPatterns')
+        if m.get('WssEnable') is not None:
+            self.wss_enable = m.get('WssEnable')
         return self
 
 
 class DescribeApiGroupResponseBodyCustomDomains(TeaModel):
     def __init__(self, domain_item=None):
         self.domain_item = domain_item  # type: list[DescribeApiGroupResponseBodyCustomDomainsDomainItem]
 
@@ -14693,14 +15101,85 @@
         if m.get('RoleArn') is not None:
             self.role_arn = m.get('RoleArn')
         if m.get('ServiceName') is not None:
             self.service_name = m.get('ServiceName')
         return self
 
 
+class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfigMockHeaders(TeaModel):
+    def __init__(self, header_name=None, header_value=None):
+        self.header_name = header_name  # type: str
+        self.header_value = header_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfigMockHeaders, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.header_name is not None:
+            result['HeaderName'] = self.header_name
+        if self.header_value is not None:
+            result['HeaderValue'] = self.header_value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HeaderName') is not None:
+            self.header_name = m.get('HeaderName')
+        if m.get('HeaderValue') is not None:
+            self.header_value = m.get('HeaderValue')
+        return self
+
+
+class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig(TeaModel):
+    def __init__(self, mock_headers=None, mock_result=None, mock_status_code=None):
+        self.mock_headers = mock_headers  # type: list[DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfigMockHeaders]
+        self.mock_result = mock_result  # type: str
+        self.mock_status_code = mock_status_code  # type: str
+
+    def validate(self):
+        if self.mock_headers:
+            for k in self.mock_headers:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['MockHeaders'] = []
+        if self.mock_headers is not None:
+            for k in self.mock_headers:
+                result['MockHeaders'].append(k.to_map() if k else None)
+        if self.mock_result is not None:
+            result['MockResult'] = self.mock_result
+        if self.mock_status_code is not None:
+            result['MockStatusCode'] = self.mock_status_code
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.mock_headers = []
+        if m.get('MockHeaders') is not None:
+            for k in m.get('MockHeaders'):
+                temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfigMockHeaders()
+                self.mock_headers.append(temp_model.from_map(k))
+        if m.get('MockResult') is not None:
+            self.mock_result = m.get('MockResult')
+        if m.get('MockStatusCode') is not None:
+            self.mock_status_code = m.get('MockStatusCode')
+        return self
+
+
 class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigOssConfig(TeaModel):
     def __init__(self, bucket_name=None, oss_region_id=None):
         self.bucket_name = bucket_name  # type: str
         self.oss_region_id = oss_region_id  # type: str
 
     def validate(self):
         pass
@@ -14778,28 +15257,31 @@
             self.vpc_scheme = m.get('VpcScheme')
         if m.get('VpcTargetHostName') is not None:
             self.vpc_target_host_name = m.get('VpcTargetHostName')
         return self
 
 
 class DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfig(TeaModel):
-    def __init__(self, event_bridge_config=None, function_compute_config=None, oss_config=None,
+    def __init__(self, event_bridge_config=None, function_compute_config=None, mock_config=None, oss_config=None,
                  service_address=None, type=None, vpc_config=None):
         self.event_bridge_config = event_bridge_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigEventBridgeConfig
         self.function_compute_config = function_compute_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigFunctionComputeConfig
+        self.mock_config = mock_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig
         self.oss_config = oss_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigOssConfig
         self.service_address = service_address  # type: str
         self.type = type  # type: str
         self.vpc_config = vpc_config  # type: DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigVpcConfig
 
     def validate(self):
         if self.event_bridge_config:
             self.event_bridge_config.validate()
         if self.function_compute_config:
             self.function_compute_config.validate()
+        if self.mock_config:
+            self.mock_config.validate()
         if self.oss_config:
             self.oss_config.validate()
         if self.vpc_config:
             self.vpc_config.validate()
 
     def to_map(self):
         _map = super(DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfig, self).to_map()
@@ -14807,14 +15289,16 @@
             return _map
 
         result = dict()
         if self.event_bridge_config is not None:
             result['EventBridgeConfig'] = self.event_bridge_config.to_map()
         if self.function_compute_config is not None:
             result['FunctionComputeConfig'] = self.function_compute_config.to_map()
+        if self.mock_config is not None:
+            result['MockConfig'] = self.mock_config.to_map()
         if self.oss_config is not None:
             result['OssConfig'] = self.oss_config.to_map()
         if self.service_address is not None:
             result['ServiceAddress'] = self.service_address
         if self.type is not None:
             result['Type'] = self.type
         if self.vpc_config is not None:
@@ -14825,14 +15309,17 @@
         m = m or dict()
         if m.get('EventBridgeConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigEventBridgeConfig()
             self.event_bridge_config = temp_model.from_map(m['EventBridgeConfig'])
         if m.get('FunctionComputeConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigFunctionComputeConfig()
             self.function_compute_config = temp_model.from_map(m['FunctionComputeConfig'])
+        if m.get('MockConfig') is not None:
+            temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigMockConfig()
+            self.mock_config = temp_model.from_map(m['MockConfig'])
         if m.get('OssConfig') is not None:
             temp_model = DescribeBackendInfoResponseBodyBackendInfoBackendModelsBackendConfigOssConfig()
             self.oss_config = temp_model.from_map(m['OssConfig'])
         if m.get('ServiceAddress') is not None:
             self.service_address = m.get('ServiceAddress')
         if m.get('Type') is not None:
             self.type = m.get('Type')
@@ -15213,14 +15700,687 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeBackendListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeDatasetInfoRequest(TeaModel):
+    def __init__(self, dataset_id=None, security_token=None):
+        self.dataset_id = dataset_id  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetInfoRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeDatasetInfoResponseBodyDatasetInfo(TeaModel):
+    def __init__(self, created_time=None, dataset_id=None, dataset_name=None, dataset_type=None, modified_time=None):
+        self.created_time = created_time  # type: str
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_name = dataset_name  # type: str
+        self.dataset_type = dataset_type  # type: str
+        self.modified_time = modified_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetInfoResponseBodyDatasetInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.created_time is not None:
+            result['CreatedTime'] = self.created_time
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_name is not None:
+            result['DatasetName'] = self.dataset_name
+        if self.dataset_type is not None:
+            result['DatasetType'] = self.dataset_type
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CreatedTime') is not None:
+            self.created_time = m.get('CreatedTime')
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetName') is not None:
+            self.dataset_name = m.get('DatasetName')
+        if m.get('DatasetType') is not None:
+            self.dataset_type = m.get('DatasetType')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        return self
+
+
+class DescribeDatasetInfoResponseBody(TeaModel):
+    def __init__(self, dataset_info=None, request_id=None):
+        self.dataset_info = dataset_info  # type: DescribeDatasetInfoResponseBodyDatasetInfo
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.dataset_info:
+            self.dataset_info.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetInfoResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_info is not None:
+            result['DatasetInfo'] = self.dataset_info.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetInfo') is not None:
+            temp_model = DescribeDatasetInfoResponseBodyDatasetInfo()
+            self.dataset_info = temp_model.from_map(m['DatasetInfo'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeDatasetInfoResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDatasetInfoResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetInfoResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeDatasetInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDatasetItemInfoRequest(TeaModel):
+    def __init__(self, dataset_id=None, dataset_item_id=None, security_token=None, value=None):
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_item_id = dataset_item_id  # type: str
+        self.security_token = security_token  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemInfoRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_item_id is not None:
+            result['DatasetItemId'] = self.dataset_item_id
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetItemId') is not None:
+            self.dataset_item_id = m.get('DatasetItemId')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeDatasetItemInfoResponseBodyDatasetItemInfo(TeaModel):
+    def __init__(self, created_time=None, dataset_id=None, dataset_item_id=None, description=None,
+                 expired_time=None, modified_time=None, value=None):
+        self.created_time = created_time  # type: str
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_item_id = dataset_item_id  # type: str
+        self.description = description  # type: str
+        self.expired_time = expired_time  # type: str
+        self.modified_time = modified_time  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemInfoResponseBodyDatasetItemInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.created_time is not None:
+            result['CreatedTime'] = self.created_time
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_item_id is not None:
+            result['DatasetItemId'] = self.dataset_item_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.expired_time is not None:
+            result['ExpiredTime'] = self.expired_time
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CreatedTime') is not None:
+            self.created_time = m.get('CreatedTime')
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetItemId') is not None:
+            self.dataset_item_id = m.get('DatasetItemId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ExpiredTime') is not None:
+            self.expired_time = m.get('ExpiredTime')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeDatasetItemInfoResponseBody(TeaModel):
+    def __init__(self, dataset_item_info=None, request_id=None):
+        self.dataset_item_info = dataset_item_info  # type: DescribeDatasetItemInfoResponseBodyDatasetItemInfo
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.dataset_item_info:
+            self.dataset_item_info.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemInfoResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_item_info is not None:
+            result['DatasetItemInfo'] = self.dataset_item_info.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetItemInfo') is not None:
+            temp_model = DescribeDatasetItemInfoResponseBodyDatasetItemInfo()
+            self.dataset_item_info = temp_model.from_map(m['DatasetItemInfo'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeDatasetItemInfoResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDatasetItemInfoResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemInfoResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeDatasetItemInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDatasetItemListRequest(TeaModel):
+    def __init__(self, dataset_id=None, dataset_item_ids=None, page_number=None, page_size=None,
+                 security_token=None):
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_item_ids = dataset_item_ids  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemListRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_item_ids is not None:
+            result['DatasetItemIds'] = self.dataset_item_ids
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetItemIds') is not None:
+            self.dataset_item_ids = m.get('DatasetItemIds')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeDatasetItemListResponseBodyDatasetItemInfoList(TeaModel):
+    def __init__(self, created_time=None, dataset_id=None, dataset_item_id=None, description=None,
+                 expired_time=None, modified_time=None, value=None):
+        self.created_time = created_time  # type: str
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_item_id = dataset_item_id  # type: str
+        self.description = description  # type: str
+        self.expired_time = expired_time  # type: str
+        self.modified_time = modified_time  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemListResponseBodyDatasetItemInfoList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.created_time is not None:
+            result['CreatedTime'] = self.created_time
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_item_id is not None:
+            result['DatasetItemId'] = self.dataset_item_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.expired_time is not None:
+            result['ExpiredTime'] = self.expired_time
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CreatedTime') is not None:
+            self.created_time = m.get('CreatedTime')
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetItemId') is not None:
+            self.dataset_item_id = m.get('DatasetItemId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ExpiredTime') is not None:
+            self.expired_time = m.get('ExpiredTime')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DescribeDatasetItemListResponseBody(TeaModel):
+    def __init__(self, dataset_item_info_list=None, page_number=None, page_size=None, request_id=None,
+                 total_count=None):
+        self.dataset_item_info_list = dataset_item_info_list  # type: list[DescribeDatasetItemListResponseBodyDatasetItemInfoList]
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.dataset_item_info_list:
+            for k in self.dataset_item_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemListResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatasetItemInfoList'] = []
+        if self.dataset_item_info_list is not None:
+            for k in self.dataset_item_info_list:
+                result['DatasetItemInfoList'].append(k.to_map() if k else None)
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.dataset_item_info_list = []
+        if m.get('DatasetItemInfoList') is not None:
+            for k in m.get('DatasetItemInfoList'):
+                temp_model = DescribeDatasetItemListResponseBodyDatasetItemInfoList()
+                self.dataset_item_info_list.append(temp_model.from_map(k))
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDatasetItemListResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDatasetItemListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetItemListResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeDatasetItemListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeDatasetListRequest(TeaModel):
+    def __init__(self, dataset_ids=None, page_number=None, page_size=None, security_token=None):
+        self.dataset_ids = dataset_ids  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetListRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_ids is not None:
+            result['DatasetIds'] = self.dataset_ids
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetIds') is not None:
+            self.dataset_ids = m.get('DatasetIds')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class DescribeDatasetListResponseBodyDatasetInfoList(TeaModel):
+    def __init__(self, created_time=None, dataset_id=None, dataset_name=None, dataset_type=None, modified_time=None):
+        self.created_time = created_time  # type: str
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_name = dataset_name  # type: str
+        self.dataset_type = dataset_type  # type: str
+        self.modified_time = modified_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDatasetListResponseBodyDatasetInfoList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.created_time is not None:
+            result['CreatedTime'] = self.created_time
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_name is not None:
+            result['DatasetName'] = self.dataset_name
+        if self.dataset_type is not None:
+            result['DatasetType'] = self.dataset_type
+        if self.modified_time is not None:
+            result['ModifiedTime'] = self.modified_time
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CreatedTime') is not None:
+            self.created_time = m.get('CreatedTime')
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetName') is not None:
+            self.dataset_name = m.get('DatasetName')
+        if m.get('DatasetType') is not None:
+            self.dataset_type = m.get('DatasetType')
+        if m.get('ModifiedTime') is not None:
+            self.modified_time = m.get('ModifiedTime')
+        return self
+
+
+class DescribeDatasetListResponseBody(TeaModel):
+    def __init__(self, dataset_info_list=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        self.dataset_info_list = dataset_info_list  # type: list[DescribeDatasetListResponseBodyDatasetInfoList]
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.dataset_info_list:
+            for k in self.dataset_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetListResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatasetInfoList'] = []
+        if self.dataset_info_list is not None:
+            for k in self.dataset_info_list:
+                result['DatasetInfoList'].append(k.to_map() if k else None)
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.dataset_info_list = []
+        if m.get('DatasetInfoList') is not None:
+            for k in m.get('DatasetInfoList'):
+                temp_model = DescribeDatasetListResponseBodyDatasetInfoList()
+                self.dataset_info_list.append(temp_model.from_map(k))
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeDatasetListResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeDatasetListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeDatasetListResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeDatasetListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDeployApiTaskRequest(TeaModel):
     def __init__(self, operation_uid=None, security_token=None):
         self.operation_uid = operation_uid  # type: str
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
@@ -25039,14 +26199,219 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyBackendModelResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyDatasetRequest(TeaModel):
+    def __init__(self, dataset_id=None, dataset_name=None, security_token=None):
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_name = dataset_name  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatasetRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_name is not None:
+            result['DatasetName'] = self.dataset_name
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetName') is not None:
+            self.dataset_name = m.get('DatasetName')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class ModifyDatasetResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatasetResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDatasetResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyDatasetResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyDatasetResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyDatasetResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ModifyDatasetItemRequest(TeaModel):
+    def __init__(self, dataset_id=None, dataset_item_id=None, description=None, expired_time=None,
+                 security_token=None):
+        self.dataset_id = dataset_id  # type: str
+        self.dataset_item_id = dataset_item_id  # type: str
+        self.description = description  # type: str
+        self.expired_time = expired_time  # type: str
+        self.security_token = security_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatasetItemRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dataset_id is not None:
+            result['DatasetId'] = self.dataset_id
+        if self.dataset_item_id is not None:
+            result['DatasetItemId'] = self.dataset_item_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.expired_time is not None:
+            result['ExpiredTime'] = self.expired_time
+        if self.security_token is not None:
+            result['SecurityToken'] = self.security_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatasetId') is not None:
+            self.dataset_id = m.get('DatasetId')
+        if m.get('DatasetItemId') is not None:
+            self.dataset_item_id = m.get('DatasetItemId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ExpiredTime') is not None:
+            self.expired_time = m.get('ExpiredTime')
+        if m.get('SecurityToken') is not None:
+            self.security_token = m.get('SecurityToken')
+        return self
+
+
+class ModifyDatasetItemResponseBody(TeaModel):
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatasetItemResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDatasetItemResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyDatasetItemResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyDatasetItemResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyDatasetItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyInstanceSpecRequest(TeaModel):
     def __init__(self, auto_pay=None, instance_id=None, instance_spec=None, modify_action=None,
                  skip_wait_switch=None, token=None):
         self.auto_pay = auto_pay  # type: bool
         self.instance_id = instance_id  # type: str
         self.instance_spec = instance_spec  # type: str
         self.modify_action = modify_action  # type: str
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO` & `alibabacloud_cloudapi20160714_py2-2.2.9/alibabacloud_cloudapi20160714_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cloudapi20160714-py2
-Version: 2.2.8
+Version: 2.2.9
 Summary: Alibaba Cloud CloudAPI (20160714) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cloudapi20160714_py2-2.2.8/setup.py` & `alibabacloud_cloudapi20160714_py2-2.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cloudapi20160714_py2.
 
-Created on 09/09/2022
+Created on 13/10/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cloudapi20160714"
 NAME = "alibabacloud_cloudapi20160714_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud CloudAPI (20160714) SDK Library for Python2"
```

