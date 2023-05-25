# Comparing `tmp/rdk-0.8.5.tar.gz` & `tmp/rdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdk-0.8.5.tar", last modified: Fri Jul 15 18:23:50 2022, max compression
+gzip compressed data, was "rdk-0.9.0.tar", last modified: Thu Jan  5 21:58:14 2023, max compression
```

## Comparing `rdk-0.8.5.tar` & `rdk-0.9.0.tar`

### file list

```diff
@@ -1,158 +1,152 @@
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.210245 rdk-0.8.5/
--rw-r--r--   0 chauyu     (504) staff       (20)    11357 2022-07-15 18:22:54.000000 rdk-0.8.5/LICENSE
--rw-r--r--   0 chauyu     (504) staff       (20)     1419 2022-07-15 18:22:54.000000 rdk-0.8.5/MANIFEST.in
--rw-r--r--   0 chauyu     (504) staff       (20)       81 2022-07-15 18:22:54.000000 rdk-0.8.5/NOTICE.txt
--rw-r--r--   0 chauyu     (504) staff       (20)    23432 2022-07-15 18:23:50.209932 rdk-0.8.5/PKG-INFO
--rw-r--r--   0 chauyu     (504) staff       (20)    23134 2022-07-15 18:22:54.000000 rdk-0.8.5/README.rst
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.162052 rdk-0.8.5/rdk/
--rw-r--r--   0 chauyu     (504) staff       (20)      595 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/__init__.py
--rw-r--r--   0 chauyu     (504) staff       (20)     2467 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/cli.py
--rw-r--r--   0 chauyu     (504) staff       (20)   188340 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/rdk.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.168145 rdk-0.8.5/rdk/template/
--rw-r--r--   0 chauyu     (504) staff       (20)      926 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/LICENSE
--rw-r--r--   0 chauyu     (504) staff       (20)     2125 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/configManagedRule.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1917 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/configManagedRuleOrganization.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3588 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/configManagedRuleWithRemediation.json
--rw-r--r--   0 chauyu     (504) staff       (20)     8986 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/configRule.json
--rw-r--r--   0 chauyu     (504) staff       (20)      285 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/configRuleAssumeRolePolicyDoc.json
--rw-r--r--   0 chauyu     (504) staff       (20)     8466 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/configRuleOrganization.json
--rw-r--r--   0 chauyu     (504) staff       (20)      558 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/deliveryPermissionsPolicy.json
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.196713 rdk-0.8.5/rdk/template/example_ci/
--rw-r--r--   0 chauyu     (504) staff       (20)     1726 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ACM_Certificate.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1199 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ApiGatewayV2_Api.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1432 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ApiGatewayV2_Stage.json
--rw-r--r--   0 chauyu     (504) staff       (20)      933 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ApiGateway_RestApi.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1302 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ApiGateway_Stage.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2140 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_AutoScalingGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2769 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_LaunchConfiguration.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2511 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_ScalingPolicy.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1368 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_ScheduledAction.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3759 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_CLOUDFRONT_DISTRIBUTION.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1934 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_CLOUDFRONT_STREAMINGDISTRIBUTION.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2339 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_CloudFormation_Stack.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1389 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_CloudWatch_Alarm.json
--rw-r--r--   0 chauyu     (504) staff       (20)      978 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Cloudtrail_Trail.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2285 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_CodeBuild_Project.json
--rw-r--r--   0 chauyu     (504) staff       (20)     4426 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_CodePipeline_Pipeline.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1666 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_DynamoDB_Table.json
--rw-r--r--   0 chauyu     (504) staff       (20)      979 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_CustomerGateway.json
--rw-r--r--   0 chauyu     (504) staff       (20)      742 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_EIP.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1373 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_FlowLog.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1358 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Host.json
--rw-r--r--   0 chauyu     (504) staff       (20)     4621 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Instance.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1024 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_InternetGateway.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1186 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_LaunchTemplate.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1484 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_NatGateway.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2959 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_NetworkAcl.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2648 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_NetworkInterface.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1483 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_RouteTable.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1481 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_SecurityGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1705 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Subnet.json
--rw-r--r--   0 chauyu     (504) staff       (20)     5290 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPC.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2241 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPCPeeringConnection.json
--rw-r--r--   0 chauyu     (504) staff       (20)     5917 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPNConnection.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1225 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPNGateway.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1523 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Volume.json
--rw-r--r--   0 chauyu     (504) staff       (20)      967 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ECR_PublicRepository.json
--rw-r--r--   0 chauyu     (504) staff       (20)      953 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ECR_Repository.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1016 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_EKS_Cluster.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3658 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ELASTICLOADBALANCING_LOADBALANCER.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1643 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ElasticBeanstalk_Application.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1323 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ElasticBeanstalk_ApplicationVersion.json
--rw-r--r--   0 chauyu     (504) staff       (20)     8625 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ElasticBeanstalk_Environment.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2823 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ElasticLoadBalancingV2_LoadBalancer.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3728 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ElasticSearch_Domain.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1759 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_IAM_Group.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2467 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_IAM_Policy.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2376 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_IAM_Role.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2813 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_IAM_User.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2288 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_KMS_Key.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2153 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_LAMBDA_FUNCTION.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1913 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_NetworkFirewall_RuleGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2367 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_OpenSearch_Domain.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3210 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBCluster.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2087 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBClusterSnapshot.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3997 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBInstance.json
--rw-r--r--   0 chauyu     (504) staff       (20)      838 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBSecurityGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1882 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBSnapshot.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2398 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBSubnetGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1262 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_RDS_EventSubscription.json
--rw-r--r--   0 chauyu     (504) staff       (20)     3879 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_Cluster.json
--rw-r--r--   0 chauyu     (504) staff       (20)     4600 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterParameterGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1349 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterSecurityGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2235 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterSnapshot.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2083 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterSubnetGroup.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1357 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_EventSubscription.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1983 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_S3_Bucket.json
--rw-r--r--   0 chauyu     (504) staff       (20)     2003 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_SNS_Topic.json
--rw-r--r--   0 chauyu     (504) staff       (20)    61388 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory.json
--rw-r--r--   0 chauyu     (504) staff       (20)    61388 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Linux.json
--rw-r--r--   0 chauyu     (504) staff       (20)    61641 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Windows.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1231 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_ShieldRegional_Protection.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1174 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/example_ci/AWS_Shield_Protection.json
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.158391 rdk-0.8.5/rdk/template/runtime/
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.198428 rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/
--rw-r--r--   0 chauyu     (504) staff       (20)     7926 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/CustomConfigHandler.cs
--rwxr-xr-x   0 chauyu     (504) staff       (20)      662 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/RuleCode.cs
--rwxr-xr-x   0 chauyu     (504) staff       (20)      743 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/aws-lambda-tools-defaults.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1158 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/csharp7.0.csproj
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.200137 rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/
--rw-r--r--   0 chauyu     (504) staff       (20)     7926 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/CustomConfigHandler.cs
--rw-r--r--   0 chauyu     (504) staff       (20)      662 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/RuleCode.cs
--rw-r--r--   0 chauyu     (504) staff       (20)      743 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/aws-lambda-tools-defaults.json
--rw-r--r--   0 chauyu     (504) staff       (20)     1158 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/csharp7.0.csproj
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.200517 rdk-0.8.5/rdk/template/runtime/java8/
--rw-r--r--   0 chauyu     (504) staff       (20)      624 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/java8/build.gradle
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.200935 rdk-0.8.5/rdk/template/runtime/java8/jars/
--rw-r--r--   0 chauyu     (504) staff       (20)       91 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/java8/jars/readme.txt
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.156205 rdk-0.8.5/rdk/template/runtime/java8/src/
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.156331 rdk-0.8.5/rdk/template/runtime/java8/src/main/
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.156460 rdk-0.8.5/rdk/template/runtime/java8/src/main/java/
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.156589 rdk-0.8.5/rdk/template/runtime/java8/src/main/java/com/
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.201674 rdk-0.8.5/rdk/template/runtime/java8/src/main/java/com/rdk/
--rw-r--r--   0 chauyu     (504) staff       (20)      718 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/java8/src/main/java/com/rdk/RuleCode.java
--rw-r--r--   0 chauyu     (504) staff       (20)     6070 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/java8/src/main/java/com/rdk/RuleUtil.java
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.202021 rdk-0.8.5/rdk/template/runtime/nodejs4.3/
--rw-r--r--   0 chauyu     (504) staff       (20)     7991 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/nodejs4.3/rule_code.js
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.202854 rdk-0.8.5/rdk/template/runtime/python3.6/
--rw-r--r--   0 chauyu     (504) staff       (20)    17658 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.6/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     7285 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.6/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.203551 rdk-0.8.5/rdk/template/runtime/python3.6-lib/
--rw-r--r--   0 chauyu     (504) staff       (20)      930 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.6-lib/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     1916 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.6-lib/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.204364 rdk-0.8.5/rdk/template/runtime/python3.7/
--rw-r--r--   0 chauyu     (504) staff       (20)    17658 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.7/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     7285 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.7/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.205157 rdk-0.8.5/rdk/template/runtime/python3.7-lib/
--rw-r--r--   0 chauyu     (504) staff       (20)      930 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.7-lib/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     1916 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.7-lib/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.205936 rdk-0.8.5/rdk/template/runtime/python3.8/
--rw-r--r--   0 chauyu     (504) staff       (20)    17658 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.8/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     7285 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.8/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.206645 rdk-0.8.5/rdk/template/runtime/python3.8-lib/
--rw-r--r--   0 chauyu     (504) staff       (20)      930 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.8-lib/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     1916 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.8-lib/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.207351 rdk-0.8.5/rdk/template/runtime/python3.9/
--rw-r--r--   0 chauyu     (504) staff       (20)    17658 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.9/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     7285 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.9/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.208041 rdk-0.8.5/rdk/template/runtime/python3.9-lib/
--rw-r--r--   0 chauyu     (504) staff       (20)      930 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.9-lib/rule_code.py
--rw-r--r--   0 chauyu     (504) staff       (20)     1916 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/runtime/python3.9-lib/rule_test.py
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.159045 rdk-0.8.5/rdk/template/terraform/
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.208700 rdk-0.8.5/rdk/template/terraform/0.11/
--rw-r--r--   0 chauyu     (504) staff       (20)     4752 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/terraform/0.11/config_rule.tf
--rw-r--r--   0 chauyu     (504) staff       (20)     1785 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/terraform/0.11/variables.tf
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.209479 rdk-0.8.5/rdk/template/terraform/0.12/
--rw-r--r--   0 chauyu     (504) staff       (20)     4690 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/terraform/0.12/config_rule.tf
--rw-r--r--   0 chauyu     (504) staff       (20)     1834 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/terraform/0.12/variables.tf
--rw-r--r--   0 chauyu     (504) staff       (20)     3141 2022-07-15 18:22:54.000000 rdk-0.8.5/rdk/template/test_event_template.json
-drwxr-xr-x   0 chauyu     (504) staff       (20)        0 2022-07-15 18:23:50.164909 rdk-0.8.5/rdk.egg-info/
--rw-r--r--   0 chauyu     (504) staff       (20)    23432 2022-07-15 18:23:49.000000 rdk-0.8.5/rdk.egg-info/PKG-INFO
--rw-r--r--   0 chauyu     (504) staff       (20)     6045 2022-07-15 18:23:50.000000 rdk-0.8.5/rdk.egg-info/SOURCES.txt
--rw-r--r--   0 chauyu     (504) staff       (20)        1 2022-07-15 18:23:49.000000 rdk-0.8.5/rdk.egg-info/dependency_links.txt
--rw-r--r--   0 chauyu     (504) staff       (20)       37 2022-07-15 18:23:49.000000 rdk-0.8.5/rdk.egg-info/entry_points.txt
--rw-r--r--   0 chauyu     (504) staff       (20)        1 2022-07-15 18:23:49.000000 rdk-0.8.5/rdk.egg-info/not-zip-safe
--rw-r--r--   0 chauyu     (504) staff       (20)       13 2022-07-15 18:23:49.000000 rdk-0.8.5/rdk.egg-info/requires.txt
--rw-r--r--   0 chauyu     (504) staff       (20)        4 2022-07-15 18:23:50.000000 rdk-0.8.5/rdk.egg-info/top_level.txt
--rw-r--r--   0 chauyu     (504) staff       (20)       38 2022-07-15 18:23:50.210352 rdk-0.8.5/setup.cfg
--rw-r--r--   0 chauyu     (504) staff       (20)     1263 2022-07-15 18:22:54.000000 rdk-0.8.5/setup.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.896253 rdk-0.9.0/
+-rw-r--r--   0 mbeacom    (505) staff       (20)    11357 2022-12-19 21:33:54.000000 rdk-0.9.0/LICENSE
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1333 2023-01-05 21:52:20.000000 rdk-0.9.0/MANIFEST.in
+-rw-r--r--   0 mbeacom    (505) staff       (20)       81 2022-12-19 21:33:54.000000 rdk-0.9.0/NOTICE.txt
+-rw-r--r--   0 mbeacom    (505) staff       (20)    26490 2023-01-05 21:58:14.896059 rdk-0.9.0/PKG-INFO
+-rw-r--r--   0 mbeacom    (505) staff       (20)    23127 2023-01-05 21:52:20.000000 rdk-0.9.0/README.rst
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.867467 rdk-0.9.0/rdk/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      595 2023-01-05 21:52:20.000000 rdk-0.9.0/rdk/__init__.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2407 2023-01-05 21:52:20.000000 rdk-0.9.0/rdk/cli.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)   187970 2023-01-05 21:52:20.000000 rdk-0.9.0/rdk/rdk.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.870698 rdk-0.9.0/rdk/template/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      926 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/LICENSE
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2125 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/configManagedRule.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1917 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/configManagedRuleOrganization.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3588 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/configManagedRuleWithRemediation.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     8986 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/configRule.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      285 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/configRuleAssumeRolePolicyDoc.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     8466 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/configRuleOrganization.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      558 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/deliveryPermissionsPolicy.json
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.886197 rdk-0.9.0/rdk/template/example_ci/
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1726 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ACM_Certificate.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1199 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ApiGatewayV2_Api.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1432 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ApiGatewayV2_Stage.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      933 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ApiGateway_RestApi.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1302 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ApiGateway_Stage.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2140 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_AutoScalingGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2769 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_LaunchConfiguration.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2511 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_ScalingPolicy.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1368 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_ScheduledAction.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3759 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_CLOUDFRONT_DISTRIBUTION.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1934 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_CLOUDFRONT_STREAMINGDISTRIBUTION.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2339 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_CloudFormation_Stack.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1389 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_CloudWatch_Alarm.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      978 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Cloudtrail_Trail.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2285 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_CodeBuild_Project.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     4426 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_CodePipeline_Pipeline.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1666 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_DynamoDB_Table.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      979 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_CustomerGateway.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      742 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_EIP.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1373 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_FlowLog.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1358 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Host.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     4621 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Instance.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1024 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_InternetGateway.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1186 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_LaunchTemplate.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1484 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_NatGateway.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2959 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_NetworkAcl.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2648 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_NetworkInterface.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1483 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_RouteTable.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1481 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_SecurityGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1705 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Subnet.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     5290 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPC.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2241 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPCPeeringConnection.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     5917 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPNConnection.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1225 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPNGateway.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1523 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Volume.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      967 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ECR_PublicRepository.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      953 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ECR_Repository.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1016 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_EKS_Cluster.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3658 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ELASTICLOADBALANCING_LOADBALANCER.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1643 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ElasticBeanstalk_Application.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1323 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ElasticBeanstalk_ApplicationVersion.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     8625 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ElasticBeanstalk_Environment.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2823 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ElasticLoadBalancingV2_LoadBalancer.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3728 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ElasticSearch_Domain.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1759 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_IAM_Group.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2467 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_IAM_Policy.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2376 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_IAM_Role.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2813 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_IAM_User.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2288 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_KMS_Key.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2153 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_LAMBDA_FUNCTION.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1913 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_NetworkFirewall_RuleGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2367 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_OpenSearch_Domain.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3210 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBCluster.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2087 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBClusterSnapshot.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3997 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBInstance.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)      838 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBSecurityGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1882 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBSnapshot.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2398 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBSubnetGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1262 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_RDS_EventSubscription.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3879 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_Cluster.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     4600 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterParameterGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1349 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterSecurityGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2235 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterSnapshot.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2083 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterSubnetGroup.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1357 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_EventSubscription.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1983 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_S3_Bucket.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     2003 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_SNS_Topic.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)    61388 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)    61388 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Linux.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)    61641 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Windows.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1231 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_ShieldRegional_Protection.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1174 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/example_ci/AWS_Shield_Protection.json
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.865848 rdk-0.9.0/rdk/template/runtime/
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.886892 rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/
+-rw-r--r--   0 mbeacom    (505) staff       (20)     7926 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/CustomConfigHandler.cs
+-rwxr-xr-x   0 mbeacom    (505) staff       (20)      662 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/RuleCode.cs
+-rwxr-xr-x   0 mbeacom    (505) staff       (20)      743 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/aws-lambda-tools-defaults.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1158 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/csharp7.0.csproj
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.887747 rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/
+-rw-r--r--   0 mbeacom    (505) staff       (20)     7926 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/CustomConfigHandler.cs
+-rw-r--r--   0 mbeacom    (505) staff       (20)      662 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/RuleCode.cs
+-rw-r--r--   0 mbeacom    (505) staff       (20)      743 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/aws-lambda-tools-defaults.json
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1158 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/csharp7.0.csproj
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.887922 rdk-0.9.0/rdk/template/runtime/java8/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      624 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/java8/build.gradle
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.888089 rdk-0.9.0/rdk/template/runtime/java8/jars/
+-rw-r--r--   0 mbeacom    (505) staff       (20)       91 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/java8/jars/readme.txt
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.865175 rdk-0.9.0/rdk/template/runtime/java8/src/
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.865226 rdk-0.9.0/rdk/template/runtime/java8/src/main/
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.865277 rdk-0.9.0/rdk/template/runtime/java8/src/main/java/
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.865332 rdk-0.9.0/rdk/template/runtime/java8/src/main/java/com/
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.888462 rdk-0.9.0/rdk/template/runtime/java8/src/main/java/com/rdk/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      718 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/java8/src/main/java/com/rdk/RuleCode.java
+-rw-r--r--   0 mbeacom    (505) staff       (20)     6070 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/java8/src/main/java/com/rdk/RuleUtil.java
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.888937 rdk-0.9.0/rdk/template/runtime/nodejs4.3/
+-rw-r--r--   0 mbeacom    (505) staff       (20)     7991 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/nodejs4.3/rule_code.js
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.889501 rdk-0.9.0/rdk/template/runtime/python3.7/
+-rw-r--r--   0 mbeacom    (505) staff       (20)    17658 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.7/rule_code.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     7285 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.7/rule_test.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.889946 rdk-0.9.0/rdk/template/runtime/python3.7-lib/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      930 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.7-lib/rule_code.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1916 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.7-lib/rule_test.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.890515 rdk-0.9.0/rdk/template/runtime/python3.8/
+-rw-r--r--   0 mbeacom    (505) staff       (20)    17658 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.8/rule_code.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     7285 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.8/rule_test.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.893711 rdk-0.9.0/rdk/template/runtime/python3.8-lib/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      930 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.8-lib/rule_code.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1916 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.8-lib/rule_test.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.894194 rdk-0.9.0/rdk/template/runtime/python3.9/
+-rw-r--r--   0 mbeacom    (505) staff       (20)    17658 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.9/rule_code.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     7285 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.9/rule_test.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.894653 rdk-0.9.0/rdk/template/runtime/python3.9-lib/
+-rw-r--r--   0 mbeacom    (505) staff       (20)      930 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.9-lib/rule_code.py
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1916 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/runtime/python3.9-lib/rule_test.py
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.866045 rdk-0.9.0/rdk/template/terraform/
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.895233 rdk-0.9.0/rdk/template/terraform/0.11/
+-rw-r--r--   0 mbeacom    (505) staff       (20)     4752 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/terraform/0.11/config_rule.tf
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1785 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/terraform/0.11/variables.tf
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.895670 rdk-0.9.0/rdk/template/terraform/0.12/
+-rw-r--r--   0 mbeacom    (505) staff       (20)     4690 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/terraform/0.12/config_rule.tf
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1834 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/terraform/0.12/variables.tf
+-rw-r--r--   0 mbeacom    (505) staff       (20)     3141 2022-12-19 21:33:54.000000 rdk-0.9.0/rdk/template/test_event_template.json
+drwxr-xr-x   0 mbeacom    (505) staff       (20)        0 2023-01-05 21:58:14.869043 rdk-0.9.0/rdk.egg-info/
+-rw-r--r--   0 mbeacom    (505) staff       (20)    26490 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/PKG-INFO
+-rw-r--r--   0 mbeacom    (505) staff       (20)     5861 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mbeacom    (505) staff       (20)        1 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mbeacom    (505) staff       (20)       38 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/entry_points.txt
+-rw-r--r--   0 mbeacom    (505) staff       (20)        1 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/not-zip-safe
+-rw-r--r--   0 mbeacom    (505) staff       (20)       13 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/requires.txt
+-rw-r--r--   0 mbeacom    (505) staff       (20)        4 2023-01-05 21:58:14.000000 rdk-0.9.0/rdk.egg-info/top_level.txt
+-rw-r--r--   0 mbeacom    (505) staff       (20)       38 2023-01-05 21:58:14.896317 rdk-0.9.0/setup.cfg
+-rw-r--r--   0 mbeacom    (505) staff       (20)     1524 2023-01-05 21:52:20.000000 rdk-0.9.0/setup.py
```

### Comparing `rdk-0.8.5/LICENSE` & `rdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/MANIFEST.in` & `rdk-0.9.0/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 include rdk/template/terraform/0.12/*
 include rdk/template/example_ci/*
 include rdk/template/runtime/*
 include rdk/template/runtime/java8/*
 include rdk/template/runtime/java8/jars/*
 include rdk/template/runtime/java8/src/main/java/com/rdk/*
 include rdk/template/runtime/nodejs4.3/*
-include rdk/template/runtime/python3.6/*
-include rdk/template/runtime/python3.6-lib/*
 include rdk/template/runtime/python3.7/*
 include rdk/template/runtime/python3.7-lib/*
 include rdk/template/runtime/python3.8/*
 include rdk/template/runtime/python3.8-lib/*
 include rdk/template/runtime/python3.9/*
 include rdk/template/runtime/python3.9-lib/*
 include rdk/template/runtime/dotnetcore1.0/*
```

### Comparing `rdk-0.8.5/PKG-INFO` & `rdk-0.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-Metadata-Version: 2.1
-Name: rdk
-Version: 0.8.5
-Summary: Rule Development Kit CLI for AWS Config
-Home-page: https://github.com/awslabs/aws-config-rdk/
-Author: RDK maintainer
-Author-email: rdk-maintainers@amazon.com
-License: Apache License Version 2.0
-License-File: LICENSE
-License-File: NOTICE.txt
-
 rdk
 ===
 Rule Development Kit
+
 We greatly appreciate feedback and bug reports at rdk-maintainers@amazon.com! You may also create an issue on this repo.
 
 The RDK is designed to support a "Compliance-as-Code" workflow that is intuitive and productive.  It abstracts away much of the undifferentiated heavy lifting associated with deploying AWS Config rules backed by custom lambda functions, and provides a streamlined develop-deploy-monitor iterative process.
 
 For complete documentation, including command reference, check out the `ReadTheDocs documentation <https://rdk.readthedocs.io/en/latest/>`_.
 
 Getting Started
 ===============
-Uses python 3.6/3.7/3.8/3.9 and is installed via pip.  Requires you to have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions.  An AWS IAM Policy Document that describes the minimum necessary permissions can be found at policy/rdk-minimum-permissions.json.
+Uses python 3.7/3.8/3.9 and is installed via pip.  Requires you to have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions.  An AWS IAM Policy Document that describes the minimum necessary permissions can be found at policy/rdk-minimum-permissions.json.
 
 Under the hood, rdk uses boto3 to make API calls to AWS, so you can set your credentials any way that boto3 recognizes (options 3 through 8 here: http://boto3.readthedocs.io/en/latest/guide/configuration.html) or pass them in with the command-line parameters --profile, --region, --access-key-id, or --secret-access-key
 
 If you just want to use the RDK, go ahead and install it using pip::
 
 $ pip install rdk
 
@@ -146,15 +136,15 @@
 
 Modify Rule
 -----------
 If you need to change the parameters of a Config rule in your working directory you can use the ``modify`` command.  Any parameters you specify will overwrite existing values, any that you do not specify will not be changed.
 
 ::
 
-  $ rdk modify MyRule --runtime python3.6 --maximum-frequency TwentyFour_Hours --input-parameters '{"desiredInstanceType":"t2.micro"}'
+  $ rdk modify MyRule --runtime python3.9 --maximum-frequency TwentyFour_Hours --input-parameters '{"desiredInstanceType":"t2.micro"}'
   Running modify!
   Modified Rule 'MyRule'.  Use the `deploy` command to push your changes to AWS.
 
 Again, on Windows the input parameters would look like::
 
   '{\"desiredInstanceType\":\"t2.micro\"}'
 
@@ -218,15 +208,15 @@
 You can use the ``-n`` and ``-f`` command line flags just like the UNIX ``tail`` command to view a larger number of log events and to continuously poll for new events.  The latter option can be useful in conjunction with manually initiating Config Evaluations for your deploy Config Rule to make sure it is behaving as expected.
 
 
 
 Running the tests
 =================
 
-The `testing` directory contains scripts and buildspec files that I use to run basic functionality tests across a variety of CLI environments (currently Ubuntu linux running python 3.6/3.7/3.8/3.9, and Windows Server running python3.6).  If there is interest I can release a CloudFormation template that could be used to build the test environment, let me know if this is something you want!
+The `testing` directory contains scripts and buildspec files that I use to run basic functionality tests across a variety of CLI environments (currently Ubuntu linux running python 3.7/3.8/3.9, and Windows Server running python3.9).  If there is interest I can release a CloudFormation template that could be used to build the test environment, let me know if this is something you want!
 
 
 Advanced Features
 =================
 Cross-Account Deployments
 -------------------------
 Features have been added to the RDK to facilitate the cross-account deployment pattern that enterprise customers have standardized on for custom Config Rules. A cross-account architecture is one in which the Lambda functions are deployed to a single central "Compliance" account (which may be the same as a central "Security" account), and the Config Rules are deployed to any number of "Satellite" accounts that are used by other teams or departments.  This gives the compliance team confidence that their Rule logic cannot be tampered with and makes it much easier for them to modify rule logic without having to go through a complex deployment process to potentially hundreds of AWS accounts.  The cross-account pattern uses two advanced RDK features - functions-only deployments and the `create-rule-template` command.
@@ -319,15 +309,15 @@
 
 To create a sample starter region group, run `rdk create-region-set` to specify the filename, add the `-o <region set output file name>` this will create a region set with the following tests and regions `"default":["us-east-1","us-west-1","eu-north-1","ap-east-1"],"aws-cn-region-set":["cn-north-1","cn-northwest-1"]`
 
 Using RDK to Generate a Lambda Layer in a region (Python3)
 ----------------------------------------------------------
 By default `rdk init --generate-lambda-layer` will generate an rdklib lambda layer while running init in whatever region it is run, to force re-generation of the layer, run `rdk init --generate-lambda-layer` again over a region
 
-To use this generated lambda layer, add the flag `--generated-lambda-layer` when running `rdk deploy`. For example: `rdk -f regions.yaml deploy LP3_TestRule_P36_lib --generated-lambda-layer`
+To use this generated lambda layer, add the flag `--generated-lambda-layer` when running `rdk deploy`. For example: `rdk -f regions.yaml deploy LP3_TestRule_P39_lib --generated-lambda-layer`
 
 If you created layer with a custom name (by running `rdk init --custom-lambda-layer`, add a similar `custom-lambda-layer` flag when running deploy.
 
 Contributing
 ============
 
 email us at rdk-maintainers@amazon.com if you have any questions. We are happy to help and discuss.
```

### Comparing `rdk-0.8.5/README.rst` & `rdk-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,354 +1,370 @@
-rdk
-===
-Rule Development Kit
-We greatly appreciate feedback and bug reports at rdk-maintainers@amazon.com! You may also create an issue on this repo.
-
-The RDK is designed to support a "Compliance-as-Code" workflow that is intuitive and productive.  It abstracts away much of the undifferentiated heavy lifting associated with deploying AWS Config rules backed by custom lambda functions, and provides a streamlined develop-deploy-monitor iterative process.
-
-For complete documentation, including command reference, check out the `ReadTheDocs documentation <https://rdk.readthedocs.io/en/latest/>`_.
-
-Getting Started
-===============
-Uses python 3.6/3.7/3.8/3.9 and is installed via pip.  Requires you to have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions.  An AWS IAM Policy Document that describes the minimum necessary permissions can be found at policy/rdk-minimum-permissions.json.
-
-Under the hood, rdk uses boto3 to make API calls to AWS, so you can set your credentials any way that boto3 recognizes (options 3 through 8 here: http://boto3.readthedocs.io/en/latest/guide/configuration.html) or pass them in with the command-line parameters --profile, --region, --access-key-id, or --secret-access-key
-
-If you just want to use the RDK, go ahead and install it using pip::
-
-$ pip install rdk
-
-Alternately, if you want to see the code and/or contribute you can clone the git repo, and then from the repo directory use pip to install the package.  Use the '-e' flag to generate symlinks so that any edits you make will be reflected when you run the installed package.
-
-If you are going to author your Lambda functions using Java you will need to have Java 8 and gradle installed.  If you are going to author your Lambda functions in C# you will need to have the dotnet CLI and the .NET Core Runtime 1.08 installed.
-::
-
-  $ pip install -e .
-
-To make sure the rdk is installed correctly, running the package from the command line without any arguments should display help information.
-
-::
-
-  $ rdk
-  usage: rdk [-h] [-p PROFILE] [-k ACCESS_KEY] [-s SECRET_ACCESS_KEY]
-           [-r REGION]
-           <command> ...
-  rdk: error: the following arguments are required: <command>, <command arguments>
-
-
-Usage
-=====
-
-Configure your env
-------------------
-To use the RDK, it's recommended to create a directory that will be your working directory.  This should be committed to a source code repo, and ideally created as a python virtualenv.  In that directory, run the ``init`` command to set up your AWS Config environment.
-
-::
-
-  $ rdk init
-  Running init!
-  Creating Config bucket config-bucket-780784666283
-  Creating IAM role config-role
-  Waiting for IAM role to propagate
-  Config Service is ON
-  Config setup complete.
-  Creating Code bucket config-rule-code-bucket-780784666283ap-southeast-1
-
-Running ``init`` subsequent times will validate your AWS Config setup and re-create any S3 buckets or IAM resources that are needed.
-
-- If you have config delivery bucket already present in some other AWS account then use **--config-bucket-exists-in-another-account** as argument:::
-
-  $ rdk init --config-bucket-exists-in-another-account
-- If you have AWS Organizations/ControlTower Setup in your AWS environment then additionally, use **--control-tower** as argument:::
-
-  $ rdk init --control-tower --config-bucket-exists-in-another-account
-- If bucket for custom lambda code is already present in current account then use **--skip-code-bucket-creation** argument:::
-
-  $ rdk init --skip-code-bucket-creation
-
-- If you want rdk to create/update and upload the rdklib-layer for you, then use **--generate-lambda-layer** argument. In supported regions, rdk will deploy the layer using the Serverless Application Repository, otherwise it will build a local lambda layer archive and upload it for use:::
-
-  $ rdk init --generate-lambda-layer 
-- If you want rdk to give a custom name to the lambda layer for you, then use **--custom-layer-namer** argument. The Serverless Application Repository currently cannot be used for custom lambda layers.:::
-
-  $ rdk init --generate-lambda-layer --custom-layer-name <LAYER_NAME>
-
-Create Rules
-------------
-In your working directory, use the ``create`` command to start creating a new custom rule.  You must specify the runtime for the lambda function that will back the Rule, and you can also specify a resource type (or comma-separated list of types) that the Rule will evaluate or a maximum frequency for a periodic rule.  This will add a new directory for the rule and populate it with several files, including a skeleton of your Lambda code.
-
-::
-
-  $ rdk create MyRule --runtime python3.8 --resource-types AWS::EC2::Instance --input-parameters '{"desiredInstanceType":"t2.micro"}'
-  Running create!
-  Local Rule files created.
-
-On Windows it is necessary to escape the double-quotes when specifying input parameters, so the `--input-parameters` argument would instead look something like this::
-
-  '{\"desiredInstanceType\":\"t2.micro\"}'
-
-Note that you can create rules that use EITHER resource-types OR maximum-frequency, but not both.  We have found that rules that try to be both event-triggered as well as periodic wind up being very complicated and so we do not recommend it as a best practice.
-
-Edit Rules Locally
----------------------------
-Once you have created the rule, edit the python file in your rule directory (in the above example it would be ``MyRule/MyRule.py``, but may be deeper into the rule directory tree depending on your chosen Lambda runtime) to add whatever logic your Rule requires in the ``evaluate_compliance`` function.  You will have access to the CI that was sent by Config, as well as any parameters configured for the Config Rule.  Your function should return either a simple compliance status (one of ``COMPLIANT``, ``NONCOMPLIANT``, or ``NOT_APPLICABLE``), or if you're using the python or node runtimes you can return a JSON object with multiple evaluation responses that the RDK will send back to AWS Config.  An example would look like::
-
-  for sg in response['SecurityGroups']:
-        evaluations.append(
-        {
-                'ComplianceResourceType': 'AWS::EC2::SecurityGroup',
-                'ComplianceResourceId': sg['GroupId'],
-                'ComplianceType': 'COMPLIANT',
-                'Annotation': 'This is an important note.',
-                'OrderingTimestamp': str(datetime.datetime.now())
-        })
-
-
-    return evaluations
-
-This is necessary for periodic rules that are not triggered by any CI change (which means the CI that is passed in will be null), and also for attaching annotations to your evaluation results.
-
-If you want to see what the JSON structure of a CI looks like for creating your logic, you can use
-
-::
-
-$ rdk sample-ci <Resource Type>
-
-to output a formatted JSON document.
-
-Write and Run Unit Tests
-------------------------
-If you are writing Config Rules using either of the Python runtimes there will be a <rule name>_test.py file deployed along with your Lambda function skeleton.  This can be used to write unit tests according to the standard Python unittest framework (documented here: https://docs.python.org/3/library/unittest.html), which can be run using the `test-local` rdk command::
-
-  $ rdk test-local MyTestRule
-  Running local test!
-  Testing MyTestRule
-  Looking for tests in /Users/mborch/Code/rdk-dev/MyTestRule
-
-  ---------------------------------------------------------------------
-
-  Ran 0 tests in 0.000s
-
-  OK
-  <unittest.runner.TextTestResult run=0 errors=0 failures=0>
-
-The test file includes setup for the MagicMock library that can be used to stub boto3 API calls if your rule logic will involve making API calls to gather additional information about your AWS environment.  For some tips on how to do this, check out this blog post: https://sgillies.net/2017/10/19/mock-is-magic.html
-
-Modify Rule
------------
-If you need to change the parameters of a Config rule in your working directory you can use the ``modify`` command.  Any parameters you specify will overwrite existing values, any that you do not specify will not be changed.
-
-::
-
-  $ rdk modify MyRule --runtime python3.6 --maximum-frequency TwentyFour_Hours --input-parameters '{"desiredInstanceType":"t2.micro"}'
-  Running modify!
-  Modified Rule 'MyRule'.  Use the `deploy` command to push your changes to AWS.
-
-Again, on Windows the input parameters would look like::
-
-  '{\"desiredInstanceType\":\"t2.micro\"}'
-
-It is worth noting that until you actually call the ``deploy`` command your rule only exists in your working directory, none of the Rule commands discussed thus far actually makes changes to your account.
-
-Deploy Rule
------------
-Once you have completed your compliance validation code and set your Rule's configuration, you can deploy the Rule to your account using the ``deploy`` command.  This will zip up your code (and the other associated code files, if any) into a deployable package (or run a gradle build if you have selected the java8 runtime or run the lambda packaging step from the dotnet CLI if you have selected the dotnetcore1.0 runtime), copy that zip file to S3, and then launch or update a CloudFormation stack that defines your Config Rule, Lambda function, and the necessary permissions and IAM Roles for it to function.  Since CloudFormation does not deeply inspect Lambda code objects in S3 to construct its changeset, the ``deploy`` command will also directly update the Lambda function for any subsequent deployments to make sure code changes are propagated correctly.
-
-::
-
-  $ rdk deploy MyRule
-  Running deploy!
-  Zipping MyRule
-  Uploading MyRule
-  Creating CloudFormation Stack for MyRule
-  Waiting for CloudFormation stack operation to complete...
-  ...
-  Waiting for CloudFormation stack operation to complete...
-  Config deploy complete.
-
-The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.  If you used the --generate-lambda-layer flag in rdk init, use the --generated-lambda-layer flag for rdk deploy.
-
-Deploy Organization Rule
-------------------------
-You can also deploy the Rule to your AWS Organization using the ``deploy-organization`` command.
-For successful evaluation of custom rules in child accounts, please make sure you do one of the following:
-
-1. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume the Role attached on the Config Service and confirm that the role trusts the master account where the Lambda function is going to be deployed.
-2. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume a custom role and define an optional parameter with key as ExecutionRoleName and set the value to your custom role name; confirm that the role trusts the master account of the organization where the Lambda function will be deployed.
-
-::
-
-  $ rdk deploy-organization MyRule
-  Running deploy!
-  Zipping MyRule
-  Uploading MyRule
-  Creating CloudFormation Stack for MyRule
-  Waiting for CloudFormation stack operation to complete...
-  ...
-  Waiting for CloudFormation stack operation to complete...
-  Config deploy complete.
-
-The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.
-This command uses 'PutOrganizationConfigRule' API for the rule deployment. If a new account joins an organization, the rule is deployed to that account. When an account leaves an organization, the rule is removed. Deployment of existing organizational AWS Config Rules will only be retried for 7 hours after an account is added to your organization if a recorder is not available. You are expected to create a recorder if one doesn't exist within 7 hours of adding an account to your organization.
-
-View Logs For Deployed Rule
----------------------------
-Once the Rule has been deployed to AWS you can get the CloudWatch logs associated with your lambda function using the ``logs`` command.
-
-::
-
-  $ rdk logs MyRule -n 5
-  2017-11-15 22:59:33 - START RequestId: 96e7639a-ca15-11e7-95a2-b1521890638d Version: $LATEST
-  2017-11-15 23:41:13 - REPORT RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda    Duration: 0.50 ms    Billed Duration: 100 ms     Memory Size: 256 MB
-                            Max Memory Used: 36 MB
-  2017-11-15 23:41:13 - END RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda
-  2017-11-15 23:41:13 - Default RDK utility class does not yet support Scheduled Notifications.
-  2017-11-15 23:41:13 - START RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda Version: $LATEST
-
-You can use the ``-n`` and ``-f`` command line flags just like the UNIX ``tail`` command to view a larger number of log events and to continuously poll for new events.  The latter option can be useful in conjunction with manually initiating Config Evaluations for your deploy Config Rule to make sure it is behaving as expected.
-
-
-
-Running the tests
-=================
-
-The `testing` directory contains scripts and buildspec files that I use to run basic functionality tests across a variety of CLI environments (currently Ubuntu linux running python 3.6/3.7/3.8/3.9, and Windows Server running python3.6).  If there is interest I can release a CloudFormation template that could be used to build the test environment, let me know if this is something you want!
-
-
-Advanced Features
-=================
-Cross-Account Deployments
--------------------------
-Features have been added to the RDK to facilitate the cross-account deployment pattern that enterprise customers have standardized on for custom Config Rules. A cross-account architecture is one in which the Lambda functions are deployed to a single central "Compliance" account (which may be the same as a central "Security" account), and the Config Rules are deployed to any number of "Satellite" accounts that are used by other teams or departments.  This gives the compliance team confidence that their Rule logic cannot be tampered with and makes it much easier for them to modify rule logic without having to go through a complex deployment process to potentially hundreds of AWS accounts.  The cross-account pattern uses two advanced RDK features - functions-only deployments and the `create-rule-template` command.
-
-**Function-Only Deployment**
-
-By using the `-f` or `--functions-only` flag on the `deploy` command the RDK will deploy only the necessary Lambda Functions, Lambda Execution Role, and Lambda Permissions to the account specified by the execution credentials.  It accomplishes this by batching up all of the Lambda function CloudFormation snippets for the selected Rule(s) into a single dynamically generated template and deploy that CloudFormation template.  One consequence of this is that subsequent deployments that specify a different set of Rules for the same stack name will update that CloudFormation stack, and any Rules that were included in the first deployment but not in the second will be removed.  You can use the `--stack-name` parameter to override the default CloudFormation stack name if you need to manage different subsets of your Lambda Functions independently.  The intended usage is to deploy the functions for all of the Config rules in the Security/Compliance account, which can be done simply by using `rdk deploy -f --all` from your working directory.
-
-**`create-rule-template` command**
-
-This command generates a CloudFormation template that defines the AWS Config rules themselves, along with the Config Role, Config data bucket, Configuration Recorder, and Delivery channel necessary for the Config rules to work in a satellite account.  You must specify the file name for the generated template using the `--output-file` or `o` command line flags.  The generated template takes a single parameter of the AccountID of the central compliance account that contains the Lambda functions that will back your custom Config Rules.  The generated template can be deployed in the desired satellite accounts through any of the means that you can deploy any other CloudFormation template, including the console, the CLI, as a CodePipeline task, or using StackSets.  The `create-rule-template` command takes all of the standard arguments for selecting Rules to include in the generated template, including lists of individual Rule names, an `--all` flag, or using the RuleSets feature described below.
-
-::
-
-  $ rdk create-rule-template -o remote-rule-template.json --all
-  Generating CloudFormation template!
-  CloudFormation template written to remote-rule-template.json
-
-
-Disable the supported resource types check
-------------------------------------------
-It is now possible to define a resource type that is not yet supported by rdk. To disable the supported resource check use the optional flag '--skip-supported-resource-check' during the create command.
-
-::
-
-  $ rdk create MyRule --runtime python3.8 --resource-types AWS::New::ResourceType --skip-supported-resource-check
-  'AWS::New::ResourceType' not found in list of accepted resource types.
-  Skip-Supported-Resource-Check Flag set (--skip-supported-resource-check), ignoring missing resource type error.
-  Running create!
-  Local Rule files created.
-
-Custom Lambda Function Name
----------------------------
-As of version 0.7.14, instead of defaulting the lambda function names to 'RDK-Rule-Function-<RULE_NAME>' it is possible to customize the name for the Lambda function to any 64 characters string as per Lambda's naming standards using the optional '--custom-lambda-name' flag while performing rdk create. This opens up new features like :
-
-1. Longer config rule name.
-2. Custom lambda function naming as per personal or enterprise standards.
-
-::
-
-  $ rdk create MyLongerRuleName --runtime python3.8 --resource-types AWS::EC2::Instance --custom-lambda-name custom-prefix-for-MyLongerRuleName
-  Running create!
-  Local Rule files created.
-
-The above example would create files with config rule name as 'MyLongerRuleName' and lambda function with the name 'custom-prefix-for-MyLongerRuleName' instead of 'RDK-Rule-Function-MyLongerRuleName'
-
-RuleSets
---------
-New as of version 0.3.11, it is possible to add RuleSet tags to rules that can be used to deploy and test groups of rules together.  Rules can belong to multiple RuleSets, and RuleSet membership is stored only in the parameters.json metadata.  The `deploy`, `create-rule-template`, and `test-local` commands are RuleSet-aware such that a RuleSet can be passed in as the target instead of `--all` or a specific named Rule.
-
-A comma-delimited list of RuleSets can be added to a Rule when you create it (using the `--rulesets` flag), as part of a `modify` command, or using new `ruleset` subcommands to add or remove individual rules from a RuleSet.
-
-Running `rdk rulesets list` will display a list of the RuleSets currently defined across all of the Rules in the working directory
-
-::
-
-  rdk-dev $ rdk rulesets list
-  RuleSets:  AnotherRuleSet MyNewSet
-
-Naming a specific RuleSet will list all of the Rules that are part of that RuleSet.
-
-::
-
-  rdk-dev $ rdk rulesets list AnotherRuleSet
-  Rules in AnotherRuleSet :  RSTest
-
-Rules can be added to or removed from RuleSets using the `add` and `remove` subcommands:
-
-::
-
-  rdk-dev $ rdk rulesets add MyNewSet RSTest
-  RSTest added to RuleSet MyNewSet
-
-  rdk-dev $ rdk rulesets remove AnotherRuleSet RSTest
-  RSTest removed from RuleSet AnotherRuleSet
-
-RuleSets are a convenient way to maintain a single repository of Config Rules that may need to have subsets of them deployed to different environments.  For example your development environment may contain some of the Rules that you run in Production but not all of them; RuleSets gives you a way to identify and selectively deploy the appropriate Rules to each environment.
-
-Managed Rules
--------------
-The RDK is able to deploy AWS Managed Rules.
-
-To do so, create a rule using "rdk create" and provide a valid SourceIdentifier via the --source-identifier CLI option. The list of Managed Rules can be found here: https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html, and note that the Identifier can be obtained by replacing the dashes with underscores and using all capitals (for example, the "guardduty-enabled-centralized" rule has the SourceIdentifier "GUARDDUTY_ENABLED_CENTRALIZED").  Just like custom Rules you will need to specify source events and/or a maximum evaluation frequency, and also pass in any Rule parameters.  The resulting Rule directory will contain only the parameters.json file, but using `rdk deploy` or `rdk create-rule-template` can be used to deploy the Managed Rule like any other Custom Rule.
-
-Deploying Rules Across Multiple Regions
----------------------------------------
-The RDK is able to run init/deploy/undeploy across multiple regions with a `rdk -f <region file> -t <region set>`
-
-If no region group is specified, rdk will deploy to the `default` region set
-
-To create a sample starter region group, run `rdk create-region-set` to specify the filename, add the `-o <region set output file name>` this will create a region set with the following tests and regions `"default":["us-east-1","us-west-1","eu-north-1","ap-east-1"],"aws-cn-region-set":["cn-north-1","cn-northwest-1"]`
-
-Using RDK to Generate a Lambda Layer in a region (Python3)
-----------------------------------------------------------
-By default `rdk init --generate-lambda-layer` will generate an rdklib lambda layer while running init in whatever region it is run, to force re-generation of the layer, run `rdk init --generate-lambda-layer` again over a region
-
-To use this generated lambda layer, add the flag `--generated-lambda-layer` when running `rdk deploy`. For example: `rdk -f regions.yaml deploy LP3_TestRule_P36_lib --generated-lambda-layer`
-
-If you created layer with a custom name (by running `rdk init --custom-lambda-layer`, add a similar `custom-lambda-layer` flag when running deploy.
-
-Contributing
-============
-
-email us at rdk-maintainers@amazon.com if you have any questions. We are happy to help and discuss.
-
-Contacts
-========
-* **Ricky Chau** - `rickychau2780 <https://github.com/rickychau2780>`_ - *current maintainer*
-* **Jarrett Andrulis** - `jarrettandrulis <https://github.com/jarrettandrulis>`_ - *current maintainer*
-* **Julio Delgado Jr** - `tekdj7 <https://github.com/tekdj7>`_ - *current maintainer*
-* **Sandeep Batchu** - `batchus <https://github.com/batchus>`_ - *current maintainer*
-
-Past Contributors
-=================
-* **Michael Borchert** - *Orignal Python version*
-* **Jonathan Rault** - *Orignal Design, testing, feedback*
-* **Greg Kim and Chris Gutierrez** - *Initial work and CI definitions*
-* **Henry Huang** - *Original CFN templates and other code*
-* **Santosh Kumar** - *maintainer*
-* **Jose Obando** - *maintainer*
-
-License
-=======
-
-This project is licensed under the Apache 2.0 License
-
-Acknowledgments
-===============
-
-* the boto3 team makes all of this magic possible.
-
-
-Link
-====
-
-* to view example of rules built with the RDK: https://github.com/awslabs/aws-config-rules/tree/master/python
+Metadata-Version: 1.1
+Name: rdk
+Version: 0.9.0
+Summary: Rule Development Kit CLI for AWS Config
+Home-page: https://github.com/awslabs/aws-config-rdk/
+Author: RDK maintainer
+Author-email: rdk-maintainers@amazon.com
+License: Apache License Version 2.0
+Description: rdk
+        ===
+        Rule Development Kit
+        
+        We greatly appreciate feedback and bug reports at rdk-maintainers@amazon.com! You may also create an issue on this repo.
+        
+        The RDK is designed to support a "Compliance-as-Code" workflow that is intuitive and productive.  It abstracts away much of the undifferentiated heavy lifting associated with deploying AWS Config rules backed by custom lambda functions, and provides a streamlined develop-deploy-monitor iterative process.
+        
+        For complete documentation, including command reference, check out the `ReadTheDocs documentation <https://rdk.readthedocs.io/en/latest/>`_.
+        
+        Getting Started
+        ===============
+        Uses python 3.7/3.8/3.9 and is installed via pip.  Requires you to have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions.  An AWS IAM Policy Document that describes the minimum necessary permissions can be found at policy/rdk-minimum-permissions.json.
+        
+        Under the hood, rdk uses boto3 to make API calls to AWS, so you can set your credentials any way that boto3 recognizes (options 3 through 8 here: http://boto3.readthedocs.io/en/latest/guide/configuration.html) or pass them in with the command-line parameters --profile, --region, --access-key-id, or --secret-access-key
+        
+        If you just want to use the RDK, go ahead and install it using pip::
+        
+        $ pip install rdk
+        
+        Alternately, if you want to see the code and/or contribute you can clone the git repo, and then from the repo directory use pip to install the package.  Use the '-e' flag to generate symlinks so that any edits you make will be reflected when you run the installed package.
+        
+        If you are going to author your Lambda functions using Java you will need to have Java 8 and gradle installed.  If you are going to author your Lambda functions in C# you will need to have the dotnet CLI and the .NET Core Runtime 1.08 installed.
+        ::
+        
+          $ pip install -e .
+        
+        To make sure the rdk is installed correctly, running the package from the command line without any arguments should display help information.
+        
+        ::
+        
+          $ rdk
+          usage: rdk [-h] [-p PROFILE] [-k ACCESS_KEY] [-s SECRET_ACCESS_KEY]
+                   [-r REGION]
+                   <command> ...
+          rdk: error: the following arguments are required: <command>, <command arguments>
+        
+        
+        Usage
+        =====
+        
+        Configure your env
+        ------------------
+        To use the RDK, it's recommended to create a directory that will be your working directory.  This should be committed to a source code repo, and ideally created as a python virtualenv.  In that directory, run the ``init`` command to set up your AWS Config environment.
+        
+        ::
+        
+          $ rdk init
+          Running init!
+          Creating Config bucket config-bucket-780784666283
+          Creating IAM role config-role
+          Waiting for IAM role to propagate
+          Config Service is ON
+          Config setup complete.
+          Creating Code bucket config-rule-code-bucket-780784666283ap-southeast-1
+        
+        Running ``init`` subsequent times will validate your AWS Config setup and re-create any S3 buckets or IAM resources that are needed.
+        
+        - If you have config delivery bucket already present in some other AWS account then use **--config-bucket-exists-in-another-account** as argument:::
+        
+          $ rdk init --config-bucket-exists-in-another-account
+        - If you have AWS Organizations/ControlTower Setup in your AWS environment then additionally, use **--control-tower** as argument:::
+        
+          $ rdk init --control-tower --config-bucket-exists-in-another-account
+        - If bucket for custom lambda code is already present in current account then use **--skip-code-bucket-creation** argument:::
+        
+          $ rdk init --skip-code-bucket-creation
+        
+        - If you want rdk to create/update and upload the rdklib-layer for you, then use **--generate-lambda-layer** argument. In supported regions, rdk will deploy the layer using the Serverless Application Repository, otherwise it will build a local lambda layer archive and upload it for use:::
+        
+          $ rdk init --generate-lambda-layer 
+        - If you want rdk to give a custom name to the lambda layer for you, then use **--custom-layer-namer** argument. The Serverless Application Repository currently cannot be used for custom lambda layers.:::
+        
+          $ rdk init --generate-lambda-layer --custom-layer-name <LAYER_NAME>
+        
+        Create Rules
+        ------------
+        In your working directory, use the ``create`` command to start creating a new custom rule.  You must specify the runtime for the lambda function that will back the Rule, and you can also specify a resource type (or comma-separated list of types) that the Rule will evaluate or a maximum frequency for a periodic rule.  This will add a new directory for the rule and populate it with several files, including a skeleton of your Lambda code.
+        
+        ::
+        
+          $ rdk create MyRule --runtime python3.8 --resource-types AWS::EC2::Instance --input-parameters '{"desiredInstanceType":"t2.micro"}'
+          Running create!
+          Local Rule files created.
+        
+        On Windows it is necessary to escape the double-quotes when specifying input parameters, so the `--input-parameters` argument would instead look something like this::
+        
+          '{\"desiredInstanceType\":\"t2.micro\"}'
+        
+        Note that you can create rules that use EITHER resource-types OR maximum-frequency, but not both.  We have found that rules that try to be both event-triggered as well as periodic wind up being very complicated and so we do not recommend it as a best practice.
+        
+        Edit Rules Locally
+        ---------------------------
+        Once you have created the rule, edit the python file in your rule directory (in the above example it would be ``MyRule/MyRule.py``, but may be deeper into the rule directory tree depending on your chosen Lambda runtime) to add whatever logic your Rule requires in the ``evaluate_compliance`` function.  You will have access to the CI that was sent by Config, as well as any parameters configured for the Config Rule.  Your function should return either a simple compliance status (one of ``COMPLIANT``, ``NONCOMPLIANT``, or ``NOT_APPLICABLE``), or if you're using the python or node runtimes you can return a JSON object with multiple evaluation responses that the RDK will send back to AWS Config.  An example would look like::
+        
+          for sg in response['SecurityGroups']:
+                evaluations.append(
+                {
+                        'ComplianceResourceType': 'AWS::EC2::SecurityGroup',
+                        'ComplianceResourceId': sg['GroupId'],
+                        'ComplianceType': 'COMPLIANT',
+                        'Annotation': 'This is an important note.',
+                        'OrderingTimestamp': str(datetime.datetime.now())
+                })
+        
+        
+            return evaluations
+        
+        This is necessary for periodic rules that are not triggered by any CI change (which means the CI that is passed in will be null), and also for attaching annotations to your evaluation results.
+        
+        If you want to see what the JSON structure of a CI looks like for creating your logic, you can use
+        
+        ::
+        
+        $ rdk sample-ci <Resource Type>
+        
+        to output a formatted JSON document.
+        
+        Write and Run Unit Tests
+        ------------------------
+        If you are writing Config Rules using either of the Python runtimes there will be a <rule name>_test.py file deployed along with your Lambda function skeleton.  This can be used to write unit tests according to the standard Python unittest framework (documented here: https://docs.python.org/3/library/unittest.html), which can be run using the `test-local` rdk command::
+        
+          $ rdk test-local MyTestRule
+          Running local test!
+          Testing MyTestRule
+          Looking for tests in /Users/mborch/Code/rdk-dev/MyTestRule
+        
+          ---------------------------------------------------------------------
+        
+          Ran 0 tests in 0.000s
+        
+          OK
+          <unittest.runner.TextTestResult run=0 errors=0 failures=0>
+        
+        The test file includes setup for the MagicMock library that can be used to stub boto3 API calls if your rule logic will involve making API calls to gather additional information about your AWS environment.  For some tips on how to do this, check out this blog post: https://sgillies.net/2017/10/19/mock-is-magic.html
+        
+        Modify Rule
+        -----------
+        If you need to change the parameters of a Config rule in your working directory you can use the ``modify`` command.  Any parameters you specify will overwrite existing values, any that you do not specify will not be changed.
+        
+        ::
+        
+          $ rdk modify MyRule --runtime python3.9 --maximum-frequency TwentyFour_Hours --input-parameters '{"desiredInstanceType":"t2.micro"}'
+          Running modify!
+          Modified Rule 'MyRule'.  Use the `deploy` command to push your changes to AWS.
+        
+        Again, on Windows the input parameters would look like::
+        
+          '{\"desiredInstanceType\":\"t2.micro\"}'
+        
+        It is worth noting that until you actually call the ``deploy`` command your rule only exists in your working directory, none of the Rule commands discussed thus far actually makes changes to your account.
+        
+        Deploy Rule
+        -----------
+        Once you have completed your compliance validation code and set your Rule's configuration, you can deploy the Rule to your account using the ``deploy`` command.  This will zip up your code (and the other associated code files, if any) into a deployable package (or run a gradle build if you have selected the java8 runtime or run the lambda packaging step from the dotnet CLI if you have selected the dotnetcore1.0 runtime), copy that zip file to S3, and then launch or update a CloudFormation stack that defines your Config Rule, Lambda function, and the necessary permissions and IAM Roles for it to function.  Since CloudFormation does not deeply inspect Lambda code objects in S3 to construct its changeset, the ``deploy`` command will also directly update the Lambda function for any subsequent deployments to make sure code changes are propagated correctly.
+        
+        ::
+        
+          $ rdk deploy MyRule
+          Running deploy!
+          Zipping MyRule
+          Uploading MyRule
+          Creating CloudFormation Stack for MyRule
+          Waiting for CloudFormation stack operation to complete...
+          ...
+          Waiting for CloudFormation stack operation to complete...
+          Config deploy complete.
+        
+        The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.  If you used the --generate-lambda-layer flag in rdk init, use the --generated-lambda-layer flag for rdk deploy.
+        
+        Deploy Organization Rule
+        ------------------------
+        You can also deploy the Rule to your AWS Organization using the ``deploy-organization`` command.
+        For successful evaluation of custom rules in child accounts, please make sure you do one of the following:
+        
+        1. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume the Role attached on the Config Service and confirm that the role trusts the master account where the Lambda function is going to be deployed.
+        2. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume a custom role and define an optional parameter with key as ExecutionRoleName and set the value to your custom role name; confirm that the role trusts the master account of the organization where the Lambda function will be deployed.
+        
+        ::
+        
+          $ rdk deploy-organization MyRule
+          Running deploy!
+          Zipping MyRule
+          Uploading MyRule
+          Creating CloudFormation Stack for MyRule
+          Waiting for CloudFormation stack operation to complete...
+          ...
+          Waiting for CloudFormation stack operation to complete...
+          Config deploy complete.
+        
+        The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.
+        This command uses 'PutOrganizationConfigRule' API for the rule deployment. If a new account joins an organization, the rule is deployed to that account. When an account leaves an organization, the rule is removed. Deployment of existing organizational AWS Config Rules will only be retried for 7 hours after an account is added to your organization if a recorder is not available. You are expected to create a recorder if one doesn't exist within 7 hours of adding an account to your organization.
+        
+        View Logs For Deployed Rule
+        ---------------------------
+        Once the Rule has been deployed to AWS you can get the CloudWatch logs associated with your lambda function using the ``logs`` command.
+        
+        ::
+        
+          $ rdk logs MyRule -n 5
+          2017-11-15 22:59:33 - START RequestId: 96e7639a-ca15-11e7-95a2-b1521890638d Version: $LATEST
+          2017-11-15 23:41:13 - REPORT RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda    Duration: 0.50 ms    Billed Duration: 100 ms     Memory Size: 256 MB
+                                    Max Memory Used: 36 MB
+          2017-11-15 23:41:13 - END RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda
+          2017-11-15 23:41:13 - Default RDK utility class does not yet support Scheduled Notifications.
+          2017-11-15 23:41:13 - START RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda Version: $LATEST
+        
+        You can use the ``-n`` and ``-f`` command line flags just like the UNIX ``tail`` command to view a larger number of log events and to continuously poll for new events.  The latter option can be useful in conjunction with manually initiating Config Evaluations for your deploy Config Rule to make sure it is behaving as expected.
+        
+        
+        
+        Running the tests
+        =================
+        
+        The `testing` directory contains scripts and buildspec files that I use to run basic functionality tests across a variety of CLI environments (currently Ubuntu linux running python 3.7/3.8/3.9, and Windows Server running python3.9).  If there is interest I can release a CloudFormation template that could be used to build the test environment, let me know if this is something you want!
+        
+        
+        Advanced Features
+        =================
+        Cross-Account Deployments
+        -------------------------
+        Features have been added to the RDK to facilitate the cross-account deployment pattern that enterprise customers have standardized on for custom Config Rules. A cross-account architecture is one in which the Lambda functions are deployed to a single central "Compliance" account (which may be the same as a central "Security" account), and the Config Rules are deployed to any number of "Satellite" accounts that are used by other teams or departments.  This gives the compliance team confidence that their Rule logic cannot be tampered with and makes it much easier for them to modify rule logic without having to go through a complex deployment process to potentially hundreds of AWS accounts.  The cross-account pattern uses two advanced RDK features - functions-only deployments and the `create-rule-template` command.
+        
+        **Function-Only Deployment**
+        
+        By using the `-f` or `--functions-only` flag on the `deploy` command the RDK will deploy only the necessary Lambda Functions, Lambda Execution Role, and Lambda Permissions to the account specified by the execution credentials.  It accomplishes this by batching up all of the Lambda function CloudFormation snippets for the selected Rule(s) into a single dynamically generated template and deploy that CloudFormation template.  One consequence of this is that subsequent deployments that specify a different set of Rules for the same stack name will update that CloudFormation stack, and any Rules that were included in the first deployment but not in the second will be removed.  You can use the `--stack-name` parameter to override the default CloudFormation stack name if you need to manage different subsets of your Lambda Functions independently.  The intended usage is to deploy the functions for all of the Config rules in the Security/Compliance account, which can be done simply by using `rdk deploy -f --all` from your working directory.
+        
+        **`create-rule-template` command**
+        
+        This command generates a CloudFormation template that defines the AWS Config rules themselves, along with the Config Role, Config data bucket, Configuration Recorder, and Delivery channel necessary for the Config rules to work in a satellite account.  You must specify the file name for the generated template using the `--output-file` or `o` command line flags.  The generated template takes a single parameter of the AccountID of the central compliance account that contains the Lambda functions that will back your custom Config Rules.  The generated template can be deployed in the desired satellite accounts through any of the means that you can deploy any other CloudFormation template, including the console, the CLI, as a CodePipeline task, or using StackSets.  The `create-rule-template` command takes all of the standard arguments for selecting Rules to include in the generated template, including lists of individual Rule names, an `--all` flag, or using the RuleSets feature described below.
+        
+        ::
+        
+          $ rdk create-rule-template -o remote-rule-template.json --all
+          Generating CloudFormation template!
+          CloudFormation template written to remote-rule-template.json
+        
+        
+        Disable the supported resource types check
+        ------------------------------------------
+        It is now possible to define a resource type that is not yet supported by rdk. To disable the supported resource check use the optional flag '--skip-supported-resource-check' during the create command.
+        
+        ::
+        
+          $ rdk create MyRule --runtime python3.8 --resource-types AWS::New::ResourceType --skip-supported-resource-check
+          'AWS::New::ResourceType' not found in list of accepted resource types.
+          Skip-Supported-Resource-Check Flag set (--skip-supported-resource-check), ignoring missing resource type error.
+          Running create!
+          Local Rule files created.
+        
+        Custom Lambda Function Name
+        ---------------------------
+        As of version 0.7.14, instead of defaulting the lambda function names to 'RDK-Rule-Function-<RULE_NAME>' it is possible to customize the name for the Lambda function to any 64 characters string as per Lambda's naming standards using the optional '--custom-lambda-name' flag while performing rdk create. This opens up new features like :
+        
+        1. Longer config rule name.
+        2. Custom lambda function naming as per personal or enterprise standards.
+        
+        ::
+        
+          $ rdk create MyLongerRuleName --runtime python3.8 --resource-types AWS::EC2::Instance --custom-lambda-name custom-prefix-for-MyLongerRuleName
+          Running create!
+          Local Rule files created.
+        
+        The above example would create files with config rule name as 'MyLongerRuleName' and lambda function with the name 'custom-prefix-for-MyLongerRuleName' instead of 'RDK-Rule-Function-MyLongerRuleName'
+        
+        RuleSets
+        --------
+        New as of version 0.3.11, it is possible to add RuleSet tags to rules that can be used to deploy and test groups of rules together.  Rules can belong to multiple RuleSets, and RuleSet membership is stored only in the parameters.json metadata.  The `deploy`, `create-rule-template`, and `test-local` commands are RuleSet-aware such that a RuleSet can be passed in as the target instead of `--all` or a specific named Rule.
+        
+        A comma-delimited list of RuleSets can be added to a Rule when you create it (using the `--rulesets` flag), as part of a `modify` command, or using new `ruleset` subcommands to add or remove individual rules from a RuleSet.
+        
+        Running `rdk rulesets list` will display a list of the RuleSets currently defined across all of the Rules in the working directory
+        
+        ::
+        
+          rdk-dev $ rdk rulesets list
+          RuleSets:  AnotherRuleSet MyNewSet
+        
+        Naming a specific RuleSet will list all of the Rules that are part of that RuleSet.
+        
+        ::
+        
+          rdk-dev $ rdk rulesets list AnotherRuleSet
+          Rules in AnotherRuleSet :  RSTest
+        
+        Rules can be added to or removed from RuleSets using the `add` and `remove` subcommands:
+        
+        ::
+        
+          rdk-dev $ rdk rulesets add MyNewSet RSTest
+          RSTest added to RuleSet MyNewSet
+        
+          rdk-dev $ rdk rulesets remove AnotherRuleSet RSTest
+          RSTest removed from RuleSet AnotherRuleSet
+        
+        RuleSets are a convenient way to maintain a single repository of Config Rules that may need to have subsets of them deployed to different environments.  For example your development environment may contain some of the Rules that you run in Production but not all of them; RuleSets gives you a way to identify and selectively deploy the appropriate Rules to each environment.
+        
+        Managed Rules
+        -------------
+        The RDK is able to deploy AWS Managed Rules.
+        
+        To do so, create a rule using "rdk create" and provide a valid SourceIdentifier via the --source-identifier CLI option. The list of Managed Rules can be found here: https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html, and note that the Identifier can be obtained by replacing the dashes with underscores and using all capitals (for example, the "guardduty-enabled-centralized" rule has the SourceIdentifier "GUARDDUTY_ENABLED_CENTRALIZED").  Just like custom Rules you will need to specify source events and/or a maximum evaluation frequency, and also pass in any Rule parameters.  The resulting Rule directory will contain only the parameters.json file, but using `rdk deploy` or `rdk create-rule-template` can be used to deploy the Managed Rule like any other Custom Rule.
+        
+        Deploying Rules Across Multiple Regions
+        ---------------------------------------
+        The RDK is able to run init/deploy/undeploy across multiple regions with a `rdk -f <region file> -t <region set>`
+        
+        If no region group is specified, rdk will deploy to the `default` region set
+        
+        To create a sample starter region group, run `rdk create-region-set` to specify the filename, add the `-o <region set output file name>` this will create a region set with the following tests and regions `"default":["us-east-1","us-west-1","eu-north-1","ap-east-1"],"aws-cn-region-set":["cn-north-1","cn-northwest-1"]`
+        
+        Using RDK to Generate a Lambda Layer in a region (Python3)
+        ----------------------------------------------------------
+        By default `rdk init --generate-lambda-layer` will generate an rdklib lambda layer while running init in whatever region it is run, to force re-generation of the layer, run `rdk init --generate-lambda-layer` again over a region
+        
+        To use this generated lambda layer, add the flag `--generated-lambda-layer` when running `rdk deploy`. For example: `rdk -f regions.yaml deploy LP3_TestRule_P39_lib --generated-lambda-layer`
+        
+        If you created layer with a custom name (by running `rdk init --custom-lambda-layer`, add a similar `custom-lambda-layer` flag when running deploy.
+        
+        Contributing
+        ============
+        
+        email us at rdk-maintainers@amazon.com if you have any questions. We are happy to help and discuss.
+        
+        Contacts
+        ========
+        * **Ricky Chau** - `rickychau2780 <https://github.com/rickychau2780>`_ - *current maintainer*
+        * **Jarrett Andrulis** - `jarrettandrulis <https://github.com/jarrettandrulis>`_ - *current maintainer*
+        * **Julio Delgado Jr** - `tekdj7 <https://github.com/tekdj7>`_ - *current maintainer*
+        * **Sandeep Batchu** - `batchus <https://github.com/batchus>`_ - *current maintainer*
+        
+        Past Contributors
+        =================
+        * **Michael Borchert** - *Orignal Python version*
+        * **Jonathan Rault** - *Orignal Design, testing, feedback*
+        * **Greg Kim and Chris Gutierrez** - *Initial work and CI definitions*
+        * **Henry Huang** - *Original CFN templates and other code*
+        * **Santosh Kumar** - *maintainer*
+        * **Jose Obando** - *maintainer*
+        
+        License
+        =======
+        
+        This project is licensed under the Apache 2.0 License
+        
+        Acknowledgments
+        ===============
+        
+        * the boto3 team makes all of this magic possible.
+        
+        
+        Link
+        ====
+        
+        * to view example of rules built with the RDK: https://github.com/awslabs/aws-config-rules/tree/master/python
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rdk-0.8.5/rdk/__init__.py` & `rdk-0.9.0/rdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 #
 #    Licensed under the Apache License, Version 2.0 (the "License"). You may not use this file except in compliance with the License. A copy of the License is located at
 #
 #        http://aws.amazon.com/apache2.0/
 #
 #    or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
 
-MY_VERSION = "0.8.5"
+MY_VERSION = "0.9.0"
```

### Comparing `rdk-0.8.5/rdk/cli.py` & `rdk-0.9.0/rdk/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 #
 #        http://aws.amazon.com/apache2.0/
 #
 #    or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
 
 import concurrent.futures
 import copy
-import six
-import time
 
-if six.PY2:
-    import rdk
-else:
-    from rdk import rdk
+from rdk import rdk
 
 
 def main():
     # Set up command-line argument parser and parse the args.
     my_parser = rdk.get_command_parser()
     args = my_parser.parse_args()
     my_rdk = rdk.rdk(args)
```

### Comparing `rdk-0.8.5/rdk/rdk.py` & `rdk-0.9.0/rdk/rdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,16 +379,14 @@
         "-R",
         "--runtime",
         required=False,
         help="Runtime for lambda function",
         choices=[
             "nodejs6.10",
             "java8",
-            "python3.6",
-            "python3.6-lib",
             "python3.7",
             "python3.7-lib",
             "python3.8",
             "python3.8-lib",
             "python3.9",
             "python3.9-lib",
             "dotnetcore1.0",
@@ -396,15 +394,15 @@
         ],
         metavar="",
     )
     runtime_group.add_argument(
         "--source-identifier", required=False, help="[optional] Used only for creating Managed Rules."
     )
     parser.add_argument("-l", "--custom-lambda-name", required=False, help="[optional] Provide custom lambda name")
-    parser.set_defaults(runtime="python3.6-lib")
+    parser.set_defaults(runtime="python3.9-lib")
     parser.add_argument(
         "-r",
         "--resource-types",
         required=False,
         help="[optional] Resource types that will trigger event-based Rule evaluation",
     )
     parser.add_argument(
@@ -554,15 +552,15 @@
         help='[optional] Boundary Policy ARN that will be added to "rdkLambdaRole".',
     )
     parser.add_argument(
         "-g",
         "--generated-lambda-layer",
         required=False,
         action="store_true",
-        help="[optional] Forces rdk deploy to use the Python(3.6-lib,3.7-lib,3.8-lib,) lambda layer generated by rdk init --generate-lambda-layer",
+        help="[optional] Forces rdk deploy to use the Python lambda layer generated by rdk init --generate-lambda-layer",
     )
     parser.add_argument(
         "--custom-layer-name",
         required=False,
         default="rdklib-layer",
         help='[optional] To use with --generated-lambda-layer, forces the flag to look for a specific lambda-layer name. If omitted, "rdklib-layer" will be used',
     )
@@ -651,15 +649,15 @@
         help='[optional] Boundary Policy ARN that will be added to "rdkLambdaRole".',
     )
     parser.add_argument(
         "-g",
         "--generated-lambda-layer",
         required=False,
         action="store_true",
-        help="[optional] Forces rdk deploy to use the Python(3.6-lib,3.7-lib,3.8-lib,) lambda layer generated by rdk init --generate-lambda-layer",
+        help="[optional] Forces rdk deploy to use the Python lambda layer generated by rdk init --generate-lambda-layer",
     )
     parser.add_argument(
         "--custom-layer-name",
         required=False,
         default="rdklib-layer",
         help='[optional] To use with --generated-lambda-layer, forces the flag to look for a specific lambda-layer name. If omitted, "rdklib-layer" will be used',
     )
@@ -722,15 +720,15 @@
     parser.add_argument("-v", "--version", required=True, help="Terraform version", choices=["0.11", "0.12"])
     parser.add_argument("-f", "--format", required=True, help="Export Format", choices=["terraform"])
     parser.add_argument(
         "-g",
         "--generated-lambda-layer",
         required=False,
         action="store_true",
-        help="[optional] Forces rdk deploy to use the Python(3.6-lib,3.7-lib,3.8-lib,) lambda layer generated by rdk init --generate-lambda-layer",
+        help="[optional] Forces rdk deploy to use the Python lambda layer generated by rdk init --generate-lambda-layer",
     )
     parser.add_argument(
         "--custom-layer-name",
         required=False,
         help='[optional] To use with --generated-lambda-layer, forces the flag to look for a specific lambda-layer name. If omitted, "rdklib-layer" will be used',
     )
 
@@ -1217,17 +1215,15 @@
         if not self.args.source_identifier:
             if not self.args.runtime:
                 print("Runtime is required for 'create' command.")
                 return 1
 
             extension_mapping = {
                 "java8": ".java",
-                "python3.6": ".py",
                 "python3.6-managed": ".py",
-                "python3.6-lib": ".py",
                 "python3.7": ".py",
                 "python3.7-lib": ".py",
                 "python3.8": ".py",
                 "python3.8-lib": ".py",
                 "python3.9": ".py",
                 "python3.9-lib": ".py",
                 "nodejs6.10": ".js",
@@ -1269,15 +1265,15 @@
                         rules_dir,
                         self.args.rulename,
                         self.args.rulename + extension_mapping[self.args.runtime],
                     )
                     shutil.copyfile(src, dst)
                     f = fileinput.input(files=dst, inplace=True)
                     for line in f:
-                        if self.args.runtime in ["python3.6-lib", "python3.7-lib", "python3.8-lib", "python3.9-lib"]:
+                        if self.args.runtime in ["python3.7-lib", "python3.8-lib", "python3.9-lib"]:
                             if self.args.resource_types:
                                 applicable_resource_list = ""
                                 for resource_type in self.args.resource_types.split(","):
                                     applicable_resource_list += "'" + resource_type + "', "
                                 print(
                                     line.replace("<%RuleName%>", self.args.rulename)
                                     .replace(
@@ -2524,16 +2520,14 @@
 
         # Construct our list of rules to test.
         rule_names = self.__get_rule_list_for_command()
 
         for rule_name in rule_names:
             rule_params, rule_tags = self.__get_rule_parameters(rule_name)
             if rule_params["SourceRuntime"] not in (
-                "python3.6",
-                "python3.6-lib",
                 "python3.7",
                 "python3.7-lib",
                 "python3.8",
                 "python3.8-lib",
                 "python3.9",
                 "python3.9-lib",
             ):
@@ -3700,16 +3694,14 @@
                     print(f"[{my_session.region_name}]: Waiting for CloudFormation stack operation to complete...")
                     time.sleep(5)
 
     def __get_handler(self, rule_name, params):
         if "SourceHandler" in params:
             return params["SourceHandler"]
         if params["SourceRuntime"] in [
-            "python3.6",
-            "python3.6-lib",
             "python3.7",
             "python3.7-lib",
             "python3.8",
             "python3.8-lib",
             "python3.9",
             "python3.9-lib",
             "nodejs6.10",
@@ -3719,15 +3711,14 @@
         elif params["SourceRuntime"] in ["java8"]:
             return "com.rdk.RuleUtil::handler"
         elif params["SourceRuntime"] in ["dotnetcore1.0", "dotnetcore2.0"]:
             return "csharp7.0::Rdk.CustomConfigHandler::FunctionHandler"
 
     def __get_runtime_string(self, params):
         if params["SourceRuntime"] in [
-            "python3.6-lib",
             "python3.6-managed",
             "python3.7-lib",
             "python3.8-lib",
             "python3.9-lib",
         ]:
             runtime = params["SourceRuntime"].split("-")
             return runtime[0]
@@ -4111,15 +4102,15 @@
         config_arn = config_client.describe_config_rules(ConfigRuleNames=[rule_name])["ConfigRules"][0]["ConfigRuleArn"]
         response = config_client.tag_resource(ResourceArn=config_arn, Tags=cfn_tags)
         return response
 
     def __get_lambda_layers(self, my_session, args, params):
         layers = []
         if "SourceRuntime" in params:
-            if params["SourceRuntime"] in ["python3.6-lib", "python3.7-lib", "python3.8-lib"]:
+            if params["SourceRuntime"] in ["python3.7-lib", "python3.8-lib", "python3.9-lib"]:
                 if hasattr(args, "generated_lambda_layer") and args.generated_lambda_layer:
                     lambda_layer_version = self.__get_existing_lambda_layer(
                         my_session, layer_name=args.custom_layer_name
                     )
                     if not lambda_layer_version:
                         print(
                             f"{my_session.region_name} generated-lambda-layer flag received, but layer [{args.custom_layer_name}] not found in {my_session.region_name}. Creating one now"
@@ -4235,15 +4226,15 @@
 
         lambda_client = my_session.client("lambda")
 
         print(f"[{region}]: Publishing Lambda Layer")
         lambda_client.publish_layer_version(
             LayerName=layer_name,
             Content={"S3Bucket": bucket_name, "S3Key": layer_name},
-            CompatibleRuntimes=["python3.6", "python3.7", "python3.8"],
+            CompatibleRuntimes=["python3.7", "python3.8", "python3.9"],
         )
 
         print(f"[{region}]: Deleting temporary S3 Bucket")
         try:
             bucket = s3_resource.Bucket(bucket_name)
             bucket.objects.all().delete()
             bucket.delete()
```

### Comparing `rdk-0.8.5/rdk/template/LICENSE` & `rdk-0.9.0/rdk/template/LICENSE`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/configManagedRule.json` & `rdk-0.9.0/rdk/template/configManagedRule.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/configManagedRuleOrganization.json` & `rdk-0.9.0/rdk/template/configManagedRuleOrganization.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/configManagedRuleWithRemediation.json` & `rdk-0.9.0/rdk/template/configManagedRuleWithRemediation.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/configRule.json` & `rdk-0.9.0/rdk/template/configRule.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/configRuleOrganization.json` & `rdk-0.9.0/rdk/template/configRuleOrganization.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/deliveryPermissionsPolicy.json` & `rdk-0.9.0/rdk/template/deliveryPermissionsPolicy.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ACM_Certificate.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ACM_Certificate.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ApiGatewayV2_Api.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ApiGatewayV2_Api.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ApiGatewayV2_Stage.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ApiGatewayV2_Stage.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ApiGateway_RestApi.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ApiGateway_RestApi.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ApiGateway_Stage.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ApiGateway_Stage.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_AutoScalingGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_AutoScalingGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_LaunchConfiguration.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_LaunchConfiguration.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_ScalingPolicy.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_ScalingPolicy.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_AutoScaling_ScheduledAction.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_AutoScaling_ScheduledAction.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_CLOUDFRONT_DISTRIBUTION.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_CLOUDFRONT_DISTRIBUTION.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_CLOUDFRONT_STREAMINGDISTRIBUTION.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_CLOUDFRONT_STREAMINGDISTRIBUTION.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_CloudFormation_Stack.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_CloudFormation_Stack.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_CloudWatch_Alarm.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_CloudWatch_Alarm.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Cloudtrail_Trail.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Cloudtrail_Trail.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_CodeBuild_Project.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_CodeBuild_Project.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_CodePipeline_Pipeline.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_CodePipeline_Pipeline.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_DynamoDB_Table.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_DynamoDB_Table.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_CustomerGateway.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_CustomerGateway.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_EIP.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_EIP.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_FlowLog.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_FlowLog.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Host.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Host.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Instance.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Instance.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_InternetGateway.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_InternetGateway.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_LaunchTemplate.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_LaunchTemplate.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_NatGateway.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_NatGateway.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_NetworkAcl.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_NetworkAcl.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_NetworkInterface.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_NetworkInterface.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_RouteTable.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_RouteTable.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_SecurityGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_SecurityGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Subnet.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Subnet.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPC.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPC.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPCPeeringConnection.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPCPeeringConnection.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPNConnection.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPNConnection.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_VPNGateway.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_VPNGateway.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EC2_Volume.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EC2_Volume.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ECR_PublicRepository.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ECR_PublicRepository.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ECR_Repository.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ECR_Repository.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_EKS_Cluster.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_EKS_Cluster.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ELASTICLOADBALANCING_LOADBALANCER.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ELASTICLOADBALANCING_LOADBALANCER.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ElasticBeanstalk_Application.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ElasticBeanstalk_Application.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ElasticBeanstalk_ApplicationVersion.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ElasticBeanstalk_ApplicationVersion.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ElasticBeanstalk_Environment.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ElasticBeanstalk_Environment.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ElasticLoadBalancingV2_LoadBalancer.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ElasticLoadBalancingV2_LoadBalancer.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ElasticSearch_Domain.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ElasticSearch_Domain.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_IAM_Group.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_IAM_Group.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_IAM_Policy.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_IAM_Policy.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_IAM_Role.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_IAM_Role.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_IAM_User.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_IAM_User.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_KMS_Key.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_KMS_Key.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_LAMBDA_FUNCTION.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_LAMBDA_FUNCTION.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_NetworkFirewall_RuleGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_NetworkFirewall_RuleGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_OpenSearch_Domain.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_OpenSearch_Domain.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBCluster.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBCluster.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBClusterSnapshot.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBClusterSnapshot.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBInstance.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBInstance.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBSecurityGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBSecurityGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBSnapshot.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBSnapshot.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_DBSubnetGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_DBSubnetGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_RDS_EventSubscription.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_RDS_EventSubscription.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_Cluster.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_Cluster.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterParameterGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterParameterGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterSecurityGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterSecurityGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterSnapshot.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterSnapshot.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_ClusterSubnetGroup.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_ClusterSubnetGroup.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Redshift_EventSubscription.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Redshift_EventSubscription.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_S3_Bucket.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_S3_Bucket.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_SNS_Topic.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_SNS_Topic.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Linux.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Linux.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Windows.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_SSM_ManagedInstanceInventory_Windows.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_ShieldRegional_Protection.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_ShieldRegional_Protection.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/example_ci/AWS_Shield_Protection.json` & `rdk-0.9.0/rdk/template/example_ci/AWS_Shield_Protection.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/CustomConfigHandler.cs` & `rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/CustomConfigHandler.cs`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/RuleCode.cs` & `rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/RuleCode.cs`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/aws-lambda-tools-defaults.json` & `rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/aws-lambda-tools-defaults.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore1.0/csharp7.0.csproj` & `rdk-0.9.0/rdk/template/runtime/dotnetcore1.0/csharp7.0.csproj`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/CustomConfigHandler.cs` & `rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/CustomConfigHandler.cs`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/RuleCode.cs` & `rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/RuleCode.cs`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/aws-lambda-tools-defaults.json` & `rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/aws-lambda-tools-defaults.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/dotnetcore2.0/csharp7.0.csproj` & `rdk-0.9.0/rdk/template/runtime/dotnetcore2.0/csharp7.0.csproj`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/java8/build.gradle` & `rdk-0.9.0/rdk/template/runtime/java8/build.gradle`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/java8/src/main/java/com/rdk/RuleCode.java` & `rdk-0.9.0/rdk/template/runtime/java8/src/main/java/com/rdk/RuleCode.java`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/java8/src/main/java/com/rdk/RuleUtil.java` & `rdk-0.9.0/rdk/template/runtime/java8/src/main/java/com/rdk/RuleUtil.java`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/nodejs4.3/rule_code.js` & `rdk-0.9.0/rdk/template/runtime/nodejs4.3/rule_code.js`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.6/rule_code.py` & `rdk-0.9.0/rdk/template/runtime/python3.7/rule_code.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.6/rule_test.py` & `rdk-0.9.0/rdk/template/runtime/python3.7/rule_test.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.6-lib/rule_code.py` & `rdk-0.9.0/rdk/template/runtime/python3.7-lib/rule_code.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.6-lib/rule_test.py` & `rdk-0.9.0/rdk/template/runtime/python3.7-lib/rule_test.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.7/rule_code.py` & `rdk-0.9.0/rdk/template/runtime/python3.8/rule_code.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.7/rule_test.py` & `rdk-0.9.0/rdk/template/runtime/python3.8/rule_test.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.7-lib/rule_code.py` & `rdk-0.9.0/rdk/template/runtime/python3.8-lib/rule_code.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.7-lib/rule_test.py` & `rdk-0.9.0/rdk/template/runtime/python3.8-lib/rule_test.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.8/rule_code.py` & `rdk-0.9.0/rdk/template/runtime/python3.9/rule_code.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.8/rule_test.py` & `rdk-0.9.0/rdk/template/runtime/python3.9/rule_test.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.8-lib/rule_code.py` & `rdk-0.9.0/rdk/template/runtime/python3.9-lib/rule_code.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/runtime/python3.8-lib/rule_test.py` & `rdk-0.9.0/rdk/template/runtime/python3.9-lib/rule_test.py`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/terraform/0.11/config_rule.tf` & `rdk-0.9.0/rdk/template/terraform/0.11/config_rule.tf`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/terraform/0.11/variables.tf` & `rdk-0.9.0/rdk/template/terraform/0.11/variables.tf`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/terraform/0.12/config_rule.tf` & `rdk-0.9.0/rdk/template/terraform/0.12/config_rule.tf`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/terraform/0.12/variables.tf` & `rdk-0.9.0/rdk/template/terraform/0.12/variables.tf`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk/template/test_event_template.json` & `rdk-0.9.0/rdk/template/test_event_template.json`

 * *Files identical despite different names*

### Comparing `rdk-0.8.5/rdk.egg-info/PKG-INFO` & `rdk-0.9.0/rdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,365 +1,370 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: rdk
-Version: 0.8.5
+Version: 0.9.0
 Summary: Rule Development Kit CLI for AWS Config
 Home-page: https://github.com/awslabs/aws-config-rdk/
 Author: RDK maintainer
 Author-email: rdk-maintainers@amazon.com
 License: Apache License Version 2.0
-License-File: LICENSE
-License-File: NOTICE.txt
-
-rdk
-===
-Rule Development Kit
-We greatly appreciate feedback and bug reports at rdk-maintainers@amazon.com! You may also create an issue on this repo.
-
-The RDK is designed to support a "Compliance-as-Code" workflow that is intuitive and productive.  It abstracts away much of the undifferentiated heavy lifting associated with deploying AWS Config rules backed by custom lambda functions, and provides a streamlined develop-deploy-monitor iterative process.
-
-For complete documentation, including command reference, check out the `ReadTheDocs documentation <https://rdk.readthedocs.io/en/latest/>`_.
-
-Getting Started
-===============
-Uses python 3.6/3.7/3.8/3.9 and is installed via pip.  Requires you to have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions.  An AWS IAM Policy Document that describes the minimum necessary permissions can be found at policy/rdk-minimum-permissions.json.
-
-Under the hood, rdk uses boto3 to make API calls to AWS, so you can set your credentials any way that boto3 recognizes (options 3 through 8 here: http://boto3.readthedocs.io/en/latest/guide/configuration.html) or pass them in with the command-line parameters --profile, --region, --access-key-id, or --secret-access-key
-
-If you just want to use the RDK, go ahead and install it using pip::
-
-$ pip install rdk
-
-Alternately, if you want to see the code and/or contribute you can clone the git repo, and then from the repo directory use pip to install the package.  Use the '-e' flag to generate symlinks so that any edits you make will be reflected when you run the installed package.
-
-If you are going to author your Lambda functions using Java you will need to have Java 8 and gradle installed.  If you are going to author your Lambda functions in C# you will need to have the dotnet CLI and the .NET Core Runtime 1.08 installed.
-::
-
-  $ pip install -e .
-
-To make sure the rdk is installed correctly, running the package from the command line without any arguments should display help information.
-
-::
-
-  $ rdk
-  usage: rdk [-h] [-p PROFILE] [-k ACCESS_KEY] [-s SECRET_ACCESS_KEY]
-           [-r REGION]
-           <command> ...
-  rdk: error: the following arguments are required: <command>, <command arguments>
-
-
-Usage
-=====
-
-Configure your env
-------------------
-To use the RDK, it's recommended to create a directory that will be your working directory.  This should be committed to a source code repo, and ideally created as a python virtualenv.  In that directory, run the ``init`` command to set up your AWS Config environment.
-
-::
-
-  $ rdk init
-  Running init!
-  Creating Config bucket config-bucket-780784666283
-  Creating IAM role config-role
-  Waiting for IAM role to propagate
-  Config Service is ON
-  Config setup complete.
-  Creating Code bucket config-rule-code-bucket-780784666283ap-southeast-1
-
-Running ``init`` subsequent times will validate your AWS Config setup and re-create any S3 buckets or IAM resources that are needed.
-
-- If you have config delivery bucket already present in some other AWS account then use **--config-bucket-exists-in-another-account** as argument:::
-
-  $ rdk init --config-bucket-exists-in-another-account
-- If you have AWS Organizations/ControlTower Setup in your AWS environment then additionally, use **--control-tower** as argument:::
-
-  $ rdk init --control-tower --config-bucket-exists-in-another-account
-- If bucket for custom lambda code is already present in current account then use **--skip-code-bucket-creation** argument:::
-
-  $ rdk init --skip-code-bucket-creation
-
-- If you want rdk to create/update and upload the rdklib-layer for you, then use **--generate-lambda-layer** argument. In supported regions, rdk will deploy the layer using the Serverless Application Repository, otherwise it will build a local lambda layer archive and upload it for use:::
-
-  $ rdk init --generate-lambda-layer 
-- If you want rdk to give a custom name to the lambda layer for you, then use **--custom-layer-namer** argument. The Serverless Application Repository currently cannot be used for custom lambda layers.:::
-
-  $ rdk init --generate-lambda-layer --custom-layer-name <LAYER_NAME>
-
-Create Rules
-------------
-In your working directory, use the ``create`` command to start creating a new custom rule.  You must specify the runtime for the lambda function that will back the Rule, and you can also specify a resource type (or comma-separated list of types) that the Rule will evaluate or a maximum frequency for a periodic rule.  This will add a new directory for the rule and populate it with several files, including a skeleton of your Lambda code.
-
-::
-
-  $ rdk create MyRule --runtime python3.8 --resource-types AWS::EC2::Instance --input-parameters '{"desiredInstanceType":"t2.micro"}'
-  Running create!
-  Local Rule files created.
-
-On Windows it is necessary to escape the double-quotes when specifying input parameters, so the `--input-parameters` argument would instead look something like this::
-
-  '{\"desiredInstanceType\":\"t2.micro\"}'
-
-Note that you can create rules that use EITHER resource-types OR maximum-frequency, but not both.  We have found that rules that try to be both event-triggered as well as periodic wind up being very complicated and so we do not recommend it as a best practice.
-
-Edit Rules Locally
----------------------------
-Once you have created the rule, edit the python file in your rule directory (in the above example it would be ``MyRule/MyRule.py``, but may be deeper into the rule directory tree depending on your chosen Lambda runtime) to add whatever logic your Rule requires in the ``evaluate_compliance`` function.  You will have access to the CI that was sent by Config, as well as any parameters configured for the Config Rule.  Your function should return either a simple compliance status (one of ``COMPLIANT``, ``NONCOMPLIANT``, or ``NOT_APPLICABLE``), or if you're using the python or node runtimes you can return a JSON object with multiple evaluation responses that the RDK will send back to AWS Config.  An example would look like::
-
-  for sg in response['SecurityGroups']:
-        evaluations.append(
-        {
-                'ComplianceResourceType': 'AWS::EC2::SecurityGroup',
-                'ComplianceResourceId': sg['GroupId'],
-                'ComplianceType': 'COMPLIANT',
-                'Annotation': 'This is an important note.',
-                'OrderingTimestamp': str(datetime.datetime.now())
-        })
-
-
-    return evaluations
-
-This is necessary for periodic rules that are not triggered by any CI change (which means the CI that is passed in will be null), and also for attaching annotations to your evaluation results.
-
-If you want to see what the JSON structure of a CI looks like for creating your logic, you can use
-
-::
-
-$ rdk sample-ci <Resource Type>
-
-to output a formatted JSON document.
-
-Write and Run Unit Tests
-------------------------
-If you are writing Config Rules using either of the Python runtimes there will be a <rule name>_test.py file deployed along with your Lambda function skeleton.  This can be used to write unit tests according to the standard Python unittest framework (documented here: https://docs.python.org/3/library/unittest.html), which can be run using the `test-local` rdk command::
-
-  $ rdk test-local MyTestRule
-  Running local test!
-  Testing MyTestRule
-  Looking for tests in /Users/mborch/Code/rdk-dev/MyTestRule
-
-  ---------------------------------------------------------------------
-
-  Ran 0 tests in 0.000s
-
-  OK
-  <unittest.runner.TextTestResult run=0 errors=0 failures=0>
-
-The test file includes setup for the MagicMock library that can be used to stub boto3 API calls if your rule logic will involve making API calls to gather additional information about your AWS environment.  For some tips on how to do this, check out this blog post: https://sgillies.net/2017/10/19/mock-is-magic.html
-
-Modify Rule
------------
-If you need to change the parameters of a Config rule in your working directory you can use the ``modify`` command.  Any parameters you specify will overwrite existing values, any that you do not specify will not be changed.
-
-::
-
-  $ rdk modify MyRule --runtime python3.6 --maximum-frequency TwentyFour_Hours --input-parameters '{"desiredInstanceType":"t2.micro"}'
-  Running modify!
-  Modified Rule 'MyRule'.  Use the `deploy` command to push your changes to AWS.
-
-Again, on Windows the input parameters would look like::
-
-  '{\"desiredInstanceType\":\"t2.micro\"}'
-
-It is worth noting that until you actually call the ``deploy`` command your rule only exists in your working directory, none of the Rule commands discussed thus far actually makes changes to your account.
-
-Deploy Rule
------------
-Once you have completed your compliance validation code and set your Rule's configuration, you can deploy the Rule to your account using the ``deploy`` command.  This will zip up your code (and the other associated code files, if any) into a deployable package (or run a gradle build if you have selected the java8 runtime or run the lambda packaging step from the dotnet CLI if you have selected the dotnetcore1.0 runtime), copy that zip file to S3, and then launch or update a CloudFormation stack that defines your Config Rule, Lambda function, and the necessary permissions and IAM Roles for it to function.  Since CloudFormation does not deeply inspect Lambda code objects in S3 to construct its changeset, the ``deploy`` command will also directly update the Lambda function for any subsequent deployments to make sure code changes are propagated correctly.
-
-::
-
-  $ rdk deploy MyRule
-  Running deploy!
-  Zipping MyRule
-  Uploading MyRule
-  Creating CloudFormation Stack for MyRule
-  Waiting for CloudFormation stack operation to complete...
-  ...
-  Waiting for CloudFormation stack operation to complete...
-  Config deploy complete.
-
-The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.  If you used the --generate-lambda-layer flag in rdk init, use the --generated-lambda-layer flag for rdk deploy.
-
-Deploy Organization Rule
-------------------------
-You can also deploy the Rule to your AWS Organization using the ``deploy-organization`` command.
-For successful evaluation of custom rules in child accounts, please make sure you do one of the following:
-
-1. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume the Role attached on the Config Service and confirm that the role trusts the master account where the Lambda function is going to be deployed.
-2. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume a custom role and define an optional parameter with key as ExecutionRoleName and set the value to your custom role name; confirm that the role trusts the master account of the organization where the Lambda function will be deployed.
-
-::
-
-  $ rdk deploy-organization MyRule
-  Running deploy!
-  Zipping MyRule
-  Uploading MyRule
-  Creating CloudFormation Stack for MyRule
-  Waiting for CloudFormation stack operation to complete...
-  ...
-  Waiting for CloudFormation stack operation to complete...
-  Config deploy complete.
-
-The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.
-This command uses 'PutOrganizationConfigRule' API for the rule deployment. If a new account joins an organization, the rule is deployed to that account. When an account leaves an organization, the rule is removed. Deployment of existing organizational AWS Config Rules will only be retried for 7 hours after an account is added to your organization if a recorder is not available. You are expected to create a recorder if one doesn't exist within 7 hours of adding an account to your organization.
-
-View Logs For Deployed Rule
----------------------------
-Once the Rule has been deployed to AWS you can get the CloudWatch logs associated with your lambda function using the ``logs`` command.
-
-::
-
-  $ rdk logs MyRule -n 5
-  2017-11-15 22:59:33 - START RequestId: 96e7639a-ca15-11e7-95a2-b1521890638d Version: $LATEST
-  2017-11-15 23:41:13 - REPORT RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda    Duration: 0.50 ms    Billed Duration: 100 ms     Memory Size: 256 MB
-                            Max Memory Used: 36 MB
-  2017-11-15 23:41:13 - END RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda
-  2017-11-15 23:41:13 - Default RDK utility class does not yet support Scheduled Notifications.
-  2017-11-15 23:41:13 - START RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda Version: $LATEST
-
-You can use the ``-n`` and ``-f`` command line flags just like the UNIX ``tail`` command to view a larger number of log events and to continuously poll for new events.  The latter option can be useful in conjunction with manually initiating Config Evaluations for your deploy Config Rule to make sure it is behaving as expected.
-
-
-
-Running the tests
-=================
-
-The `testing` directory contains scripts and buildspec files that I use to run basic functionality tests across a variety of CLI environments (currently Ubuntu linux running python 3.6/3.7/3.8/3.9, and Windows Server running python3.6).  If there is interest I can release a CloudFormation template that could be used to build the test environment, let me know if this is something you want!
-
-
-Advanced Features
-=================
-Cross-Account Deployments
--------------------------
-Features have been added to the RDK to facilitate the cross-account deployment pattern that enterprise customers have standardized on for custom Config Rules. A cross-account architecture is one in which the Lambda functions are deployed to a single central "Compliance" account (which may be the same as a central "Security" account), and the Config Rules are deployed to any number of "Satellite" accounts that are used by other teams or departments.  This gives the compliance team confidence that their Rule logic cannot be tampered with and makes it much easier for them to modify rule logic without having to go through a complex deployment process to potentially hundreds of AWS accounts.  The cross-account pattern uses two advanced RDK features - functions-only deployments and the `create-rule-template` command.
-
-**Function-Only Deployment**
-
-By using the `-f` or `--functions-only` flag on the `deploy` command the RDK will deploy only the necessary Lambda Functions, Lambda Execution Role, and Lambda Permissions to the account specified by the execution credentials.  It accomplishes this by batching up all of the Lambda function CloudFormation snippets for the selected Rule(s) into a single dynamically generated template and deploy that CloudFormation template.  One consequence of this is that subsequent deployments that specify a different set of Rules for the same stack name will update that CloudFormation stack, and any Rules that were included in the first deployment but not in the second will be removed.  You can use the `--stack-name` parameter to override the default CloudFormation stack name if you need to manage different subsets of your Lambda Functions independently.  The intended usage is to deploy the functions for all of the Config rules in the Security/Compliance account, which can be done simply by using `rdk deploy -f --all` from your working directory.
-
-**`create-rule-template` command**
-
-This command generates a CloudFormation template that defines the AWS Config rules themselves, along with the Config Role, Config data bucket, Configuration Recorder, and Delivery channel necessary for the Config rules to work in a satellite account.  You must specify the file name for the generated template using the `--output-file` or `o` command line flags.  The generated template takes a single parameter of the AccountID of the central compliance account that contains the Lambda functions that will back your custom Config Rules.  The generated template can be deployed in the desired satellite accounts through any of the means that you can deploy any other CloudFormation template, including the console, the CLI, as a CodePipeline task, or using StackSets.  The `create-rule-template` command takes all of the standard arguments for selecting Rules to include in the generated template, including lists of individual Rule names, an `--all` flag, or using the RuleSets feature described below.
-
-::
-
-  $ rdk create-rule-template -o remote-rule-template.json --all
-  Generating CloudFormation template!
-  CloudFormation template written to remote-rule-template.json
-
-
-Disable the supported resource types check
-------------------------------------------
-It is now possible to define a resource type that is not yet supported by rdk. To disable the supported resource check use the optional flag '--skip-supported-resource-check' during the create command.
-
-::
-
-  $ rdk create MyRule --runtime python3.8 --resource-types AWS::New::ResourceType --skip-supported-resource-check
-  'AWS::New::ResourceType' not found in list of accepted resource types.
-  Skip-Supported-Resource-Check Flag set (--skip-supported-resource-check), ignoring missing resource type error.
-  Running create!
-  Local Rule files created.
-
-Custom Lambda Function Name
----------------------------
-As of version 0.7.14, instead of defaulting the lambda function names to 'RDK-Rule-Function-<RULE_NAME>' it is possible to customize the name for the Lambda function to any 64 characters string as per Lambda's naming standards using the optional '--custom-lambda-name' flag while performing rdk create. This opens up new features like :
-
-1. Longer config rule name.
-2. Custom lambda function naming as per personal or enterprise standards.
-
-::
-
-  $ rdk create MyLongerRuleName --runtime python3.8 --resource-types AWS::EC2::Instance --custom-lambda-name custom-prefix-for-MyLongerRuleName
-  Running create!
-  Local Rule files created.
-
-The above example would create files with config rule name as 'MyLongerRuleName' and lambda function with the name 'custom-prefix-for-MyLongerRuleName' instead of 'RDK-Rule-Function-MyLongerRuleName'
-
-RuleSets
---------
-New as of version 0.3.11, it is possible to add RuleSet tags to rules that can be used to deploy and test groups of rules together.  Rules can belong to multiple RuleSets, and RuleSet membership is stored only in the parameters.json metadata.  The `deploy`, `create-rule-template`, and `test-local` commands are RuleSet-aware such that a RuleSet can be passed in as the target instead of `--all` or a specific named Rule.
-
-A comma-delimited list of RuleSets can be added to a Rule when you create it (using the `--rulesets` flag), as part of a `modify` command, or using new `ruleset` subcommands to add or remove individual rules from a RuleSet.
-
-Running `rdk rulesets list` will display a list of the RuleSets currently defined across all of the Rules in the working directory
-
-::
-
-  rdk-dev $ rdk rulesets list
-  RuleSets:  AnotherRuleSet MyNewSet
-
-Naming a specific RuleSet will list all of the Rules that are part of that RuleSet.
-
-::
-
-  rdk-dev $ rdk rulesets list AnotherRuleSet
-  Rules in AnotherRuleSet :  RSTest
-
-Rules can be added to or removed from RuleSets using the `add` and `remove` subcommands:
-
-::
-
-  rdk-dev $ rdk rulesets add MyNewSet RSTest
-  RSTest added to RuleSet MyNewSet
-
-  rdk-dev $ rdk rulesets remove AnotherRuleSet RSTest
-  RSTest removed from RuleSet AnotherRuleSet
-
-RuleSets are a convenient way to maintain a single repository of Config Rules that may need to have subsets of them deployed to different environments.  For example your development environment may contain some of the Rules that you run in Production but not all of them; RuleSets gives you a way to identify and selectively deploy the appropriate Rules to each environment.
-
-Managed Rules
--------------
-The RDK is able to deploy AWS Managed Rules.
-
-To do so, create a rule using "rdk create" and provide a valid SourceIdentifier via the --source-identifier CLI option. The list of Managed Rules can be found here: https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html, and note that the Identifier can be obtained by replacing the dashes with underscores and using all capitals (for example, the "guardduty-enabled-centralized" rule has the SourceIdentifier "GUARDDUTY_ENABLED_CENTRALIZED").  Just like custom Rules you will need to specify source events and/or a maximum evaluation frequency, and also pass in any Rule parameters.  The resulting Rule directory will contain only the parameters.json file, but using `rdk deploy` or `rdk create-rule-template` can be used to deploy the Managed Rule like any other Custom Rule.
-
-Deploying Rules Across Multiple Regions
----------------------------------------
-The RDK is able to run init/deploy/undeploy across multiple regions with a `rdk -f <region file> -t <region set>`
-
-If no region group is specified, rdk will deploy to the `default` region set
-
-To create a sample starter region group, run `rdk create-region-set` to specify the filename, add the `-o <region set output file name>` this will create a region set with the following tests and regions `"default":["us-east-1","us-west-1","eu-north-1","ap-east-1"],"aws-cn-region-set":["cn-north-1","cn-northwest-1"]`
-
-Using RDK to Generate a Lambda Layer in a region (Python3)
-----------------------------------------------------------
-By default `rdk init --generate-lambda-layer` will generate an rdklib lambda layer while running init in whatever region it is run, to force re-generation of the layer, run `rdk init --generate-lambda-layer` again over a region
-
-To use this generated lambda layer, add the flag `--generated-lambda-layer` when running `rdk deploy`. For example: `rdk -f regions.yaml deploy LP3_TestRule_P36_lib --generated-lambda-layer`
-
-If you created layer with a custom name (by running `rdk init --custom-lambda-layer`, add a similar `custom-lambda-layer` flag when running deploy.
-
-Contributing
-============
-
-email us at rdk-maintainers@amazon.com if you have any questions. We are happy to help and discuss.
-
-Contacts
-========
-* **Ricky Chau** - `rickychau2780 <https://github.com/rickychau2780>`_ - *current maintainer*
-* **Jarrett Andrulis** - `jarrettandrulis <https://github.com/jarrettandrulis>`_ - *current maintainer*
-* **Julio Delgado Jr** - `tekdj7 <https://github.com/tekdj7>`_ - *current maintainer*
-* **Sandeep Batchu** - `batchus <https://github.com/batchus>`_ - *current maintainer*
-
-Past Contributors
-=================
-* **Michael Borchert** - *Orignal Python version*
-* **Jonathan Rault** - *Orignal Design, testing, feedback*
-* **Greg Kim and Chris Gutierrez** - *Initial work and CI definitions*
-* **Henry Huang** - *Original CFN templates and other code*
-* **Santosh Kumar** - *maintainer*
-* **Jose Obando** - *maintainer*
-
-License
-=======
-
-This project is licensed under the Apache 2.0 License
-
-Acknowledgments
-===============
-
-* the boto3 team makes all of this magic possible.
-
-
-Link
-====
-
-* to view example of rules built with the RDK: https://github.com/awslabs/aws-config-rules/tree/master/python
+Description: rdk
+        ===
+        Rule Development Kit
+        
+        We greatly appreciate feedback and bug reports at rdk-maintainers@amazon.com! You may also create an issue on this repo.
+        
+        The RDK is designed to support a "Compliance-as-Code" workflow that is intuitive and productive.  It abstracts away much of the undifferentiated heavy lifting associated with deploying AWS Config rules backed by custom lambda functions, and provides a streamlined develop-deploy-monitor iterative process.
+        
+        For complete documentation, including command reference, check out the `ReadTheDocs documentation <https://rdk.readthedocs.io/en/latest/>`_.
+        
+        Getting Started
+        ===============
+        Uses python 3.7/3.8/3.9 and is installed via pip.  Requires you to have an AWS account and sufficient permissions to manage the Config service, and to create S3 Buckets, Roles, and Lambda Functions.  An AWS IAM Policy Document that describes the minimum necessary permissions can be found at policy/rdk-minimum-permissions.json.
+        
+        Under the hood, rdk uses boto3 to make API calls to AWS, so you can set your credentials any way that boto3 recognizes (options 3 through 8 here: http://boto3.readthedocs.io/en/latest/guide/configuration.html) or pass them in with the command-line parameters --profile, --region, --access-key-id, or --secret-access-key
+        
+        If you just want to use the RDK, go ahead and install it using pip::
+        
+        $ pip install rdk
+        
+        Alternately, if you want to see the code and/or contribute you can clone the git repo, and then from the repo directory use pip to install the package.  Use the '-e' flag to generate symlinks so that any edits you make will be reflected when you run the installed package.
+        
+        If you are going to author your Lambda functions using Java you will need to have Java 8 and gradle installed.  If you are going to author your Lambda functions in C# you will need to have the dotnet CLI and the .NET Core Runtime 1.08 installed.
+        ::
+        
+          $ pip install -e .
+        
+        To make sure the rdk is installed correctly, running the package from the command line without any arguments should display help information.
+        
+        ::
+        
+          $ rdk
+          usage: rdk [-h] [-p PROFILE] [-k ACCESS_KEY] [-s SECRET_ACCESS_KEY]
+                   [-r REGION]
+                   <command> ...
+          rdk: error: the following arguments are required: <command>, <command arguments>
+        
+        
+        Usage
+        =====
+        
+        Configure your env
+        ------------------
+        To use the RDK, it's recommended to create a directory that will be your working directory.  This should be committed to a source code repo, and ideally created as a python virtualenv.  In that directory, run the ``init`` command to set up your AWS Config environment.
+        
+        ::
+        
+          $ rdk init
+          Running init!
+          Creating Config bucket config-bucket-780784666283
+          Creating IAM role config-role
+          Waiting for IAM role to propagate
+          Config Service is ON
+          Config setup complete.
+          Creating Code bucket config-rule-code-bucket-780784666283ap-southeast-1
+        
+        Running ``init`` subsequent times will validate your AWS Config setup and re-create any S3 buckets or IAM resources that are needed.
+        
+        - If you have config delivery bucket already present in some other AWS account then use **--config-bucket-exists-in-another-account** as argument:::
+        
+          $ rdk init --config-bucket-exists-in-another-account
+        - If you have AWS Organizations/ControlTower Setup in your AWS environment then additionally, use **--control-tower** as argument:::
+        
+          $ rdk init --control-tower --config-bucket-exists-in-another-account
+        - If bucket for custom lambda code is already present in current account then use **--skip-code-bucket-creation** argument:::
+        
+          $ rdk init --skip-code-bucket-creation
+        
+        - If you want rdk to create/update and upload the rdklib-layer for you, then use **--generate-lambda-layer** argument. In supported regions, rdk will deploy the layer using the Serverless Application Repository, otherwise it will build a local lambda layer archive and upload it for use:::
+        
+          $ rdk init --generate-lambda-layer 
+        - If you want rdk to give a custom name to the lambda layer for you, then use **--custom-layer-namer** argument. The Serverless Application Repository currently cannot be used for custom lambda layers.:::
+        
+          $ rdk init --generate-lambda-layer --custom-layer-name <LAYER_NAME>
+        
+        Create Rules
+        ------------
+        In your working directory, use the ``create`` command to start creating a new custom rule.  You must specify the runtime for the lambda function that will back the Rule, and you can also specify a resource type (or comma-separated list of types) that the Rule will evaluate or a maximum frequency for a periodic rule.  This will add a new directory for the rule and populate it with several files, including a skeleton of your Lambda code.
+        
+        ::
+        
+          $ rdk create MyRule --runtime python3.8 --resource-types AWS::EC2::Instance --input-parameters '{"desiredInstanceType":"t2.micro"}'
+          Running create!
+          Local Rule files created.
+        
+        On Windows it is necessary to escape the double-quotes when specifying input parameters, so the `--input-parameters` argument would instead look something like this::
+        
+          '{\"desiredInstanceType\":\"t2.micro\"}'
+        
+        Note that you can create rules that use EITHER resource-types OR maximum-frequency, but not both.  We have found that rules that try to be both event-triggered as well as periodic wind up being very complicated and so we do not recommend it as a best practice.
+        
+        Edit Rules Locally
+        ---------------------------
+        Once you have created the rule, edit the python file in your rule directory (in the above example it would be ``MyRule/MyRule.py``, but may be deeper into the rule directory tree depending on your chosen Lambda runtime) to add whatever logic your Rule requires in the ``evaluate_compliance`` function.  You will have access to the CI that was sent by Config, as well as any parameters configured for the Config Rule.  Your function should return either a simple compliance status (one of ``COMPLIANT``, ``NONCOMPLIANT``, or ``NOT_APPLICABLE``), or if you're using the python or node runtimes you can return a JSON object with multiple evaluation responses that the RDK will send back to AWS Config.  An example would look like::
+        
+          for sg in response['SecurityGroups']:
+                evaluations.append(
+                {
+                        'ComplianceResourceType': 'AWS::EC2::SecurityGroup',
+                        'ComplianceResourceId': sg['GroupId'],
+                        'ComplianceType': 'COMPLIANT',
+                        'Annotation': 'This is an important note.',
+                        'OrderingTimestamp': str(datetime.datetime.now())
+                })
+        
+        
+            return evaluations
+        
+        This is necessary for periodic rules that are not triggered by any CI change (which means the CI that is passed in will be null), and also for attaching annotations to your evaluation results.
+        
+        If you want to see what the JSON structure of a CI looks like for creating your logic, you can use
+        
+        ::
+        
+        $ rdk sample-ci <Resource Type>
+        
+        to output a formatted JSON document.
+        
+        Write and Run Unit Tests
+        ------------------------
+        If you are writing Config Rules using either of the Python runtimes there will be a <rule name>_test.py file deployed along with your Lambda function skeleton.  This can be used to write unit tests according to the standard Python unittest framework (documented here: https://docs.python.org/3/library/unittest.html), which can be run using the `test-local` rdk command::
+        
+          $ rdk test-local MyTestRule
+          Running local test!
+          Testing MyTestRule
+          Looking for tests in /Users/mborch/Code/rdk-dev/MyTestRule
+        
+          ---------------------------------------------------------------------
+        
+          Ran 0 tests in 0.000s
+        
+          OK
+          <unittest.runner.TextTestResult run=0 errors=0 failures=0>
+        
+        The test file includes setup for the MagicMock library that can be used to stub boto3 API calls if your rule logic will involve making API calls to gather additional information about your AWS environment.  For some tips on how to do this, check out this blog post: https://sgillies.net/2017/10/19/mock-is-magic.html
+        
+        Modify Rule
+        -----------
+        If you need to change the parameters of a Config rule in your working directory you can use the ``modify`` command.  Any parameters you specify will overwrite existing values, any that you do not specify will not be changed.
+        
+        ::
+        
+          $ rdk modify MyRule --runtime python3.9 --maximum-frequency TwentyFour_Hours --input-parameters '{"desiredInstanceType":"t2.micro"}'
+          Running modify!
+          Modified Rule 'MyRule'.  Use the `deploy` command to push your changes to AWS.
+        
+        Again, on Windows the input parameters would look like::
+        
+          '{\"desiredInstanceType\":\"t2.micro\"}'
+        
+        It is worth noting that until you actually call the ``deploy`` command your rule only exists in your working directory, none of the Rule commands discussed thus far actually makes changes to your account.
+        
+        Deploy Rule
+        -----------
+        Once you have completed your compliance validation code and set your Rule's configuration, you can deploy the Rule to your account using the ``deploy`` command.  This will zip up your code (and the other associated code files, if any) into a deployable package (or run a gradle build if you have selected the java8 runtime or run the lambda packaging step from the dotnet CLI if you have selected the dotnetcore1.0 runtime), copy that zip file to S3, and then launch or update a CloudFormation stack that defines your Config Rule, Lambda function, and the necessary permissions and IAM Roles for it to function.  Since CloudFormation does not deeply inspect Lambda code objects in S3 to construct its changeset, the ``deploy`` command will also directly update the Lambda function for any subsequent deployments to make sure code changes are propagated correctly.
+        
+        ::
+        
+          $ rdk deploy MyRule
+          Running deploy!
+          Zipping MyRule
+          Uploading MyRule
+          Creating CloudFormation Stack for MyRule
+          Waiting for CloudFormation stack operation to complete...
+          ...
+          Waiting for CloudFormation stack operation to complete...
+          Config deploy complete.
+        
+        The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.  If you used the --generate-lambda-layer flag in rdk init, use the --generated-lambda-layer flag for rdk deploy.
+        
+        Deploy Organization Rule
+        ------------------------
+        You can also deploy the Rule to your AWS Organization using the ``deploy-organization`` command.
+        For successful evaluation of custom rules in child accounts, please make sure you do one of the following:
+        
+        1. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume the Role attached on the Config Service and confirm that the role trusts the master account where the Lambda function is going to be deployed.
+        2. Set ASSUME_ROLE_MODE in Lambda code to True, to get the lambda to assume a custom role and define an optional parameter with key as ExecutionRoleName and set the value to your custom role name; confirm that the role trusts the master account of the organization where the Lambda function will be deployed.
+        
+        ::
+        
+          $ rdk deploy-organization MyRule
+          Running deploy!
+          Zipping MyRule
+          Uploading MyRule
+          Creating CloudFormation Stack for MyRule
+          Waiting for CloudFormation stack operation to complete...
+          ...
+          Waiting for CloudFormation stack operation to complete...
+          Config deploy complete.
+        
+        The exact output will vary depending on Lambda runtime.  You can use the --all flag to deploy all of the rules in your working directory.
+        This command uses 'PutOrganizationConfigRule' API for the rule deployment. If a new account joins an organization, the rule is deployed to that account. When an account leaves an organization, the rule is removed. Deployment of existing organizational AWS Config Rules will only be retried for 7 hours after an account is added to your organization if a recorder is not available. You are expected to create a recorder if one doesn't exist within 7 hours of adding an account to your organization.
+        
+        View Logs For Deployed Rule
+        ---------------------------
+        Once the Rule has been deployed to AWS you can get the CloudWatch logs associated with your lambda function using the ``logs`` command.
+        
+        ::
+        
+          $ rdk logs MyRule -n 5
+          2017-11-15 22:59:33 - START RequestId: 96e7639a-ca15-11e7-95a2-b1521890638d Version: $LATEST
+          2017-11-15 23:41:13 - REPORT RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda    Duration: 0.50 ms    Billed Duration: 100 ms     Memory Size: 256 MB
+                                    Max Memory Used: 36 MB
+          2017-11-15 23:41:13 - END RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda
+          2017-11-15 23:41:13 - Default RDK utility class does not yet support Scheduled Notifications.
+          2017-11-15 23:41:13 - START RequestId: 68e0304f-ca1b-11e7-b735-81ebae95acda Version: $LATEST
+        
+        You can use the ``-n`` and ``-f`` command line flags just like the UNIX ``tail`` command to view a larger number of log events and to continuously poll for new events.  The latter option can be useful in conjunction with manually initiating Config Evaluations for your deploy Config Rule to make sure it is behaving as expected.
+        
+        
+        
+        Running the tests
+        =================
+        
+        The `testing` directory contains scripts and buildspec files that I use to run basic functionality tests across a variety of CLI environments (currently Ubuntu linux running python 3.7/3.8/3.9, and Windows Server running python3.9).  If there is interest I can release a CloudFormation template that could be used to build the test environment, let me know if this is something you want!
+        
+        
+        Advanced Features
+        =================
+        Cross-Account Deployments
+        -------------------------
+        Features have been added to the RDK to facilitate the cross-account deployment pattern that enterprise customers have standardized on for custom Config Rules. A cross-account architecture is one in which the Lambda functions are deployed to a single central "Compliance" account (which may be the same as a central "Security" account), and the Config Rules are deployed to any number of "Satellite" accounts that are used by other teams or departments.  This gives the compliance team confidence that their Rule logic cannot be tampered with and makes it much easier for them to modify rule logic without having to go through a complex deployment process to potentially hundreds of AWS accounts.  The cross-account pattern uses two advanced RDK features - functions-only deployments and the `create-rule-template` command.
+        
+        **Function-Only Deployment**
+        
+        By using the `-f` or `--functions-only` flag on the `deploy` command the RDK will deploy only the necessary Lambda Functions, Lambda Execution Role, and Lambda Permissions to the account specified by the execution credentials.  It accomplishes this by batching up all of the Lambda function CloudFormation snippets for the selected Rule(s) into a single dynamically generated template and deploy that CloudFormation template.  One consequence of this is that subsequent deployments that specify a different set of Rules for the same stack name will update that CloudFormation stack, and any Rules that were included in the first deployment but not in the second will be removed.  You can use the `--stack-name` parameter to override the default CloudFormation stack name if you need to manage different subsets of your Lambda Functions independently.  The intended usage is to deploy the functions for all of the Config rules in the Security/Compliance account, which can be done simply by using `rdk deploy -f --all` from your working directory.
+        
+        **`create-rule-template` command**
+        
+        This command generates a CloudFormation template that defines the AWS Config rules themselves, along with the Config Role, Config data bucket, Configuration Recorder, and Delivery channel necessary for the Config rules to work in a satellite account.  You must specify the file name for the generated template using the `--output-file` or `o` command line flags.  The generated template takes a single parameter of the AccountID of the central compliance account that contains the Lambda functions that will back your custom Config Rules.  The generated template can be deployed in the desired satellite accounts through any of the means that you can deploy any other CloudFormation template, including the console, the CLI, as a CodePipeline task, or using StackSets.  The `create-rule-template` command takes all of the standard arguments for selecting Rules to include in the generated template, including lists of individual Rule names, an `--all` flag, or using the RuleSets feature described below.
+        
+        ::
+        
+          $ rdk create-rule-template -o remote-rule-template.json --all
+          Generating CloudFormation template!
+          CloudFormation template written to remote-rule-template.json
+        
+        
+        Disable the supported resource types check
+        ------------------------------------------
+        It is now possible to define a resource type that is not yet supported by rdk. To disable the supported resource check use the optional flag '--skip-supported-resource-check' during the create command.
+        
+        ::
+        
+          $ rdk create MyRule --runtime python3.8 --resource-types AWS::New::ResourceType --skip-supported-resource-check
+          'AWS::New::ResourceType' not found in list of accepted resource types.
+          Skip-Supported-Resource-Check Flag set (--skip-supported-resource-check), ignoring missing resource type error.
+          Running create!
+          Local Rule files created.
+        
+        Custom Lambda Function Name
+        ---------------------------
+        As of version 0.7.14, instead of defaulting the lambda function names to 'RDK-Rule-Function-<RULE_NAME>' it is possible to customize the name for the Lambda function to any 64 characters string as per Lambda's naming standards using the optional '--custom-lambda-name' flag while performing rdk create. This opens up new features like :
+        
+        1. Longer config rule name.
+        2. Custom lambda function naming as per personal or enterprise standards.
+        
+        ::
+        
+          $ rdk create MyLongerRuleName --runtime python3.8 --resource-types AWS::EC2::Instance --custom-lambda-name custom-prefix-for-MyLongerRuleName
+          Running create!
+          Local Rule files created.
+        
+        The above example would create files with config rule name as 'MyLongerRuleName' and lambda function with the name 'custom-prefix-for-MyLongerRuleName' instead of 'RDK-Rule-Function-MyLongerRuleName'
+        
+        RuleSets
+        --------
+        New as of version 0.3.11, it is possible to add RuleSet tags to rules that can be used to deploy and test groups of rules together.  Rules can belong to multiple RuleSets, and RuleSet membership is stored only in the parameters.json metadata.  The `deploy`, `create-rule-template`, and `test-local` commands are RuleSet-aware such that a RuleSet can be passed in as the target instead of `--all` or a specific named Rule.
+        
+        A comma-delimited list of RuleSets can be added to a Rule when you create it (using the `--rulesets` flag), as part of a `modify` command, or using new `ruleset` subcommands to add or remove individual rules from a RuleSet.
+        
+        Running `rdk rulesets list` will display a list of the RuleSets currently defined across all of the Rules in the working directory
+        
+        ::
+        
+          rdk-dev $ rdk rulesets list
+          RuleSets:  AnotherRuleSet MyNewSet
+        
+        Naming a specific RuleSet will list all of the Rules that are part of that RuleSet.
+        
+        ::
+        
+          rdk-dev $ rdk rulesets list AnotherRuleSet
+          Rules in AnotherRuleSet :  RSTest
+        
+        Rules can be added to or removed from RuleSets using the `add` and `remove` subcommands:
+        
+        ::
+        
+          rdk-dev $ rdk rulesets add MyNewSet RSTest
+          RSTest added to RuleSet MyNewSet
+        
+          rdk-dev $ rdk rulesets remove AnotherRuleSet RSTest
+          RSTest removed from RuleSet AnotherRuleSet
+        
+        RuleSets are a convenient way to maintain a single repository of Config Rules that may need to have subsets of them deployed to different environments.  For example your development environment may contain some of the Rules that you run in Production but not all of them; RuleSets gives you a way to identify and selectively deploy the appropriate Rules to each environment.
+        
+        Managed Rules
+        -------------
+        The RDK is able to deploy AWS Managed Rules.
+        
+        To do so, create a rule using "rdk create" and provide a valid SourceIdentifier via the --source-identifier CLI option. The list of Managed Rules can be found here: https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html, and note that the Identifier can be obtained by replacing the dashes with underscores and using all capitals (for example, the "guardduty-enabled-centralized" rule has the SourceIdentifier "GUARDDUTY_ENABLED_CENTRALIZED").  Just like custom Rules you will need to specify source events and/or a maximum evaluation frequency, and also pass in any Rule parameters.  The resulting Rule directory will contain only the parameters.json file, but using `rdk deploy` or `rdk create-rule-template` can be used to deploy the Managed Rule like any other Custom Rule.
+        
+        Deploying Rules Across Multiple Regions
+        ---------------------------------------
+        The RDK is able to run init/deploy/undeploy across multiple regions with a `rdk -f <region file> -t <region set>`
+        
+        If no region group is specified, rdk will deploy to the `default` region set
+        
+        To create a sample starter region group, run `rdk create-region-set` to specify the filename, add the `-o <region set output file name>` this will create a region set with the following tests and regions `"default":["us-east-1","us-west-1","eu-north-1","ap-east-1"],"aws-cn-region-set":["cn-north-1","cn-northwest-1"]`
+        
+        Using RDK to Generate a Lambda Layer in a region (Python3)
+        ----------------------------------------------------------
+        By default `rdk init --generate-lambda-layer` will generate an rdklib lambda layer while running init in whatever region it is run, to force re-generation of the layer, run `rdk init --generate-lambda-layer` again over a region
+        
+        To use this generated lambda layer, add the flag `--generated-lambda-layer` when running `rdk deploy`. For example: `rdk -f regions.yaml deploy LP3_TestRule_P39_lib --generated-lambda-layer`
+        
+        If you created layer with a custom name (by running `rdk init --custom-lambda-layer`, add a similar `custom-lambda-layer` flag when running deploy.
+        
+        Contributing
+        ============
+        
+        email us at rdk-maintainers@amazon.com if you have any questions. We are happy to help and discuss.
+        
+        Contacts
+        ========
+        * **Ricky Chau** - `rickychau2780 <https://github.com/rickychau2780>`_ - *current maintainer*
+        * **Jarrett Andrulis** - `jarrettandrulis <https://github.com/jarrettandrulis>`_ - *current maintainer*
+        * **Julio Delgado Jr** - `tekdj7 <https://github.com/tekdj7>`_ - *current maintainer*
+        * **Sandeep Batchu** - `batchus <https://github.com/batchus>`_ - *current maintainer*
+        
+        Past Contributors
+        =================
+        * **Michael Borchert** - *Orignal Python version*
+        * **Jonathan Rault** - *Orignal Design, testing, feedback*
+        * **Greg Kim and Chris Gutierrez** - *Initial work and CI definitions*
+        * **Henry Huang** - *Original CFN templates and other code*
+        * **Santosh Kumar** - *maintainer*
+        * **Jose Obando** - *maintainer*
+        
+        License
+        =======
+        
+        This project is licensed under the Apache 2.0 License
+        
+        Acknowledgments
+        ===============
+        
+        * the boto3 team makes all of this magic possible.
+        
+        
+        Link
+        ====
+        
+        * to view example of rules built with the RDK: https://github.com/awslabs/aws-config-rules/tree/master/python
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rdk-0.8.5/rdk.egg-info/SOURCES.txt` & `rdk-0.9.0/rdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -103,18 +103,14 @@
 rdk/template/runtime/dotnetcore2.0/aws-lambda-tools-defaults.json
 rdk/template/runtime/dotnetcore2.0/csharp7.0.csproj
 rdk/template/runtime/java8/build.gradle
 rdk/template/runtime/java8/jars/readme.txt
 rdk/template/runtime/java8/src/main/java/com/rdk/RuleCode.java
 rdk/template/runtime/java8/src/main/java/com/rdk/RuleUtil.java
 rdk/template/runtime/nodejs4.3/rule_code.js
-rdk/template/runtime/python3.6/rule_code.py
-rdk/template/runtime/python3.6/rule_test.py
-rdk/template/runtime/python3.6-lib/rule_code.py
-rdk/template/runtime/python3.6-lib/rule_test.py
 rdk/template/runtime/python3.7/rule_code.py
 rdk/template/runtime/python3.7/rule_test.py
 rdk/template/runtime/python3.7-lib/rule_code.py
 rdk/template/runtime/python3.7-lib/rule_test.py
 rdk/template/runtime/python3.8/rule_code.py
 rdk/template/runtime/python3.8/rule_test.py
 rdk/template/runtime/python3.8-lib/rule_code.py
```

### Comparing `rdk-0.8.5/setup.py` & `rdk-0.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,14 +26,21 @@
     author_email="rdk-maintainers@amazon.com",
     license="Apache License Version 2.0",
     packages=["rdk"],
     install_requires=[
         "boto3",
         "pyyaml",
     ],
+    classifiers=[
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+    ],
     entry_points={
         "console_scripts": [
             "rdk=rdk.cli:main",
         ],
     },
     zip_safe=False,
     include_package_data=True,
```

