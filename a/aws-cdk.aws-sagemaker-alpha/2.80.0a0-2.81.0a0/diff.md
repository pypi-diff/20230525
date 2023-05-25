# Comparing `tmp/aws-cdk.aws-sagemaker-alpha-2.80.0a0.tar.gz` & `tmp/aws-cdk.aws-sagemaker-alpha-2.81.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src119495194/src/packages/@aws-cdk/aws-sagemaker-alpha/dist/python/aws-cdk.aws-sagemaker-alpha-2.80.0a0.tar", last modified: Fri May 19 21:06:04 2023, max compression
+gzip compressed data, was "/codebuild/output/src215479335/src/packages/@aws-cdk/aws-sagemaker-alpha/dist/python/aws-cdk.aws-sagemaker-alpha-2.81.0a0.tar", last modified: Thu May 25 16:41:57 2023, max compression
```

## Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0.tar` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9936 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8931 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1884 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/
--rw-r--r--   0 root         (0) root         (0)   239805 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92080 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.80.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:05:57.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9936 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 21:06:04.000000 aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8931 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/
+-rw-r--r--   0 root         (0) root         (0)   240804 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92124 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.81.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:41:47.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-05-25 16:41:56.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-25 16:41:57.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 16:41:56.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-25 16:41:56.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 16:41:56.000000 aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/LICENSE` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/PKG-INFO` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-sagemaker-alpha
-Version: 2.80.0a0
+Version: 2.81.0a0
 Summary: The CDK Construct Library for AWS::SageMaker
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/README.md` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/setup.py` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-sagemaker-alpha",
-    "version": "2.80.0.a0",
+    "version": "2.81.0.a0",
     "description": "The CDK Construct Library for AWS::SageMaker",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_cdk.aws_sagemaker_alpha",
         "aws_cdk.aws_sagemaker_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_sagemaker_alpha._jsii": [
-            "aws-sagemaker-alpha@2.80.0-alpha.0.jsii.tgz"
+            "aws-sagemaker-alpha@2.81.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_sagemaker_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.80.0",
+        "aws-cdk-lib==2.81.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,14 +556,15 @@
 
     @jsii.member(jsii_name="fromAsset")
     @builtins.classmethod
     def from_asset(
         cls,
         directory: builtins.str,
         *,
+        asset_name: typing.Optional[builtins.str] = None,
         build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         build_secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         cache_from: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]]] = None,
         cache_to: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]] = None,
         file: typing.Optional[builtins.str] = None,
         invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
@@ -574,14 +575,15 @@
         exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
         follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
         ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
     ) -> "ContainerImage":
         '''(experimental) Reference an image that's constructed directly from sources on disk.
 
         :param directory: The directory where the Dockerfile is stored.
+        :param asset_name: Unique identifier of the docker image asset and its potential revisions. Required if using AppScopedStagingSynthesizer. Default: - no asset name
         :param build_args: Build args to pass to the ``docker build`` command. Since Docker build arguments are resolved before deployment, keys and values cannot refer to unresolved tokens (such as ``lambda.functionArn`` or ``queue.queueUrl``). Default: - no build args are passed
         :param build_secrets: Build secrets. Docker BuildKit must be enabled to use build secrets. Default: - no build secrets
         :param cache_from: Cache from options to pass to the ``docker build`` command. Default: - no cache from options are passed to the build command
         :param cache_to: Cache to options to pass to the ``docker build`` command. Default: - no cache to options are passed to the build command
         :param file: Path to the Dockerfile (relative to the directory). Default: 'Dockerfile'
         :param invalidation: Options to control which parameters are used to invalidate the asset hash. Default: - hash all parameters
         :param network_mode: Networking mode for the RUN commands during build. Support docker API 1.25+. Default: - no networking mode specified (the default networking mode ``NetworkMode.DEFAULT`` will be used)
@@ -595,14 +597,15 @@
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9de8152b52ea9bc7ab7afc08793a9a98145196c9c9f1ff7cee2103ce1cfdb482)
             check_type(argname="argument directory", value=directory, expected_type=type_hints["directory"])
         options = _aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetOptions(
+            asset_name=asset_name,
             build_args=build_args,
             build_secrets=build_secrets,
             cache_from=cache_from,
             cache_to=cache_to,
             file=file,
             invalidation=invalidation,
             network_mode=network_mode,
@@ -3697,39 +3700,42 @@
 
     @jsii.member(jsii_name="fromAsset")
     @builtins.classmethod
     def from_asset(
         cls,
         path: builtins.str,
         *,
+        deploy_time: typing.Optional[builtins.bool] = None,
         readers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IGrantable]] = None,
         asset_hash: typing.Optional[builtins.str] = None,
         asset_hash_type: typing.Optional[_aws_cdk_ceddda9d.AssetHashType] = None,
         bundling: typing.Optional[typing.Union[_aws_cdk_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
         follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
         ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
     ) -> "ModelData":
         '''(experimental) Constructs model data that will be uploaded to S3 as part of the CDK app deployment.
 
         :param path: The local path to a model artifact file as a gzipped tar file.
+        :param deploy_time: Whether or not the asset needs to exist beyond deployment time; i.e. are copied over to a different location and not needed afterwards. Setting this property to true has an impact on the lifecycle of the asset, because we will assume that it is safe to delete after the CloudFormation deployment succeeds. For example, Lambda Function assets are copied over to Lambda during deployment. Therefore, it is not necessary to store the asset in S3, so we consider those deployTime assets. Default: false
         :param readers: A list of principals that should be able to read this asset from S3. You can use ``asset.grantRead(principal)`` to grant read permissions later. Default: - No principals that can read file asset.
         :param asset_hash: Specify a custom hash for this asset. If ``assetHashType`` is set it must be set to ``AssetHashType.CUSTOM``. For consistency, this custom hash will be SHA256 hashed and encoded as hex. The resulting hash will be the asset hash. NOTE: the hash is used in order to identify a specific revision of the asset, and used for optimizing and caching deployment activities related to this asset such as packaging, uploading to Amazon S3, etc. If you chose to customize the hash, you will need to make sure it is updated every time the asset changes, or otherwise it is possible that some deployments will not be invalidated. Default: - based on ``assetHashType``
         :param asset_hash_type: Specifies the type of hash to calculate for this asset. If ``assetHash`` is configured, this option must be ``undefined`` or ``AssetHashType.CUSTOM``. Default: - the default is ``AssetHashType.SOURCE``, but if ``assetHash`` is explicitly specified this value defaults to ``AssetHashType.CUSTOM``.
         :param bundling: Bundle the asset by executing a command in a Docker container or a custom bundling provider. The asset path will be mounted at ``/asset-input``. The Docker container is responsible for putting content at ``/asset-output``. The content at ``/asset-output`` will be zipped and used as the final asset. Default: - uploaded as-is to S3 if the asset is a regular file or a .zip file, archived into a .zip file and uploaded to S3 otherwise
         :param exclude: File paths matching the patterns will be excluded. See ``ignoreMode`` to set the matching behavior. Has no effect on Assets bundled using the ``bundling`` property. Default: - nothing is excluded
         :param follow_symlinks: A strategy for how to handle symlinks. Default: SymlinkFollowMode.NEVER
         :param ignore_mode: The ignore behavior to use for ``exclude`` patterns. Default: IgnoreMode.GLOB
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4addbae90cf26605669fced6862f03af9ca520de66de2c834cb76b219426416f)
             check_type(argname="argument path", value=path, expected_type=type_hints["path"])
         options = _aws_cdk_aws_s3_assets_ceddda9d.AssetOptions(
+            deploy_time=deploy_time,
             readers=readers,
             asset_hash=asset_hash,
             asset_hash_type=asset_hash_type,
             bundling=bundling,
             exclude=exclude,
             follow_symlinks=follow_symlinks,
             ignore_mode=ignore_mode,
@@ -4688,14 +4694,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9de8152b52ea9bc7ab7afc08793a9a98145196c9c9f1ff7cee2103ce1cfdb482(
     directory: builtins.str,
     *,
+    asset_name: typing.Optional[builtins.str] = None,
     build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     build_secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     cache_from: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]]] = None,
     cache_to: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]] = None,
     file: typing.Optional[builtins.str] = None,
     invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
@@ -4898,14 +4905,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__4addbae90cf26605669fced6862f03af9ca520de66de2c834cb76b219426416f(
     path: builtins.str,
     *,
+    deploy_time: typing.Optional[builtins.bool] = None,
     readers: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.IGrantable]] = None,
     asset_hash: typing.Optional[builtins.str] = None,
     asset_hash_type: typing.Optional[_aws_cdk_ceddda9d.AssetHashType] = None,
     bundling: typing.Optional[typing.Union[_aws_cdk_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     exclude: typing.Optional[typing.Sequence[builtins.str]] = None,
     follow_symlinks: typing.Optional[_aws_cdk_ceddda9d.SymlinkFollowMode] = None,
     ignore_mode: typing.Optional[_aws_cdk_ceddda9d.IgnoreMode] = None,
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-sagemaker-alpha
-Version: 2.80.0a0
+Version: 2.81.0a0
 Summary: The CDK Construct Library for AWS::SageMaker
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.80.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-sagemaker-alpha-2.81.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_sagemaker_alpha/__init__.py
 src/aws_cdk/aws_sagemaker_alpha/py.typed
 src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
-src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.80.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.81.0-alpha.0.jsii.tgz
```

