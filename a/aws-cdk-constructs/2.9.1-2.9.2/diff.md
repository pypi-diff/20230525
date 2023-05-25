# Comparing `tmp/aws_cdk_constructs-2.9.1.tar.gz` & `tmp/aws_cdk_constructs-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cdk_constructs-2.9.1.tar", last modified: Tue Feb 21 15:25:51 2023, max compression
+gzip compressed data, was "aws_cdk_constructs-2.9.2.tar", last modified: Tue Feb 28 14:49:20 2023, max compression
```

## Comparing `aws_cdk_constructs-2.9.1.tar` & `aws_cdk_constructs-2.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7538 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6694 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.091824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/api/
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3096 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/api/api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/bucket/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/bucket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18750 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/bucket/bucket.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/database/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/database/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29747 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/database/database.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/ecs/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/ecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12761 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/ecs/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)    21480 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/ecs/microservice.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/efs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/efs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12061 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/efs/volume.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/load_balancer/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/load_balancer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25301 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/load_balancer/alb.py
--rw-rw-rw-   0 root         (0) root         (0)     8969 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/load_balancer/nlb.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/base_user_data.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/manage_connection_to_nlb_instance_security_group_ingress/
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/manage_connection_to_nlb_instance_security_group_ingress/lambda_function.js
--rw-rw-rw-   0 root         (0) root         (0)    62098 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/microservice.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/security_group/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/security_group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3258 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/security_group/security_group.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_iac/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_iac/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26263 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_iac/service_user_for_iac.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_static_assets/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_static_assets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5280 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_static_assets/service_user_for_static_assets.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7538 2023-02-21 15:25:51.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-02-21 15:25:51.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-21 15:25:51.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-02-21 15:25:51.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-02-21 15:25:51.000000 aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-21 15:25:51.095824 aws_cdk_constructs-2.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-02-21 15:25:13.000000 aws_cdk_constructs-2.9.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.549214 aws_cdk_constructs-2.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2023-02-28 14:49:20.549214 aws_cdk_constructs-2.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6694 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/api/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3096 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/api/api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/bucket/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/bucket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18750 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/bucket/bucket.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/database/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/database/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29747 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/database/database.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/ecs/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/ecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12761 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/ecs/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)    21480 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/ecs/microservice.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/efs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/efs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12061 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/efs/volume.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/load_balancer/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/load_balancer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25301 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/load_balancer/alb.py
+-rw-rw-rw-   0 root         (0) root         (0)     8969 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/load_balancer/nlb.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/base_user_data.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/manage_connection_to_nlb_instance_security_group_ingress/
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/manage_connection_to_nlb_instance_security_group_ingress/lambda_function.js
+-rw-rw-rw-   0 root         (0) root         (0)    62277 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/microservice.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/security_group/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/security_group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3258 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/security_group/security_group.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_iac/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_iac/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26263 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_iac/service_user_for_iac.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.549214 aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_static_assets/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_static_assets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5280 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_static_assets/service_user_for_static_assets.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-02-28 14:49:20.545214 aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2023-02-28 14:49:20.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-02-28 14:49:20.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-02-28 14:49:20.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-02-28 14:49:20.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-02-28 14:49:20.000000 aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-02-28 14:49:20.549214 aws_cdk_constructs-2.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2023-02-28 14:48:43.000000 aws_cdk_constructs-2.9.2/setup.py
```

### Comparing `aws_cdk_constructs-2.9.1/PKG-INFO` & `aws_cdk_constructs-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_cdk_constructs
-Version: 2.9.1
+Version: 2.9.2
 Summary: AWS CDK constructs
 Home-page: https://bitbucket.org/cioapps/aws-cdk-constructs
 Author: author
 Author-email: author@foa.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aws_cdk_constructs-2.9.1/README.md` & `aws_cdk_constructs-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/api/api.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/api/api.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/bucket/bucket.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/bucket/bucket.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/database/database.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/database/database.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/ecs/cluster.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/ecs/microservice.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/ecs/microservice.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/efs/volume.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/efs/volume.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/load_balancer/alb.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/load_balancer/alb.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/load_balancer/nlb.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/load_balancer/nlb.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/base_user_data.sh` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/base_user_data.sh`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/manage_connection_to_nlb_instance_security_group_ingress/lambda_function.js` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/manage_connection_to_nlb_instance_security_group_ingress/lambda_function.js`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/microservice/microservice.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/microservice/microservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     @property
     def alb_logs_bucket(self):
         """Returns S3 bucket that the Application Load Balancer is using for storing the logs
 
         Returns:
             str: the S3 bucket that the Application Load Balancer is using for storing the logs
         """
-        return self._alb_logs_bucket
+        return self.alb_construct._alb_logs_bucket
 
     @property
     def tcp_connection_ec2_traffic_port(self):
         """Returns the EC2 traffic port as TCP connection
 
         Returns:
             aws_ec2.Port.tcp: the EC2 traffic port
@@ -251,15 +251,15 @@
     @property
     def load_balancer_security_group(self):
         """Returns the security group in use by the application load balancer
 
         Returns:
             aws_ec2.SecurityGroup: the security group in use by the application load balancer
         """
-        return self.alb_security_group
+        return self.alb_construct.security_group
 
     @property
     def ec2_instance_security_group(self):
         """Return the security group in use by the EC2 instance
 
         Returns:
             aws_ec2.SecurityGroup: the security group in use by the EC2 instance
@@ -278,29 +278,29 @@
     @property
     def efs(self):
         """Return the EFS resource, in case it was created
 
         Returns:
             aws_efs.FileSystem: he EFS resource
         """
-        return self._efs
+        return self._efs.efs
 
     @property
     def efs_security_group(self):
         """Return the EFS's security group, in case it was created
 
         Returns:
             aws_ec2.SecurityGroup: the security group in use by the EFS FileSystem
         """
         return self._efs_security_group
 
     def get_efs_construct(self):
         """Return the FAO CDK EFS construct
         """
-        return self.efs
+        return self._efs
 
     def enable_fao_private_access(self, security_group, port=None):
         """Apply the correct ingress rules to the provided security group to enable access from the FAO internal networks
         
         Args:
             security_group (aws_ec2.SecurityGroup): The security group to configure to enable access from FAO network
             port (aws_ec2.Port.tcp): the port to allow, if None tcp_connection_traffic_port will be used
@@ -420,19 +420,19 @@
         ec2_traffic_protocol=_alb.Protocol.HTTP,
         upstream_security_group=None,
         ec2_health_check_path=None,
         user_data_s3_key="user-data.sh",
         downstream_security_group=None,
         downstream_port=None,
         ssl_certificate_arn=None,
-        will_be_ha=True,
+        will_be_ha='false',
         ebs_volume_size=None,
         ebs_snapshot_id=None,
-        will_use_efs=False,
-        will_use_cdn=False,
+        will_use_efs='false',
+        will_use_cdn='false',
         access_log_bucket_name="fao-elb-logs",
         authorization_endpoint=None,
         token_endpoint=None,
         issuer=None,
         client_id=None,
         client_secret=None,
         user_info_endpoint=None,
@@ -660,14 +660,15 @@
                 network_load_balancer_subnet_1=network_load_balancer_subnet_1,
                 network_load_balancer_subnet_2=network_load_balancer_subnet_2,
                 ec2_traffic_port=ec2_traffic_port,
                 dns_record=dns_record,
                 create_dns=create_dns
             )
             self.nlb = nlb.nlb
+            self.nlb_construct = nlb
             self._tg = nlb.tg
         else:
             alb = Alb(scope=self,
                       id='alb',
                       app_name=app_name,
                       environment=environment,
                       environments_parameters=environments_parameters,
@@ -690,14 +691,15 @@
                       token_endpoint=token_endpoint,
                       issuer=issuer,
                       client_id=client_id,
                       client_secret=client_secret,
                       user_info_endpoint=user_info_endpoint,
                       upstream_security_group=upstream_security_group )
             self.alb = alb.alb
+            self.alb_construct = alb
             self._tg = alb.tg
 
         # ~~~~~~~~~~~~~~~~
         # Instance profile
         # ~~~~~~~~~~~~~~~~
 
         self._ec2_role = _iam.Role(
@@ -874,14 +876,15 @@
                                   id=main_component_name+"-efsvolumefromms",   # EFS name to maintain compatibility with the old naming convention
                                   vpc=self._vpc,
                                   environment=environment,
                                   app_name=self._app_name,
                                   environments_parameters=environments_parameters,
                                   to_be_backed_up=to_be_backed_up,
                                   aws_back_up=aws_back_up)
+            self._efs_security_group = self._efs._efs_security_group
             # you will find an additional EFS instruction after ASG
 
         # ~~~~~~~~~~~~~~~~
         # User data
         # ~~~~~~~~~~~~~~~~
 
         # Look to the path of your current working directory
```

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/security_group/security_group.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/security_group/security_group.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_iac/service_user_for_iac.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_iac/service_user_for_iac.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/service_user_for_static_assets/service_user_for_static_assets.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/service_user_for_static_assets/service_user_for_static_assets.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs/utils.py` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs/utils.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/PKG-INFO` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-constructs
-Version: 2.9.1
+Version: 2.9.2
 Summary: AWS CDK constructs
 Home-page: https://bitbucket.org/cioapps/aws-cdk-constructs
 Author: author
 Author-email: author@foa.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aws_cdk_constructs-2.9.1/aws_cdk_constructs.egg-info/SOURCES.txt` & `aws_cdk_constructs-2.9.2/aws_cdk_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_cdk_constructs-2.9.1/setup.py` & `aws_cdk_constructs-2.9.2/setup.py`

 * *Files identical despite different names*

