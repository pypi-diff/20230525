# Comparing `tmp/aliyun-python-sdk-ecs-4.9.6.tar.gz` & `tmp/aliyun-python-sdk-ecs-4.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ecs-4.9.6.tar", last modified: Wed Aug 15 03:05:49 2018, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ecs-4.9.7.tar", last modified: Tue Aug 21 09:48:16 2018, max compression
```

## Comparing `aliyun-python-sdk-ecs-4.9.6.tar` & `aliyun-python-sdk-ecs-4.9.7.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/
--rw-r--r--   0 jenkins    (504) jenkins    (503)    15596 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)       13 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)        1 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (504) jenkins    (503)       30 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/PKG-INFO
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2586 2018-08-15 02:32:55.000000 aliyun-python-sdk-ecs-4.9.6/setup.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)       38 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/setup.cfg
--rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-08-15 02:31:18.000000 aliyun-python-sdk-ecs-4.9.6/MANIFEST.in
--rw-r--r--   0 jenkins    (504) jenkins    (503)      351 2018-08-15 02:32:06.000000 aliyun-python-sdk-ecs-4.9.6/README.rst
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/
--rw-r--r--   0 jenkins    (504) jenkins    (503)       21 2018-08-15 02:42:20.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/__init__.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/
--rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-08-15 02:31:18.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/__init__.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-15 03:05:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4306 2018-08-15 02:31:00.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RevokeSecurityGroupEgressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2454 2018-08-15 02:30:36.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeHpcClustersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1926 2018-08-15 02:30:33.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReActivateInstancesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2316 2018-08-15 02:31:18.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AllocateEipAddressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3037 2018-08-15 02:31:14.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3455 2018-08-15 02:30:29.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeLaunchTemplatesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2613 2018-08-15 02:30:59.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTagsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2282 2018-08-15 02:31:02.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVRouterAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1934 2018-08-15 02:31:02.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReleaseEipAddressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2312 2018-08-15 02:30:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AddBandwidthPackageIpsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2216 2018-08-15 02:31:01.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ResizeDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2432 2018-08-15 02:30:46.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNewProjectEipMonitorDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2444 2018-08-15 02:30:29.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyLaunchTemplateDefaultVersionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2412 2018-08-15 02:30:58.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RenewInstanceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2216 2018-08-15 02:30:50.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EipNotifyPaidRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2152 2018-08-15 02:30:39.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachNetworkInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2310 2018-08-15 02:30:56.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteRouterInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3804 2018-08-15 02:30:54.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ImportImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2254 2018-08-15 02:31:05.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyImageAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2104 2018-08-15 02:31:00.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/StartInstanceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2865 2018-08-15 02:30:45.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeKeyPairsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3607 2018-08-15 02:30:29.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeLaunchTemplateVersionsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)    11829 2018-08-15 02:30:30.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateLaunchTemplateRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4212 2018-08-15 02:30:32.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAvailableResourceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2753 2018-08-15 02:30:31.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacePermissionsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2240 2018-08-15 02:30:36.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateHpcClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1876 2018-08-15 02:31:12.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteVpcRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4314 2018-08-15 02:30:38.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupEgressRuleRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2454 2018-08-15 02:30:55.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceSpecRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2493 2018-08-15 02:30:29.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateVersionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2110 2018-08-15 02:30:36.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteHpcClusterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2478 2018-08-15 02:30:46.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceAutoRenewAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3125 2018-08-15 02:31:15.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CopyImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2025 2018-08-15 02:30:28.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAccountAttributesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2434 2018-08-15 02:31:00.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/StopInstanceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2801 2018-08-15 02:31:14.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateSnapshotRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2900 2018-08-15 02:31:05.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyDiskAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1980 2018-08-15 02:30:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteBandwidthPackageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2366 2018-08-15 02:30:44.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyDeploymentSetAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2696 2018-08-15 02:30:38.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeCommandsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-08-15 02:31:18.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/__init__.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2461 2018-08-15 02:30:59.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeResourceByTagsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2360 2018-08-15 02:30:41.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2314 2018-08-15 02:31:04.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceVpcAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1930 2018-08-15 02:30:42.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachInstanceRamRoleRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2078 2018-08-15 02:30:31.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/GetInstanceScreenshotRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2174 2018-08-15 02:30:54.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeletePhysicalConnectionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1914 2018-08-15 02:30:45.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachKeyPairRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1938 2018-08-15 02:31:09.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceVncPasswdRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2410 2018-08-15 02:31:10.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceMonitorDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     5714 2018-08-15 02:31:05.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyImageSharePermissionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1932 2018-08-15 02:31:09.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceVncUrlRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3629 2018-08-15 02:31:15.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2307 2018-08-15 02:30:45.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateKeyPairRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2499 2018-08-15 02:30:47.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RemoveBandwidthPackageIpsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1750 2018-08-15 02:30:35.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ConvertNatPublicIpToEipRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1724 2018-08-15 02:30:32.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEventDetailRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2378 2018-08-15 02:30:54.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ExportImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2426 2018-08-15 02:30:43.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRenewalPriceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3504 2018-08-15 02:30:52.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVirtualBorderRouterAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2888 2018-08-15 02:30:40.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRecommendInstanceTypeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2154 2018-08-15 02:30:47.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyBandwidthPackageSpecRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4126 2018-08-15 02:31:04.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceSpecRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2296 2018-08-15 02:31:03.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySnapshotAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4297 2018-08-15 02:30:33.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstancesFullStatusRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1700 2018-08-15 02:30:55.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelTaskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2056 2018-08-15 02:31:06.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2670 2018-08-15 02:30:43.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDeploymentSetTopologyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2542 2018-08-15 02:30:28.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEniMonitorDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2366 2018-08-15 02:31:03.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2412 2018-08-15 02:31:11.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEipMonitorDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2412 2018-08-15 02:30:47.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNatGatewaysRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2892 2018-08-15 02:30:55.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTasksRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2218 2018-08-15 02:30:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EipFillProductRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3062 2018-08-15 02:30:29.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ValidateSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2380 2018-08-15 02:31:07.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVpcsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2719 2018-08-15 02:30:39.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyNetworkInterfaceAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1964 2018-08-15 02:30:51.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ApplyAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1744 2018-08-15 02:30:45.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteKeyPairsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3990 2018-08-15 02:31:01.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReplaceSystemDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2246 2018-08-15 02:31:07.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVRoutersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1936 2018-08-15 02:30:35.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelAgreementRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1944 2018-08-15 02:30:55.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceTypeFamiliesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2714 2018-08-15 02:30:38.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateCommandRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2070 2018-08-15 02:30:58.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteHaVipRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4140 2018-08-15 02:31:11.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEipAddressesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2152 2018-08-15 02:30:40.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachNetworkInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     5668 2018-08-15 02:30:43.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribePriceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2124 2018-08-15 02:31:06.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/JoinSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2029 2018-08-15 02:30:30.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/InstallCloudAssistantRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2308 2018-08-15 02:30:40.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/JoinResourceGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2394 2018-08-15 02:30:57.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnassociateHaVipRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4584 2018-08-15 02:31:15.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3944 2018-08-15 02:31:06.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1736 2018-08-15 02:30:47.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeUserDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3068 2018-08-15 02:30:37.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSpotPriceHistoryRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1924 2018-08-15 02:31:08.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeLimitationRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2494 2018-08-15 02:30:48.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeForwardTableEntriesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1886 2018-08-15 02:30:41.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachClassicLinkVpcRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2112 2018-08-15 02:31:04.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceVncPasswdRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2277 2018-08-15 02:30:59.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RemoveTagsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2640 2018-08-15 02:30:46.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceAutoRenewAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1792 2018-08-15 02:30:57.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ActivateRouterInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2296 2018-08-15 02:31:13.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteInstanceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2710 2018-08-15 02:31:02.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReInitDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2382 2018-08-15 02:30:51.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)    11587 2018-08-15 02:31:15.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateInstanceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2089 2018-08-15 02:30:41.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSecurityGroupReferencesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2832 2018-08-15 02:30:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateForwardEntryRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2294 2018-08-15 02:31:17.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AssociateEipAddressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4336 2018-08-15 02:31:17.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2487 2018-08-15 02:30:37.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/InvokeCommandRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2175 2018-08-15 02:30:37.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/StopInvocationRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2271 2018-08-15 02:30:59.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AddTagsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1944 2018-08-15 02:31:16.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CheckDiskEnableAutoSnapshotValidationRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2823 2018-08-15 02:31:13.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteRouteEntryRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1956 2018-08-15 02:30:44.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteDeploymentSetRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1930 2018-08-15 02:30:42.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachInstanceRamRoleRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1926 2018-08-15 02:30:44.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ImportKeyPairRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2340 2018-08-15 02:30:52.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/TerminatePhysicalConnectionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2076 2018-08-15 02:31:16.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/BindIpRangeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2326 2018-08-15 02:30:51.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeImageSupportInstanceTypesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1956 2018-08-15 02:31:13.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2202 2018-08-15 02:30:31.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteNetworkInterfacePermissionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2184 2018-08-15 02:30:30.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2082 2018-08-15 02:31:02.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RebootInstanceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1884 2018-08-15 02:31:13.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2054 2018-08-15 02:31:01.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ResetDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     5718 2018-08-15 02:30:56.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateRouterInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3506 2018-08-15 02:31:04.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceNetworkSpecRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1908 2018-08-15 02:31:12.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteVSwitchRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2248 2018-08-15 02:30:58.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AssociateHaVipRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1914 2018-08-15 02:30:45.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachKeyPairRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2570 2018-08-15 02:31:14.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateVpcRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2732 2018-08-15 02:31:14.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateVSwitchRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1932 2018-08-15 02:30:35.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/SignAgreementRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1938 2018-08-15 02:31:10.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2307 2018-08-15 02:30:30.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnassignPrivateIpAddressesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2298 2018-08-15 02:31:08.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSecurityGroupAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1932 2018-08-15 02:30:48.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteNatGatewayRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2550 2018-08-15 02:30:57.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeHaVipsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3179 2018-08-15 02:31:15.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateRouteEntryRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2248 2018-08-15 02:30:52.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RecoverVirtualBorderRouterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1886 2018-08-15 02:30:41.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachClassicLinkVpcRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4461 2018-08-15 02:30:33.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceHistoryEventsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     5243 2018-08-15 02:31:07.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2346 2018-08-15 02:31:08.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRegionsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2552 2018-08-15 02:31:03.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVpcAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2252 2018-08-15 02:30:51.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/TerminateVirtualBorderRouterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1980 2018-08-15 02:30:39.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteNetworkInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)    11344 2018-08-15 02:30:30.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateLaunchTemplateVersionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1954 2018-08-15 02:31:10.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstancePhysicalAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3170 2018-08-15 02:30:40.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceChargeTypeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2116 2018-08-15 02:31:05.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyEipAddressAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2336 2018-08-15 02:30:50.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyExRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2334 2018-08-15 02:30:54.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelPhysicalConnectionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1978 2018-08-15 02:31:09.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceTypesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2234 2018-08-15 02:30:41.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeClassicLinkInstancesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2034 2018-08-15 02:31:13.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1942 2018-08-15 02:31:09.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeIntranetAttributeKbRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1900 2018-08-15 02:31:16.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelCopyImageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2250 2018-08-15 02:30:58.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTagKeysRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1926 2018-08-15 02:30:35.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteRecycleBinRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2298 2018-08-15 02:31:00.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnassociateEipAddressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3266 2018-08-15 02:30:37.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInvocationsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1812 2018-08-15 02:30:50.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2258 2018-08-15 02:31:10.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeImageSharePermissionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2386 2018-08-15 02:30:56.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRouterInterfacesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3482 2018-08-15 02:30:56.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2266 2018-08-15 02:30:42.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceRamRoleRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4312 2018-08-15 02:31:17.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupEgressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1760 2018-08-15 02:30:36.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotsUsageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1768 2018-08-15 02:31:12.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4262 2018-08-15 02:30:39.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2058 2018-08-15 02:31:12.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteSnapshotRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2424 2018-08-15 02:31:17.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachDiskRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2948 2018-08-15 02:31:04.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2334 2018-08-15 02:30:52.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EnablePhysicalConnectionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2282 2018-08-15 02:31:02.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVSwitchAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2514 2018-08-15 02:30:53.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAccessPointsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2618 2018-08-15 02:30:50.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyExRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1748 2018-08-15 02:31:12.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeClustersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2595 2018-08-15 02:30:31.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AssignPrivateIpAddressesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4129 2018-08-15 02:31:07.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSecurityGroupsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2426 2018-08-15 02:30:58.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateHaVipRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2050 2018-08-15 02:30:43.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AddIpRangeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1796 2018-08-15 02:30:56.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeactivateRouterInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1734 2018-08-15 02:30:51.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2300 2018-08-15 02:31:06.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeZonesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2134 2018-08-15 02:31:01.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReleasePublicIpAddressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2744 2018-08-15 02:30:37.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyCommandRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2404 2018-08-15 02:30:35.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRecycleBinRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2442 2018-08-15 02:30:35.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyHpcClusterAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)    12562 2018-08-15 02:30:34.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RunInstancesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3072 2018-08-15 02:30:40.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyPrepayInstanceSpecRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2816 2018-08-15 02:30:38.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInvocationResultsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2406 2018-08-15 02:31:09.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceStatusRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2378 2018-08-15 02:31:12.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDiskMonitorDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2338 2018-08-15 02:30:31.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateNetworkInterfacePermissionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1908 2018-08-15 02:30:38.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteCommandRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2432 2018-08-15 02:31:03.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyIntranetBandwidthKbRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     8591 2018-08-15 02:31:10.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstancesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2148 2018-08-15 02:30:46.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceAutoReleaseTimeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2502 2018-08-15 02:30:48.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeBandwidthPackagesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2266 2018-08-15 02:30:57.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyHaVipAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4338 2018-08-15 02:30:42.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupRuleRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2286 2018-08-15 02:31:05.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyImageShareGroupPermissionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2043 2018-08-15 02:30:30.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeCloudAssistantStatusRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2144 2018-08-15 02:30:48.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteForwardEntryRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2238 2018-08-15 02:30:43.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotMonitorDataRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2216 2018-08-15 02:30:50.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EipFillParamsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2394 2018-08-15 02:30:53.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2958 2018-08-15 02:30:44.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateDeploymentSetRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3028 2018-08-15 02:30:47.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyForwardEntryRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2112 2018-08-15 02:30:34.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyUserBusinessBehaviorRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2914 2018-08-15 02:30:53.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribePhysicalConnectionsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2720 2018-08-15 02:30:32.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeBandwidthLimitationRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2618 2018-08-15 02:30:46.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotLinksRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2668 2018-08-15 02:30:53.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3748 2018-08-15 02:30:54.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateVirtualBorderRouterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3178 2018-08-15 02:30:44.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDeploymentSetsRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3076 2018-08-15 02:30:49.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateNatGatewayRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3495 2018-08-15 02:30:40.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateNetworkInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1790 2018-08-15 02:30:57.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ConnectRouterInterfaceRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     5499 2018-08-15 02:31:11.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeImagesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2400 2018-08-15 02:31:08.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeIpRangesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2126 2018-08-15 02:31:06.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/LeaveSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1936 2018-08-15 02:30:32.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/GetInstanceConsoleOutputRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3900 2018-08-15 02:30:54.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreatePhysicalConnectionRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2080 2018-08-15 02:30:59.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnbindIpRangeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3050 2018-08-15 02:30:32.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeResourcesModificationRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1938 2018-08-15 02:30:34.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeUserBusinessBehaviorRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3824 2018-08-15 02:30:52.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyPhysicalConnectionAttributeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2094 2018-08-15 02:30:42.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotPackageRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3942 2018-08-15 02:31:16.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CheckAutoSnapshotPolicyRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     4330 2018-08-15 02:31:01.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RevokeSecurityGroupRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2610 2018-08-15 02:30:39.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyDiskChargeTypeRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2248 2018-08-15 02:31:17.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AllocatePublicIpAddressRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2704 2018-08-15 02:31:07.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVSwitchesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3462 2018-08-15 02:30:33.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDisksFullStatusRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2964 2018-08-15 02:31:08.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRouteTablesRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     7202 2018-08-15 02:31:11.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDisksRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     2246 2018-08-15 02:30:53.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteVirtualBorderRouterRequest.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1722 2018-08-15 02:30:55.000000 aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTaskAttributeRequest.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)    15596 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       13 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        1 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       30 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/PKG-INFO
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2586 2018-08-21 09:22:07.000000 aliyun-python-sdk-ecs-4.9.7/setup.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       38 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/setup.cfg
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:20:27.000000 aliyun-python-sdk-ecs-4.9.7/MANIFEST.in
+-rw-r--r--   0 jenkins    (504) jenkins    (503)      351 2018-08-21 09:21:16.000000 aliyun-python-sdk-ecs-4.9.7/README.rst
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       21 2018-08-21 09:31:32.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/__init__.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:20:27.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/__init__.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:48:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4306 2018-08-21 09:20:10.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RevokeSecurityGroupEgressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2454 2018-08-21 09:19:45.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeHpcClustersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1926 2018-08-21 09:19:42.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReActivateInstancesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2316 2018-08-21 09:20:27.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AllocateEipAddressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3037 2018-08-21 09:20:24.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3455 2018-08-21 09:19:38.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeLaunchTemplatesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2613 2018-08-21 09:20:09.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTagsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2282 2018-08-21 09:20:12.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVRouterAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1934 2018-08-21 09:20:12.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReleaseEipAddressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2312 2018-08-21 09:19:59.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AddBandwidthPackageIpsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2216 2018-08-21 09:20:11.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ResizeDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2432 2018-08-21 09:19:56.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNewProjectEipMonitorDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2444 2018-08-21 09:19:38.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyLaunchTemplateDefaultVersionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2412 2018-08-21 09:20:08.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RenewInstanceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2216 2018-08-21 09:19:59.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EipNotifyPaidRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2152 2018-08-21 09:19:48.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachNetworkInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2310 2018-08-21 09:20:06.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteRouterInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3804 2018-08-21 09:20:04.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ImportImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2254 2018-08-21 09:20:15.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyImageAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2104 2018-08-21 09:20:10.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/StartInstanceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2865 2018-08-21 09:19:55.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeKeyPairsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3607 2018-08-21 09:19:38.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeLaunchTemplateVersionsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)    11829 2018-08-21 09:19:39.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateLaunchTemplateRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4212 2018-08-21 09:19:42.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAvailableResourceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2753 2018-08-21 09:19:40.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacePermissionsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2240 2018-08-21 09:19:45.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateHpcClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1876 2018-08-21 09:20:22.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteVpcRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4314 2018-08-21 09:19:47.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupEgressRuleRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2454 2018-08-21 09:20:05.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceSpecRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2493 2018-08-21 09:19:39.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateVersionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2110 2018-08-21 09:19:45.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteHpcClusterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2478 2018-08-21 09:19:55.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceAutoRenewAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3125 2018-08-21 09:20:25.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CopyImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2025 2018-08-21 09:19:38.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAccountAttributesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2434 2018-08-21 09:20:10.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/StopInstanceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2801 2018-08-21 09:20:24.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateSnapshotRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2900 2018-08-21 09:20:15.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyDiskAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1980 2018-08-21 09:19:58.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteBandwidthPackageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2366 2018-08-21 09:19:53.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyDeploymentSetAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2696 2018-08-21 09:19:47.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeCommandsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        0 2018-08-21 09:20:27.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/__init__.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2461 2018-08-21 09:20:09.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeResourceByTagsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2360 2018-08-21 09:19:50.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2314 2018-08-21 09:20:13.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceVpcAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1930 2018-08-21 09:19:52.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachInstanceRamRoleRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2078 2018-08-21 09:19:41.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/GetInstanceScreenshotRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2174 2018-08-21 09:20:03.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeletePhysicalConnectionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1914 2018-08-21 09:19:54.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachKeyPairRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1938 2018-08-21 09:20:19.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceVncPasswdRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2410 2018-08-21 09:20:20.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceMonitorDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     5714 2018-08-21 09:20:14.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyImageSharePermissionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1932 2018-08-21 09:20:19.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceVncUrlRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3629 2018-08-21 09:20:25.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2307 2018-08-21 09:19:55.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateKeyPairRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2499 2018-08-21 09:19:56.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RemoveBandwidthPackageIpsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1750 2018-08-21 09:19:44.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ConvertNatPublicIpToEipRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1724 2018-08-21 09:19:41.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEventDetailRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2378 2018-08-21 09:20:04.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ExportImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2426 2018-08-21 09:19:52.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRenewalPriceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3504 2018-08-21 09:20:01.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVirtualBorderRouterAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2888 2018-08-21 09:19:49.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRecommendInstanceTypeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2154 2018-08-21 09:19:57.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyBandwidthPackageSpecRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4126 2018-08-21 09:20:14.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceSpecRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2296 2018-08-21 09:20:13.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySnapshotAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4297 2018-08-21 09:19:42.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstancesFullStatusRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1700 2018-08-21 09:20:05.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelTaskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2056 2018-08-21 09:20:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2670 2018-08-21 09:19:53.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDeploymentSetTopologyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2542 2018-08-21 09:19:37.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEniMonitorDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2366 2018-08-21 09:20:13.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2412 2018-08-21 09:20:21.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEipMonitorDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2412 2018-08-21 09:19:57.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNatGatewaysRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2892 2018-08-21 09:20:04.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTasksRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2218 2018-08-21 09:19:59.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EipFillProductRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3062 2018-08-21 09:19:38.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ValidateSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2380 2018-08-21 09:20:17.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVpcsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2719 2018-08-21 09:19:48.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyNetworkInterfaceAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1964 2018-08-21 09:20:00.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ApplyAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1744 2018-08-21 09:19:55.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteKeyPairsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3990 2018-08-21 09:20:11.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReplaceSystemDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2246 2018-08-21 09:20:17.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVRoutersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1936 2018-08-21 09:19:44.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelAgreementRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1944 2018-08-21 09:20:05.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceTypeFamiliesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2714 2018-08-21 09:19:47.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateCommandRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2070 2018-08-21 09:20:07.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteHaVipRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4140 2018-08-21 09:20:21.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEipAddressesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2152 2018-08-21 09:19:49.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachNetworkInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     5668 2018-08-21 09:19:53.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribePriceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2124 2018-08-21 09:20:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/JoinSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2029 2018-08-21 09:19:39.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/InstallCloudAssistantRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2308 2018-08-21 09:19:50.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/JoinResourceGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2394 2018-08-21 09:20:07.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnassociateHaVipRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4584 2018-08-21 09:20:25.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3944 2018-08-21 09:20:15.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1736 2018-08-21 09:19:56.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeUserDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3068 2018-08-21 09:19:46.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSpotPriceHistoryRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1924 2018-08-21 09:20:18.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeLimitationRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2494 2018-08-21 09:19:57.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeForwardTableEntriesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1886 2018-08-21 09:19:50.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachClassicLinkVpcRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2112 2018-08-21 09:20:14.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceVncPasswdRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2277 2018-08-21 09:20:08.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RemoveTagsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2640 2018-08-21 09:19:55.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceAutoRenewAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1792 2018-08-21 09:20:07.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ActivateRouterInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2296 2018-08-21 09:20:23.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteInstanceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2710 2018-08-21 09:20:12.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReInitDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2382 2018-08-21 09:20:00.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)    11813 2018-08-21 09:20:24.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateInstanceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2089 2018-08-21 09:19:50.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSecurityGroupReferencesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2832 2018-08-21 09:19:58.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateForwardEntryRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2294 2018-08-21 09:20:27.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AssociateEipAddressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4336 2018-08-21 09:20:26.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2487 2018-08-21 09:19:46.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/InvokeCommandRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2175 2018-08-21 09:19:46.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/StopInvocationRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2271 2018-08-21 09:20:09.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AddTagsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1944 2018-08-21 09:20:25.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CheckDiskEnableAutoSnapshotValidationRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2823 2018-08-21 09:20:23.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteRouteEntryRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1956 2018-08-21 09:19:54.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteDeploymentSetRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1930 2018-08-21 09:19:51.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachInstanceRamRoleRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1926 2018-08-21 09:19:54.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ImportKeyPairRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2340 2018-08-21 09:20:01.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/TerminatePhysicalConnectionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2076 2018-08-21 09:20:26.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/BindIpRangeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2326 2018-08-21 09:20:01.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeImageSupportInstanceTypesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1956 2018-08-21 09:20:23.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2202 2018-08-21 09:19:40.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteNetworkInterfacePermissionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2184 2018-08-21 09:19:39.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2082 2018-08-21 09:20:12.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RebootInstanceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1884 2018-08-21 09:20:23.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2054 2018-08-21 09:20:11.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ResetDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     5718 2018-08-21 09:20:06.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateRouterInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3506 2018-08-21 09:20:14.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceNetworkSpecRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1908 2018-08-21 09:20:22.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteVSwitchRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2248 2018-08-21 09:20:08.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AssociateHaVipRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1914 2018-08-21 09:19:55.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachKeyPairRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2570 2018-08-21 09:20:24.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateVpcRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2732 2018-08-21 09:20:23.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateVSwitchRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1932 2018-08-21 09:19:43.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/SignAgreementRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1938 2018-08-21 09:20:20.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2307 2018-08-21 09:19:40.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnassignPrivateIpAddressesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2298 2018-08-21 09:20:18.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSecurityGroupAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1932 2018-08-21 09:19:58.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteNatGatewayRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2550 2018-08-21 09:20:07.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeHaVipsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3179 2018-08-21 09:20:24.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateRouteEntryRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2248 2018-08-21 09:20:01.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RecoverVirtualBorderRouterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1886 2018-08-21 09:19:51.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachClassicLinkVpcRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4461 2018-08-21 09:19:42.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceHistoryEventsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     5243 2018-08-21 09:20:17.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2346 2018-08-21 09:20:18.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRegionsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2552 2018-08-21 09:20:13.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVpcAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2252 2018-08-21 09:20:01.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/TerminateVirtualBorderRouterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1980 2018-08-21 09:19:49.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteNetworkInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)    11344 2018-08-21 09:19:39.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateLaunchTemplateVersionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1954 2018-08-21 09:20:20.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstancePhysicalAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3170 2018-08-21 09:19:50.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceChargeTypeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2116 2018-08-21 09:20:15.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyEipAddressAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2336 2018-08-21 09:20:00.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyExRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2334 2018-08-21 09:20:04.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelPhysicalConnectionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1978 2018-08-21 09:20:19.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceTypesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2234 2018-08-21 09:19:51.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeClassicLinkInstancesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2034 2018-08-21 09:20:23.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1942 2018-08-21 09:20:19.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeIntranetAttributeKbRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1900 2018-08-21 09:20:26.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelCopyImageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2250 2018-08-21 09:20:08.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTagKeysRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1926 2018-08-21 09:19:44.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteRecycleBinRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2298 2018-08-21 09:20:09.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnassociateEipAddressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3266 2018-08-21 09:19:46.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInvocationsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1812 2018-08-21 09:20:00.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2258 2018-08-21 09:20:20.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeImageSharePermissionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2386 2018-08-21 09:20:06.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRouterInterfacesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3482 2018-08-21 09:20:05.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2266 2018-08-21 09:19:52.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceRamRoleRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4312 2018-08-21 09:20:26.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupEgressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1760 2018-08-21 09:19:45.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotsUsageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1768 2018-08-21 09:20:22.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4262 2018-08-21 09:19:48.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2058 2018-08-21 09:20:22.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteSnapshotRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2424 2018-08-21 09:20:26.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachDiskRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3174 2018-08-21 09:20:14.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2334 2018-08-21 09:20:02.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EnablePhysicalConnectionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2282 2018-08-21 09:20:12.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVSwitchAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2514 2018-08-21 09:20:03.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAccessPointsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2618 2018-08-21 09:19:59.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyExRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1748 2018-08-21 09:20:22.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeClustersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2595 2018-08-21 09:19:40.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AssignPrivateIpAddressesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4129 2018-08-21 09:20:17.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSecurityGroupsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2426 2018-08-21 09:20:08.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateHaVipRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2050 2018-08-21 09:19:53.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AddIpRangeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1796 2018-08-21 09:20:06.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeactivateRouterInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1734 2018-08-21 09:20:00.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2300 2018-08-21 09:20:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeZonesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2134 2018-08-21 09:20:11.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReleasePublicIpAddressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2744 2018-08-21 09:19:46.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyCommandRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2404 2018-08-21 09:19:44.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRecycleBinRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2442 2018-08-21 09:19:45.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyHpcClusterAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)    12788 2018-08-21 09:19:43.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RunInstancesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3072 2018-08-21 09:19:49.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyPrepayInstanceSpecRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2816 2018-08-21 09:19:47.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInvocationResultsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2406 2018-08-21 09:20:19.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceStatusRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2378 2018-08-21 09:20:21.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDiskMonitorDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2338 2018-08-21 09:19:41.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateNetworkInterfacePermissionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1908 2018-08-21 09:19:47.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteCommandRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2432 2018-08-21 09:20:13.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyIntranetBandwidthKbRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     8591 2018-08-21 09:20:20.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstancesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2148 2018-08-21 09:19:56.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceAutoReleaseTimeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2502 2018-08-21 09:19:57.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeBandwidthPackagesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2266 2018-08-21 09:20:07.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyHaVipAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4338 2018-08-21 09:19:52.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupRuleRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2286 2018-08-21 09:20:15.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyImageShareGroupPermissionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2043 2018-08-21 09:19:40.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeCloudAssistantStatusRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2144 2018-08-21 09:19:58.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteForwardEntryRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2238 2018-08-21 09:19:52.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotMonitorDataRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2216 2018-08-21 09:19:59.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EipFillParamsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2394 2018-08-21 09:20:02.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2958 2018-08-21 09:19:54.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateDeploymentSetRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3028 2018-08-21 09:19:57.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyForwardEntryRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2112 2018-08-21 09:19:43.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyUserBusinessBehaviorRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2914 2018-08-21 09:20:02.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribePhysicalConnectionsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2720 2018-08-21 09:19:42.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeBandwidthLimitationRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2618 2018-08-21 09:19:56.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotLinksRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2668 2018-08-21 09:20:02.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3748 2018-08-21 09:20:03.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateVirtualBorderRouterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3178 2018-08-21 09:19:54.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDeploymentSetsRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3076 2018-08-21 09:19:58.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateNatGatewayRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3495 2018-08-21 09:19:49.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateNetworkInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1790 2018-08-21 09:20:06.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ConnectRouterInterfaceRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     5499 2018-08-21 09:20:21.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeImagesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2400 2018-08-21 09:20:18.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeIpRangesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2126 2018-08-21 09:20:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/LeaveSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1936 2018-08-21 09:19:41.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/GetInstanceConsoleOutputRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3900 2018-08-21 09:20:04.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreatePhysicalConnectionRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2080 2018-08-21 09:20:09.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnbindIpRangeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3050 2018-08-21 09:19:41.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeResourcesModificationRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1938 2018-08-21 09:19:43.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeUserBusinessBehaviorRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3824 2018-08-21 09:20:02.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyPhysicalConnectionAttributeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2094 2018-08-21 09:19:52.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotPackageRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3942 2018-08-21 09:20:25.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CheckAutoSnapshotPolicyRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     4330 2018-08-21 09:20:11.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RevokeSecurityGroupRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2610 2018-08-21 09:19:48.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyDiskChargeTypeRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2248 2018-08-21 09:20:27.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AllocatePublicIpAddressRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2704 2018-08-21 09:20:16.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVSwitchesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3462 2018-08-21 09:19:43.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDisksFullStatusRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2964 2018-08-21 09:20:18.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRouteTablesRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     7202 2018-08-21 09:20:21.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDisksRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     2246 2018-08-21 09:20:03.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteVirtualBorderRouterRequest.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1722 2018-08-21 09:20:05.000000 aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTaskAttributeRequest.py
```

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/SOURCES.txt` & `aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyun_python_sdk_ecs.egg-info/PKG-INFO` & `aliyun-python-sdk-ecs-4.9.7/aliyun_python_sdk_ecs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ecs
-Version: 4.9.6
+Version: 4.9.7
 Summary: The ecs module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-ecs
         This is the ecs module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-ecs-4.9.6/PKG-INFO` & `aliyun-python-sdk-ecs-4.9.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ecs
-Version: 4.9.6
+Version: 4.9.7
 Summary: The ecs module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-ecs
         This is the ecs module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-ecs-4.9.6/setup.py` & `aliyun-python-sdk-ecs-4.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RevokeSecurityGroupEgressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RevokeSecurityGroupEgressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeHpcClustersRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeHpcClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReActivateInstancesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReActivateInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AllocateEipAddressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AllocateEipAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeLaunchTemplatesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeLaunchTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTagsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVRouterAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVRouterAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReleaseEipAddressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReleaseEipAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AddBandwidthPackageIpsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AddBandwidthPackageIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ResizeDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ResizeDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNewProjectEipMonitorDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNewProjectEipMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyLaunchTemplateDefaultVersionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyLaunchTemplateDefaultVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RenewInstanceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RenewInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EipNotifyPaidRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EipNotifyPaidRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachNetworkInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteRouterInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteRouterInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ImportImageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ImportImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyImageAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyImageAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/StartInstanceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/StartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeKeyPairsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeKeyPairsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeLaunchTemplateVersionsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeLaunchTemplateVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateLaunchTemplateRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateLaunchTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAvailableResourceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAvailableResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacePermissionsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacePermissionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateHpcClusterRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateHpcClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteVpcRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupEgressRuleRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupEgressRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceSpecRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateVersionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteHpcClusterRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteHpcClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceAutoRenewAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CopyImageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CopyImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAccountAttributesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAccountAttributesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/StopInstanceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/StopInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateSnapshotRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyDiskAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyDiskAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteBandwidthPackageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteBandwidthPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyDeploymentSetAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyDeploymentSetAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeCommandsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeCommandsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeResourceByTagsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeResourceByTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceVpcAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceVpcAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachInstanceRamRoleRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachInstanceRamRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/GetInstanceScreenshotRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/GetInstanceScreenshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeletePhysicalConnectionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeletePhysicalConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachKeyPairRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceVncPasswdRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceVncPasswdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceMonitorDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyImageSharePermissionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyImageSharePermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceVncUrlRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceVncUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateKeyPairRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RemoveBandwidthPackageIpsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RemoveBandwidthPackageIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ConvertNatPublicIpToEipRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ConvertNatPublicIpToEipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEventDetailRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEventDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ExportImageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ExportImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRenewalPriceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRenewalPriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVirtualBorderRouterAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVirtualBorderRouterAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRecommendInstanceTypeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRecommendInstanceTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyBandwidthPackageSpecRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyBandwidthPackageSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceSpecRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySnapshotAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySnapshotAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstancesFullStatusRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstancesFullStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelTaskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDeploymentSetTopologyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDeploymentSetTopologyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEniMonitorDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEniMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEipMonitorDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEipMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNatGatewaysRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNatGatewaysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTasksRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EipFillProductRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EipFillProductRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ValidateSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ValidateSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVpcsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVpcsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyNetworkInterfaceAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyNetworkInterfaceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ApplyAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ApplyAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteKeyPairsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteKeyPairsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReplaceSystemDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReplaceSystemDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVRoutersRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVRoutersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelAgreementRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelAgreementRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceTypeFamiliesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceTypeFamiliesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateCommandRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteHaVipRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteHaVipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeEipAddressesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeEipAddressesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachNetworkInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribePriceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribePriceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/JoinSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/JoinSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/InstallCloudAssistantRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/InstallCloudAssistantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/JoinResourceGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/JoinResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnassociateHaVipRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnassociateHaVipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateImageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeUserDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeUserDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSpotPriceHistoryRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSpotPriceHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeLimitationRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeLimitationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeForwardTableEntriesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeForwardTableEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachClassicLinkVpcRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachClassicLinkVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceVncPasswdRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceVncPasswdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RemoveTagsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RemoveTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceAutoRenewAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceAutoRenewAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ActivateRouterInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ActivateRouterInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteInstanceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReInitDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReInitDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateInstanceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateInstanceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -294,14 +294,20 @@
 
 	def get_ClusterId(self):
 		return self.get_query_params().get('ClusterId')
 
 	def set_ClusterId(self,ClusterId):
 		self.add_query_param('ClusterId',ClusterId)
 
+	def get_CreditSpecification(self):
+		return self.get_query_params().get('CreditSpecification')
+
+	def set_CreditSpecification(self,CreditSpecification):
+		self.add_query_param('CreditSpecification',CreditSpecification)
+
 	def get_DataDisks(self):
 		return self.get_query_params().get('DataDisks')
 
 	def set_DataDisks(self,DataDisks):
 		for i in range(len(DataDisks)):	
 			if DataDisks[i].get('DiskName') is not None:
 				self.add_query_param('DataDisk.' + str(i + 1) + '.DiskName' , DataDisks[i].get('DiskName'))
```

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSecurityGroupReferencesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSecurityGroupReferencesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateForwardEntryRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateForwardEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AssociateEipAddressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AssociateEipAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/InvokeCommandRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/InvokeCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/StopInvocationRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/StopInvocationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AddTagsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AddTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CheckDiskEnableAutoSnapshotValidationRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CheckDiskEnableAutoSnapshotValidationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteRouteEntryRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteDeploymentSetRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteDeploymentSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DetachInstanceRamRoleRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DetachInstanceRamRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ImportKeyPairRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ImportKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/TerminatePhysicalConnectionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/TerminatePhysicalConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/BindIpRangeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/BindIpRangeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeImageSupportInstanceTypesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeImageSupportInstanceTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteNetworkInterfacePermissionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteNetworkInterfacePermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteLaunchTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RebootInstanceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RebootInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ResetDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ResetDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateRouterInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateRouterInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceNetworkSpecRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceNetworkSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteVSwitchRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteVSwitchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AssociateHaVipRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AssociateHaVipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachKeyPairRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateVpcRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateVSwitchRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateVSwitchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/SignAgreementRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/SignAgreementRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnassignPrivateIpAddressesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnassignPrivateIpAddressesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSecurityGroupAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSecurityGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteNatGatewayRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteNatGatewayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeHaVipsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeHaVipsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateRouteEntryRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateRouteEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RecoverVirtualBorderRouterRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RecoverVirtualBorderRouterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachClassicLinkVpcRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachClassicLinkVpcRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceHistoryEventsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceHistoryEventsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRegionsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVpcAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVpcAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/TerminateVirtualBorderRouterRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/TerminateVirtualBorderRouterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteNetworkInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateLaunchTemplateVersionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateLaunchTemplateVersionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstancePhysicalAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstancePhysicalAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceChargeTypeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceChargeTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyEipAddressAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyEipAddressAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyExRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyExRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelPhysicalConnectionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelPhysicalConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceTypesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceTypesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeClassicLinkInstancesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeClassicLinkInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteImageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeIntranetAttributeKbRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeIntranetAttributeKbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelCopyImageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelCopyImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTagKeysRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteRecycleBinRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteRecycleBinRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnassociateEipAddressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnassociateEipAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInvocationsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInvocationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeImageSharePermissionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeImageSharePermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRouterInterfacesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRouterInterfacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyRouterInterfaceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceRamRoleRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceRamRoleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupEgressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AuthorizeSecurityGroupEgressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotsUsageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotsUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeNetworkInterfacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteSnapshotRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AttachDiskRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AttachDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceAttributeRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,50 +19,20 @@
 
 from aliyunsdkcore.request import RpcRequest
 class ModifyInstanceAttributeRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'Ecs', '2014-05-26', 'ModifyInstanceAttribute','ecs')
 
-	def get_UserData(self):
-		return self.get_query_params().get('UserData')
-
-	def set_UserData(self,UserData):
-		self.add_query_param('UserData',UserData)
-
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
-	def get_Password(self):
-		return self.get_query_params().get('Password')
-
-	def set_Password(self,Password):
-		self.add_query_param('Password',Password)
-
-	def get_HostName(self):
-		return self.get_query_params().get('HostName')
-
-	def set_HostName(self,HostName):
-		self.add_query_param('HostName',HostName)
-
-	def get_InstanceId(self):
-		return self.get_query_params().get('InstanceId')
-
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_InstanceName(self):
-		return self.get_query_params().get('InstanceName')
-
-	def set_InstanceName(self,InstanceName):
-		self.add_query_param('InstanceName',InstanceName)
-
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
 	def get_Recyclable(self):
@@ -79,12 +49,48 @@
 
 	def get_Description(self):
 		return self.get_query_params().get('Description')
 
 	def set_Description(self,Description):
 		self.add_query_param('Description',Description)
 
+	def get_CreditSpecification(self):
+		return self.get_query_params().get('CreditSpecification')
+
+	def set_CreditSpecification(self,CreditSpecification):
+		self.add_query_param('CreditSpecification',CreditSpecification)
+
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_UserData(self):
+		return self.get_query_params().get('UserData')
+
+	def set_UserData(self,UserData):
+		self.add_query_param('UserData',UserData)
+
+	def get_Password(self):
+		return self.get_query_params().get('Password')
+
+	def set_Password(self,Password):
+		self.add_query_param('Password',Password)
+
+	def get_HostName(self):
+		return self.get_query_params().get('HostName')
+
+	def set_HostName(self,HostName):
+		self.add_query_param('HostName',HostName)
+
+	def get_InstanceId(self):
+		return self.get_query_params().get('InstanceId')
+
+	def set_InstanceId(self,InstanceId):
+		self.add_query_param('InstanceId',InstanceId)
+
+	def get_InstanceName(self):
+		return self.get_query_params().get('InstanceName')
+
+	def set_InstanceName(self,InstanceName):
+		self.add_query_param('InstanceName',InstanceName)
```

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EnablePhysicalConnectionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EnablePhysicalConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyVSwitchAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyVSwitchAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeAccessPointsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeAccessPointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyExRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyAutoSnapshotPolicyExRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeClustersRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AssignPrivateIpAddressesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AssignPrivateIpAddressesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSecurityGroupsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSecurityGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateHaVipRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateHaVipRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AddIpRangeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AddIpRangeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeactivateRouterInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeactivateRouterInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CancelAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CancelAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeZonesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ReleasePublicIpAddressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ReleasePublicIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyCommandRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRecycleBinRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRecycleBinRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyHpcClusterAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyHpcClusterAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RunInstancesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RunInstancesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,20 @@
 
 	def get_DedicatedHostId(self):
 		return self.get_query_params().get('DedicatedHostId')
 
 	def set_DedicatedHostId(self,DedicatedHostId):
 		self.add_query_param('DedicatedHostId',DedicatedHostId)
 
+	def get_CreditSpecification(self):
+		return self.get_query_params().get('CreditSpecification')
+
+	def set_CreditSpecification(self,CreditSpecification):
+		self.add_query_param('CreditSpecification',CreditSpecification)
+
 	def get_DataDisks(self):
 		return self.get_query_params().get('DataDisks')
 
 	def set_DataDisks(self,DataDisks):
 		for i in range(len(DataDisks)):	
 			if DataDisks[i].get('Size') is not None:
 				self.add_query_param('DataDisk.' + str(i + 1) + '.Size' , DataDisks[i].get('Size'))
```

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyPrepayInstanceSpecRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyPrepayInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInvocationResultsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInvocationResultsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstanceStatusRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstanceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDiskMonitorDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDiskMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateNetworkInterfacePermissionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateNetworkInterfacePermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteCommandRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyIntranetBandwidthKbRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyIntranetBandwidthKbRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeInstancesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyInstanceAutoReleaseTimeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyInstanceAutoReleaseTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeBandwidthPackagesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeBandwidthPackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyHaVipAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyHaVipAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifySecurityGroupRuleRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifySecurityGroupRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyImageShareGroupPermissionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyImageShareGroupPermissionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeCloudAssistantStatusRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeCloudAssistantStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteForwardEntryRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteForwardEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotMonitorDataRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/EipFillParamsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/EipFillParamsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateDeploymentSetRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateDeploymentSetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyForwardEntryRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyForwardEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyUserBusinessBehaviorRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyUserBusinessBehaviorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribePhysicalConnectionsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribePhysicalConnectionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeBandwidthLimitationRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeBandwidthLimitationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotLinksRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotLinksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVirtualBorderRoutersForPhysicalConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateVirtualBorderRouterRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateVirtualBorderRouterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDeploymentSetsRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDeploymentSetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateNatGatewayRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateNatGatewayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreateNetworkInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreateNetworkInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ConnectRouterInterfaceRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ConnectRouterInterfaceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeImagesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeIpRangesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeIpRangesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/LeaveSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/LeaveSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/GetInstanceConsoleOutputRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/GetInstanceConsoleOutputRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CreatePhysicalConnectionRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CreatePhysicalConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/UnbindIpRangeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/UnbindIpRangeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeResourcesModificationRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeResourcesModificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeUserBusinessBehaviorRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeUserBusinessBehaviorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyPhysicalConnectionAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyPhysicalConnectionAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeSnapshotPackageRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeSnapshotPackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/CheckAutoSnapshotPolicyRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/CheckAutoSnapshotPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/RevokeSecurityGroupRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/RevokeSecurityGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/ModifyDiskChargeTypeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/ModifyDiskChargeTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/AllocatePublicIpAddressRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/AllocatePublicIpAddressRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeVSwitchesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeVSwitchesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDisksFullStatusRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDisksFullStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeRouteTablesRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeRouteTablesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeDisksRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeDisksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DeleteVirtualBorderRouterRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DeleteVirtualBorderRouterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ecs-4.9.6/aliyunsdkecs/request/v20140526/DescribeTaskAttributeRequest.py` & `aliyun-python-sdk-ecs-4.9.7/aliyunsdkecs/request/v20140526/DescribeTaskAttributeRequest.py`

 * *Files identical despite different names*

