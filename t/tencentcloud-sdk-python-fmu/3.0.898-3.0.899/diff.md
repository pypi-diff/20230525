# Comparing `tmp/tencentcloud-sdk-python-fmu-3.0.898.tar.gz` & `tmp/tencentcloud-sdk-python-fmu-3.0.899.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.898.tar", last modified: Wed May 24 01:57:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-fmu-3.0.899.tar", last modified: Thu May 25 00:27:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-fmu-3.0.898.tar` & `tencentcloud-sdk-python-fmu-3.0.899.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/
--rw-r--r--   0 root         (0) root         (0)    10552 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/fmu_client.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31049 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:57:24.000000 tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/
+-rw-r--r--   0 root         (0) root         (0)    10552 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/fmu_client.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31051 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud_sdk_python_fmu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud_sdk_python_fmu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud_sdk_python_fmu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:27:10.000000 tencentcloud-sdk-python-fmu-3.0.899/tencentcloud_sdk_python_fmu.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/README.rst` & `tencentcloud-sdk-python-fmu-3.0.899/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/__init__.py` & `tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/fmu_client.py` & `tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/fmu_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/errorcodes.py` & `tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud/fmu/v20191213/models.py` & `tencentcloud-sdk-python-fmu-3.0.899/tencentcloud/fmu/v20191213/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Url、Image必须提供一个，如果都提供，只使用 Url。  
 图片存储于腾讯云的Url可保障更高下载速度和稳定性，建议图片存储于腾讯云。  
 非腾讯云存储的Url速度和稳定性可能受一定影响。 
 支持PNG、JPG、JPEG、BMP，不支持 GIF 图片。
         :type Url: str
         :param Whitening: 美白程度，取值范围[0,100]。0不美白，100代表最高程度。默认值30。
         :type Whitening: int
-        :param Smoothing: 磨皮程度，取值范围[0,30]。0不磨皮，30代表最高程度。默认值10。
+        :param Smoothing: 磨皮程度，取值范围[0,100]。0不磨皮，100代表最高程度。默认值10。
         :type Smoothing: int
         :param FaceLifting: 瘦脸程度，取值范围[0,100]。0不瘦脸，100代表最高程度。默认值70。
         :type FaceLifting: int
         :param EyeEnlarging: 大眼程度，取值范围[0,100]。0不大眼，100代表最高程度。默认值70。
         :type EyeEnlarging: int
         :param RspImgType: 返回图像方式（base64 或 url ) ，二选一。url有效期为1天。
         :type RspImgType: str
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.899/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/setup.py` & `tencentcloud-sdk-python-fmu-3.0.899/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-fmu-3.0.898/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO` & `tencentcloud-sdk-python-fmu-3.0.899/tencentcloud_sdk_python_fmu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-fmu
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Fmu SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

