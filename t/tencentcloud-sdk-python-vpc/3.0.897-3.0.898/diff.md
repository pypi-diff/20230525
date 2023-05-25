# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.897.tar", last modified: Tue May 23 02:36:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.898.tar", last modified: Wed May 24 02:11:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.897.tar` & `tencentcloud-sdk-python-vpc-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332171 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41601 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851409 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:36:05.000000 tencentcloud-sdk-python-vpc-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332227 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41601 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851583 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:11:32.000000 tencentcloud-sdk-python-vpc-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.898/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/README.rst` & `tencentcloud-sdk-python-vpc-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1712,15 +1712,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateVpnGatewaySslServer(self, request):
-        """创建 Server端
+        """本接口（CreateVpnGatewaySslServer）用于创建SSL-VPN Server端。
 
         :param request: Request instance for CreateVpnGatewaySslServer.
         :type request: :class:`tencentcloud.vpc.v20170312.models.CreateVpnGatewaySslServerRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.CreateVpnGatewaySslServerResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5602,37 +5602,37 @@
 class CreateVpnGatewaySslServerRequest(AbstractModel):
     """CreateVpnGatewaySslServer请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param VpnGatewayId: VPN实例ID
+        :param VpnGatewayId: VPN网关实例ID。
         :type VpnGatewayId: str
-        :param SslVpnServerName: SSL_VPN_SERVER 实例名
+        :param SslVpnServerName: SSL-VPN-SERVER 实例名称，长度不超过60个字节。
         :type SslVpnServerName: str
-        :param LocalAddress: 本端地址网段
+        :param LocalAddress: 云端地址（CIDR）列表。
         :type LocalAddress: list of str
-        :param RemoteAddress: 客户端地址网段
+        :param RemoteAddress: 客户端地址网段。
         :type RemoteAddress: str
-        :param SslVpnProtocol: SSL VPN服务端监听协议。当前仅支持 UDP。默认UDP
+        :param SslVpnProtocol: SSL VPN服务端监听协议。当前仅支持 UDP，默认UDP。
         :type SslVpnProtocol: str
-        :param SslVpnPort: SSL VPN服务端监听协议端口。默认1194。
+        :param SslVpnPort: SSL VPN服务端监听协议端口，默认1194。
         :type SslVpnPort: int
-        :param IntegrityAlgorithm: 认证算法。可选 'SHA1', 'MD5', 'NONE'。默认NONE
+        :param IntegrityAlgorithm: 认证算法。可选 'SHA1', 'MD5', 'NONE'，默认NONE。
         :type IntegrityAlgorithm: str
-        :param EncryptAlgorithm: 加密算法。可选 'AES-128-CBC', 'AES-192-CBC', 'AES-256-CBC', 'NONE'。默认NONE
+        :param EncryptAlgorithm: 加密算法。可选 'AES-128-CBC','AES-192-CBC', 'AES-256-CBC', 'NONE'，默认NONE。
         :type EncryptAlgorithm: str
-        :param Compress: 是否支持压缩。当前仅支持不支持压缩。默认False
+        :param Compress: 是否支持压缩。当前仅支持不支持压缩，默认False。
         :type Compress: bool
-        :param SsoEnabled: 是否开启SSO认证
+        :param SsoEnabled: 是否开启SSO认证。默认为False
         :type SsoEnabled: bool
-        :param AccessPolicyEnabled: 是否开启策略访问控制
+        :param AccessPolicyEnabled: 是否开启策略访问控制。默认为False
         :type AccessPolicyEnabled: bool
-        :param SamlData: SAML-DATA
+        :param SamlData: SAML-DATA，开启SSO时传。
         :type SamlData: str
         """
         self.VpnGatewayId = None
         self.SslVpnServerName = None
         self.LocalAddress = None
         self.RemoteAddress = None
         self.SslVpnProtocol = None
@@ -5670,17 +5670,17 @@
 class CreateVpnGatewaySslServerResponse(AbstractModel):
     """CreateVpnGatewaySslServer返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TaskId: 创建SSL-VPN server 异步任务ID
+        :param TaskId: 创建SSL-VPN server 异步任务ID。
         :type TaskId: int
-        :param SslVpnServerId: SSL-VPN server 唯一ID
+        :param SslVpnServerId: SSL-VPN-SERVER 唯一ID。
         :type SslVpnServerId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TaskId = None
         self.SslVpnServerId = None
         self.RequestId = None
@@ -8873,15 +8873,15 @@
         :type SourceRegion: str
         :param DestinationRegion: 目的地域。
         :type DestinationRegion: str
         :param CcnId: 云联网ID。
         :type CcnId: str
         :param CcnUin: 云联网所属账号。
         :type CcnUin: str
-        :param Period: 时间粒度。
+        :param Period: 时间粒度。单位为:秒，如60为60s的时间粒度
         :type Period: int
         :param StartTime: 开始时间。
         :type StartTime: str
         :param EndTime: 结束时间。
         :type EndTime: str
         """
         self.SourceRegion = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.898/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.897'
+__version__ = '3.0.898'
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.898/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.897/setup.py` & `tencentcloud-sdk-python-vpc-3.0.898/setup.py`

 * *Files identical despite different names*

