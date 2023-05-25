# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.898.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.899.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.898.tar", last modified: Wed May 24 02:02:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.899.tar", last modified: Thu May 25 00:32:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.898.tar` & `tencentcloud-sdk-python-ocr-3.0.899.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113613 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   506230 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-24 02:02:58.000000 tencentcloud-sdk-python-ocr-3.0.898/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 02:02:59.000000 tencentcloud-sdk-python-ocr-3.0.898/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113845 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   507696 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/README.rst` & `tencentcloud-sdk-python-ocr-3.0.899/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1773,15 +1773,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizeTableAccurateOCR(self, request):
-        """本接口支持中英文图片/PDF内常规表格、无线表格、多表格的检测和识别，返回每个单元格的文字内容，支持旋转的表格图片识别，且支持将识别结果保存为 Excel 格式。识别效果比表格识别V2更好，覆盖场景更加广泛，对表格难例场景，如无线表格、嵌套表格（有线表格中包含无线表格）的识别效果均优于表格识别V2。
+        """本接口支持中英文图片/PDF内常规表格、无线表格、多表格的检测和识别，返回每个单元格的文字内容，支持旋转的表格图片识别，且支持将识别结果保存为 Excel 格式。识别效果比表格识别V2更好，覆盖场景更加广泛，对表格难例场景，如无线表格、嵌套表格（有线表格中包含无线表格）的识别效果均优于表格识别V2。点击[立即体验](https://cloud.tencent.com/product/smart-ocr)。
 
         :param request: Request instance for RecognizeTableAccurateOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeTableAccurateOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizeTableAccurateOCRResponse`
 
         """
         try:
@@ -2170,15 +2170,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def VatInvoiceOCR(self, request):
-        """本接口支持增值税专用发票、增值税普通发票、增值税电子发票全字段的内容检测和识别，包括发票代码、发票号码、打印发票代码、打印发票号码、开票日期、合计金额、校验码、税率、合计税额、价税合计、购买方识别号、复核、销售方识别号、开票人、密码区1、密码区2、密码区3、密码区4、发票名称、购买方名称、销售方名称、服务名称、备注、规格型号、数量、单价、金额、税额、收款人等字段。
+        """本接口支持增值税专用发票、增值税普通发票、增值税电子专票、增值税电子普票、电子发票（普通发票）、电子发票（增值税专用发票）德全字段的内容检测和识别，包括发票代码、发票号码、打印发票代码、打印发票号码、开票日期、合计金额、校验码、税率、合计税额、价税合计、购买方识别号、复核、销售方识别号、开票人、密码区1、密码区2、密码区3、密码区4、发票名称、购买方名称、销售方名称、服务名称、备注、规格型号、数量、单价、金额、税额、收款人等字段，点击[立即试用](https://cloud.tencent.com/product/ocr)。
 
         默认接口请求频率限制：10次/秒。
 
         :param request: Request instance for VatInvoiceOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.VatInvoiceOCRResponse`
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7423,19 +7423,22 @@
 
     """
 
     def __init__(self):
         r"""
         :param ImageBase64: 图片/PDF的 Base64 值。
 要求图片/PDF经Base64编码后不超过 7M，分辨率建议600*800以上，支持PNG、JPG、JPEG、BMP、PDF格式。
+图片支持的像素范围：需介于20-10000px之间。
 图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
         :type ImageBase64: str
         :param ImageUrl: 图片/PDF的 Url 地址。
 要求图片/PDF经Base64编码后不超过 7M，分辨率建议600*800以上，支持PNG、JPG、JPEG、BMP、PDF格式。
-图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。非腾讯云存储的 Url 速度和稳定性可能受一定影响。
+图片支持的像素范围：需介于20-10000px之间。
+图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。非腾讯云存储的 Url 速度和稳定
+性可能受一定影响。
         :type ImageUrl: str
         :param PdfPageNumber: 需要识别的PDF页面的对应页码，仅支持PDF单页识别，当上传文件为PDF且IsPdf参数值为true时有效，默认值为1。
         :type PdfPageNumber: int
         """
         self.ImageBase64 = None
         self.ImageUrl = None
         self.PdfPageNumber = None
@@ -11376,38 +11379,66 @@
         :type AmountWithoutTax: str
         :param TaxRate: 税率
         :type TaxRate: str
         :param TaxAmount: 税额
         :type TaxAmount: str
         :param TaxClassifyCode: 税收分类编码
         :type TaxClassifyCode: str
+        :param VehicleType: 运输工具类型
+        :type VehicleType: str
+        :param VehicleBrand: 运输工具牌号
+        :type VehicleBrand: str
+        :param DeparturePlace: 起始地
+        :type DeparturePlace: str
+        :param ArrivalPlace: 到达地
+        :type ArrivalPlace: str
+        :param TransportItemsName: 运输货物名称
+        :type TransportItemsName: str
+        :param ConstructionPlace: 建筑服务发生地
+        :type ConstructionPlace: str
+        :param ConstructionName: 建筑项目名称
+        :type ConstructionName: str
         """
         self.LineNo = None
         self.Name = None
         self.Spec = None
         self.Unit = None
         self.Quantity = None
         self.UnitPrice = None
         self.AmountWithoutTax = None
         self.TaxRate = None
         self.TaxAmount = None
         self.TaxClassifyCode = None
+        self.VehicleType = None
+        self.VehicleBrand = None
+        self.DeparturePlace = None
+        self.ArrivalPlace = None
+        self.TransportItemsName = None
+        self.ConstructionPlace = None
+        self.ConstructionName = None
 
 
     def _deserialize(self, params):
         self.LineNo = params.get("LineNo")
         self.Name = params.get("Name")
         self.Spec = params.get("Spec")
         self.Unit = params.get("Unit")
         self.Quantity = params.get("Quantity")
         self.UnitPrice = params.get("UnitPrice")
         self.AmountWithoutTax = params.get("AmountWithoutTax")
         self.TaxRate = params.get("TaxRate")
         self.TaxAmount = params.get("TaxAmount")
         self.TaxClassifyCode = params.get("TaxClassifyCode")
+        self.VehicleType = params.get("VehicleType")
+        self.VehicleBrand = params.get("VehicleBrand")
+        self.DeparturePlace = params.get("DeparturePlace")
+        self.ArrivalPlace = params.get("ArrivalPlace")
+        self.TransportItemsName = params.get("TransportItemsName")
+        self.ConstructionPlace = params.get("ConstructionPlace")
+        self.ConstructionName = params.get("ConstructionName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11487,19 +11518,21 @@
     """
 
     def __init__(self):
         r"""
         :param ImageBase64: 图片/PDF的 Base64 值。
 支持的文件格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
 支持的图片/PDF大小：所下载文件经Base64编码后不超过 7M。文件下载时间不超过 3 秒。
+支持的图片像素：需介于20-10000px之间。
 输入参数 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
         :type ImageBase64: str
         :param ImageUrl: 图片/PDF的 Url 地址。
 支持的文件格式：PNG、JPG、JPEG、PDF，暂不支持 GIF 格式。
 支持的图片/PDF大小：所下载文件经 Base64 编码后不超过 7M。文件下载时间不超过 3 秒。
+支持的图片像素：需介于20-10000px之间。
 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。
 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
         :type ImageUrl: str
         :param IsPdf: 是否开启PDF识别，默认值为false，开启后可同时支持图片和PDF的识别。
         :type IsPdf: bool
         :param PdfPageNumber: 需要识别的PDF页面的对应页码，仅支持PDF单页识别，当上传文件为PDF且IsPdf参数值为true时有效，默认值为1。
         :type PdfPageNumber: int
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.899/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.898
+Version: 3.0.899
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.898/setup.py` & `tencentcloud-sdk-python-ocr-3.0.899/setup.py`

 * *Files identical despite different names*

