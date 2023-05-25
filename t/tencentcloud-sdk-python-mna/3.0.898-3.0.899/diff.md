# Comparing `tmp/tencentcloud-sdk-python-mna-3.0.898.tar.gz` & `tmp/tencentcloud-sdk-python-mna-3.0.899.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.898.tar", last modified: Wed May 24 02:01:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mna-3.0.899.tar", last modified: Thu May 25 00:31:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mna-3.0.898.tar` & `tencentcloud-sdk-python-mna-3.0.899.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43030 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/models.py
--rw-r--r--   0 root         (0) root         (0)    12081 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/mna_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud_sdk_python_mna.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/tencentcloud_sdk_python_mna.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:01:43.000000 tencentcloud-sdk-python-mna-3.0.898/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43033 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/models.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/mna_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud_sdk_python_mna.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud_sdk_python_mna.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud_sdk_python_mna.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud_sdk_python_mna.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/tencentcloud_sdk_python_mna.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:31:31.000000 tencentcloud-sdk-python-mna-3.0.899/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:31:32.000000 tencentcloud-sdk-python-mna-3.0.899/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mna-3.0.898/README.rst` & `tencentcloud-sdk-python-mna-3.0.899/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/errorcodes.py` & `tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/models.py` & `tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -953,19 +953,19 @@
 
     """
 
     def __init__(self):
         r"""
         :param NetDetails: 流量详细信息
         :type NetDetails: list of NetDetails
-        :param MaxValue: 查找时间段流量使用最大值（单位：bit）
+        :param MaxValue: 查找时间段流量使用最大值（单位：byte）
         :type MaxValue: float
-        :param AvgValue: 查找时间段流量使用平均值（单位：bit）
+        :param AvgValue: 查找时间段流量使用平均值（单位：byte）
         :type AvgValue: float
-        :param TotalValue: 查找时间段流量使用总量（单位：bit）
+        :param TotalValue: 查找时间段流量使用总量（单位：byte）
         :type TotalValue: float
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.NetDetails = None
         self.MaxValue = None
         self.AvgValue = None
```

### Comparing `tencentcloud-sdk-python-mna-3.0.898/tencentcloud/mna/v20210119/mna_client.py` & `tencentcloud-sdk-python-mna-3.0.899/tencentcloud/mna/v20210119/mna_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mna-3.0.898/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mna-3.0.899/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mna-3.0.898/tencentcloud_sdk_python_mna.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.899/tencentcloud_sdk_python_mna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.898/PKG-INFO` & `tencentcloud-sdk-python-mna-3.0.899/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mna
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Mna SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mna-3.0.898/setup.py` & `tencentcloud-sdk-python-mna-3.0.899/setup.py`

 * *Files identical despite different names*

