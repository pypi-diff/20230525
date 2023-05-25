# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.898.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.899.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.898.tar", last modified: Wed May 24 01:57:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.899.tar", last modified: Thu May 25 00:26:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.898.tar` & `tencentcloud-sdk-python-essbasic-3.0.899.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15914 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230929 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-24 01:57:05.000000 tencentcloud-sdk-python-essbasic-3.0.898/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:57:06.000000 tencentcloud-sdk-python-essbasic-3.0.898/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16065 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   231689 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:26:47.000000 tencentcloud-sdk-python-essbasic-3.0.899/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.899/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.898'
+__version__ = '3.0.899'
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,17 @@
 
 # 图片不正确。
 INVALIDPARAMETER_IMAGE = 'InvalidParameter.Image'
 
 # Id不存在或者符合规范。
 INVALIDPARAMETER_INVALIDID = 'InvalidParameter.InvalidId'
 
+# 参数Limit不正确
+INVALIDPARAMETER_LIMIT = 'InvalidParameter.Limit'
+
 # 印章名称长度超出。
 INVALIDPARAMETER_LIMITSEALNAME = 'InvalidParameter.LimitSealName'
 
 # 菜单栏状态非法。
 INVALIDPARAMETER_MENUSTATUS = 'InvalidParameter.MenuStatus'
 
 # 缺少必填参数的值。
@@ -211,14 +214,17 @@
 
 # 姓名不符合要求。
 INVALIDPARAMETER_NAME = 'InvalidParameter.Name'
 
 # 不支持的手机号。
 INVALIDPARAMETER_NONSUPPORTMOBILE = 'InvalidParameter.NonsupportMobile'
 
+# 参数Offset不正确
+INVALIDPARAMETER_OFFSET = 'InvalidParameter.Offset'
+
 # OpenId不合法。
 INVALIDPARAMETER_OPENID = 'InvalidParameter.OpenId'
 
 # OrganizationId不合法。
 INVALIDPARAMETER_ORGANIZATIONID = 'InvalidParameter.OrganizationId'
 
 # 企业名称不合法。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,25 +195,28 @@
         :type FormFields: list of FormField
         :param NeedSignReview: 本企业(发起方企业)是否需要签署审批，true：开启本企业签署审批
         :type NeedSignReview: bool
         :param UserData: 用户流程自定义数据参数
         :type UserData: str
         :param CcInfos: 抄送人信息
         :type CcInfos: list of CcInfo
+        :param NeedCreateReview: 是否需要发起前审核，当指定NeedCreateReview=true，则发起后，需要使用接口：ChannelCreateFlowSignReview，来完成发起前审核，审核通过后，可以继续查看，签署合同
+        :type NeedCreateReview: bool
         """
         self.FlowName = None
         self.FlowType = None
         self.FlowDescription = None
         self.Deadline = None
         self.Unordered = None
         self.IntelligentStatus = None
         self.FormFields = None
         self.NeedSignReview = None
         self.UserData = None
         self.CcInfos = None
+        self.NeedCreateReview = None
 
 
     def _deserialize(self, params):
         self.FlowName = params.get("FlowName")
         self.FlowType = params.get("FlowType")
         self.FlowDescription = params.get("FlowDescription")
         self.Deadline = params.get("Deadline")
@@ -229,14 +232,15 @@
         self.UserData = params.get("UserData")
         if params.get("CcInfos") is not None:
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = CcInfo()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
+        self.NeedCreateReview = params.get("NeedCreateReview")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1862,43 +1866,43 @@
         r"""
         :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param Offset: 查询起始偏移，最大2000
         :type Offset: int
         :param Limit: 查询数量，最大200
         :type Limit: str
-        :param Operator: 操作人信息
-        :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         :param Filters: 查询的关键字段:
-Key:"RoleType",Vales:["1"]查询系统角色，Values:["2]查询自定义角色
+Key:"RoleType",Values:["1"]查询系统角色，Values:["2"]查询自定义角色
 Key:"RoleStatus",Values:["1"]查询启用角色，Values:["2"]查询禁用角色
         :type Filters: list of Filter
+        :param Operator: 操作人信息
+        :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self.Agent = None
         self.Offset = None
         self.Limit = None
-        self.Operator = None
         self.Filters = None
+        self.Operator = None
 
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
-        if params.get("Operator") is not None:
-            self.Operator = UserInfo()
-            self.Operator._deserialize(params.get("Operator"))
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3956,25 +3960,28 @@
         :type DeadLine: int
         :param CustomData: 用户自定义数据
         :type CustomData: str
         :param FlowApproverInfos: 合同(流程)的签署人数组
         :type FlowApproverInfos: list of FlowApproverDetail
         :param CcInfos: 合同(流程)关注方信息列表
         :type CcInfos: list of FlowApproverDetail
+        :param NeedCreateReview: 是否需要发起前审批，当NeedCreateReview为true，表明当前流程是需要发起前审核的合同，可能无法进行查看，签署操作，需要等审核完成后，才可以继续后续流程
+        :type NeedCreateReview: bool
         """
         self.FlowId = None
         self.FlowName = None
         self.FlowType = None
         self.FlowStatus = None
         self.FlowMessage = None
         self.CreateOn = None
         self.DeadLine = None
         self.CustomData = None
         self.FlowApproverInfos = None
         self.CcInfos = None
+        self.NeedCreateReview = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.FlowName = params.get("FlowName")
         self.FlowType = params.get("FlowType")
         self.FlowStatus = params.get("FlowStatus")
@@ -3990,14 +3997,15 @@
                 self.FlowApproverInfos.append(obj)
         if params.get("CcInfos") is not None:
             self.CcInfos = []
             for item in params.get("CcInfos"):
                 obj = FlowApproverDetail()
                 obj._deserialize(item)
                 self.CcInfos.append(obj)
+        self.NeedCreateReview = params.get("NeedCreateReview")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.899/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.899/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.898/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.899/setup.py`

 * *Files identical despite different names*

