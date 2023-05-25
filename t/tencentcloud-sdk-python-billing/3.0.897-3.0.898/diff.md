# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.897.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.898.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.897.tar", last modified: Tue May 23 02:14:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.898.tar", last modified: Wed May 24 01:45:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.897.tar` & `tencentcloud-sdk-python-billing-3.0.898.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)     2904 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   149520 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)    20134 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:14:29.000000 tencentcloud-sdk-python-billing-3.0.897/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155292 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)    20134 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-24 01:45:58.000000 tencentcloud-sdk-python-billing-3.0.898/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.897/README.rst` & `tencentcloud-sdk-python-billing-3.0.898/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.897/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.898/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,59 +21,59 @@
 class ActionSummaryOverviewItem(AbstractModel):
     """按交易类型汇总消费详情
 
     """
 
     def __init__(self):
         r"""
-        :param ActionType: 交易类型：包年包月新购/续费/升降配/退款、按量计费扣费、调账补偿/扣费等类型
+        :param ActionType: 交易类型编码
         :type ActionType: str
-        :param ActionTypeName: 交易类型名称
+        :param ActionTypeName: 交易类型：如包年包月新购、包年包月续费、按量计费扣费等类型
         :type ActionTypeName: str
-        :param RealTotalCost: 实际花费
-        :type RealTotalCost: str
         :param RealTotalCostRatio: 费用所占百分比，两位小数
         :type RealTotalCostRatio: str
-        :param CashPayAmount: 现金金额
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
         :param BillMonth: 账单月份，格式2019-08
         :type BillMonth: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
-        :param TransferPayAmount: 分成金金额
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TransferPayAmount: str
         """
         self.ActionType = None
         self.ActionTypeName = None
-        self.RealTotalCost = None
         self.RealTotalCostRatio = None
+        self.RealTotalCost = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
+        self.TransferPayAmount = None
         self.BillMonth = None
         self.TotalCost = None
-        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.ActionType = params.get("ActionType")
         self.ActionTypeName = params.get("ActionTypeName")
-        self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
+        self.RealTotalCost = params.get("RealTotalCost")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         self.BillMonth = params.get("BillMonth")
         self.TotalCost = params.get("TotalCost")
-        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -110,66 +110,66 @@
 class BillDetail(AbstractModel):
     """账单明细数据对象
 
     """
 
     def __init__(self):
         r"""
-        :param BusinessCodeName: 产品名称：云产品大类，如云服务器CVM、云数据库MySQL
+        :param BusinessCodeName: 产品名称：用户所采购的各类云产品，例如：云服务器 CVM
         :type BusinessCodeName: str
-        :param ProductCodeName: 子产品名称：云产品子类，如云服务器CVM-标准型S1
+        :param ProductCodeName: 子产品名称：用户采购的具体产品细分类型，例如：云服务器 CVM-标准型 S1
         :type ProductCodeName: str
-        :param PayModeName: 计费模式：包年包月和按量计费
+        :param PayModeName: 计费模式：资源的计费模式，区分为包年包月和按量计费
         :type PayModeName: str
-        :param ProjectName: 项目:资源所属项目
+        :param ProjectName: 项目名称：资源归属的项目，用户在控制台给资源自主分配项目，未分配则是默认项目
         :type ProjectName: str
-        :param RegionName: 区域：资源所属地域，如华南地区（广州）
+        :param RegionName: 地域：资源所属地域，如华南地区（广州）
         :type RegionName: str
         :param ZoneName: 可用区：资源所属可用区，如广州三区
         :type ZoneName: str
-        :param ResourceId: 资源实例ID
+        :param ResourceId: 资源 ID：账单中出账对象 ID，不同产品因资源形态不同，资源内容不完全相同，如云服务器 CVM 为对应的实例 ID
         :type ResourceId: str
-        :param ResourceName: 实例名称
+        :param ResourceName: 资源别名：用户在控制台为资源设置的名称，如果未设置，则默认为空
         :type ResourceName: str
-        :param ActionTypeName: 交易类型
+        :param ActionTypeName: 交易类型，如包年包月新购、包年包月续费、按量计费扣费等类型
         :type ActionTypeName: str
-        :param OrderId: 订单ID
+        :param OrderId: 订单ID：包年包月计费模式下订购的订单号
         :type OrderId: str
-        :param BillId: 交易ID
+        :param BillId: 交易ID：结算扣费单号
         :type BillId: str
-        :param PayTime: 扣费时间
+        :param PayTime: 扣费时间：结算扣费时间
         :type PayTime: str
-        :param FeeBeginTime: 开始使用时间
+        :param FeeBeginTime: 开始使用时间：产品服务开始使用时间
         :type FeeBeginTime: str
-        :param FeeEndTime: 结束使用时间
+        :param FeeEndTime: 结束使用时间：产品服务结束使用时间
         :type FeeEndTime: str
         :param ComponentSet: 组件列表
         :type ComponentSet: list of BillDetailComponent
-        :param PayerUin: 支付者UIN
+        :param PayerUin: 支付者UIN：支付者的账号 ID，账号 ID 是用户在腾讯云的唯一账号标识
         :type PayerUin: str
-        :param OwnerUin: 使用者UIN
+        :param OwnerUin: 使用者UIN：实际使用资源的账号 ID
         :type OwnerUin: str
-        :param OperateUin: 操作者UIN
+        :param OperateUin: 操作者UIN：操作者账号 ID（预付费资源下单或后付费操作开通资源账号的 ID 或者角色 ID ）
         :type OperateUin: str
-        :param Tags: Tag 信息
+        :param Tags: 标签信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of BillTagInfo
-        :param BusinessCode: 产品名称代码
+        :param BusinessCode: 产品编码
 注意：此字段可能返回 null，表示取不到有效值。
         :type BusinessCode: str
-        :param ProductCode: 子产品名称代码
+        :param ProductCode: 子产品编码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ProductCode: str
-        :param ActionType: 交易类型代码
+        :param ActionType: 交易类型编码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ActionType: str
-        :param RegionId: 区域ID
+        :param RegionId: 地域ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegionId: str
-        :param ProjectId: 项目ID:资源所属项目ID
+        :param ProjectId: 项目ID
         :type ProjectId: int
         :param PriceInfo: 价格属性
 注意：此字段可能返回 null，表示取不到有效值。
         :type PriceInfo: list of str
         """
         self.BusinessCodeName = None
         self.ProductCodeName = None
@@ -246,74 +246,77 @@
 class BillDetailComponent(AbstractModel):
     """账单明细组件对象
 
     """
 
     def __init__(self):
         r"""
-        :param ComponentCodeName: 组件类型:资源组件类型的名称，如内存、硬盘等
+        :param ComponentCodeName: 组件类型：用户购买的产品或服务对应的组件大类，例如：云服务器 CVM 的组件：CPU、内存等
         :type ComponentCodeName: str
-        :param ItemCodeName: 组件名称:资源组件的名称，如云数据库MySQL-内存等
+        :param ItemCodeName: 组件名称：用户购买的产品或服务，所包含的具体组件
         :type ItemCodeName: str
-        :param SinglePrice: 组件刊例价:资源组件的原始价格，保持原始粒度
+        :param SinglePrice: 组件刊例价：组件的官网原始单价（如果客户享受一口价/合同价则默认不展示）
         :type SinglePrice: str
-        :param SpecifiedPrice: 组件指定价
+        :param SpecifiedPrice: 组件指定价（已废弃）
         :type SpecifiedPrice: str
-        :param PriceUnit: 价格单位
+        :param PriceUnit: 组件价格单位：组件价格的单位，单位构成：元/用量单位/时长单位
         :type PriceUnit: str
-        :param UsedAmount: 组件用量
+        :param UsedAmount: 组件用量：该组件实际结算用量，组件用量 = 组件原始用量 - 抵扣用量（含资源包
         :type UsedAmount: str
-        :param UsedAmountUnit: 组件用量单位
+        :param UsedAmountUnit: 组件用量单位：组件用量对应的单位
         :type UsedAmountUnit: str
-        :param TimeSpan: 使用时长
+        :param TimeSpan: 使用时长：资源使用的时长
         :type TimeSpan: str
-        :param TimeUnitName: 时长单位
+        :param TimeUnitName: 时长单位：资源使用时长的单位
         :type TimeUnitName: str
-        :param Cost: 组件原价
+        :param Cost: 组件原价：原价 = 组件刊例价 * 组件用量 * 使用时长（如果客户享受一口价/合同价则默认不展示，退费类场景也默认不展示）
         :type Cost: str
-        :param Discount: 折扣率，本资源享受的折扣率（如果客户享受一口价/合同价则默认不展示，退费场景也默认不展示）
+        :param Discount: 折扣率：本资源享受的折扣率（如果客户享受一口价/合同价则默认不展示，退费场景也默认不展示）
         :type Discount: str
         :param ReduceType: 优惠类型
         :type ReduceType: str
-        :param RealCost: 优惠后总价
+        :param RealCost: 优惠后总价：优惠后总价=（原价 - 预留实例抵扣原价 - 节省计划抵扣原价）* 折扣率
         :type RealCost: str
-        :param VoucherPayAmount: 代金券支付金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
-        :param CashPayAmount: 现金支付金额
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送账户支付金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param ItemCode: 组件类型代码
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
+        :param ItemCode: 组件类型编码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ItemCode: str
-        :param ComponentCode: 组件名称代码
+        :param ComponentCode: 组件名称编码
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentCode: str
-        :param ContractPrice: 组件单价
+        :param ContractPrice: 组件单价：组件的折后单价，组件单价 = 刊例价 * 折扣
 注意：此字段可能返回 null，表示取不到有效值。
         :type ContractPrice: str
-        :param InstanceType: 资源包、预留实例、节省计划、竞价实例这四类特殊实例本身的扣费行为，此字段体现对应的实例类型。枚举值如下：
+        :param InstanceType: 实例类型：购买的产品服务对应的实例类型，包括资源包、RI、SP、竞价实例。正常的实例展示默认为不展示
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceType: str
-        :param RiTimeSpan: 预留实例抵扣的使用时长，时长单位与被抵扣的时长单位保持一致
+        :param RiTimeSpan: 预留实例抵扣的使用时长：本产品或服务使用预留实例抵扣的使用时长
 注意：此字段可能返回 null，表示取不到有效值。
         :type RiTimeSpan: str
-        :param OriginalCostWithRI: 预留实例抵扣组件原价，本产品或服务使用预留实例抵扣的组件原价金额
+        :param OriginalCostWithRI: 预留实例抵扣组件原价：本产品或服务使用预留实例抵扣的组件原价金额
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCostWithRI: str
-        :param SPDeductionRate: 节省计划抵扣率，节省计划可用余额额度范围内，节省计划对于此组件打的折扣率
+        :param SPDeductionRate: 节省计划抵扣率：节省计划可用余额额度范围内，节省计划对于此组件打的折扣率
 注意：此字段可能返回 null，表示取不到有效值。
         :type SPDeductionRate: str
-        :param SPDeduction: 节省计划抵扣金额，节省计划抵扣的SP包面值
+        :param SPDeduction: 节省计划抵扣金额（已废弃）
 注意：此字段可能返回 null，表示取不到有效值。
         :type SPDeduction: str
-        :param OriginalCostWithSP: 节省计划抵扣组件原价，节省计划抵扣原价=节省计划包抵扣金额/节省计划抵扣率
+        :param OriginalCostWithSP: 节省计划抵扣组件原价：节省计划抵扣原价=节省计划包抵扣金额/节省计划抵扣率
 注意：此字段可能返回 null，表示取不到有效值。
         :type OriginalCostWithSP: str
-        :param BlendedDiscount: 混合折扣率，综合各类折扣抵扣信息后的最终折扣率，混合折扣率 = 优惠后总价 / 组件原价
+        :param BlendedDiscount: 混合折扣率：综合各类折扣抵扣信息后的最终折扣率，混合折扣率 = 优惠后总价 / 组件原价
 注意：此字段可能返回 null，表示取不到有效值。
         :type BlendedDiscount: str
         """
         self.ComponentCodeName = None
         self.ItemCodeName = None
         self.SinglePrice = None
         self.SpecifiedPrice = None
@@ -325,14 +328,15 @@
         self.Cost = None
         self.Discount = None
         self.ReduceType = None
         self.RealCost = None
         self.VoucherPayAmount = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
+        self.TransferPayAmount = None
         self.ItemCode = None
         self.ComponentCode = None
         self.ContractPrice = None
         self.InstanceType = None
         self.RiTimeSpan = None
         self.OriginalCostWithRI = None
         self.SPDeductionRate = None
@@ -354,14 +358,15 @@
         self.Cost = params.get("Cost")
         self.Discount = params.get("Discount")
         self.ReduceType = params.get("ReduceType")
         self.RealCost = params.get("RealCost")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         self.ItemCode = params.get("ItemCode")
         self.ComponentCode = params.get("ComponentCode")
         self.ContractPrice = params.get("ContractPrice")
         self.InstanceType = params.get("InstanceType")
         self.RiTimeSpan = params.get("RiTimeSpan")
         self.OriginalCostWithRI = params.get("OriginalCostWithRI")
         self.SPDeductionRate = params.get("SPDeductionRate")
@@ -380,97 +385,91 @@
 class BillResourceSummary(AbstractModel):
     """账单资源汇总数据对象
 
     """
 
     def __init__(self):
         r"""
-        :param BusinessCodeName: 产品名称：云产品大类，如云服务器CVM、云数据库MySQL
+        :param BusinessCodeName: 产品名称：用户所采购的各类云产品，例如：云服务器 CVM
         :type BusinessCodeName: str
-        :param ProductCodeName: 子产品名称：云产品子类，如云服务器CVM-标准型S1， 当没有获取到子产品名称时，返回"-"
+        :param ProductCodeName: 子产品名称：用户采购的具体产品细分类型，例如：云服务器 CVM-标准型 S1
         :type ProductCodeName: str
-        :param PayModeName: 计费模式：包年包月和按量计费
+        :param PayModeName: 计费模式：资源的计费模式，区分为包年包月和按量计费
         :type PayModeName: str
-        :param ProjectName: 项目
+        :param ProjectName: 项目名称：资源归属的项目，用户在控制台给资源自主分配项目，未分配则是默认项目
         :type ProjectName: str
-        :param RegionName: 地域
+        :param RegionName: 地域：资源所属地域，如华南地区（广州）
         :type RegionName: str
-        :param ZoneName: 可用区
+        :param ZoneName: 可用区：资源所属可用区，如广州三区
         :type ZoneName: str
-        :param ResourceId: 资源实例ID
+        :param ResourceId: 资源 ID：账单中出账对象 ID，不同产品因资源形态不同，资源内容不完全相同，如云服务器 CVM 为对应的实例 ID	
         :type ResourceId: str
-        :param ResourceName: 资源实例名称
+        :param ResourceName: 资源别名：用户在控制台为资源设置的名称，如果未设置，则默认为空
         :type ResourceName: str
-        :param ActionTypeName: 交易类型：包年包月新购/续费/升降配/退款、按量计费扣费、调账补偿/扣费等类型
+        :param ActionTypeName: 交易类型：如包年包月新购、包年包月续费、按量计费扣费等类型
         :type ActionTypeName: str
-        :param OrderId: 订单ID
+        :param OrderId: 订单ID：包年包月计费模式下订购的订单号
         :type OrderId: str
-        :param PayTime: 扣费时间
+        :param PayTime: 扣费时间：结算扣费时间
         :type PayTime: str
-        :param FeeBeginTime: 开始使用时间
+        :param FeeBeginTime: 开始使用时间：产品服务开始使用时间
         :type FeeBeginTime: str
-        :param FeeEndTime: 结束使用时间
+        :param FeeEndTime: 结束使用时间：产品服务结束使用时间
         :type FeeEndTime: str
-        :param ConfigDesc: 配置描述
+        :param ConfigDesc: 配置描述：该资源下的计费项名称和用量合并展示，仅在资源账单体现
         :type ConfigDesc: str
-        :param ExtendField1: 扩展字段1
+        :param ExtendField1: 扩展字段1：产品对应的扩展属性信息，仅在资源账单体现
         :type ExtendField1: str
-        :param ExtendField2: 扩展字段2
+        :param ExtendField2: 扩展字段2：产品对应的扩展属性信息，仅在资源账单体现
         :type ExtendField2: str
-        :param TotalCost: 原价，单位为元
+        :param TotalCost: 原价：原价 = 组件刊例价 * 组件用量 * 使用时长（如果客户享受一口价/合同价则默认不展示，退费类场景也默认不展示）
         :type TotalCost: str
-        :param Discount: 折扣率
-当聚合之后折扣不唯一或者合同价的情况下，返回“-”
+        :param Discount: 折扣率：本资源享受的折扣率（如果客户享受一口价/合同价则默认不展示，退费场景也默认不展示）
         :type Discount: str
         :param ReduceType: 优惠类型
         :type ReduceType: str
-        :param RealTotalCost: 优惠后总价，单位为元
+        :param RealTotalCost: 优惠后总价
         :type RealTotalCost: str
-        :param VoucherPayAmount: 代金券支付金额，单位为元
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
-        :param CashPayAmount: 现金账户支付金额，单位为元
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送账户支付金额，单位为元
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param ExtendField3: 扩展字段3
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
+        :param ExtendField3: 扩展字段3：产品对应的扩展属性信息，仅在资源账单体现
         :type ExtendField3: str
-        :param ExtendField4: 扩展字段4
+        :param ExtendField4: 扩展字段4：产品对应的扩展属性信息，仅在资源账单体现
         :type ExtendField4: str
-        :param ExtendField5: 扩展字段5
+        :param ExtendField5: 扩展字段5：产品对应的扩展属性信息，仅在资源账单体现
         :type ExtendField5: str
-        :param Tags: Tag 信息
+        :param Tags: 标签信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of BillTagInfo
-        :param PayerUin: 付款方uin
+        :param PayerUin: 支付者UIN：支付者的账号 ID，账号 ID 是用户在腾讯云的唯一账号标识
         :type PayerUin: str
-        :param OwnerUin: 资源所有者uin,无值则返回"-"
+        :param OwnerUin: 使用者UIN：实际使用资源的账号 ID
         :type OwnerUin: str
-        :param OperateUin: 操作者uin,无值则返回"-"
+        :param OperateUin: 操作者UIN：操作者账号 ID（预付费资源下单或后付费操作开通资源账号的 ID 或者角色 ID ）
         :type OperateUin: str
-        :param BusinessCode: 产品名称代码
+        :param BusinessCode: 产品编码
         :type BusinessCode: str
-        :param ProductCode: 子产品名称代码
+        :param ProductCode: 子产品编码
         :type ProductCode: str
-        :param RegionId: 区域ID
+        :param RegionId: 地域ID
         :type RegionId: int
-        :param InstanceType: 资源包、预留实例、节省计划、竞价实例这四类特殊实例本身的扣费行为，此字段体现对应的实例类型。枚举值如下：
-
-ri=Standard RI
-
-svp=Savings Plan
-
-si=Spot Instances
-
-rp=Resource Pack
+        :param InstanceType: 实例类型：购买的产品服务对应的实例类型，包括资源包、RI、SP、竞价实例。正常的实例展示默认为不展示
         :type InstanceType: str
-        :param OriginalCostWithRI: 按组件原价的口径换算的预留实例抵扣金额
+        :param OriginalCostWithRI: 预留实例抵扣组件原价：本产品或服务使用预留实例抵扣的组件原价金额	
         :type OriginalCostWithRI: str
-        :param SPDeduction: 节省计划抵扣的SP包面值
+        :param SPDeduction: 节省计划抵扣金额（已废弃）
         :type SPDeduction: str
-        :param OriginalCostWithSP: 按组件原价的口径换算的节省计划抵扣金额
+        :param OriginalCostWithSP: 节省计划抵扣组件原价：节省计划抵扣原价=节省计划包抵扣金额/节省计划抵扣率	
         :type OriginalCostWithSP: str
         """
         self.BusinessCodeName = None
         self.ProductCodeName = None
         self.PayModeName = None
         self.ProjectName = None
         self.RegionName = None
@@ -488,14 +487,15 @@
         self.TotalCost = None
         self.Discount = None
         self.ReduceType = None
         self.RealTotalCost = None
         self.VoucherPayAmount = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
+        self.TransferPayAmount = None
         self.ExtendField3 = None
         self.ExtendField4 = None
         self.ExtendField5 = None
         self.Tags = None
         self.PayerUin = None
         self.OwnerUin = None
         self.OperateUin = None
@@ -528,14 +528,15 @@
         self.TotalCost = params.get("TotalCost")
         self.Discount = params.get("Discount")
         self.ReduceType = params.get("ReduceType")
         self.RealTotalCost = params.get("RealTotalCost")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         self.ExtendField3 = params.get("ExtendField3")
         self.ExtendField4 = params.get("ExtendField4")
         self.ExtendField5 = params.get("ExtendField5")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = BillTagInfo()
@@ -655,59 +656,59 @@
 class BusinessSummaryOverviewItem(AbstractModel):
     """按产品汇总产品详情
 
     """
 
     def __init__(self):
         r"""
-        :param BusinessCode: 产品名称代码
+        :param BusinessCode: 产品编码
 注意：此字段可能返回 null，表示取不到有效值。
         :type BusinessCode: str
-        :param BusinessCodeName: 产品名称：云产品大类，如云服务器CVM、云数据库MySQL
+        :param BusinessCodeName: 产品名称：用户所采购的各类云产品，例如：云服务器 CVM
         :type BusinessCodeName: str
-        :param RealTotalCost: 实际花费
-        :type RealTotalCost: str
         :param RealTotalCostRatio: 费用所占百分比，两位小数
         :type RealTotalCostRatio: str
-        :param CashPayAmount: 现金金额
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+        :type TransferPayAmount: str
         :param BillMonth: 账单月份，格式2019-08
         :type BillMonth: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
-        :param TransferPayAmount: 分成金金额
-        :type TransferPayAmount: str
         """
         self.BusinessCode = None
         self.BusinessCodeName = None
-        self.RealTotalCost = None
         self.RealTotalCostRatio = None
+        self.RealTotalCost = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
+        self.TransferPayAmount = None
         self.BillMonth = None
         self.TotalCost = None
-        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.BusinessCode = params.get("BusinessCode")
         self.BusinessCodeName = params.get("BusinessCodeName")
-        self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
+        self.RealTotalCost = params.get("RealTotalCost")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         self.BillMonth = params.get("BillMonth")
         self.TotalCost = params.get("TotalCost")
-        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -716,42 +717,43 @@
 class BusinessSummaryTotal(AbstractModel):
     """按产品汇总总费用
 
     """
 
     def __init__(self):
         r"""
-        :param RealTotalCost: 总花费
+        :param RealTotalCost: 优惠后总价
+
         :type RealTotalCost: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param CashPayAmount: 现金金额
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+        :type TransferPayAmount: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
-        :param TransferPayAmount: 分成金金额
-        :type TransferPayAmount: str
         """
         self.RealTotalCost = None
         self.VoucherPayAmount = None
         self.IncentivePayAmount = None
         self.CashPayAmount = None
-        self.TotalCost = None
         self.TransferPayAmount = None
+        self.TotalCost = None
 
 
     def _deserialize(self, params):
         self.RealTotalCost = params.get("RealTotalCost")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.CashPayAmount = params.get("CashPayAmount")
-        self.TotalCost = params.get("TotalCost")
         self.TransferPayAmount = params.get("TransferPayAmount")
+        self.TotalCost = params.get("TotalCost")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1991,52 +1993,54 @@
 class DescribeBillResourceSummaryRequest(AbstractModel):
     """DescribeBillResourceSummary请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Offset: 偏移量
+        :param Offset: 分页偏移量，Offset=0表示第一页，如果Limit=100，则Offset=100表示第二页，Offset=200表示第三页，依次类推
         :type Offset: int
         :param Limit: 数量，最大值为1000
         :type Limit: int
-        :param Month: 月份，格式为yyyy-mm。不能早于开通账单2.0的月份，最多可拉取24个月内的数据。
+        :param Month: 月份，格式为yyyy-mm。不能早于开通账单2.0的月份
         :type Month: str
         :param PeriodType: 周期类型，byUsedTime按计费周期/byPayTime按扣费周期。需要与费用中心该月份账单的周期保持一致。您可前往[账单概览](https://console.cloud.tencent.com/expense/bill/overview)页面顶部查看确认您的账单统计周期类型。
         :type PeriodType: str
         :param NeedRecordNum: 是否需要访问列表的总记录数，用于前端分页
 1-表示需要， 0-表示不需要
         :type NeedRecordNum: int
-        :param ActionType: 查询交易类型，如下：
+        :param ActionType: 查询交易类型（请使用交易类型名称入参），入参示例枚举如下：
 包年包月新购
 包年包月续费
 包年包月配置变更
-包年包月退款
-按量计费扣费
-按量计费小时结
-按量计费日结
-按量计费月结
-线下项目扣费
-线下产品扣费
-调账扣费
-调账补偿
-竞价实例小时结
-线下项目调账补偿
-线下产品调账补偿
-优惠扣费
-优惠补偿
-按量计费迁入资源
-按量计费迁出资源
-包年包月迁入资源
-包年包月迁出资源
-预付费用
-小时费用
-预留实例退款
-按量计费冲正
-包年包月转按量
+包年包月退款 
+按量计费扣费 
+线下项目扣费 
+线下产品扣费 
+调账扣费 
+调账补偿 
+按量计费小时结 
+按量计费日结 
+按量计费月结 
+竞价实例小时结 
+线下项目调账补偿 
+线下产品调账补偿 
+优惠扣费 
+优惠补偿 
+按量计费迁入资源 
+按量计费迁出资源 
+包年包月迁入资源 
+包年包月迁出资源 
+预付费用 
+小时费用 
+预留实例退款 
+按量计费冲正 
+包年包月转按量 
+保底扣款 
+节省计划小时费用
         :type ActionType: str
         :param ResourceId: 查询指定资源信息
         :type ResourceId: str
         :param PayMode: 付费模式 prePay/postPay
         :type PayMode: str
         :param BusinessCode: 产品名称代码
 备注：如需获取当月使用过的BusinessCode，请调用API：<a href="https://cloud.tencent.com/document/product/555/35761">获取产品汇总费用分布</a>
@@ -2077,15 +2081,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param ResourceSummarySet: 资源汇总列表
         :type ResourceSummarySet: list of BillResourceSummary
-        :param Total: 资源汇总列表总数
+        :param Total: 资源汇总列表总数，入参NeedRecordNum为0时不返回
 注意：此字段可能返回 null，表示取不到有效值。
         :type Total: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.ResourceSummarySet = None
         self.Total = None
@@ -2138,15 +2142,16 @@
 class DescribeBillSummaryByPayModeResponse(AbstractModel):
     """DescribeBillSummaryByPayMode返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Ready: 数据是否准备好，0未准备好，1准备好
+        :param Ready: 数据是否准备好，0未准备好，1准备好。
+Ready=0，为当前UIN首次进行初始化出账，预计需要5~10分钟，请于10分钟后重试
         :type Ready: int
         :param SummaryOverview: 各付费模式花费分布详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryOverview: list of PayModeSummaryOverviewItem
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
@@ -2210,15 +2215,16 @@
 class DescribeBillSummaryByProductResponse(AbstractModel):
     """DescribeBillSummaryByProduct返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Ready: 数据是否准备好，0未准备好，1准备好
+        :param Ready: 数据是否准备好，0未准备好，1准备好。
+Ready=0，为当前UIN首次进行初始化出账，预计需要5~10分钟，请于10分钟后重试
         :type Ready: int
         :param SummaryTotal: 总花费详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryTotal: :class:`tencentcloud.billing.v20180709.models.BusinessSummaryTotal`
         :param SummaryOverview: 各产品花费分布
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryOverview: list of BusinessSummaryOverviewItem
@@ -2281,14 +2287,15 @@
     """DescribeBillSummaryByProject返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Ready: 数据是否准备好，0未准备好，1准备好
+Ready=0，为当前UIN首次进行初始化出账，预计需要5~10分钟，请于10分钟后重试
         :type Ready: int
         :param SummaryOverview: 各项目花费分布详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryOverview: list of ProjectSummaryOverviewItem
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
@@ -2344,14 +2351,15 @@
     """DescribeBillSummaryByRegion返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Ready: 数据是否准备好，0未准备好，1准备好
+Ready=0，为当前UIN首次进行初始化出账，预计需要5~10分钟，请于10分钟后重试
         :type Ready: int
         :param SummaryOverview: 各地域花费分布详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryOverview: list of RegionSummaryOverviewItem
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
@@ -2415,14 +2423,15 @@
     """DescribeBillSummaryByTag返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param Ready: 数据是否准备好，0未准备好，1准备好
+Ready=0，为当前UIN首次进行初始化出账，预计需要5~10分钟，请于10分钟后重试
         :type Ready: int
         :param SummaryOverview: 各标签值花费分布详情
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryOverview: list of TagSummaryOverviewItem
         :param SummaryTotal: 总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type SummaryTotal: :class:`tencentcloud.billing.v20180709.models.SummaryTotal`
@@ -3492,69 +3501,69 @@
         self.OrderIds = params.get("OrderIds")
         self.ResourceIds = params.get("ResourceIds")
         self.BigDealIds = params.get("BigDealIds")
         self.RequestId = params.get("RequestId")
 
 
 class PayModeSummaryOverviewItem(AbstractModel):
-    """按付费模式汇总消费详情
+    """按计费模式汇总消费详情
 
     """
 
     def __init__(self):
         r"""
-        :param PayMode: 付费模式
+        :param PayMode: 计费模式编码
         :type PayMode: str
-        :param PayModeName: 付费模式名称
+        :param PayModeName: 计费模式：区分为包年包月和按量计费
         :type PayModeName: str
-        :param RealTotalCost: 实际花费
-        :type RealTotalCost: str
         :param RealTotalCostRatio: 费用所占百分比，两位小数
         :type RealTotalCostRatio: str
-        :param Detail: 按交易类型：包年包月新购/续费/升降配/退款、按量计费扣费、调账补偿/扣费等类型汇总消费详情
-        :type Detail: list of ActionSummaryOverviewItem
-        :param CashPayAmount: 现金金额
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+        :type TransferPayAmount: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
-        :param TransferPayAmount: 分成金金额
-        :type TransferPayAmount: str
+        :param Detail: 按交易类型汇总消费详情
+        :type Detail: list of ActionSummaryOverviewItem
         """
         self.PayMode = None
         self.PayModeName = None
-        self.RealTotalCost = None
         self.RealTotalCostRatio = None
-        self.Detail = None
+        self.RealTotalCost = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
-        self.TotalCost = None
         self.TransferPayAmount = None
+        self.TotalCost = None
+        self.Detail = None
 
 
     def _deserialize(self, params):
         self.PayMode = params.get("PayMode")
         self.PayModeName = params.get("PayModeName")
-        self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
+        self.RealTotalCost = params.get("RealTotalCost")
+        self.CashPayAmount = params.get("CashPayAmount")
+        self.IncentivePayAmount = params.get("IncentivePayAmount")
+        self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
+        self.TotalCost = params.get("TotalCost")
         if params.get("Detail") is not None:
             self.Detail = []
             for item in params.get("Detail"):
                 obj = ActionSummaryOverviewItem()
                 obj._deserialize(item)
                 self.Detail.append(obj)
-        self.CashPayAmount = params.get("CashPayAmount")
-        self.IncentivePayAmount = params.get("IncentivePayAmount")
-        self.VoucherPayAmount = params.get("VoucherPayAmount")
-        self.TotalCost = params.get("TotalCost")
-        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3593,56 +3602,56 @@
 
     """
 
     def __init__(self):
         r"""
         :param ProjectId: 项目ID
         :type ProjectId: str
-        :param ProjectName: 项目名称
+        :param ProjectName: 项目名称：资源归属的项目，用户在控制台给资源自主分配项目，未分配则是默认项目
         :type ProjectName: str
-        :param RealTotalCost: 实际花费
-        :type RealTotalCost: str
         :param RealTotalCostRatio: 费用所占百分比，两位小数
         :type RealTotalCostRatio: str
-        :param CashPayAmount: 现金金额
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+        :type TransferPayAmount: str
         :param BillMonth: 账单月份，格式2019-08
         :type BillMonth: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
-        :param TransferPayAmount: 分成金金额
-        :type TransferPayAmount: str
         """
         self.ProjectId = None
         self.ProjectName = None
-        self.RealTotalCost = None
         self.RealTotalCostRatio = None
+        self.RealTotalCost = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
+        self.TransferPayAmount = None
         self.BillMonth = None
         self.TotalCost = None
-        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.ProjectId = params.get("ProjectId")
         self.ProjectName = params.get("ProjectName")
-        self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
+        self.RealTotalCost = params.get("RealTotalCost")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         self.BillMonth = params.get("BillMonth")
         self.TotalCost = params.get("TotalCost")
-        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3654,56 +3663,56 @@
     """
 
     def __init__(self):
         r"""
         :param RegionId: 地域ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegionId: str
-        :param RegionName: 地域名称
+        :param RegionName: 地域名称：资源所属地域，例如华南地区（广州）
         :type RegionName: str
-        :param RealTotalCost: 实际花费
-        :type RealTotalCost: str
         :param RealTotalCostRatio: 费用所占百分比，两位小数
         :type RealTotalCostRatio: str
-        :param CashPayAmount: 现金金额
+        :param RealTotalCost: 优惠后总价
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
         :type IncentivePayAmount: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
         :type VoucherPayAmount: str
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
+        :type TransferPayAmount: str
         :param BillMonth: 账单月份，格式2019-08
         :type BillMonth: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
-        :param TransferPayAmount: 分成金金额
-        :type TransferPayAmount: str
         """
         self.RegionId = None
         self.RegionName = None
-        self.RealTotalCost = None
         self.RealTotalCostRatio = None
+        self.RealTotalCost = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
+        self.TransferPayAmount = None
         self.BillMonth = None
         self.TotalCost = None
-        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.RegionId = params.get("RegionId")
         self.RegionName = params.get("RegionName")
-        self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
+        self.RealTotalCost = params.get("RealTotalCost")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         self.BillMonth = params.get("BillMonth")
         self.TotalCost = params.get("TotalCost")
-        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3712,15 +3721,15 @@
 class SummaryTotal(AbstractModel):
     """总数
 
     """
 
     def __init__(self):
         r"""
-        :param RealTotalCost: 总数
+        :param RealTotalCost: 优惠后总价
 注意：此字段可能返回 null，表示取不到有效值。
         :type RealTotalCost: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalCost: str
         """
         self.RealTotalCost = None
@@ -3745,55 +3754,55 @@
     """
 
     def __init__(self):
         r"""
         :param TagValue: 标签值
 注意：此字段可能返回 null，表示取不到有效值。
         :type TagValue: str
-        :param RealTotalCost: 实际花费
-注意：此字段可能返回 null，表示取不到有效值。
-        :type RealTotalCost: str
         :param RealTotalCostRatio: 费用所占百分比，两位小数
 注意：此字段可能返回 null，表示取不到有效值。
         :type RealTotalCostRatio: str
-        :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
+        :param RealTotalCost: 优惠后总价
 注意：此字段可能返回 null，表示取不到有效值。
-        :type TotalCost: str
-        :param CashPayAmount: 现金金额
+        :type RealTotalCost: str
+        :param CashPayAmount: 现金账户支出：通过现金账户支付的金额
 注意：此字段可能返回 null，表示取不到有效值。
         :type CashPayAmount: str
-        :param IncentivePayAmount: 赠送金金额
+        :param IncentivePayAmount: 赠送账户支出：使用赠送金支付的金额
 注意：此字段可能返回 null，表示取不到有效值。
         :type IncentivePayAmount: str
-        :param VoucherPayAmount: 代金券金额
+        :param VoucherPayAmount: 优惠券支出：使用各类优惠券（如代金券、现金券等）支付的金额
 注意：此字段可能返回 null，表示取不到有效值。
         :type VoucherPayAmount: str
-        :param TransferPayAmount: 分成金金额
+        :param TransferPayAmount: 分成金账户支出：通过分成金账户支付的金额
 注意：此字段可能返回 null，表示取不到有效值。
         :type TransferPayAmount: str
+        :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCost: str
         """
         self.TagValue = None
-        self.RealTotalCost = None
         self.RealTotalCostRatio = None
-        self.TotalCost = None
+        self.RealTotalCost = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
         self.TransferPayAmount = None
+        self.TotalCost = None
 
 
     def _deserialize(self, params):
         self.TagValue = params.get("TagValue")
-        self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
-        self.TotalCost = params.get("TotalCost")
+        self.RealTotalCost = params.get("RealTotalCost")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
         self.TransferPayAmount = params.get("TransferPayAmount")
+        self.TotalCost = params.get("TotalCost")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-billing-3.0.897/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.898/tencentcloud/billing/v20180709/billing_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeBillSummaryByPayMode(self, request):
-        """获取按付费模式汇总费用分布
+        """获取按计费模式汇总费用分布
 
         :param request: Request instance for DescribeBillSummaryByPayMode.
         :type request: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByPayModeRequest`
         :rtype: :class:`tencentcloud.billing.v20180709.models.DescribeBillSummaryByPayModeResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-billing-3.0.897/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.898/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.897/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.898/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.897
+Version: 3.0.898
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.897/setup.py` & `tencentcloud-sdk-python-billing-3.0.898/setup.py`

 * *Files identical despite different names*

