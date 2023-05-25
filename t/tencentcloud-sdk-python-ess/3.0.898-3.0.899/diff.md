# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.898.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.899.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.898.tar", last modified: Wed May 24 01:57:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.899.tar", last modified: Thu May 25 00:26:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.898.tar` & `tencentcloud-sdk-python-ess-3.0.899.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23810 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223352 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 01:56:59.000000 tencentcloud-sdk-python-ess-3.0.898/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:57:00.000000 tencentcloud-sdk-python-ess-3.0.898/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23810 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223633 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.898/README.rst` & `tencentcloud-sdk-python-ess-3.0.899/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.898/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,15 +926,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param QrCodeUrl: 二维码下载链接
         :type QrCodeUrl: str
-        :param ExpiredTime: 二维码失效时间 unix 时间戳 精确到秒
+        :param ExpiredTime: 二维码失效时间 UNIX 时间戳 精确到秒
         :type ExpiredTime: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.QrCodeUrl = None
         self.ExpiredTime = None
         self.RequestId = None
@@ -2404,34 +2404,38 @@
         :type AutoSignConfig: :class:`tencentcloud.ess.v20201111.models.AutoSignConfig`
         :param UrlType: 链接类型，空-默认小程序端链接，H5SIGN-h5端链接
         :type UrlType: str
         :param NotifyType: 通知类型，默认不填为不通知开通方，填写 SMS 为短信通知。
         :type NotifyType: str
         :param NotifyAddress: 若上方填写为 SMS，则此处为手机号
         :type NotifyAddress: str
+        :param ExpiredTime: 链接的过期时间，格式为Unix时间戳，不能早于当前时间，且最大为30天。如果不传，默认有效期为7天。
+        :type ExpiredTime: int
         """
         self.Operator = None
         self.SceneKey = None
         self.AutoSignConfig = None
         self.UrlType = None
         self.NotifyType = None
         self.NotifyAddress = None
+        self.ExpiredTime = None
 
 
     def _deserialize(self, params):
         if params.get("Operator") is not None:
             self.Operator = UserInfo()
             self.Operator._deserialize(params.get("Operator"))
         self.SceneKey = params.get("SceneKey")
         if params.get("AutoSignConfig") is not None:
             self.AutoSignConfig = AutoSignConfig()
             self.AutoSignConfig._deserialize(params.get("AutoSignConfig"))
         self.UrlType = params.get("UrlType")
         self.NotifyType = params.get("NotifyType")
         self.NotifyAddress = params.get("NotifyAddress")
+        self.ExpiredTime = params.get("ExpiredTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.898/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.898/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.899/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.898/setup.py` & `tencentcloud-sdk-python-ess-3.0.899/setup.py`

 * *Files identical despite different names*

