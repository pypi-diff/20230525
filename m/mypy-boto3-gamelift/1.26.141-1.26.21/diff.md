# Comparing `tmp/mypy-boto3-gamelift-1.26.141.tar.gz` & `tmp/mypy-boto3-gamelift-1.26.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamelift-1.26.141.tar", last modified: Thu May 25 19:32:48 2023, max compression
+gzip compressed data, was "mypy-boto3-gamelift-1.26.21.tar", last modified: Thu Dec  1 20:25:43 2022, max compression
```

## Comparing `mypy-boto3-gamelift-1.26.141.tar` & `mypy-boto3-gamelift-1.26.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.424743 mypy-boto3-gamelift-1.26.141/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28898 2023-05-25 19:32:48.420742 mypy-boto3-gamelift-1.26.141/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27405 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.420742 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84696 2023-05-25 19:31:57.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    84563 2023-05-25 19:31:57.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-05-25 19:31:57.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20493 2023-05-25 19:31:57.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26546 2023-05-25 19:31:57.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26522 2023-05-25 19:31:57.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97993 2023-05-25 19:32:00.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97894 2023-05-25 19:31:59.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.420742 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28898 2023-05-25 19:32:48.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-25 19:32:48.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:48.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:48.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 19:32:48.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 19:32:48.000000 mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:32:48.424743 mypy-boto3-gamelift-1.26.141/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 19:31:56.000000 mypy-boto3-gamelift-1.26.141/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.798803 mypy-boto3-gamelift-1.26.21/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    28806 2022-12-01 20:25:43.794803 mypy-boto3-gamelift-1.26.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    27365 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.790803 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (122)     5348 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5347 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84394 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84261 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    20116 2022-12-01 20:25:30.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20114 2022-12-01 20:25:30.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    26546 2022-12-01 20:25:30.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26522 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    97714 2022-12-01 20:25:32.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    97615 2022-12-01 20:25:31.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.794803 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28806 2022-12-01 20:25:43.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2022-12-01 20:25:43.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-01 20:25:43.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2022-12-01 20:25:43.000000 mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 20:25:43.798803 mypy-boto3-gamelift-1.26.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2022-12-01 20:25:29.000000 mypy-boto3-gamelift-1.26.21/setup.py
```

### Comparing `mypy-boto3-gamelift-1.26.141/LICENSE` & `mypy-boto3-gamelift-1.26.21/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-gamelift-1.26.141/PKG-INFO` & `mypy-boto3-gamelift-1.26.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.26.141
-Summary: Type annotations for boto3.GameLift 1.26.141 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.21
+Summary: Type annotations for boto3.GameLift 1.26.21 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamelift?color=blue)](https://pypistats.org/packages/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,15 +392,14 @@
     DescribeInstancesPaginatorName,
     DescribeMatchmakingConfigurationsPaginatorName,
     DescribeMatchmakingRuleSetsPaginatorName,
     DescribePlayerSessionsPaginatorName,
     DescribeScalingPoliciesPaginatorName,
     EC2InstanceTypeType,
     EventCodeType,
-    FilterInstanceStatusType,
     FleetActionType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerClaimStatusType,
     GameServerGroupActionType,
     GameServerGroupDeleteOptionType,
@@ -463,15 +461,15 @@
     AcceptMatchInputRequestTypeDef,
     RoutingStrategyTypeDef,
     AnywhereConfigurationTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
     BuildTypeDef,
     CertificateConfigurationTypeDef,
-    ClaimFilterOptionTypeDef,
+    ClaimGameServerInputRequestTypeDef,
     GameServerTypeDef,
     ResponseMetadataTypeDef,
     ComputeTypeDef,
     TagTypeDef,
     S3LocationTypeDef,
     IpPermissionTypeDef,
     LocationConfigurationTypeDef,
@@ -580,15 +578,14 @@
     UpdateGameServerInputRequestTypeDef,
     UpdateGameSessionInputRequestTypeDef,
     ValidateMatchmakingRuleSetInputRequestTypeDef,
     VpcPeeringConnectionStatusTypeDef,
     AliasTypeDef,
     UpdateAliasInputRequestTypeDef,
     PlayerTypeDef,
-    ClaimGameServerInputRequestTypeDef,
     ClaimGameServerOutputTypeDef,
     DescribeBuildOutputTypeDef,
     DescribeGameServerOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
@@ -744,42 +741,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-gamelift-1.26.141/README.md` & `mypy-boto3-gamelift-1.26.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamelift?color=blue)](https://pypistats.org/packages/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,15 +361,14 @@
     DescribeInstancesPaginatorName,
     DescribeMatchmakingConfigurationsPaginatorName,
     DescribeMatchmakingRuleSetsPaginatorName,
     DescribePlayerSessionsPaginatorName,
     DescribeScalingPoliciesPaginatorName,
     EC2InstanceTypeType,
     EventCodeType,
-    FilterInstanceStatusType,
     FleetActionType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerClaimStatusType,
     GameServerGroupActionType,
     GameServerGroupDeleteOptionType,
@@ -431,15 +430,15 @@
     AcceptMatchInputRequestTypeDef,
     RoutingStrategyTypeDef,
     AnywhereConfigurationTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
     BuildTypeDef,
     CertificateConfigurationTypeDef,
-    ClaimFilterOptionTypeDef,
+    ClaimGameServerInputRequestTypeDef,
     GameServerTypeDef,
     ResponseMetadataTypeDef,
     ComputeTypeDef,
     TagTypeDef,
     S3LocationTypeDef,
     IpPermissionTypeDef,
     LocationConfigurationTypeDef,
@@ -548,15 +547,14 @@
     UpdateGameServerInputRequestTypeDef,
     UpdateGameSessionInputRequestTypeDef,
     ValidateMatchmakingRuleSetInputRequestTypeDef,
     VpcPeeringConnectionStatusTypeDef,
     AliasTypeDef,
     UpdateAliasInputRequestTypeDef,
     PlayerTypeDef,
-    ClaimGameServerInputRequestTypeDef,
     ClaimGameServerOutputTypeDef,
     DescribeBuildOutputTypeDef,
     DescribeGameServerOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
@@ -712,42 +710,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/__init__.py` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/__init__.pyi` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/__main__.py` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameLift 1.26.141\nVersion:         1.26.141\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.GameLift 1.26.21\nVersion:         1.26.21\nBuilder version:"
+        " 7.11.11\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.141")
+    print("1.26.21")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/client.py` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 from .type_defs import (
     AnywhereConfigurationTypeDef,
     CertificateConfigurationTypeDef,
-    ClaimFilterOptionTypeDef,
     ClaimGameServerOutputTypeDef,
     CreateAliasOutputTypeDef,
     CreateBuildOutputTypeDef,
     CreateFleetLocationsOutputTypeDef,
     CreateFleetOutputTypeDef,
     CreateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
@@ -248,25 +247,20 @@
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#can_paginate)
         """
 
     def claim_game_server(
-        self,
-        *,
-        GameServerGroupName: str,
-        GameServerId: str = ...,
-        GameServerData: str = ...,
-        FilterOption: ClaimFilterOptionTypeDef = ...
+        self, *, GameServerGroupName: str, GameServerId: str = ..., GameServerData: str = ...
     ) -> ClaimGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Locates an available game server and temporarily reserves it to
-        host gameplay and players.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Locates an available game server and temporarily reserves it to host
+        gameplay and players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.claim_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#claim_game_server)
         """
 
     def close(self) -> None:
         """
@@ -331,16 +325,16 @@
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
         Locations: Sequence[LocationConfigurationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ComputeType: ComputeTypeType = ...,
         AnywhereConfiguration: AnywhereConfigurationTypeDef = ...
     ) -> CreateFleetOutputTypeDef:
         """
-        Creates a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances to host
-        your custom game server or Realtime Servers.
+        Creates a fleet of Amazon Elastic Compute Cloud (Amazon Elastic Compute Cloud)
+        instances to host your custom game server or Realtime Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_fleet)
         """
 
     def create_fleet_locations(
         self, *, FleetId: str, Locations: Sequence[LocationConfigurationTypeDef]
@@ -365,18 +359,17 @@
         AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,
         BalancingStrategy: BalancingStrategyType = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         VpcSubnets: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Creates a Amazon GameLift FleetIQ game server group for
-        managing game hosting on a collection of Amazon Elastic Compute Cloud instances
-        for game hosting.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Creates a GameLift FleetIQ game server group for managing game hosting
+        on a collection of Amazon Elastic Compute Cloud instances for game hosting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_game_server_group)
         """
 
     def create_game_session(
         self,
@@ -562,17 +555,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_fleet_locations)
         """
 
     def delete_game_server_group(
         self, *, GameServerGroupName: str, DeleteOption: GameServerGroupDeleteOptionType = ...
     ) -> DeleteGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Terminates a game server group and permanently deletes the game
-        server group record.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Terminates a game server group and permanently deletes the game server
+        group record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_game_server_group)
         """
 
     def delete_game_session_queue(self, *, Name: str) -> Dict[str, Any]:
         """
@@ -650,16 +643,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#deregister_compute)
         """
 
     def deregister_game_server(
         self, *, GameServerGroupName: str, GameServerId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Removes the game server from a game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Removes the game server from a game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.deregister_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#deregister_game_server)
         """
 
     def describe_alias(self, *, AliasId: str) -> DescribeAliasOutputTypeDef:
         """
@@ -789,44 +782,44 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_utilization)
         """
 
     def describe_game_server(
         self, *, GameServerGroupName: str, GameServerId: str
     ) -> DescribeGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves information for a registered game server.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves information for a registered game server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_server)
         """
 
     def describe_game_server_group(
         self, *, GameServerGroupName: str
     ) -> DescribeGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves information on a game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves information on a game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_server_group)
         """
 
     def describe_game_server_instances(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
         Limit: int = ...,
         NextToken: str = ...
     ) -> DescribeGameServerInstancesOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves status information about the Amazon EC2 instances
-        associated with a Amazon GameLift FleetIQ game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves status information about the Amazon EC2 instances associated
+        with a GameLift FleetIQ game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_server_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_server_instances)
         """
 
     def describe_game_session_details(
         self,
@@ -1031,24 +1024,23 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_access)
         """
 
     def get_compute_auth_token(
         self, *, FleetId: str, ComputeName: str
     ) -> GetComputeAuthTokenOutputTypeDef:
         """
-        Requests an authentication token from Amazon GameLift.
+        Requests an authorization token from GameLift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_auth_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_auth_token)
         """
 
     def get_game_session_log_url(self, *, GameSessionId: str) -> GetGameSessionLogUrlOutputTypeDef:
         """
-        Retrieves the location of stored game session logs for a specified game session
-        on Amazon GameLift managed fleets.
+        Retrieves the location of stored game session logs for a specified game session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_game_session_log_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_game_session_log_url)
         """
 
     def get_instance_access(
         self, *, FleetId: str, InstanceId: str
@@ -1122,17 +1114,17 @@
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
         Limit: int = ...,
         NextToken: str = ...
     ) -> ListGameServersOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves information on all game servers that are currently
-        active in a specified game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves information on all game servers that are currently active in
+        a specified game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_game_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_game_servers)
         """
 
     def list_locations(
         self, *, Filters: Sequence[LocationFilterType] = ..., Limit: int = ..., NextToken: str = ...
@@ -1151,15 +1143,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_scripts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_scripts)
         """
 
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Retrieves all tags assigned to a Amazon GameLift resource.
+        Retrieves all tags that are assigned to a GameLift resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_tags_for_resource)
         """
 
     def put_scaling_policy(
         self,
@@ -1205,17 +1197,17 @@
         GameServerGroupName: str,
         GameServerId: str,
         InstanceId: str,
         ConnectionInfo: str = ...,
         GameServerData: str = ...
     ) -> RegisterGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Creates a new game server resource and notifies Amazon GameLift
-        FleetIQ that the game server is ready to host gameplay and players.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Creates a new game server resource and notifies GameLift FleetIQ that
+        the game server is ready to host gameplay and players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.register_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#register_game_server)
         """
 
     def request_upload_credentials(self, *, BuildId: str) -> RequestUploadCredentialsOutputTypeDef:
         """
@@ -1237,16 +1229,16 @@
     def resume_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
     ) -> ResumeGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Reinstates activity on a game server group after it has been
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Reinstates activity on a game server group after it has been
         suspended.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resume_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#resume_game_server_group)
         """
 
     def search_game_sessions(
@@ -1356,33 +1348,33 @@
     def suspend_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
     ) -> SuspendGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Temporarily stops activity on a game server group without
-        terminating instances or the game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Temporarily stops activity on a game server group without terminating
+        instances or the game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.suspend_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#suspend_game_server_group)
         """
 
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Assigns a tag to an Amazon GameLift resource.
+        Assigns a tag to a GameLift resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#tag_resource)
         """
 
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes a tag assigned to a Amazon GameLift resource.
+        Removes a tag that is assigned to a GameLift resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#untag_resource)
         """
 
     def update_alias(
         self,
@@ -1465,17 +1457,17 @@
         GameServerGroupName: str,
         GameServerId: str,
         GameServerData: str = ...,
         UtilizationStatus: GameServerUtilizationStatusType = ...,
         HealthCheck: Literal["HEALTHY"] = ...
     ) -> UpdateGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Updates information about a registered game server to help
-        Amazon GameLift FleetIQ to track game server availability.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Updates information about a registered game server to help GameLift
+        FleetIQ to track game server availability.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_game_server)
         """
 
     def update_game_server_group(
         self,
@@ -1483,17 +1475,16 @@
         GameServerGroupName: str,
         RoleArn: str = ...,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         BalancingStrategy: BalancingStrategyType = ...
     ) -> UpdateGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Updates Amazon GameLift FleetIQ-specific properties for a game
-        server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Updates GameLift FleetIQ-specific properties for a game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_game_server_group)
         """
 
     def update_game_session(
         self,
@@ -1557,15 +1548,15 @@
         """
 
     def update_runtime_configuration(
         self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
-        Amazon GameLift how to launch server processes on all instances in the fleet.
+        GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
         """
 
     def update_script(
         self,
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/client.pyi` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 from .type_defs import (
     AnywhereConfigurationTypeDef,
     CertificateConfigurationTypeDef,
-    ClaimFilterOptionTypeDef,
     ClaimGameServerOutputTypeDef,
     CreateAliasOutputTypeDef,
     CreateBuildOutputTypeDef,
     CreateFleetLocationsOutputTypeDef,
     CreateFleetOutputTypeDef,
     CreateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
@@ -241,25 +240,20 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#can_paginate)
         """
     def claim_game_server(
-        self,
-        *,
-        GameServerGroupName: str,
-        GameServerId: str = ...,
-        GameServerData: str = ...,
-        FilterOption: ClaimFilterOptionTypeDef = ...
+        self, *, GameServerGroupName: str, GameServerId: str = ..., GameServerData: str = ...
     ) -> ClaimGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Locates an available game server and temporarily reserves it to
-        host gameplay and players.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Locates an available game server and temporarily reserves it to host
+        gameplay and players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.claim_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#claim_game_server)
         """
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
@@ -320,16 +314,16 @@
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
         Locations: Sequence[LocationConfigurationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ComputeType: ComputeTypeType = ...,
         AnywhereConfiguration: AnywhereConfigurationTypeDef = ...
     ) -> CreateFleetOutputTypeDef:
         """
-        Creates a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances to host
-        your custom game server or Realtime Servers.
+        Creates a fleet of Amazon Elastic Compute Cloud (Amazon Elastic Compute Cloud)
+        instances to host your custom game server or Realtime Servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_fleet)
         """
     def create_fleet_locations(
         self, *, FleetId: str, Locations: Sequence[LocationConfigurationTypeDef]
     ) -> CreateFleetLocationsOutputTypeDef:
@@ -352,18 +346,17 @@
         AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,
         BalancingStrategy: BalancingStrategyType = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         VpcSubnets: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Creates a Amazon GameLift FleetIQ game server group for
-        managing game hosting on a collection of Amazon Elastic Compute Cloud instances
-        for game hosting.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Creates a GameLift FleetIQ game server group for managing game hosting
+        on a collection of Amazon Elastic Compute Cloud instances for game hosting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_game_server_group)
         """
     def create_game_session(
         self,
         *,
@@ -534,17 +527,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_fleet_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_fleet_locations)
         """
     def delete_game_server_group(
         self, *, GameServerGroupName: str, DeleteOption: GameServerGroupDeleteOptionType = ...
     ) -> DeleteGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Terminates a game server group and permanently deletes the game
-        server group record.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Terminates a game server group and permanently deletes the game server
+        group record.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_game_server_group)
         """
     def delete_game_session_queue(self, *, Name: str) -> Dict[str, Any]:
         """
         Deletes a game session queue.
@@ -612,16 +605,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.deregister_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#deregister_compute)
         """
     def deregister_game_server(
         self, *, GameServerGroupName: str, GameServerId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Removes the game server from a game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Removes the game server from a game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.deregister_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#deregister_game_server)
         """
     def describe_alias(self, *, AliasId: str) -> DescribeAliasOutputTypeDef:
         """
         Retrieves properties for an alias.
@@ -738,42 +731,42 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_utilization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_utilization)
         """
     def describe_game_server(
         self, *, GameServerGroupName: str, GameServerId: str
     ) -> DescribeGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves information for a registered game server.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves information for a registered game server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_server)
         """
     def describe_game_server_group(
         self, *, GameServerGroupName: str
     ) -> DescribeGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves information on a game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves information on a game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_server_group)
         """
     def describe_game_server_instances(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
         Limit: int = ...,
         NextToken: str = ...
     ) -> DescribeGameServerInstancesOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves status information about the Amazon EC2 instances
-        associated with a Amazon GameLift FleetIQ game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves status information about the Amazon EC2 instances associated
+        with a GameLift FleetIQ game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_server_instances)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_server_instances)
         """
     def describe_game_session_details(
         self,
         *,
@@ -961,23 +954,22 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_access)
         """
     def get_compute_auth_token(
         self, *, FleetId: str, ComputeName: str
     ) -> GetComputeAuthTokenOutputTypeDef:
         """
-        Requests an authentication token from Amazon GameLift.
+        Requests an authorization token from GameLift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_auth_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_auth_token)
         """
     def get_game_session_log_url(self, *, GameSessionId: str) -> GetGameSessionLogUrlOutputTypeDef:
         """
-        Retrieves the location of stored game session logs for a specified game session
-        on Amazon GameLift managed fleets.
+        Retrieves the location of stored game session logs for a specified game session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_game_session_log_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_game_session_log_url)
         """
     def get_instance_access(
         self, *, FleetId: str, InstanceId: str
     ) -> GetInstanceAccessOutputTypeDef:
@@ -1044,17 +1036,17 @@
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
         Limit: int = ...,
         NextToken: str = ...
     ) -> ListGameServersOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Retrieves information on all game servers that are currently
-        active in a specified game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Retrieves information on all game servers that are currently active in
+        a specified game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_game_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_game_servers)
         """
     def list_locations(
         self, *, Filters: Sequence[LocationFilterType] = ..., Limit: int = ..., NextToken: str = ...
     ) -> ListLocationsOutputTypeDef:
@@ -1070,15 +1062,15 @@
         Amazon Web Services account in use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_scripts)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_scripts)
         """
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
-        Retrieves all tags assigned to a Amazon GameLift resource.
+        Retrieves all tags that are assigned to a GameLift resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_tags_for_resource)
         """
     def put_scaling_policy(
         self,
         *,
@@ -1121,17 +1113,17 @@
         GameServerGroupName: str,
         GameServerId: str,
         InstanceId: str,
         ConnectionInfo: str = ...,
         GameServerData: str = ...
     ) -> RegisterGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Creates a new game server resource and notifies Amazon GameLift
-        FleetIQ that the game server is ready to host gameplay and players.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Creates a new game server resource and notifies GameLift FleetIQ that
+        the game server is ready to host gameplay and players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.register_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#register_game_server)
         """
     def request_upload_credentials(self, *, BuildId: str) -> RequestUploadCredentialsOutputTypeDef:
         """
         Retrieves a fresh set of credentials for use when uploading a new set of game
@@ -1150,16 +1142,16 @@
     def resume_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
     ) -> ResumeGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Reinstates activity on a game server group after it has been
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Reinstates activity on a game server group after it has been
         suspended.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resume_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#resume_game_server_group)
         """
     def search_game_sessions(
         self,
@@ -1260,31 +1252,31 @@
     def suspend_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
     ) -> SuspendGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Temporarily stops activity on a game server group without
-        terminating instances or the game server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Temporarily stops activity on a game server group without terminating
+        instances or the game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.suspend_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#suspend_game_server_group)
         """
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Assigns a tag to an Amazon GameLift resource.
+        Assigns a tag to a GameLift resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#tag_resource)
         """
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes a tag assigned to a Amazon GameLift resource.
+        Removes a tag that is assigned to a GameLift resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#untag_resource)
         """
     def update_alias(
         self,
         *,
@@ -1361,34 +1353,33 @@
         GameServerGroupName: str,
         GameServerId: str,
         GameServerData: str = ...,
         UtilizationStatus: GameServerUtilizationStatusType = ...,
         HealthCheck: Literal["HEALTHY"] = ...
     ) -> UpdateGameServerOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Updates information about a registered game server to help
-        Amazon GameLift FleetIQ to track game server availability.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Updates information about a registered game server to help GameLift
+        FleetIQ to track game server availability.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_game_server)
         """
     def update_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         RoleArn: str = ...,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         BalancingStrategy: BalancingStrategyType = ...
     ) -> UpdateGameServerGroupOutputTypeDef:
         """
-        **This operation is used with the Amazon GameLift FleetIQ solution and game
-        server groups.** Updates Amazon GameLift FleetIQ-specific properties for a game
-        server group.
+        **This operation is used with the GameLift FleetIQ solution and game server
+        groups.** Updates GameLift FleetIQ-specific properties for a game server group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_server_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_game_server_group)
         """
     def update_game_session(
         self,
         *,
@@ -1448,15 +1439,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
     def update_runtime_configuration(
         self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
         Updates the current runtime configuration for the specified fleet, which tells
-        Amazon GameLift how to launch server processes on all instances in the fleet.
+        GameLift how to launch server processes on all instances in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
         """
     def update_script(
         self,
         *,
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/literals.py` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceptanceTypeType",
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
@@ -39,15 +38,14 @@
     "DescribeInstancesPaginatorName",
     "DescribeMatchmakingConfigurationsPaginatorName",
     "DescribeMatchmakingRuleSetsPaginatorName",
     "DescribePlayerSessionsPaginatorName",
     "DescribeScalingPoliciesPaginatorName",
     "EC2InstanceTypeType",
     "EventCodeType",
-    "FilterInstanceStatusType",
     "FleetActionType",
     "FleetStatusType",
     "FleetTypeType",
     "FlexMatchModeType",
     "GameServerClaimStatusType",
     "GameServerGroupActionType",
     "GameServerGroupDeleteOptionType",
@@ -88,15 +86,14 @@
     "GameLiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptanceTypeType = Literal["ACCEPT", "REJECT"]
 BackfillModeType = Literal["AUTOMATIC", "MANUAL"]
 BalancingStrategyType = Literal["ON_DEMAND_ONLY", "SPOT_ONLY", "SPOT_PREFERRED"]
 BuildStatusType = Literal["FAILED", "INITIALIZED", "READY"]
 CertificateTypeType = Literal["DISABLED", "GENERATED"]
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
@@ -267,15 +264,14 @@
     "SERVER_PROCESS_FORCE_TERMINATED",
     "SERVER_PROCESS_INVALID_PATH",
     "SERVER_PROCESS_PROCESS_EXIT_TIMEOUT",
     "SERVER_PROCESS_PROCESS_READY_TIMEOUT",
     "SERVER_PROCESS_SDK_INITIALIZATION_TIMEOUT",
     "SERVER_PROCESS_TERMINATED_UNHEALTHY",
 ]
-FilterInstanceStatusType = Literal["ACTIVE", "DRAINING"]
 FleetActionType = Literal["AUTO_SCALING"]
 FleetStatusType = Literal[
     "ACTIVATING",
     "ACTIVE",
     "BUILDING",
     "DELETING",
     "DOWNLOADING",
@@ -422,15 +418,15 @@
     "CurrentPlayerSessions",
     "IdleInstances",
     "PercentAvailableGameSessions",
     "PercentIdleInstances",
     "QueueDepth",
     "WaitTime",
 ]
-OperatingSystemType = Literal["AMAZON_LINUX", "AMAZON_LINUX_2", "WINDOWS_2012", "WINDOWS_2016"]
+OperatingSystemType = Literal["AMAZON_LINUX", "AMAZON_LINUX_2", "WINDOWS_2012"]
 PlayerSessionCreationPolicyType = Literal["ACCEPT_ALL", "DENY_ALL"]
 PlayerSessionStatusType = Literal["ACTIVE", "COMPLETED", "RESERVED", "TIMEDOUT"]
 PolicyTypeType = Literal["RuleBased", "TargetBased"]
 PriorityTypeType = Literal["COST", "DESTINATION", "LATENCY", "LOCATION"]
 ProtectionPolicyType = Literal["FullProtection", "NoProtection"]
 RoutingStrategyTypeType = Literal["SIMPLE", "TERMINAL"]
 ScalingAdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
@@ -479,26 +475,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -584,15 +578,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -603,38 +596,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -647,15 +636,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -674,15 +662,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -722,15 +709,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -764,20 +750,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/literals.pyi` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AcceptanceTypeType",
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
@@ -38,15 +39,14 @@
     "DescribeInstancesPaginatorName",
     "DescribeMatchmakingConfigurationsPaginatorName",
     "DescribeMatchmakingRuleSetsPaginatorName",
     "DescribePlayerSessionsPaginatorName",
     "DescribeScalingPoliciesPaginatorName",
     "EC2InstanceTypeType",
     "EventCodeType",
-    "FilterInstanceStatusType",
     "FleetActionType",
     "FleetStatusType",
     "FleetTypeType",
     "FlexMatchModeType",
     "GameServerClaimStatusType",
     "GameServerGroupActionType",
     "GameServerGroupDeleteOptionType",
@@ -87,14 +87,15 @@
     "GameLiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AcceptanceTypeType = Literal["ACCEPT", "REJECT"]
 BackfillModeType = Literal["AUTOMATIC", "MANUAL"]
 BalancingStrategyType = Literal["ON_DEMAND_ONLY", "SPOT_ONLY", "SPOT_PREFERRED"]
 BuildStatusType = Literal["FAILED", "INITIALIZED", "READY"]
 CertificateTypeType = Literal["DISABLED", "GENERATED"]
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
@@ -265,15 +266,14 @@
     "SERVER_PROCESS_FORCE_TERMINATED",
     "SERVER_PROCESS_INVALID_PATH",
     "SERVER_PROCESS_PROCESS_EXIT_TIMEOUT",
     "SERVER_PROCESS_PROCESS_READY_TIMEOUT",
     "SERVER_PROCESS_SDK_INITIALIZATION_TIMEOUT",
     "SERVER_PROCESS_TERMINATED_UNHEALTHY",
 ]
-FilterInstanceStatusType = Literal["ACTIVE", "DRAINING"]
 FleetActionType = Literal["AUTO_SCALING"]
 FleetStatusType = Literal[
     "ACTIVATING",
     "ACTIVE",
     "BUILDING",
     "DELETING",
     "DOWNLOADING",
@@ -420,15 +420,15 @@
     "CurrentPlayerSessions",
     "IdleInstances",
     "PercentAvailableGameSessions",
     "PercentIdleInstances",
     "QueueDepth",
     "WaitTime",
 ]
-OperatingSystemType = Literal["AMAZON_LINUX", "AMAZON_LINUX_2", "WINDOWS_2012", "WINDOWS_2016"]
+OperatingSystemType = Literal["AMAZON_LINUX", "AMAZON_LINUX_2", "WINDOWS_2012"]
 PlayerSessionCreationPolicyType = Literal["ACCEPT_ALL", "DENY_ALL"]
 PlayerSessionStatusType = Literal["ACTIVE", "COMPLETED", "RESERVED", "TIMEDOUT"]
 PolicyTypeType = Literal["RuleBased", "TargetBased"]
 PriorityTypeType = Literal["COST", "DESTINATION", "LATENCY", "LOCATION"]
 ProtectionPolicyType = Literal["FullProtection", "NoProtection"]
 RoutingStrategyTypeType = Literal["SIMPLE", "TERMINAL"]
 ScalingAdjustmentTypeType = Literal["ChangeInCapacity", "ExactCapacity", "PercentChangeInCapacity"]
@@ -477,26 +477,24 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -582,15 +580,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -601,38 +598,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -645,15 +638,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -672,15 +664,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -720,15 +711,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -762,20 +752,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/paginator.py` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/paginator.pyi` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/type_defs.py` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     BuildStatusType,
     CertificateTypeType,
     ComparisonOperatorTypeType,
     ComputeStatusType,
     ComputeTypeType,
     EC2InstanceTypeType,
     EventCodeType,
-    FilterInstanceStatusType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerGroupDeleteOptionType,
     GameServerGroupInstanceTypeType,
     GameServerGroupStatusType,
     GameServerInstanceStatusType,
@@ -71,15 +70,15 @@
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
-    "ClaimFilterOptionTypeDef",
+    "ClaimGameServerInputRequestTypeDef",
     "GameServerTypeDef",
     "ResponseMetadataTypeDef",
     "ComputeTypeDef",
     "TagTypeDef",
     "S3LocationTypeDef",
     "IpPermissionTypeDef",
     "LocationConfigurationTypeDef",
@@ -188,15 +187,14 @@
     "UpdateGameServerInputRequestTypeDef",
     "UpdateGameSessionInputRequestTypeDef",
     "ValidateMatchmakingRuleSetInputRequestTypeDef",
     "VpcPeeringConnectionStatusTypeDef",
     "AliasTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "PlayerTypeDef",
-    "ClaimGameServerInputRequestTypeDef",
     "ClaimGameServerOutputTypeDef",
     "DescribeBuildOutputTypeDef",
     "DescribeGameServerOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetComputeAccessOutputTypeDef",
     "GetComputeAuthTokenOutputTypeDef",
     "GetGameSessionLogUrlOutputTypeDef",
@@ -410,22 +408,36 @@
 CertificateConfigurationTypeDef = TypedDict(
     "CertificateConfigurationTypeDef",
     {
         "CertificateType": CertificateTypeType,
     },
 )
 
-ClaimFilterOptionTypeDef = TypedDict(
-    "ClaimFilterOptionTypeDef",
+_RequiredClaimGameServerInputRequestTypeDef = TypedDict(
+    "_RequiredClaimGameServerInputRequestTypeDef",
     {
-        "InstanceStatuses": Sequence[FilterInstanceStatusType],
+        "GameServerGroupName": str,
+    },
+)
+_OptionalClaimGameServerInputRequestTypeDef = TypedDict(
+    "_OptionalClaimGameServerInputRequestTypeDef",
+    {
+        "GameServerId": str,
+        "GameServerData": str,
     },
     total=False,
 )
 
+
+class ClaimGameServerInputRequestTypeDef(
+    _RequiredClaimGameServerInputRequestTypeDef, _OptionalClaimGameServerInputRequestTypeDef
+):
+    pass
+
+
 GameServerTypeDef = TypedDict(
     "GameServerTypeDef",
     {
         "GameServerGroupName": str,
         "GameServerGroupArn": str,
         "GameServerId": str,
         "InstanceId": str,
@@ -1818,37 +1830,14 @@
         "PlayerAttributes": Dict[str, AttributeValueTypeDef],
         "Team": str,
         "LatencyInMs": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredClaimGameServerInputRequestTypeDef = TypedDict(
-    "_RequiredClaimGameServerInputRequestTypeDef",
-    {
-        "GameServerGroupName": str,
-    },
-)
-_OptionalClaimGameServerInputRequestTypeDef = TypedDict(
-    "_OptionalClaimGameServerInputRequestTypeDef",
-    {
-        "GameServerId": str,
-        "GameServerData": str,
-        "FilterOption": ClaimFilterOptionTypeDef,
-    },
-    total=False,
-)
-
-
-class ClaimGameServerInputRequestTypeDef(
-    _RequiredClaimGameServerInputRequestTypeDef, _OptionalClaimGameServerInputRequestTypeDef
-):
-    pass
-
-
 ClaimGameServerOutputTypeDef = TypedDict(
     "ClaimGameServerOutputTypeDef",
     {
         "GameServer": GameServerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift/type_defs.pyi` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     BuildStatusType,
     CertificateTypeType,
     ComparisonOperatorTypeType,
     ComputeStatusType,
     ComputeTypeType,
     EC2InstanceTypeType,
     EventCodeType,
-    FilterInstanceStatusType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerGroupDeleteOptionType,
     GameServerGroupInstanceTypeType,
     GameServerGroupStatusType,
     GameServerInstanceStatusType,
@@ -70,15 +69,15 @@
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
-    "ClaimFilterOptionTypeDef",
+    "ClaimGameServerInputRequestTypeDef",
     "GameServerTypeDef",
     "ResponseMetadataTypeDef",
     "ComputeTypeDef",
     "TagTypeDef",
     "S3LocationTypeDef",
     "IpPermissionTypeDef",
     "LocationConfigurationTypeDef",
@@ -187,15 +186,14 @@
     "UpdateGameServerInputRequestTypeDef",
     "UpdateGameSessionInputRequestTypeDef",
     "ValidateMatchmakingRuleSetInputRequestTypeDef",
     "VpcPeeringConnectionStatusTypeDef",
     "AliasTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "PlayerTypeDef",
-    "ClaimGameServerInputRequestTypeDef",
     "ClaimGameServerOutputTypeDef",
     "DescribeBuildOutputTypeDef",
     "DescribeGameServerOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetComputeAccessOutputTypeDef",
     "GetComputeAuthTokenOutputTypeDef",
     "GetGameSessionLogUrlOutputTypeDef",
@@ -409,22 +407,34 @@
 CertificateConfigurationTypeDef = TypedDict(
     "CertificateConfigurationTypeDef",
     {
         "CertificateType": CertificateTypeType,
     },
 )
 
-ClaimFilterOptionTypeDef = TypedDict(
-    "ClaimFilterOptionTypeDef",
+_RequiredClaimGameServerInputRequestTypeDef = TypedDict(
+    "_RequiredClaimGameServerInputRequestTypeDef",
     {
-        "InstanceStatuses": Sequence[FilterInstanceStatusType],
+        "GameServerGroupName": str,
+    },
+)
+_OptionalClaimGameServerInputRequestTypeDef = TypedDict(
+    "_OptionalClaimGameServerInputRequestTypeDef",
+    {
+        "GameServerId": str,
+        "GameServerData": str,
     },
     total=False,
 )
 
+class ClaimGameServerInputRequestTypeDef(
+    _RequiredClaimGameServerInputRequestTypeDef, _OptionalClaimGameServerInputRequestTypeDef
+):
+    pass
+
 GameServerTypeDef = TypedDict(
     "GameServerTypeDef",
     {
         "GameServerGroupName": str,
         "GameServerGroupArn": str,
         "GameServerId": str,
         "InstanceId": str,
@@ -1771,35 +1781,14 @@
         "PlayerAttributes": Dict[str, AttributeValueTypeDef],
         "Team": str,
         "LatencyInMs": Dict[str, int],
     },
     total=False,
 )
 
-_RequiredClaimGameServerInputRequestTypeDef = TypedDict(
-    "_RequiredClaimGameServerInputRequestTypeDef",
-    {
-        "GameServerGroupName": str,
-    },
-)
-_OptionalClaimGameServerInputRequestTypeDef = TypedDict(
-    "_OptionalClaimGameServerInputRequestTypeDef",
-    {
-        "GameServerId": str,
-        "GameServerData": str,
-        "FilterOption": ClaimFilterOptionTypeDef,
-    },
-    total=False,
-)
-
-class ClaimGameServerInputRequestTypeDef(
-    _RequiredClaimGameServerInputRequestTypeDef, _OptionalClaimGameServerInputRequestTypeDef
-):
-    pass
-
 ClaimGameServerOutputTypeDef = TypedDict(
     "ClaimGameServerOutputTypeDef",
     {
         "GameServer": GameServerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/PKG-INFO` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.26.141
-Summary: Type annotations for boto3.GameLift 1.26.141 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.21
+Summary: Type annotations for boto3.GameLift 1.26.21 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-gamelift?color=blue)](https://pypistats.org/packages/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,15 +392,14 @@
     DescribeInstancesPaginatorName,
     DescribeMatchmakingConfigurationsPaginatorName,
     DescribeMatchmakingRuleSetsPaginatorName,
     DescribePlayerSessionsPaginatorName,
     DescribeScalingPoliciesPaginatorName,
     EC2InstanceTypeType,
     EventCodeType,
-    FilterInstanceStatusType,
     FleetActionType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerClaimStatusType,
     GameServerGroupActionType,
     GameServerGroupDeleteOptionType,
@@ -463,15 +461,15 @@
     AcceptMatchInputRequestTypeDef,
     RoutingStrategyTypeDef,
     AnywhereConfigurationTypeDef,
     AttributeValueTypeDef,
     AwsCredentialsTypeDef,
     BuildTypeDef,
     CertificateConfigurationTypeDef,
-    ClaimFilterOptionTypeDef,
+    ClaimGameServerInputRequestTypeDef,
     GameServerTypeDef,
     ResponseMetadataTypeDef,
     ComputeTypeDef,
     TagTypeDef,
     S3LocationTypeDef,
     IpPermissionTypeDef,
     LocationConfigurationTypeDef,
@@ -580,15 +578,14 @@
     UpdateGameServerInputRequestTypeDef,
     UpdateGameSessionInputRequestTypeDef,
     ValidateMatchmakingRuleSetInputRequestTypeDef,
     VpcPeeringConnectionStatusTypeDef,
     AliasTypeDef,
     UpdateAliasInputRequestTypeDef,
     PlayerTypeDef,
-    ClaimGameServerInputRequestTypeDef,
     ClaimGameServerOutputTypeDef,
     DescribeBuildOutputTypeDef,
     DescribeGameServerOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComputeAccessOutputTypeDef,
     GetComputeAuthTokenOutputTypeDef,
     GetGameSessionLogUrlOutputTypeDef,
@@ -744,42 +741,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-gamelift-1.26.141/mypy_boto3_gamelift.egg-info/SOURCES.txt` & `mypy-boto3-gamelift-1.26.21/mypy_boto3_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.26.141/setup.py` & `mypy-boto3-gamelift-1.26.21/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """
 Setup script for mypy-boto3-gamelift.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-gamelift",
-    version="1.26.141",
+    version="1.26.21",
     packages=["mypy_boto3_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GameLift 1.26.141 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.GameLift 1.26.21 service generated with mypy-boto3-builder"
+        " 7.11.11"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 gamelift type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_gamelift": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_gamelift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

