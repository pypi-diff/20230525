# Comparing `tmp/tencentcloud-sdk-python-taf-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-taf-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-taf-3.0.897.tar", last modified: Tue May 23 02:30:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-taf-3.0.898.tar", last modified: Wed May 24 02:05:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-taf-3.0.897.tar` & `tencentcloud-sdk-python-taf-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/
--rw-r--r--   0 root         (0) root         (0)     4808 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/taf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud_sdk_python_taf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud_sdk_python_taf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud_sdk_python_taf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud_sdk_python_taf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/tencentcloud_sdk_python_taf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:30:58.000000 tencentcloud-sdk-python-taf-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/
+-rw-r--r--   0 root         (0) root         (0)     4808 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/taf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud_sdk_python_taf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud_sdk_python_taf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud_sdk_python_taf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud_sdk_python_taf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/tencentcloud_sdk_python_taf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:05:57.000000 tencentcloud-sdk-python-taf-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-taf-3.0.897/README.rst` & `tencentcloud-sdk-python-taf-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-taf-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-taf-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/errorcodes.py` & `tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/models.py` & `tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,24 +288,34 @@
         :type ModelId: int
         :param IsFound: 是否正常返回结果
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFound: int
         :param Score: 返回分值
 注意：此字段可能返回 null，表示取不到有效值。
         :type Score: float
+        :param ModelType: 模型类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModelType: int
+        :param Uid: 入参Uid
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uid: str
         """
         self.ModelId = None
         self.IsFound = None
         self.Score = None
+        self.ModelType = None
+        self.Uid = None
 
 
     def _deserialize(self, params):
         self.ModelId = params.get("ModelId")
         self.IsFound = params.get("IsFound")
         self.Score = params.get("Score")
+        self.ModelType = params.get("ModelType")
+        self.Uid = params.get("Uid")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-taf-3.0.897/tencentcloud/taf/v20200210/taf_client.py` & `tencentcloud-sdk-python-taf-3.0.898/tencentcloud/taf/v20200210/taf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-taf-3.0.897/tencentcloud_sdk_python_taf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-taf-3.0.898/tencentcloud_sdk_python_taf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-taf
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Taf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-taf-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-taf-3.0.898/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-taf
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Taf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-taf-3.0.897/setup.py` & `tencentcloud-sdk-python-taf-3.0.898/setup.py`

 * *Files identical despite different names*

