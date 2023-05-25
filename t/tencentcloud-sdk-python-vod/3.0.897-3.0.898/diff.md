# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.897.tar", last modified: Tue May 23 02:35:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.898.tar", last modified: Wed May 24 02:11:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.897.tar` & `tencentcloud-sdk-python-vod-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1183641 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:35:58.000000 tencentcloud-sdk-python-vod-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 02:11:24.000000 tencentcloud-sdk-python-vod-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1183869 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:11:24.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 02:11:24.000000 tencentcloud-sdk-python-vod-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:11:25.000000 tencentcloud-sdk-python-vod-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.897/README.rst` & `tencentcloud-sdk-python-vod-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.897/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.898/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13291,24 +13291,30 @@
         :param Height: 视频流高度（或短边）的最大值，取值范围：0 和 [128, 4096]，单位：px。
 <li>当 Width、Height 均为 0，则分辨率取基准分辨率；</li>
 <li>当 Width 为 0，Height 非 0，则 Width 按基准分辨率比例缩放；</li>
 <li>当 Width 非 0，Height 为 0，则 Height 按基准分辨率比例缩放；</li>
 <li>当 Width、Height 均非 0，则分辨率按用户指定。</li>
 默认值：0。
         :type Height: int
+        :param Fps: 视频帧率，取值范围：[0, 100]，单位：Hz。
+当取值为0，将自动为视频设置帧率。
+默认值为 0。
+        :type Fps: int
         """
         self.ResolutionAdaptive = None
         self.Width = None
         self.Height = None
+        self.Fps = None
 
 
     def _deserialize(self, params):
         self.ResolutionAdaptive = params.get("ResolutionAdaptive")
         self.Width = params.get("Width")
         self.Height = params.get("Height")
+        self.Fps = params.get("Fps")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vod-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.897/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.898/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.898/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.897/setup.py` & `tencentcloud-sdk-python-vod-3.0.898/setup.py`

 * *Files identical despite different names*

