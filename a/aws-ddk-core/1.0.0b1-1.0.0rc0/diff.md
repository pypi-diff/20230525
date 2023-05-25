# Comparing `tmp/aws-ddk-core-1.0.0b1.tar.gz` & `tmp/aws-ddk-core-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ddk-core-1.0.0b1.tar", last modified: Mon Apr 17 23:35:42 2023, max compression
+gzip compressed data, was "aws-ddk-core-1.0.0rc0.tar", last modified: Wed May 17 19:00:02 2023, max compression
```

## Comparing `aws-ddk-core-1.0.0b1.tar` & `aws-ddk-core-1.0.0rc0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.045497 aws-ddk-core-1.0.0b1/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)    11358 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/LICENSE
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       23 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/MANIFEST.in
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       67 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/NOTICE
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     8819 2023-04-17 23:35:42.045054 aws-ddk-core-1.0.0b1/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     7891 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/README.md
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      236 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/pyproject.toml
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       38 2023-04-17 23:35:42.045613 aws-ddk-core-1.0.0b1/setup.cfg
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     1979 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/setup.py
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.036244 aws-ddk-core-1.0.0b1/src/
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.040506 aws-ddk-core-1.0.0b1/src/aws_ddk_core/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)   474193 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/__init__.py
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.043344 aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      600 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/__init__.py
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)   850443 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.0-beta.1.jsii.tgz
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/py.typed
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.042548 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     8819 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      407 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/SOURCES.txt
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/dependency_links.txt
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      313 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/requires.txt
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       13 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/top_level.txt
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.306179 aws-ddk-core-1.0.0rc0/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)    11358 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/LICENSE
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       23 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/MANIFEST.in
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       67 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/NOTICE
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     6066 2023-05-17 19:00:02.305837 aws-ddk-core-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     5052 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/README.md
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      234 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/pyproject.toml
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       38 2023-05-17 19:00:02.306284 aws-ddk-core-1.0.0rc0/setup.cfg
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     2082 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/setup.py
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.291633 aws-ddk-core-1.0.0rc0/src/
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.295908 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)   540084 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/__init__.py
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.298863 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      583 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/__init__.py
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)  5515151 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.0-rc.0.jsii.tgz
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/py.typed
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.298126 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     6066 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      405 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      313 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/requires.txt
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       13 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/top_level.txt
```

### Comparing `aws-ddk-core-1.0.0b1/LICENSE` & `aws-ddk-core-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.0.0b1/PKG-INFO` & `aws-ddk-core-1.0.0rc0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.0b1
+Version: 1.0.0rc0
 Summary: AWS DataOps Development Kit
-Home-page: https://github.com/awslabs/aws-ddk
+Home-page: https://github.com/awslabs/aws-ddk/tree/typescript-conversion
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
-Project-URL: Source, https://github.com/awslabs/aws-ddk
-Platform: UNKNOWN
+Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/typescript-conversion
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # AWS DataOps Development Kit (DDK)
 
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/bandit.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/cfn-nag.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/cli-tests.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/core-tests.yml/badge.svg)
+![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
 
 The **DDK Core** is a library of CDK constructs that you can use to build data workflows and modern data architecture on AWS, following our best practice. The DDK Core is modular and extensible, if our best practice doesn't work for you, then you can update and share your own version with the rest of your organisation by leveraging a private **AWS Code Artifact** repository.
 
 You can compose constructs from the DDK Core into a **DDK App**.  Your DDK App can also add contain constructs from the CDK Framework or the [AWS Construct Library](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html).
 
-You can use the **DDK CLI** to manage your DDK App.  You can use it to create a new app from a template, or deploy your DDK app to AWS.
-
 ## Overview
 
 For a detailed walk-through, check out our [Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/3644b48b-1d7c-43ef-a353-6edcd96385af/en-US) or
 take a look at [examples](https://github.com/aws-samples/aws-ddk-examples).
 
 ### Build Data Pipelines
 
@@ -58,151 +53,51 @@
 and are encouraged to share them with the community.
 
 Let's take a look at an example below:
 
 ```python
 ...
 
-firehose_s3_stage = KinesisToS3Stage(
+firehose_s3_stage = FirehoseToS3Stage(
     self,
     "ddk-firehose-s3",
-    environment_id=environment_id,
     bucket=ddk_bucket,
     data_output_prefix="raw/",
 )
 sqs_lambda_stage = SqsToLambdaStage(
     scope=self,
     id="ddk-sqs-lambda",
-    environment_id=environment_id,
     code=Code.from_asset("./lambda"),
     handler="index.lambda_handler",
     layers=[
         LayerVersion.from_layer_version_arn(
             self,
             "ddk-lambda-layer-wrangler",
-            f"arn:aws:lambda:{self.region}:336392948345:layer:AWSDataWrangler-Python39:2",
+            f"arn:aws:lambda:{self.region}:336392948345:layer:AWSSDKPandas-Python39:1",
         )
     ]
 )
 
 (
     DataPipeline(scope=self, id="ddk-pipeline")
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[KinesisToS3Stage](https://awslabs.github.io/aws-ddk/release/stable/api/core/stubs/aws_ddk_core.stages.KinesisToS3Stage.html), and
-[SQSToLambdaStage()](https://awslabs.github.io/aws-ddk/release/stable/api/core/stubs/aws_ddk_core.stages.SqsToLambdaStage.html).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
-### Resource Configuration
-
-Another core feature of DDK is ability to provide environment-dependent configuration to your resources.
-
-In the example below, we create Kinesis Data Stream using
-[KinesisStreamsFactory](https://awslabs.github.io/aws-ddk/release/latest/api/core/stubs/aws_ddk_core.resources.KinesisStreamsFactory.html#aws_ddk_core.resources.KinesisStreamsFactory).
-
-```python
-...
-from aws_ddk_core.resources import KinesisStreamsFactory
-
-...
-data_stream = KinesisStreamsFactory.data_stream(
-    self, id=f"example-data-stream", environment_id=environment_id,
-)
-...
-```
-
-Resources created by DDK factories are automatically configured with properties from `ddk.json`.
-
-```json
-{
-    "environments": {
-        "test": {
-            "account": "3333333333333",
-            "region": "us-east-1",
-            "resources": {
-                "example-data-stream": {"shard_count": 5},
-            }
-        }
-    }
-}
-```
-
-In this example, the Kinesis Data Stream will be configured with `5` shards.
-
-### Starting a new project
-
-Install or update the AWS DDK from PyPi.
-
-![pip install aws-ddk](./docs/source/_static/pip-install.gif)
-
-Create a new project:
-
-```console
-ddk init sample-app
-```
-
-This will create a `sample-app` directory inside the current folder.
-Inside that directory, it will generate the initial project structure, and initialize a virtual environment.
-
-```console
-sample-app
-├── .gitignore
-├── .venv
-├── README.md
-├── app.py
-├── cdk.json
-├── ddk.json
-├── ddk_app
-│   ├── __init__.py
-│   └── ddk_app_stack.py
-├── requirements-dev.txt
-├── requirements.txt
-├── setup.py
-└── source.bat
-```
-
-To activate the virtual environment, and install the dependencies, run:
-
-```console
-source .venv/bin/activate && pip install -r requirements.txt
-```
-
-Next, let us examine the code. If you look at app.py, it will look like this:
-
-```python
-import aws_cdk as cdk
-from ddk_app.ddk_app_stack import DdkApplicationStack
-
-app = cdk.App()
-DdkApplicationStack(app, "DdkApplication", "dev")
-
-app.synth()
-```
-
-If your AWS account hasn't been used to deploy DDK apps before, then you need to bootstrap your environment:
-
-```console
-ddk bootstrap
-```
-
-You can then deploy your DDK app:
-
-```console
-ddk deploy
-```
-
 ### Official Resources
 
 * [Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/3644b48b-1d7c-43ef-a353-6edcd96385af/en-US)
 * [Documentation](https://awslabs.github.io/aws-ddk/)
 * [API Reference](https://awslabs.github.io/aws-ddk/release/stable/api/index)
 * [Examples](https://github.com/aws-samples/aws-ddk-examples/)
 
@@ -218,9 +113,7 @@
 ## Other Ways to Support
 
 One way you can support our project is by letting others know that your organisation uses the DDK.  If you would like us to include your company's name and/or logo in this README file, please raise a 'Support the DDK' issue.  Note that by raising a this issue (and related pull request), you are granting AWS permission to use your company’s name (and logo) for the limited purpose described here and you are confirming that you have authority to grant such permission.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
-
-
```

### Comparing `aws-ddk-core-1.0.0b1/README.md` & `aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,47 @@
+Metadata-Version: 2.1
+Name: aws-ddk-core
+Version: 1.0.0rc0
+Summary: AWS DataOps Development Kit
+Home-page: https://github.com/awslabs/aws-ddk/tree/typescript-conversion
+Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
+License: Apache-2.0
+Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/typescript-conversion
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: NOTICE
+
 # AWS DataOps Development Kit (DDK)
 
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/bandit.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/cfn-nag.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/cli-tests.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/core-tests.yml/badge.svg)
+![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
 
 The **DDK Core** is a library of CDK constructs that you can use to build data workflows and modern data architecture on AWS, following our best practice. The DDK Core is modular and extensible, if our best practice doesn't work for you, then you can update and share your own version with the rest of your organisation by leveraging a private **AWS Code Artifact** repository.
 
 You can compose constructs from the DDK Core into a **DDK App**.  Your DDK App can also add contain constructs from the CDK Framework or the [AWS Construct Library](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html).
 
-You can use the **DDK CLI** to manage your DDK App.  You can use it to create a new app from a template, or deploy your DDK app to AWS.
-
 ## Overview
 
 For a detailed walk-through, check out our [Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/3644b48b-1d7c-43ef-a353-6edcd96385af/en-US) or
 take a look at [examples](https://github.com/aws-samples/aws-ddk-examples).
 
 ### Build Data Pipelines
 
@@ -33,151 +53,51 @@
 and are encouraged to share them with the community.
 
 Let's take a look at an example below:
 
 ```python
 ...
 
-firehose_s3_stage = KinesisToS3Stage(
+firehose_s3_stage = FirehoseToS3Stage(
     self,
     "ddk-firehose-s3",
-    environment_id=environment_id,
     bucket=ddk_bucket,
     data_output_prefix="raw/",
 )
 sqs_lambda_stage = SqsToLambdaStage(
     scope=self,
     id="ddk-sqs-lambda",
-    environment_id=environment_id,
     code=Code.from_asset("./lambda"),
     handler="index.lambda_handler",
     layers=[
         LayerVersion.from_layer_version_arn(
             self,
             "ddk-lambda-layer-wrangler",
-            f"arn:aws:lambda:{self.region}:336392948345:layer:AWSDataWrangler-Python39:2",
+            f"arn:aws:lambda:{self.region}:336392948345:layer:AWSSDKPandas-Python39:1",
         )
     ]
 )
 
 (
     DataPipeline(scope=self, id="ddk-pipeline")
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[KinesisToS3Stage](https://awslabs.github.io/aws-ddk/release/stable/api/core/stubs/aws_ddk_core.stages.KinesisToS3Stage.html), and
-[SQSToLambdaStage()](https://awslabs.github.io/aws-ddk/release/stable/api/core/stubs/aws_ddk_core.stages.SqsToLambdaStage.html).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
-### Resource Configuration
-
-Another core feature of DDK is ability to provide environment-dependent configuration to your resources.
-
-In the example below, we create Kinesis Data Stream using
-[KinesisStreamsFactory](https://awslabs.github.io/aws-ddk/release/latest/api/core/stubs/aws_ddk_core.resources.KinesisStreamsFactory.html#aws_ddk_core.resources.KinesisStreamsFactory).
-
-```python
-...
-from aws_ddk_core.resources import KinesisStreamsFactory
-
-...
-data_stream = KinesisStreamsFactory.data_stream(
-    self, id=f"example-data-stream", environment_id=environment_id,
-)
-...
-```
-
-Resources created by DDK factories are automatically configured with properties from `ddk.json`.
-
-```json
-{
-    "environments": {
-        "test": {
-            "account": "3333333333333",
-            "region": "us-east-1",
-            "resources": {
-                "example-data-stream": {"shard_count": 5},
-            }
-        }
-    }
-}
-```
-
-In this example, the Kinesis Data Stream will be configured with `5` shards.
-
-### Starting a new project
-
-Install or update the AWS DDK from PyPi.
-
-![pip install aws-ddk](./docs/source/_static/pip-install.gif)
-
-Create a new project:
-
-```console
-ddk init sample-app
-```
-
-This will create a `sample-app` directory inside the current folder.
-Inside that directory, it will generate the initial project structure, and initialize a virtual environment.
-
-```console
-sample-app
-├── .gitignore
-├── .venv
-├── README.md
-├── app.py
-├── cdk.json
-├── ddk.json
-├── ddk_app
-│   ├── __init__.py
-│   └── ddk_app_stack.py
-├── requirements-dev.txt
-├── requirements.txt
-├── setup.py
-└── source.bat
-```
-
-To activate the virtual environment, and install the dependencies, run:
-
-```console
-source .venv/bin/activate && pip install -r requirements.txt
-```
-
-Next, let us examine the code. If you look at app.py, it will look like this:
-
-```python
-import aws_cdk as cdk
-from ddk_app.ddk_app_stack import DdkApplicationStack
-
-app = cdk.App()
-DdkApplicationStack(app, "DdkApplication", "dev")
-
-app.synth()
-```
-
-If your AWS account hasn't been used to deploy DDK apps before, then you need to bootstrap your environment:
-
-```console
-ddk bootstrap
-```
-
-You can then deploy your DDK app:
-
-```console
-ddk deploy
-```
-
 ### Official Resources
 
 * [Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/3644b48b-1d7c-43ef-a353-6edcd96385af/en-US)
 * [Documentation](https://awslabs.github.io/aws-ddk/)
 * [API Reference](https://awslabs.github.io/aws-ddk/release/stable/api/index)
 * [Examples](https://github.com/aws-samples/aws-ddk-examples/)
```

### Comparing `aws-ddk-core-1.0.0b1/setup.py` & `aws-ddk-core-1.0.0rc0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ddk-core",
-    "version": "1.0.0.b1",
+    "version": "1.0.0.rc0",
     "description": "AWS DataOps Development Kit",
     "license": "Apache-2.0",
-    "url": "https://github.com/awslabs/aws-ddk",
+    "url": "https://github.com/awslabs/aws-ddk/tree/typescript-conversion",
     "long_description_content_type": "text/markdown",
     "author": "AWS Professional Services<aws-proserve-orion-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
-        "Source": "https://github.com/awslabs/aws-ddk"
+        "Source": "https://github.com/awslabs/aws-ddk/tree/typescript-conversion"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "aws_ddk_core",
         "aws_ddk_core._jsii"
     ],
     "package_data": {
         "aws_ddk_core._jsii": [
-            "aws-ddk-core@1.0.0-beta.1.jsii.tgz"
+            "aws-ddk-core@1.0.0-rc.0.jsii.tgz"
         ],
         "aws_ddk_core": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.71.0, <3.0.0",
         "aws-cdk.aws-glue-alpha>=2.71.0.a0, <3.0.0",
         "aws-cdk.aws-kinesisfirehose-alpha>=2.71.0.a0, <3.0.0",
         "aws-cdk.aws-kinesisfirehose-destinations-alpha>=2.71.0.a0, <3.0.0",
         "aws-cdk.integ-tests-alpha>=2.71.0.a0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `aws-ddk-core-1.0.0b1/src/aws_ddk_core/__init__.py` & `aws-ddk-core-1.0.0rc0/src/aws_ddk_core/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 '''
 # AWS DataOps Development Kit (DDK)
 
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/bandit.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/cfn-nag.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/cli-tests.yml/badge.svg)
-![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/core-tests.yml/badge.svg)
+![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
 
 The **DDK Core** is a library of CDK constructs that you can use to build data workflows and modern data architecture on AWS, following our best practice. The DDK Core is modular and extensible, if our best practice doesn't work for you, then you can update and share your own version with the rest of your organisation by leveraging a private **AWS Code Artifact** repository.
 
 You can compose constructs from the DDK Core into a **DDK App**.  Your DDK App can also add contain constructs from the CDK Framework or the [AWS Construct Library](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html).
 
-You can use the **DDK CLI** to manage your DDK App.  You can use it to create a new app from a template, or deploy your DDK app to AWS.
-
 ## Overview
 
 For a detailed walk-through, check out our [Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/3644b48b-1d7c-43ef-a353-6edcd96385af/en-US) or
 take a look at [examples](https://github.com/aws-samples/aws-ddk-examples).
 
 ### Build Data Pipelines
 
@@ -34,151 +29,51 @@
 and are encouraged to share them with the community.
 
 Let's take a look at an example below:
 
 ```python
 ...
 
-firehose_s3_stage = KinesisToS3Stage(
+firehose_s3_stage = FirehoseToS3Stage(
     self,
     "ddk-firehose-s3",
-    environment_id=environment_id,
     bucket=ddk_bucket,
     data_output_prefix="raw/",
 )
 sqs_lambda_stage = SqsToLambdaStage(
     scope=self,
     id="ddk-sqs-lambda",
-    environment_id=environment_id,
     code=Code.from_asset("./lambda"),
     handler="index.lambda_handler",
     layers=[
         LayerVersion.from_layer_version_arn(
             self,
             "ddk-lambda-layer-wrangler",
-            f"arn:aws:lambda:{self.region}:336392948345:layer:AWSDataWrangler-Python39:2",
+            f"arn:aws:lambda:{self.region}:336392948345:layer:AWSSDKPandas-Python39:1",
         )
     ]
 )
 
 (
     DataPipeline(scope=self, id="ddk-pipeline")
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[KinesisToS3Stage](https://awslabs.github.io/aws-ddk/release/stable/api/core/stubs/aws_ddk_core.stages.KinesisToS3Stage.html), and
-[SQSToLambdaStage()](https://awslabs.github.io/aws-ddk/release/stable/api/core/stubs/aws_ddk_core.stages.SqsToLambdaStage.html).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
-### Resource Configuration
-
-Another core feature of DDK is ability to provide environment-dependent configuration to your resources.
-
-In the example below, we create Kinesis Data Stream using
-[KinesisStreamsFactory](https://awslabs.github.io/aws-ddk/release/latest/api/core/stubs/aws_ddk_core.resources.KinesisStreamsFactory.html#aws_ddk_core.resources.KinesisStreamsFactory).
-
-```python
-...
-from aws_ddk_core.resources import KinesisStreamsFactory
-
-...
-data_stream = KinesisStreamsFactory.data_stream(
-    self, id=f"example-data-stream", environment_id=environment_id,
-)
-...
-```
-
-Resources created by DDK factories are automatically configured with properties from `ddk.json`.
-
-```json
-{
-    "environments": {
-        "test": {
-            "account": "3333333333333",
-            "region": "us-east-1",
-            "resources": {
-                "example-data-stream": {"shard_count": 5},
-            }
-        }
-    }
-}
-```
-
-In this example, the Kinesis Data Stream will be configured with `5` shards.
-
-### Starting a new project
-
-Install or update the AWS DDK from PyPi.
-
-![pip install aws-ddk](./docs/source/_static/pip-install.gif)
-
-Create a new project:
-
-```console
-ddk init sample-app
-```
-
-This will create a `sample-app` directory inside the current folder.
-Inside that directory, it will generate the initial project structure, and initialize a virtual environment.
-
-```console
-sample-app
-├── .gitignore
-├── .venv
-├── README.md
-├── app.py
-├── cdk.json
-├── ddk.json
-├── ddk_app
-│   ├── __init__.py
-│   └── ddk_app_stack.py
-├── requirements-dev.txt
-├── requirements.txt
-├── setup.py
-└── source.bat
-```
-
-To activate the virtual environment, and install the dependencies, run:
-
-```console
-source .venv/bin/activate && pip install -r requirements.txt
-```
-
-Next, let us examine the code. If you look at app.py, it will look like this:
-
-```python
-import aws_cdk as cdk
-from ddk_app.ddk_app_stack import DdkApplicationStack
-
-app = cdk.App()
-DdkApplicationStack(app, "DdkApplication", "dev")
-
-app.synth()
-```
-
-If your AWS account hasn't been used to deploy DDK apps before, then you need to bootstrap your environment:
-
-```console
-ddk bootstrap
-```
-
-You can then deploy your DDK app:
-
-```console
-ddk deploy
-```
-
 ### Official Resources
 
 * [Workshop](https://catalog.us-east-1.prod.workshops.aws/workshops/3644b48b-1d7c-43ef-a353-6edcd96385af/en-US)
 * [Documentation](https://awslabs.github.io/aws-ddk/)
 * [API Reference](https://awslabs.github.io/aws-ddk/release/stable/api/index)
 * [Examples](https://github.com/aws-samples/aws-ddk-examples/)
 
@@ -253,18 +148,19 @@
     def __init__(
         self,
         *,
         stage: _aws_cdk_ceddda9d.Stage,
         stage_id: builtins.str,
         manual_approvals: typing.Optional[builtins.bool] = None,
     ) -> None:
-        '''
-        :param stage: 
-        :param stage_id: 
-        :param manual_approvals: 
+        '''Properties for adding an application stage.
+
+        :param stage: Application stage instance.
+        :param stage_id: Identifier of the stage.
+        :param manual_approvals: Configure manual approvals. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b76c36dbcfdd4e997564efc9be54eb407b35cd3e027b00901b31d379e392170e)
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
             check_type(argname="argument stage_id", value=stage_id, expected_type=type_hints["stage_id"])
             check_type(argname="argument manual_approvals", value=manual_approvals, expected_type=type_hints["manual_approvals"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -272,26 +168,32 @@
             "stage_id": stage_id,
         }
         if manual_approvals is not None:
             self._values["manual_approvals"] = manual_approvals
 
     @builtins.property
     def stage(self) -> _aws_cdk_ceddda9d.Stage:
+        '''Application stage instance.'''
         result = self._values.get("stage")
         assert result is not None, "Required property 'stage' is missing"
         return typing.cast(_aws_cdk_ceddda9d.Stage, result)
 
     @builtins.property
     def stage_id(self) -> builtins.str:
+        '''Identifier of the stage.'''
         result = self._values.get("stage_id")
         assert result is not None, "Required property 'stage_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def manual_approvals(self) -> typing.Optional[builtins.bool]:
+        '''Configure manual approvals.
+
+        :default: false
+        '''
         result = self._values.get("manual_approvals")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -316,18 +218,19 @@
     def __init__(
         self,
         *,
         stage_id: builtins.str,
         stages: typing.Sequence[_aws_cdk_ceddda9d.Stage],
         manual_approvals: typing.Optional[builtins.bool] = None,
     ) -> None:
-        '''
-        :param stage_id: 
-        :param stages: 
-        :param manual_approvals: 
+        '''Properties for adding an application wave.
+
+        :param stage_id: Identifier of the wave.
+        :param stages: Application stage instance.
+        :param manual_approvals: Configure manual approvals. Default: false
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1c5ca54834b066a96cdaae8f32086d4638af32527e6bdd7356e96d6b16db8c0d)
             check_type(argname="argument stage_id", value=stage_id, expected_type=type_hints["stage_id"])
             check_type(argname="argument stages", value=stages, expected_type=type_hints["stages"])
             check_type(argname="argument manual_approvals", value=manual_approvals, expected_type=type_hints["manual_approvals"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -335,26 +238,32 @@
             "stages": stages,
         }
         if manual_approvals is not None:
             self._values["manual_approvals"] = manual_approvals
 
     @builtins.property
     def stage_id(self) -> builtins.str:
+        '''Identifier of the wave.'''
         result = self._values.get("stage_id")
         assert result is not None, "Required property 'stage_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def stages(self) -> typing.List[_aws_cdk_ceddda9d.Stage]:
+        '''Application stage instance.'''
         result = self._values.get("stages")
         assert result is not None, "Required property 'stages' is missing"
         return typing.cast(typing.List[_aws_cdk_ceddda9d.Stage], result)
 
     @builtins.property
     def manual_approvals(self) -> typing.Optional[builtins.bool]:
+        '''Configure manual approvals.
+
+        :default: false
+        '''
         result = self._values.get("manual_approvals")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -374,35 +283,42 @@
 class AddCustomStageProps:
     def __init__(
         self,
         *,
         stage_name: builtins.str,
         steps: typing.Sequence[_aws_cdk_pipelines_ceddda9d.Step],
     ) -> None:
-        '''
-        :param stage_name: 
-        :param steps: 
+        '''Properties for adding a custom stage.
+
+        :param stage_name: Name of the stage.
+        :param steps: Steps to add to this stage. List of Step objects. See `Documentation on aws_cdk.pipelines.Step <https://docs.aws.amazon.com/cdk/api/v1/python/aws_cdk.pipelines/Step.html>`_ for more detail.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8660c7ffe37e5e521438a6f05e109d7d73960491ec724c71005fa435cb1ba0cb)
             check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
             check_type(argname="argument steps", value=steps, expected_type=type_hints["steps"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "stage_name": stage_name,
             "steps": steps,
         }
 
     @builtins.property
     def stage_name(self) -> builtins.str:
+        '''Name of the stage.'''
         result = self._values.get("stage_name")
         assert result is not None, "Required property 'stage_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def steps(self) -> typing.List[_aws_cdk_pipelines_ceddda9d.Step]:
+        '''Steps to add to this stage. List of Step objects.
+
+        See `Documentation on aws_cdk.pipelines.Step <https://docs.aws.amazon.com/cdk/api/v1/python/aws_cdk.pipelines/Step.html>`_
+        for more detail.
+        '''
         result = self._values.get("steps")
         assert result is not None, "Required property 'steps' is missing"
         return typing.cast(typing.List[_aws_cdk_pipelines_ceddda9d.Step], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -422,28 +338,30 @@
 )
 class AddNotificationsProps:
     def __init__(
         self,
         *,
         notification_rule: typing.Optional[_aws_cdk_aws_codestarnotifications_ceddda9d.NotificationRule] = None,
     ) -> None:
-        '''
-        :param notification_rule: 
+        '''Properties for adding notifications.
+
+        :param notification_rule: Override notification rule.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f6b36a0552668c2be6f5870fa1fc235676fcd1d8e1633ffdcd8fe2ab50a5eb9c)
             check_type(argname="argument notification_rule", value=notification_rule, expected_type=type_hints["notification_rule"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if notification_rule is not None:
             self._values["notification_rule"] = notification_rule
 
     @builtins.property
     def notification_rule(
         self,
     ) -> typing.Optional[_aws_cdk_aws_codestarnotifications_ceddda9d.NotificationRule]:
+        '''Override notification rule.'''
         result = self._values.get("notification_rule")
         return typing.cast(typing.Optional[_aws_cdk_aws_codestarnotifications_ceddda9d.NotificationRule], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -567,17 +485,18 @@
 class AddSecurityLintStageProps:
     def __init__(
         self,
         *,
         cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param cloud_assembly_file_set: 
-        :param stage_name: 
+        '''Properties for adding a security lint stage.
+
+        :param cloud_assembly_file_set: Cloud assembly file set producer.
+        :param stage_name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f5c6a426f2b47035ddfb61265fb0fc5f914c183c57db8be19fd6917fe3755000)
             check_type(argname="argument cloud_assembly_file_set", value=cloud_assembly_file_set, expected_type=type_hints["cloud_assembly_file_set"])
             check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if cloud_assembly_file_set is not None:
@@ -585,19 +504,21 @@
         if stage_name is not None:
             self._values["stage_name"] = stage_name
 
     @builtins.property
     def cloud_assembly_file_set(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer]:
+        '''Cloud assembly file set producer.'''
         result = self._values.get("cloud_assembly_file_set")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer], result)
 
     @builtins.property
     def stage_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("stage_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -707,18 +628,19 @@
     def __init__(
         self,
         *,
         cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
         commands: typing.Optional[typing.Sequence[builtins.str]] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param cloud_assembly_file_set: 
-        :param commands: 
-        :param stage_name: 
+        '''Properties for adding a test stage.
+
+        :param cloud_assembly_file_set: Cloud assembly file set.
+        :param commands: Additional commands to run in the test. Default: "./test.sh"
+        :param stage_name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0efd164879f28724d26fec5d40738d32540d827f1e7d46271d569f72a3a0a21f)
             check_type(argname="argument cloud_assembly_file_set", value=cloud_assembly_file_set, expected_type=type_hints["cloud_assembly_file_set"])
             check_type(argname="argument commands", value=commands, expected_type=type_hints["commands"])
             check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -729,24 +651,30 @@
         if stage_name is not None:
             self._values["stage_name"] = stage_name
 
     @builtins.property
     def cloud_assembly_file_set(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer]:
+        '''Cloud assembly file set.'''
         result = self._values.get("cloud_assembly_file_set")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer], result)
 
     @builtins.property
     def commands(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Additional commands to run in the test.
+
+        :default: "./test.sh"
+        '''
         result = self._values.get("commands")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def stage_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("stage_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -789,27 +717,28 @@
         docker_enabled_for_synth: typing.Optional[builtins.bool] = None,
         publish_assets_in_parallel: typing.Optional[builtins.bool] = None,
         reuse_cross_region_support_stacks: typing.Optional[builtins.bool] = None,
         self_mutation: typing.Optional[builtins.bool] = None,
         self_mutation_code_build_defaults: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         synth_code_build_defaults: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
-        :param asset_publishing_code_build_defaults: 
-        :param cli_version: 
-        :param code_build_defaults: 
-        :param code_pipeline: 
-        :param docker_credentials: 
-        :param docker_enabled_for_self_mutation: 
-        :param docker_enabled_for_synth: 
-        :param publish_assets_in_parallel: 
-        :param reuse_cross_region_support_stacks: 
-        :param self_mutation: 
-        :param self_mutation_code_build_defaults: 
-        :param synth_code_build_defaults: 
+        '''Additional properties for building the CodePipeline.
+
+        :param asset_publishing_code_build_defaults: Additional customizations to apply to the asset publishing CodeBuild projects. Default: - Only ``codeBuildDefaults`` are applied
+        :param cli_version: CDK CLI version to use in self-mutation and asset publishing steps. Default: latest version
+        :param code_build_defaults: Customize the CodeBuild projects created for this pipeline. Default: - All projects run non-privileged build, SMALL instance, LinuxBuildImage.STANDARD_6_0
+        :param code_pipeline: An existing Pipeline to be reused and built upon. Default: - a new underlying pipeline is created.
+        :param docker_credentials: A list of credentials used to authenticate to Docker registries. Specify any credentials necessary within the pipeline to build, synth, update, or publish assets. Default: []
+        :param docker_enabled_for_self_mutation: Enable Docker for the self-mutate step. Default: false
+        :param docker_enabled_for_synth: Enable Docker for the 'synth' step. Default: false
+        :param publish_assets_in_parallel: Publish assets in multiple CodeBuild projects. Default: true
+        :param reuse_cross_region_support_stacks: Reuse the same cross region support stack for all pipelines in the App. Default: - true (Use the same support stack for all pipelines in App)
+        :param self_mutation: Whether the pipeline will update itself. This needs to be set to ``true`` to allow the pipeline to reconfigure itself when assets or stages are being added to it, and ``true`` is the recommended setting. You can temporarily set this to ``false`` while you are iterating on the pipeline itself and prefer to deploy changes using ``cdk deploy``. Default: true
+        :param self_mutation_code_build_defaults: Additional customizations to apply to the self mutation CodeBuild projects. Default: - Only ``codeBuildDefaults`` are applied
+        :param synth_code_build_defaults: Additional customizations to apply to the synthesize CodeBuild projects. Default: - Only ``codeBuildDefaults`` are applied
         '''
         if isinstance(asset_publishing_code_build_defaults, dict):
             asset_publishing_code_build_defaults = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**asset_publishing_code_build_defaults)
         if isinstance(code_build_defaults, dict):
             code_build_defaults = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**code_build_defaults)
         if isinstance(self_mutation_code_build_defaults, dict):
             self_mutation_code_build_defaults = _aws_cdk_pipelines_ceddda9d.CodeBuildOptions(**self_mutation_code_build_defaults)
@@ -855,79 +784,136 @@
         if synth_code_build_defaults is not None:
             self._values["synth_code_build_defaults"] = synth_code_build_defaults
 
     @builtins.property
     def asset_publishing_code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
+        '''Additional customizations to apply to the asset publishing CodeBuild projects.
+
+        :default: - Only ``codeBuildDefaults`` are applied
+        '''
         result = self._values.get("asset_publishing_code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def cli_version(self) -> typing.Optional[builtins.str]:
+        '''CDK CLI version to use in self-mutation and asset publishing steps.
+
+        :default: latest version
+        '''
         result = self._values.get("cli_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
+        '''Customize the CodeBuild projects created for this pipeline.
+
+        :default: - All projects run non-privileged build, SMALL instance, LinuxBuildImage.STANDARD_6_0
+        '''
         result = self._values.get("code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def code_pipeline(
         self,
     ) -> typing.Optional[_aws_cdk_aws_codepipeline_ceddda9d.Pipeline]:
+        '''An existing Pipeline to be reused and built upon.
+
+        :default: - a new underlying pipeline is created.
+        '''
         result = self._values.get("code_pipeline")
         return typing.cast(typing.Optional[_aws_cdk_aws_codepipeline_ceddda9d.Pipeline], result)
 
     @builtins.property
     def docker_credentials(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_pipelines_ceddda9d.DockerCredential]]:
+        '''A list of credentials used to authenticate to Docker registries.
+
+        Specify any credentials necessary within the pipeline to build, synth, update, or publish assets.
+
+        :default: []
+        '''
         result = self._values.get("docker_credentials")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_pipelines_ceddda9d.DockerCredential]], result)
 
     @builtins.property
     def docker_enabled_for_self_mutation(self) -> typing.Optional[builtins.bool]:
+        '''Enable Docker for the self-mutate step.
+
+        :default: false
+        '''
         result = self._values.get("docker_enabled_for_self_mutation")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def docker_enabled_for_synth(self) -> typing.Optional[builtins.bool]:
+        '''Enable Docker for the 'synth' step.
+
+        :default: false
+        '''
         result = self._values.get("docker_enabled_for_synth")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def publish_assets_in_parallel(self) -> typing.Optional[builtins.bool]:
+        '''Publish assets in multiple CodeBuild projects.
+
+        :default: true
+        '''
         result = self._values.get("publish_assets_in_parallel")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def reuse_cross_region_support_stacks(self) -> typing.Optional[builtins.bool]:
+        '''Reuse the same cross region support stack for all pipelines in the App.
+
+        :default: - true (Use the same support stack for all pipelines in App)
+        '''
         result = self._values.get("reuse_cross_region_support_stacks")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def self_mutation(self) -> typing.Optional[builtins.bool]:
+        '''Whether the pipeline will update itself.
+
+        This needs to be set to ``true`` to allow the pipeline to reconfigure
+        itself when assets or stages are being added to it, and ``true`` is the
+        recommended setting.
+
+        You can temporarily set this to ``false`` while you are iterating
+        on the pipeline itself and prefer to deploy changes using ``cdk deploy``.
+
+        :default: true
+        '''
         result = self._values.get("self_mutation")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def self_mutation_code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
+        '''Additional customizations to apply to the self mutation CodeBuild projects.
+
+        :default: - Only ``codeBuildDefaults`` are applied
+        '''
         result = self._values.get("self_mutation_code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     @builtins.property
     def synth_code_build_defaults(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions]:
+        '''Additional customizations to apply to the synthesize CodeBuild projects.
+
+        :default: - Only ``codeBuildDefaults`` are applied
+        '''
         result = self._values.get("synth_code_build_defaults")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -954,19 +940,20 @@
         self,
         *,
         metric: _aws_cdk_aws_cloudwatch_ceddda9d.IMetric,
         comparison_operator: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator] = None,
         evaluation_periods: typing.Optional[jsii.Number] = None,
         threshold: typing.Optional[jsii.Number] = None,
     ) -> None:
-        '''
-        :param metric: 
-        :param comparison_operator: 
-        :param evaluation_periods: 
-        :param threshold: 
+        '''Properties for the alarm being added to the DataStage.
+
+        :param metric: Metric to use for creating the stage's CloudWatch Alarm.
+        :param comparison_operator: Comparison operator to use for alarm. Default: GREATER_THAN_THRESHOLD
+        :param evaluation_periods: The value against which the specified alarm statistic is compared. Default: 5
+        :param threshold: The number of periods over which data is compared to the specified threshold. Default: 1
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9739513f93590856f8f02851ab5bfe24bf3c845f3e37410565b3668ac8406da2)
             check_type(argname="argument metric", value=metric, expected_type=type_hints["metric"])
             check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
             check_type(argname="argument evaluation_periods", value=evaluation_periods, expected_type=type_hints["evaluation_periods"])
             check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
@@ -978,32 +965,45 @@
         if evaluation_periods is not None:
             self._values["evaluation_periods"] = evaluation_periods
         if threshold is not None:
             self._values["threshold"] = threshold
 
     @builtins.property
     def metric(self) -> _aws_cdk_aws_cloudwatch_ceddda9d.IMetric:
+        '''Metric to use for creating the stage's CloudWatch Alarm.'''
         result = self._values.get("metric")
         assert result is not None, "Required property 'metric' is missing"
         return typing.cast(_aws_cdk_aws_cloudwatch_ceddda9d.IMetric, result)
 
     @builtins.property
     def comparison_operator(
         self,
     ) -> typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator]:
+        '''Comparison operator to use for alarm.
+
+        :default: GREATER_THAN_THRESHOLD
+        '''
         result = self._values.get("comparison_operator")
         return typing.cast(typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator], result)
 
     @builtins.property
     def evaluation_periods(self) -> typing.Optional[jsii.Number]:
+        '''The value against which the specified alarm statistic is compared.
+
+        :default: 5
+        '''
         result = self._values.get("evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def threshold(self) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1016,14 +1016,19 @@
 
 
 class BaseStack(
     _aws_cdk_ceddda9d.Stack,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.BaseStack",
 ):
+    '''Base Stack to inherit from.
+
+    Includes configurable termination protection, synthesizer, permissions boundary and tags.
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
@@ -1034,20 +1039,24 @@
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param config: 
-        :param environment_id: 
-        :param permissions_boundary_arn: 
+        '''Create a stack.
+
+        Includes termination protection settings, multi-level (application, environment,
+        and stack-level) tags, and permissions boundary.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stack.
+        :param config: Configuration or path to file which contains the configuration.
+        :param environment_id: Identifier of the environment. Default: "dev"
+        :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
@@ -1099,19 +1108,47 @@
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = PermissionsBoundaryProps(
             environment_id=environment_id, prefix=prefix, qualifier=qualifier
         )
 
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.IManagedPolicy, jsii.sinvoke(cls, "createDefaultPermissionsBoundary", [scope, id, props]))
 
-    @builtins.property
-    @jsii.member(jsii_name="terminationProtection")
-    def termination_protection(self) -> typing.Optional[builtins.bool]:
-        '''Whether termination protection is enabled for this stack.'''
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "terminationProtection"))
+    @jsii.member(jsii_name="exportValue")
+    def export_value(
+        self,
+        exported_value: typing.Any,
+        *,
+        name: typing.Optional[builtins.str] = None,
+    ) -> builtins.str:
+        '''Create a CloudFormation Export for a string value.
+
+        Returns a string representing the corresponding ``Fn.importValue()``
+        expression for this Export. You can control the name for the export by
+        passing the ``name`` option.
+
+        If you don't supply a value for ``name``, the value you're exporting must be
+        a Resource attribute (for example: ``bucket.bucketName``) and it will be
+        given the same name as the automatic cross-stack reference that would be created
+        if you used the attribute in another Stack.
+
+        One of the uses for this method is to *remove* the relationship between
+        two Stacks established by automatic cross-stack references. It will
+        temporarily ensure that the CloudFormation Export still exists while you
+        remove the reference from the consuming stack. After that, you can remove
+        the resource and the manual export.
+
+        :param exported_value: -
+        :param name: The name of the export to create. Default: - A name is automatically chosen
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b2efe5dde2538acae1f48243a64a4ddfc2bc79e8400b2883ddf4986fbd5984c8)
+            check_type(argname="argument exported_value", value=exported_value, expected_type=type_hints["exported_value"])
+        options = _aws_cdk_ceddda9d.ExportValueOptions(name=name)
+
+        return typing.cast(builtins.str, jsii.invoke(self, "exportValue", [exported_value, options]))
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.BaseStackProps",
     jsii_struct_bases=[_aws_cdk_ceddda9d.StackProps],
     name_mapping={
         "analytics_reporting": "analyticsReporting",
@@ -1141,27 +1178,28 @@
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
         config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
+        '''Properties of ``BaseStack``.
+
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
-        :param config: 
-        :param environment_id: 
-        :param permissions_boundary_arn: 
+        :param config: Configuration or path to file which contains the configuration.
+        :param environment_id: Identifier of the environment. Default: "dev"
+        :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a429ca722d1fec889b8120d065d6c339e922faac9a9e70454e565500ff82514c)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
@@ -1361,24 +1399,30 @@
         :default: false
         '''
         result = self._values.get("termination_protection")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def config(self) -> typing.Optional[typing.Union[builtins.str, "Configuration"]]:
+        '''Configuration or path to file which contains the configuration.'''
         result = self._values.get("config")
         return typing.cast(typing.Optional[typing.Union[builtins.str, "Configuration"]], result)
 
     @builtins.property
     def environment_id(self) -> typing.Optional[builtins.str]:
+        '''Identifier of the environment.
+
+        :default: "dev"
+        '''
         result = self._values.get("environment_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def permissions_boundary_arn(self) -> typing.Optional[builtins.str]:
+        '''ARN of the permissions boundary managed policy.'''
         result = self._values.get("permissions_boundary_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1556,14 +1600,40 @@
 
 
 class CICDPipelineStack(
     BaseStack,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.CICDPipelineStack",
 ):
+    '''Create a stack that contains DDK Continuous Integration and Delivery (CI/CD) pipeline.
+
+    The pipeline is based on
+    `CDK self-mutating pipeline <https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.pipelines-readme.html>`_
+    but includes several DDK-specific features, including:
+
+    - Ability to configure some properties via JSON config e.g. manual approvals for application stages
+    - Defaults for source/synth - CodeCommit & cdk synth, with ability to override them
+    - Ability to connect to private artifactory to pull artifacts from at synth
+    - Security best practices - ensures pipeline buckets block non-SSL, and are KMS-encrypted with rotated keys
+    - Builder interface to avoid chunky constructor methods
+
+    The user should be able to reuse the pipeline in multiple DDK applications hoping to save LOC.
+
+    Example::
+
+        const stack = new CICDPipelineStack(app, "dummy-pipeline", { environmentId: "dev", pipelineName: "dummy-pipeline" })
+          .addSourceAction({ repositoryName: "dummy-repository" })
+          .addSynthAction()
+          .buildPipeline()
+          .add_checks()
+          .addStage({ stageId: "dev", stage: devStage, manualApprovals: true })
+          .synth()
+          .add_notifications();
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         cdk_language: typing.Optional[builtins.str] = None,
         pipeline_name: typing.Optional[builtins.str] = None,
@@ -1576,22 +1646,23 @@
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param cdk_language: 
-        :param pipeline_name: 
-        :param config: 
-        :param environment_id: 
-        :param permissions_boundary_arn: 
+        '''Creates a new CICD Pipeline stack.
+
+        :param scope: Parent of this stack, usually an ``App`` or a ``Stage``, but could be any construct.
+        :param id: The construct ID of this stack. If ``stackName`` is not explicitly defined, this id (and any parent IDs) will be used to determine the physical ID of the stack.
+        :param cdk_language: Language of the CDK construct definitions. Default: "typescript"
+        :param pipeline_name: Name of the pipeline.
+        :param config: Configuration or path to file which contains the configuration.
+        :param environment_id: Identifier of the environment. Default: "dev"
+        :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
@@ -1619,54 +1690,69 @@
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="addChecks")
     def add_checks(self) -> "CICDPipelineStack":
+        '''Add checks to the pipeline (e.g. linting, security, tests...).
+
+        :return: reference to this pipeline.
+        '''
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addChecks", []))
 
     @jsii.member(jsii_name="addCustomStage")
     def add_custom_stage(
         self,
         *,
         stage_name: builtins.str,
         steps: typing.Sequence[_aws_cdk_pipelines_ceddda9d.Step],
     ) -> "CICDPipelineStack":
-        '''
-        :param stage_name: 
-        :param steps: 
+        '''Add custom stage to the pipeline.
+
+        :param stage_name: Name of the stage.
+        :param steps: Steps to add to this stage. List of Step objects. See `Documentation on aws_cdk.pipelines.Step <https://docs.aws.amazon.com/cdk/api/v1/python/aws_cdk.pipelines/Step.html>`_ for more detail.
+
+        :return: reference to this pipeline.
         '''
         props = AddCustomStageProps(stage_name=stage_name, steps=steps)
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addCustomStage", [props]))
 
     @jsii.member(jsii_name="addNotifications")
     def add_notifications(
         self,
         *,
         notification_rule: typing.Optional[_aws_cdk_aws_codestarnotifications_ceddda9d.NotificationRule] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param notification_rule: 
+        '''Add pipeline notifications.
+
+        Create notification rule that sends events to the specified SNS topic.
+
+        :param notification_rule: Override notification rule.
+
+        :return: reference to this pipeline.
         '''
         props = AddNotificationsProps(notification_rule=notification_rule)
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addNotifications", [props]))
 
     @jsii.member(jsii_name="addSecurityLintStage")
     def add_security_lint_stage(
         self,
         *,
         cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param cloud_assembly_file_set: 
-        :param stage_name: 
+        '''Add linting - cfn-nag, and bandit.
+
+        :param cloud_assembly_file_set: Cloud assembly file set producer.
+        :param stage_name: Name of the stage.
+
+        :return: reference to this pipeline.
         '''
         props = AddSecurityLintStageProps(
             cloud_assembly_file_set=cloud_assembly_file_set, stage_name=stage_name
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addSecurityLintStage", [props]))
 
@@ -1674,18 +1760,21 @@
     def add_source_action(
         self,
         *,
         repository_name: builtins.str,
         branch: typing.Optional[builtins.str] = None,
         source_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodePipelineSource] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param repository_name: 
-        :param branch: 
-        :param source_action: 
+        '''Add source action.
+
+        :param repository_name: Name of the SCM repository.
+        :param branch: Branch of the SCM repository.
+        :param source_action: Override source action.
+
+        :return: reference to this pipeline.
         '''
         props = SourceActionProps(
             repository_name=repository_name, branch=branch, source_action=source_action
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addSourceAction", [props]))
 
@@ -1693,18 +1782,23 @@
     def add_stage(
         self,
         *,
         stage: _aws_cdk_ceddda9d.Stage,
         stage_id: builtins.str,
         manual_approvals: typing.Optional[builtins.bool] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param stage: 
-        :param stage_id: 
-        :param manual_approvals: 
+        '''Add application stage to the CICD pipeline.
+
+        This stage deploys your application infrastructure.
+
+        :param stage: Application stage instance.
+        :param stage_id: Identifier of the stage.
+        :param manual_approvals: Configure manual approvals. Default: false
+
+        :return: reference to this pipeline.
         '''
         props = AddApplicationStageProps(
             stage=stage, stage_id=stage_id, manual_approvals=manual_approvals
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addStage", [props]))
 
@@ -1716,22 +1810,27 @@
         cdk_version: typing.Optional[builtins.str] = None,
         codeartifact_domain: typing.Optional[builtins.str] = None,
         codeartifact_domain_owner: typing.Optional[builtins.str] = None,
         codeartifact_repository: typing.Optional[builtins.str] = None,
         role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         synth_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param additional_install_commands: 
-        :param cdk_version: 
-        :param codeartifact_domain: 
-        :param codeartifact_domain_owner: 
-        :param codeartifact_repository: 
-        :param role_policy_statements: 
-        :param synth_action: 
+        '''Add synth action.
+
+        During synth can connect and pull artifacts from a private artifactory.
+
+        :param additional_install_commands: Additional install commands.
+        :param cdk_version: CDK versio to use during the synth action. Default: "latest"
+        :param codeartifact_domain: Name of the CodeArtifact domain.
+        :param codeartifact_domain_owner: CodeArtifact domain owner account.
+        :param codeartifact_repository: Name of the CodeArtifact repository to pull artifacts from.
+        :param role_policy_statements: Additional policies to add to the synth action role.
+        :param synth_action: Override synth action.
+
+        :return: reference to this pipeline.
         '''
         props = SynthActionProps(
             additional_install_commands=additional_install_commands,
             cdk_version=cdk_version,
             codeartifact_domain=codeartifact_domain,
             codeartifact_domain_owner=codeartifact_domain_owner,
             codeartifact_repository=codeartifact_repository,
@@ -1745,18 +1844,21 @@
     def add_test_stage(
         self,
         *,
         cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
         commands: typing.Optional[typing.Sequence[builtins.str]] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param cloud_assembly_file_set: 
-        :param commands: 
-        :param stage_name: 
+        '''Add test - e.g. pytest.
+
+        :param cloud_assembly_file_set: Cloud assembly file set.
+        :param commands: Additional commands to run in the test. Default: "./test.sh"
+        :param stage_name: Name of the stage.
+
+        :return: reference to this pipeline.
         '''
         props = AddTestStageProps(
             cloud_assembly_file_set=cloud_assembly_file_set,
             commands=commands,
             stage_name=stage_name,
         )
 
@@ -1766,18 +1868,21 @@
     def add_wave(
         self,
         *,
         stage_id: builtins.str,
         stages: typing.Sequence[_aws_cdk_ceddda9d.Stage],
         manual_approvals: typing.Optional[builtins.bool] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param stage_id: 
-        :param stages: 
-        :param manual_approvals: 
+        '''Add multiple application stages in parallel to the CICD pipeline.
+
+        :param stage_id: Identifier of the wave.
+        :param stages: Application stage instance.
+        :param manual_approvals: Configure manual approvals. Default: false
+
+        :return: reference to this pipeline.
         '''
         props = AddApplicationWaveProps(
             stage_id=stage_id, stages=stages, manual_approvals=manual_approvals
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addWave", [props]))
 
@@ -1794,27 +1899,30 @@
         docker_enabled_for_synth: typing.Optional[builtins.bool] = None,
         publish_assets_in_parallel: typing.Optional[builtins.bool] = None,
         reuse_cross_region_support_stacks: typing.Optional[builtins.bool] = None,
         self_mutation: typing.Optional[builtins.bool] = None,
         self_mutation_code_build_defaults: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         synth_code_build_defaults: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.CodeBuildOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> "CICDPipelineStack":
-        '''
-        :param asset_publishing_code_build_defaults: 
-        :param cli_version: 
-        :param code_build_defaults: 
-        :param code_pipeline: 
-        :param docker_credentials: 
-        :param docker_enabled_for_self_mutation: 
-        :param docker_enabled_for_synth: 
-        :param publish_assets_in_parallel: 
-        :param reuse_cross_region_support_stacks: 
-        :param self_mutation: 
-        :param self_mutation_code_build_defaults: 
-        :param synth_code_build_defaults: 
+        '''Build the pipeline structure.
+
+        :param asset_publishing_code_build_defaults: Additional customizations to apply to the asset publishing CodeBuild projects. Default: - Only ``codeBuildDefaults`` are applied
+        :param cli_version: CDK CLI version to use in self-mutation and asset publishing steps. Default: latest version
+        :param code_build_defaults: Customize the CodeBuild projects created for this pipeline. Default: - All projects run non-privileged build, SMALL instance, LinuxBuildImage.STANDARD_6_0
+        :param code_pipeline: An existing Pipeline to be reused and built upon. Default: - a new underlying pipeline is created.
+        :param docker_credentials: A list of credentials used to authenticate to Docker registries. Specify any credentials necessary within the pipeline to build, synth, update, or publish assets. Default: []
+        :param docker_enabled_for_self_mutation: Enable Docker for the self-mutate step. Default: false
+        :param docker_enabled_for_synth: Enable Docker for the 'synth' step. Default: false
+        :param publish_assets_in_parallel: Publish assets in multiple CodeBuild projects. Default: true
+        :param reuse_cross_region_support_stacks: Reuse the same cross region support stack for all pipelines in the App. Default: - true (Use the same support stack for all pipelines in App)
+        :param self_mutation: Whether the pipeline will update itself. This needs to be set to ``true`` to allow the pipeline to reconfigure itself when assets or stages are being added to it, and ``true`` is the recommended setting. You can temporarily set this to ``false`` while you are iterating on the pipeline itself and prefer to deploy changes using ``cdk deploy``. Default: true
+        :param self_mutation_code_build_defaults: Additional customizations to apply to the self mutation CodeBuild projects. Default: - Only ``codeBuildDefaults`` are applied
+        :param synth_code_build_defaults: Additional customizations to apply to the synthesize CodeBuild projects. Default: - Only ``codeBuildDefaults`` are applied
+
+        :return: reference to this pipeline.
         '''
         props = AdditionalPipelineProps(
             asset_publishing_code_build_defaults=asset_publishing_code_build_defaults,
             cli_version=cli_version,
             code_build_defaults=code_build_defaults,
             code_pipeline=code_pipeline,
             docker_credentials=docker_credentials,
@@ -1827,14 +1935,18 @@
             synth_code_build_defaults=synth_code_build_defaults,
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "buildPipeline", [props]))
 
     @jsii.member(jsii_name="synth")
     def synth(self) -> "CICDPipelineStack":
+        '''Synthesize the pipeline.
+
+        :return: reference to this pipeline.
+        '''
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "synth", []))
 
     @builtins.property
     @jsii.member(jsii_name="cdkLanguage")
     def cdk_language(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "cdkLanguage"))
 
@@ -1975,29 +2087,30 @@
         termination_protection: typing.Optional[builtins.bool] = None,
         config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         cdk_language: typing.Optional[builtins.str] = None,
         pipeline_name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
+        '''CICD Pipeline Stack properties.
+
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param synthesizer: Synthesis method to use while deploying this stack. The Stack Synthesizer controls aspects of synthesis and deployment, like how assets are referenced and what IAM roles to use. For more information, see the README of the main CDK package. If not specified, the ``defaultStackSynthesizer`` from ``App`` will be used. If that is not specified, ``DefaultStackSynthesizer`` is used if ``@aws-cdk/core:newStyleStackSynthesis`` is set to ``true`` or the CDK major version is v2. In CDK v1 ``LegacyStackSynthesizer`` is the default if no other synthesizer is specified. Default: - The synthesizer specified on ``App``, or ``DefaultStackSynthesizer`` otherwise.
         :param tags: Stack tags that will be applied to all the taggable resources and the stack itself. Default: {}
         :param termination_protection: Whether to enable termination protection for this stack. Default: false
-        :param config: 
-        :param environment_id: 
-        :param permissions_boundary_arn: 
-        :param cdk_language: 
-        :param pipeline_name: 
+        :param config: Configuration or path to file which contains the configuration.
+        :param environment_id: Identifier of the environment. Default: "dev"
+        :param permissions_boundary_arn: ARN of the permissions boundary managed policy.
+        :param cdk_language: Language of the CDK construct definitions. Default: "typescript"
+        :param pipeline_name: Name of the pipeline.
         '''
         if isinstance(env, dict):
             env = _aws_cdk_ceddda9d.Environment(**env)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a92abb1f3b57ec36ef721160ab799be2851ede5d3e872162fc75be713f4d3293)
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
@@ -2203,34 +2316,45 @@
         :default: false
         '''
         result = self._values.get("termination_protection")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def config(self) -> typing.Optional[typing.Union[builtins.str, "Configuration"]]:
+        '''Configuration or path to file which contains the configuration.'''
         result = self._values.get("config")
         return typing.cast(typing.Optional[typing.Union[builtins.str, "Configuration"]], result)
 
     @builtins.property
     def environment_id(self) -> typing.Optional[builtins.str]:
+        '''Identifier of the environment.
+
+        :default: "dev"
+        '''
         result = self._values.get("environment_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def permissions_boundary_arn(self) -> typing.Optional[builtins.str]:
+        '''ARN of the permissions boundary managed policy.'''
         result = self._values.get("permissions_boundary_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cdk_language(self) -> typing.Optional[builtins.str]:
+        '''Language of the CDK construct definitions.
+
+        :default: "typescript"
+        '''
         result = self._values.get("cdk_language")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def pipeline_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the pipeline.'''
         result = self._values.get("pipeline_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -2435,54 +2559,60 @@
     jsii_type="aws-ddk-core.Configuration",
     jsii_struct_bases=[],
     name_mapping={
         "environments": "environments",
         "account": "account",
         "bootstrap": "bootstrap",
         "ddk_bootstrap_config_key": "ddkBootstrapConfigKey",
+        "props": "props",
         "region": "region",
         "tags": "tags",
     },
 )
 class Configuration:
     def __init__(
         self,
         *,
         environments: typing.Mapping[builtins.str, typing.Union["EnvironmentConfiguration", typing.Dict[builtins.str, typing.Any]]],
         account: typing.Optional[builtins.str] = None,
         bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         ddk_bootstrap_config_key: typing.Optional[builtins.str] = None,
+        props: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         region: typing.Optional[builtins.str] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
         '''
         :param environments: 
         :param account: 
         :param bootstrap: 
         :param ddk_bootstrap_config_key: 
+        :param props: 
         :param region: 
         :param tags: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__daeed9e6cb5e50c39b922933d297c173f25183423bf700dfd9f8b0fe3765c923)
             check_type(argname="argument environments", value=environments, expected_type=type_hints["environments"])
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
             check_type(argname="argument bootstrap", value=bootstrap, expected_type=type_hints["bootstrap"])
             check_type(argname="argument ddk_bootstrap_config_key", value=ddk_bootstrap_config_key, expected_type=type_hints["ddk_bootstrap_config_key"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument region", value=region, expected_type=type_hints["region"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "environments": environments,
         }
         if account is not None:
             self._values["account"] = account
         if bootstrap is not None:
             self._values["bootstrap"] = bootstrap
         if ddk_bootstrap_config_key is not None:
             self._values["ddk_bootstrap_config_key"] = ddk_bootstrap_config_key
+        if props is not None:
+            self._values["props"] = props
         if region is not None:
             self._values["region"] = region
         if tags is not None:
             self._values["tags"] = tags
 
     @builtins.property
     def environments(self) -> typing.Mapping[builtins.str, "EnvironmentConfiguration"]:
@@ -2502,14 +2632,19 @@
 
     @builtins.property
     def ddk_bootstrap_config_key(self) -> typing.Optional[builtins.str]:
         result = self._values.get("ddk_bootstrap_config_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def props(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("props")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
     def region(self) -> typing.Optional[builtins.str]:
         result = self._values.get("region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         result = self._values.get("tags")
@@ -2542,14 +2677,28 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__83dd06108e5a02547d07299060f92123340b3d7ec7e9e6f36a8e28ce02b22a22)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument config", value=config, expected_type=type_hints["config"])
             check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
         jsii.create(self.__class__, self, [scope, config, environment_id])
 
+    @jsii.member(jsii_name="getConfig")
+    @builtins.classmethod
+    def get_config(
+        cls,
+        *,
+        config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
+    ) -> typing.Optional[Configuration]:
+        '''
+        :param config: 
+        '''
+        props = GetConfigProps(config=config)
+
+        return typing.cast(typing.Optional[Configuration], jsii.sinvoke(cls, "getConfig", [props]))
+
     @jsii.member(jsii_name="getEnvConfig")
     @builtins.classmethod
     def get_env_config(
         cls,
         *,
         config_path: builtins.str,
         environment_id: builtins.str,
@@ -2567,24 +2716,24 @@
     @jsii.member(jsii_name="getEnvironment")
     @builtins.classmethod
     def get_environment(
         cls,
         *,
         config_path: builtins.str,
         environment_id: typing.Optional[builtins.str] = None,
-    ) -> "EnvironmentResult":
+    ) -> _aws_cdk_ceddda9d.Environment:
         '''
         :param config_path: 
         :param environment_id: 
         '''
         props = GetEnvironmentProps(
             config_path=config_path, environment_id=environment_id
         )
 
-        return typing.cast("EnvironmentResult", jsii.sinvoke(cls, "getEnvironment", [props]))
+        return typing.cast(_aws_cdk_ceddda9d.Environment, jsii.sinvoke(cls, "getEnvironment", [props]))
 
     @jsii.member(jsii_name="getTags")
     @builtins.classmethod
     def get_tags(
         cls,
         *,
         config_path: builtins.str,
@@ -2875,21 +3024,22 @@
         delivery_stream_name: typing.Optional[builtins.str] = None,
         destinations: typing.Optional[typing.Sequence[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]] = None,
         encryption: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption] = None,
         encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
         role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
         source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
     ) -> None:
-        '''
-        :param delivery_stream_name: 
-        :param destinations: 
-        :param encryption: 
-        :param encryption_key: 
-        :param role: 
-        :param source_stream: 
+        '''Properties of the Firehose Delivery stream to be created.
+
+        :param delivery_stream_name: A name for the delivery stream. Default: - a name is generated by CloudFormation.
+        :param destinations: The destinations that this delivery stream will deliver data to. Only a singleton array is supported at this time.
+        :param encryption: Indicates the type of customer master key (CMK) to use for server-side encryption, if any. Default: StreamEncryption.UNENCRYPTED - unless ``encryptionKey`` is provided, in which case this will be implicitly set to ``StreamEncryption.CUSTOMER_MANAGED``
+        :param encryption_key: Customer managed key to server-side encrypt data in the stream. Default: - no KMS key will be used; if ``encryption`` is set to ``CUSTOMER_MANAGED``, a KMS key will be created for you
+        :param role: The IAM role associated with this delivery stream. Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side. Default: - a role will be created with default permissions.
+        :param source_stream: The Kinesis data stream to use as a source for this delivery stream. Default: - data must be written to the delivery stream via a direct put.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ef7997fe1d9215e0814459fdbbb95740e62a7f0437cd0df0dcd43ac255b163e4)
             check_type(argname="argument delivery_stream_name", value=delivery_stream_name, expected_type=type_hints["delivery_stream_name"])
             check_type(argname="argument destinations", value=destinations, expected_type=type_hints["destinations"])
             check_type(argname="argument encryption", value=encryption, expected_type=type_hints["encryption"])
             check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
@@ -2907,43 +3057,69 @@
         if role is not None:
             self._values["role"] = role
         if source_stream is not None:
             self._values["source_stream"] = source_stream
 
     @builtins.property
     def delivery_stream_name(self) -> typing.Optional[builtins.str]:
+        '''A name for the delivery stream.
+
+        :default: - a name is generated by CloudFormation.
+        '''
         result = self._values.get("delivery_stream_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def destinations(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]]:
+        '''The destinations that this delivery stream will deliver data to.
+
+        Only a singleton array is supported at this time.
+        '''
         result = self._values.get("destinations")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]], result)
 
     @builtins.property
     def encryption(
         self,
     ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption]:
+        '''Indicates the type of customer master key (CMK) to use for server-side encryption, if any.
+
+        :default: StreamEncryption.UNENCRYPTED - unless ``encryptionKey`` is provided, in which case this will be implicitly set to ``StreamEncryption.CUSTOMER_MANAGED``
+        '''
         result = self._values.get("encryption")
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption], result)
 
     @builtins.property
     def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+        '''Customer managed key to server-side encrypt data in the stream.
+
+        :default: - no KMS key will be used; if ``encryption`` is set to ``CUSTOMER_MANAGED``, a KMS key will be created for you
+        '''
         result = self._values.get("encryption_key")
         return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
 
     @builtins.property
     def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        '''The IAM role associated with this delivery stream.
+
+        Assumed by Kinesis Data Firehose to read from sources and encrypt data server-side.
+
+        :default: - a role will be created with default permissions.
+        '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
 
     @builtins.property
     def source_stream(self) -> typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream]:
+        '''The Kinesis data stream to use as a source for this delivery stream.
+
+        :default: - data must be written to the delivery stream via a direct put.
+        '''
         result = self._values.get("source_stream")
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -2957,48 +3133,54 @@
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.EnvironmentConfiguration",
     jsii_struct_bases=[],
     name_mapping={
         "account": "account",
         "bootstrap": "bootstrap",
+        "props": "props",
         "region": "region",
         "resources": "resources",
         "tags": "tags",
     },
 )
 class EnvironmentConfiguration:
     def __init__(
         self,
         *,
         account: typing.Optional[builtins.str] = None,
         bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        props: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         region: typing.Optional[builtins.str] = None,
         resources: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
         '''
         :param account: 
         :param bootstrap: 
+        :param props: 
         :param region: 
         :param resources: 
         :param tags: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf306c436463dcb56197f32e9c4793604595ef2ca8f42b2d72de058d5806870c)
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
             check_type(argname="argument bootstrap", value=bootstrap, expected_type=type_hints["bootstrap"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
             check_type(argname="argument region", value=region, expected_type=type_hints["region"])
             check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if account is not None:
             self._values["account"] = account
         if bootstrap is not None:
             self._values["bootstrap"] = bootstrap
+        if props is not None:
+            self._values["props"] = props
         if region is not None:
             self._values["region"] = region
         if resources is not None:
             self._values["resources"] = resources
         if tags is not None:
             self._values["tags"] = tags
 
@@ -3009,14 +3191,19 @@
 
     @builtins.property
     def bootstrap(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         result = self._values.get("bootstrap")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
+    def props(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("props")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
     def region(self) -> typing.Optional[builtins.str]:
         result = self._values.get("region")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         result = self._values.get("resources")
@@ -3036,57 +3223,47 @@
     def __repr__(self) -> str:
         return "EnvironmentConfiguration(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="aws-ddk-core.EnvironmentResult",
+    jsii_type="aws-ddk-core.GetConfigProps",
     jsii_struct_bases=[],
-    name_mapping={"account": "account", "region": "region"},
+    name_mapping={"config": "config"},
 )
-class EnvironmentResult:
+class GetConfigProps:
     def __init__(
         self,
         *,
-        account: typing.Optional[builtins.str] = None,
-        region: typing.Optional[builtins.str] = None,
+        config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
-        :param account: 
-        :param region: 
+        :param config: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c2515674b45134976862352edd7f3a4f56dddd10e860df69a14d633b55dfe768)
-            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
-            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            type_hints = typing.get_type_hints(_typecheckingstub__5dba6810d9499d40d626ee84f10a13e1cade1e4a1602afa74c9dd333695965bd)
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if account is not None:
-            self._values["account"] = account
-        if region is not None:
-            self._values["region"] = region
-
-    @builtins.property
-    def account(self) -> typing.Optional[builtins.str]:
-        result = self._values.get("account")
-        return typing.cast(typing.Optional[builtins.str], result)
+        if config is not None:
+            self._values["config"] = config
 
     @builtins.property
-    def region(self) -> typing.Optional[builtins.str]:
-        result = self._values.get("region")
-        return typing.cast(typing.Optional[builtins.str], result)
+    def config(self) -> typing.Optional[typing.Union[builtins.str, Configuration]]:
+        result = self._values.get("config")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, Configuration]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "EnvironmentResult(%s)" % ", ".join(
+        return "GetConfigProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.GetEnvConfigProps",
     jsii_struct_bases=[],
@@ -3714,18 +3891,19 @@
     def __init__(
         self,
         *,
         repository_name: builtins.str,
         branch: typing.Optional[builtins.str] = None,
         source_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodePipelineSource] = None,
     ) -> None:
-        '''
-        :param repository_name: 
-        :param branch: 
-        :param source_action: 
+        '''Properties for the source action.
+
+        :param repository_name: Name of the SCM repository.
+        :param branch: Branch of the SCM repository.
+        :param source_action: Override source action.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8c722ae4d9bf55cce29be798641c0fc2edce1bd6666919da164ce1643888b11e)
             check_type(argname="argument repository_name", value=repository_name, expected_type=type_hints["repository_name"])
             check_type(argname="argument branch", value=branch, expected_type=type_hints["branch"])
             check_type(argname="argument source_action", value=source_action, expected_type=type_hints["source_action"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -3734,27 +3912,30 @@
         if branch is not None:
             self._values["branch"] = branch
         if source_action is not None:
             self._values["source_action"] = source_action
 
     @builtins.property
     def repository_name(self) -> builtins.str:
+        '''Name of the SCM repository.'''
         result = self._values.get("repository_name")
         assert result is not None, "Required property 'repository_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def branch(self) -> typing.Optional[builtins.str]:
+        '''Branch of the SCM repository.'''
         result = self._values.get("branch")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_action(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodePipelineSource]:
+        '''Override source action.'''
         result = self._values.get("source_action")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodePipelineSource], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -3859,15 +4040,16 @@
         code: _aws_cdk_aws_lambda_ceddda9d.Code,
         handler: builtins.str,
         runtime: _aws_cdk_aws_lambda_ceddda9d.Runtime,
         errors_alarm_threshold: typing.Optional[jsii.Number] = None,
         errors_comparison_operator: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator] = None,
         errors_evaluation_periods: typing.Optional[jsii.Number] = None,
     ) -> None:
-        '''
+        '''Properties for the Lambda Function created by ``SqsToLambdaStage``.
+
         :param max_event_age: The maximum age of a request that Lambda sends to a function for processing. Minimum: 60 seconds Maximum: 6 hours Default: Duration.hours(6)
         :param on_failure: The destination for failed invocations. Default: - no destination
         :param on_success: The destination for successful invocations. Default: - no destination
         :param retry_attempts: The maximum number of times to retry when the function returns an error. Minimum: 0 Maximum: 2 Default: 2
         :param adot_instrumentation: Specify the configuration of AWS Distro for OpenTelemetry (ADOT) instrumentation. Default: - No ADOT instrumentation
         :param allow_all_outbound: Whether to allow the Lambda to send all network traffic. If set to false, you must individually add traffic rules to allow the Lambda to connect to network targets. Default: true
         :param allow_public_subnet: Lambda Functions in a public subnet can NOT access the internet. Use this property to acknowledge this limitation and still place the function in a public subnet. Default: false
@@ -3900,17 +4082,17 @@
         :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
         :param tracing: Enable AWS X-Ray Tracing for Lambda Function. Default: Tracing.Disabled
         :param vpc: VPC network to place Lambda network interfaces. Specify this if the Lambda function needs to access resources in a VPC. This is required when ``vpcSubnets`` is specified. Default: - Function is not placed within a VPC.
         :param vpc_subnets: Where to place the network interfaces within the VPC. This requires ``vpc`` to be specified in order for interfaces to actually be placed in the subnets. If ``vpc`` is not specify, this will raise an error. Note: Internet access for Lambda Functions requires a NAT Gateway, so picking public subnets is not allowed (unless ``allowPublicSubnet`` is set to ``true``). Default: - the Vpc default strategy if not specified
         :param code: The source code of your Lambda function. You can point to a file in an Amazon Simple Storage Service (Amazon S3) bucket or specify your source code as inline text.
         :param handler: The name of the method within your code that Lambda calls to execute your function. The format includes the file name. It can also include namespaces and other qualifiers, depending on the runtime. For more information, see https://docs.aws.amazon.com/lambda/latest/dg/foundation-progmodel.html. Use ``Handler.FROM_IMAGE`` when defining a function from a Docker image. NOTE: If you specify your source code as inline text by specifying the ZipFile property within the Code property, specify index.function_name as the handler.
         :param runtime: The runtime environment for the Lambda function that you are uploading. For valid values, see the Runtime property in the AWS Lambda Developer Guide. Use ``Runtime.FROM_IMAGE`` when defining a function from a Docker image.
-        :param errors_alarm_threshold: 
-        :param errors_comparison_operator: 
-        :param errors_evaluation_periods: 
+        :param errors_alarm_threshold: Amount of errored function invocations before triggering CloudWatch alarm. Default: 5
+        :param errors_comparison_operator: Comparison operator for evaluating alarms. Default: cloudwatch.ComparisonOperator.GREATER_THAN_THRESHOLD
+        :param errors_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
         '''
         if isinstance(adot_instrumentation, dict):
             adot_instrumentation = _aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig(**adot_instrumentation)
         if isinstance(current_version_options, dict):
             current_version_options = _aws_cdk_aws_lambda_ceddda9d.VersionOptions(**current_version_options)
         if isinstance(log_retention_retry_options, dict):
             log_retention_retry_options = _aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions(**log_retention_retry_options)
@@ -4536,26 +4718,38 @@
         '''
         result = self._values.get("runtime")
         assert result is not None, "Required property 'runtime' is missing"
         return typing.cast(_aws_cdk_aws_lambda_ceddda9d.Runtime, result)
 
     @builtins.property
     def errors_alarm_threshold(self) -> typing.Optional[jsii.Number]:
+        '''Amount of errored function invocations before triggering CloudWatch alarm.
+
+        :default: 5
+        '''
         result = self._values.get("errors_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def errors_comparison_operator(
         self,
     ) -> typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator]:
+        '''Comparison operator for evaluating alarms.
+
+        :default: cloudwatch.ComparisonOperator.GREATER_THAN_THRESHOLD
+        '''
         result = self._values.get("errors_comparison_operator")
         return typing.cast(typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator], result)
 
     @builtins.property
     def errors_evaluation_periods(self) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("errors_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -4568,76 +4762,99 @@
 
 
 class Stage(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="aws-ddk-core.Stage",
 ):
+    '''Abstract class representing a stage.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param description: 
-        :param name: 
+        '''Constructs the stage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e9cf7c3474ce139a45c8e31d476f0b548b9db19082dbea4dffb9287504da5dff)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = StageProps(description=description, name=name)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "description"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     @abc.abstractmethod
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "name"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     @abc.abstractmethod
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         ...
 
 
 class _StageProxy(Stage):
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, Stage).__jsii_proxy_class__ = lambda : _StageProxy
 
 
 @jsii.data_type(
@@ -4648,35 +4865,38 @@
 class StageProps:
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
+        '''Properties for the base abstract stage.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5e854dfb73af2b1e5b672ba3ec79ee122851867f8bde404e9918340757b3847c)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -4711,23 +4931,24 @@
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
+        '''Properties of a state machine stage.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5069a8477e1d868a51858f29afe4a12917625d0a7370bc4090fd23bf809c081c)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
@@ -4751,57 +4972,74 @@
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
             self._values["state_machine_name"] = state_machine_name
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def additional_role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
         result = self._values.get("additional_role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
         result = self._values.get("state_machine_input")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
         result = self._values.get("state_machine_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -4834,22 +5072,23 @@
         cdk_version: typing.Optional[builtins.str] = None,
         codeartifact_domain: typing.Optional[builtins.str] = None,
         codeartifact_domain_owner: typing.Optional[builtins.str] = None,
         codeartifact_repository: typing.Optional[builtins.str] = None,
         role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         synth_action: typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep] = None,
     ) -> None:
-        '''
-        :param additional_install_commands: 
-        :param cdk_version: 
-        :param codeartifact_domain: 
-        :param codeartifact_domain_owner: 
-        :param codeartifact_repository: 
-        :param role_policy_statements: 
-        :param synth_action: 
+        '''Properties for the synth action.
+
+        :param additional_install_commands: Additional install commands.
+        :param cdk_version: CDK versio to use during the synth action. Default: "latest"
+        :param codeartifact_domain: Name of the CodeArtifact domain.
+        :param codeartifact_domain_owner: CodeArtifact domain owner account.
+        :param codeartifact_repository: Name of the CodeArtifact repository to pull artifacts from.
+        :param role_policy_statements: Additional policies to add to the synth action role.
+        :param synth_action: Override synth action.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__05acfa3cda54a17101814d614a246f97dc36de4bf27ef87f72f7aa4824dd7b35)
             check_type(argname="argument additional_install_commands", value=additional_install_commands, expected_type=type_hints["additional_install_commands"])
             check_type(argname="argument cdk_version", value=cdk_version, expected_type=type_hints["cdk_version"])
             check_type(argname="argument codeartifact_domain", value=codeartifact_domain, expected_type=type_hints["codeartifact_domain"])
             check_type(argname="argument codeartifact_domain_owner", value=codeartifact_domain_owner, expected_type=type_hints["codeartifact_domain_owner"])
@@ -4870,48 +5109,58 @@
         if role_policy_statements is not None:
             self._values["role_policy_statements"] = role_policy_statements
         if synth_action is not None:
             self._values["synth_action"] = synth_action
 
     @builtins.property
     def additional_install_commands(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Additional install commands.'''
         result = self._values.get("additional_install_commands")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def cdk_version(self) -> typing.Optional[builtins.str]:
+        '''CDK versio to use during the synth action.
+
+        :default: "latest"
+        '''
         result = self._values.get("cdk_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def codeartifact_domain(self) -> typing.Optional[builtins.str]:
+        '''Name of the CodeArtifact domain.'''
         result = self._values.get("codeartifact_domain")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def codeartifact_domain_owner(self) -> typing.Optional[builtins.str]:
+        '''CodeArtifact domain owner account.'''
         result = self._values.get("codeartifact_domain_owner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def codeartifact_repository(self) -> typing.Optional[builtins.str]:
+        '''Name of the CodeArtifact repository to pull artifacts from.'''
         result = self._values.get("codeartifact_repository")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional policies to add to the synth action role.'''
         result = self._values.get("role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def synth_action(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep]:
+        '''Override synth action.'''
         result = self._values.get("synth_action")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.CodeBuildStep], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -4956,28 +5205,29 @@
         state_machine_name: typing.Optional[builtins.str] = None,
         destination_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         flow_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         flow_name: typing.Optional[builtins.str] = None,
         flow_tasks: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.TaskProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         source_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param destination_flow_config: 
-        :param flow_execution_status_check_period: 
-        :param flow_name: 
-        :param flow_tasks: 
-        :param source_flow_config: 
+        '''Properties of the AppFlow Ingestion stage.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param destination_flow_config: The flow ``appflow.CfnFlow.DestinationFlowConfigProperty`` properties.
+        :param flow_execution_status_check_period: Time to wait between flow execution status checks. Default: aws_cdk.Duration.seconds(15)
+        :param flow_name: Name of the AppFlow flow to run. If None, an AppFlow flow is created.
+        :param flow_tasks: The flow tasks properties.
+        :param source_flow_config: The flow ``appflow.CfnFlow.SourceFlowConfigProperty`` properties.
         '''
         if isinstance(destination_flow_config, dict):
             destination_flow_config = _aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty(**destination_flow_config)
         if isinstance(source_flow_config, dict):
             source_flow_config = _aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty(**source_flow_config)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__50f57d5c758f4bb8a7385b25c9dd1756786a7af562ac0cf743837ff675065839)
@@ -5020,90 +5270,118 @@
         if flow_tasks is not None:
             self._values["flow_tasks"] = flow_tasks
         if source_flow_config is not None:
             self._values["source_flow_config"] = source_flow_config
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def additional_role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
         result = self._values.get("additional_role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
         result = self._values.get("state_machine_input")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
         result = self._values.get("state_machine_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def destination_flow_config(
         self,
     ) -> typing.Optional[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty]:
+        '''The flow ``appflow.CfnFlow.DestinationFlowConfigProperty`` properties.'''
         result = self._values.get("destination_flow_config")
         return typing.cast(typing.Optional[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty], result)
 
     @builtins.property
     def flow_execution_status_check_period(
         self,
     ) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''Time to wait between flow execution status checks.
+
+        :default: aws_cdk.Duration.seconds(15)
+        '''
         result = self._values.get("flow_execution_status_check_period")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def flow_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the AppFlow flow to run.
+
+        If None, an AppFlow flow is created.
+        '''
         result = self._values.get("flow_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def flow_tasks(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.TaskProperty]]:
+        '''The flow tasks properties.'''
         result = self._values.get("flow_tasks")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.TaskProperty]], result)
 
     @builtins.property
     def source_flow_config(
         self,
     ) -> typing.Optional[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty]:
+        '''The flow ``appflow.CfnFlow.SourceFlowConfigProperty`` properties.'''
         result = self._values.get("source_flow_config")
         return typing.cast(typing.Optional[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5128,14 +5406,15 @@
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "catalog_name": "catalogName",
         "database_name": "databaseName",
         "encryption_key": "encryptionKey",
         "encryption_option": "encryptionOption",
         "output_location": "outputLocation",
+        "parallel": "parallel",
         "query_string": "queryString",
         "query_string_path": "queryStringPath",
         "work_group": "workGroup",
     },
 )
 class AthenaToSQLStageProps(StateMachineStageProps):
     def __init__(
@@ -5150,35 +5429,38 @@
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         catalog_name: typing.Optional[builtins.str] = None,
         database_name: typing.Optional[builtins.str] = None,
         encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key] = None,
         encryption_option: typing.Optional[_aws_cdk_aws_stepfunctions_tasks_ceddda9d.EncryptionOption] = None,
         output_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
-        query_string: typing.Optional[builtins.str] = None,
+        parallel: typing.Optional[builtins.bool] = None,
+        query_string: typing.Optional[typing.Sequence[builtins.str]] = None,
         query_string_path: typing.Optional[builtins.str] = None,
         work_group: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param catalog_name: 
-        :param database_name: 
-        :param encryption_key: 
-        :param encryption_option: 
-        :param output_location: 
-        :param query_string: 
-        :param query_string_path: 
-        :param work_group: 
+        '''Properties for ``AthenaSQLStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param catalog_name: Catalog name.
+        :param database_name: Database name.
+        :param encryption_key: Encryption KMS key.
+        :param encryption_option: Encryption configuration.
+        :param output_location: Output S3 location.
+        :param parallel: flag to determine parallel or sequential execution. Default: false
+        :param query_string: SQL queries that will be started.
+        :param query_string_path: dynamic path in statemachine for SQL query to be started.
+        :param work_group: Athena workgroup name.
         '''
         if isinstance(output_location, dict):
             output_location = _aws_cdk_aws_s3_ceddda9d.Location(**output_location)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d02b2a3868910a4789cbcba2028e07a331d2da507e4b4c951dd7801d735bc0ac)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
@@ -5189,14 +5471,15 @@
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument catalog_name", value=catalog_name, expected_type=type_hints["catalog_name"])
             check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
             check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
             check_type(argname="argument encryption_option", value=encryption_option, expected_type=type_hints["encryption_option"])
             check_type(argname="argument output_location", value=output_location, expected_type=type_hints["output_location"])
+            check_type(argname="argument parallel", value=parallel, expected_type=type_hints["parallel"])
             check_type(argname="argument query_string", value=query_string, expected_type=type_hints["query_string"])
             check_type(argname="argument query_string_path", value=query_string_path, expected_type=type_hints["query_string_path"])
             check_type(argname="argument work_group", value=work_group, expected_type=type_hints["work_group"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
@@ -5219,108 +5502,144 @@
             self._values["database_name"] = database_name
         if encryption_key is not None:
             self._values["encryption_key"] = encryption_key
         if encryption_option is not None:
             self._values["encryption_option"] = encryption_option
         if output_location is not None:
             self._values["output_location"] = output_location
+        if parallel is not None:
+            self._values["parallel"] = parallel
         if query_string is not None:
             self._values["query_string"] = query_string
         if query_string_path is not None:
             self._values["query_string_path"] = query_string_path
         if work_group is not None:
             self._values["work_group"] = work_group
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def additional_role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
         result = self._values.get("additional_role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
         result = self._values.get("state_machine_input")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
         result = self._values.get("state_machine_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def catalog_name(self) -> typing.Optional[builtins.str]:
+        '''Catalog name.'''
         result = self._values.get("catalog_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def database_name(self) -> typing.Optional[builtins.str]:
+        '''Database name.'''
         result = self._values.get("database_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key]:
+        '''Encryption KMS key.'''
         result = self._values.get("encryption_key")
         return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key], result)
 
     @builtins.property
     def encryption_option(
         self,
     ) -> typing.Optional[_aws_cdk_aws_stepfunctions_tasks_ceddda9d.EncryptionOption]:
+        '''Encryption configuration.'''
         result = self._values.get("encryption_option")
         return typing.cast(typing.Optional[_aws_cdk_aws_stepfunctions_tasks_ceddda9d.EncryptionOption], result)
 
     @builtins.property
     def output_location(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.Location]:
+        '''Output S3 location.'''
         result = self._values.get("output_location")
         return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.Location], result)
 
     @builtins.property
-    def query_string(self) -> typing.Optional[builtins.str]:
+    def parallel(self) -> typing.Optional[builtins.bool]:
+        '''flag to determine parallel or sequential execution.
+
+        :default: false
+        '''
+        result = self._values.get("parallel")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def query_string(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''SQL queries that will be started.'''
         result = self._values.get("query_string")
-        return typing.cast(typing.Optional[builtins.str], result)
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def query_string_path(self) -> typing.Optional[builtins.str]:
+        '''dynamic path in statemachine for SQL query to be started.'''
         result = self._values.get("query_string_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def work_group(self) -> typing.Optional[builtins.str]:
+        '''Athena workgroup name.'''
         result = self._values.get("work_group")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5397,44 +5716,45 @@
         profile_configuration: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         project_name: typing.Optional[builtins.str] = None,
         recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
         timeout: typing.Optional[jsii.Number] = None,
         validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param create_job: 
-        :param database_outputs: 
-        :param data_catalog_outputs: 
-        :param dataset_name: 
-        :param encryption_key_arn: 
-        :param encryption_mode: 
-        :param job_name: 
-        :param job_role_arn: 
-        :param job_sample: 
-        :param job_type: 
-        :param log_subscription: 
-        :param max_capacity: 
-        :param max_retries: 
-        :param output_location: 
-        :param outputs: 
-        :param profile_configuration: 
-        :param project_name: 
-        :param recipe: 
-        :param tags: 
-        :param timeout: 
-        :param validation_configurations: 
+        '''Properties for ``DataBrewTransformStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param create_job: Whether to create the DataBrew job or not.
+        :param database_outputs: Represents a list of JDBC database output objects which defines the output destination for a DataBrew recipe job to write into.
+        :param data_catalog_outputs: One or more artifacts that represent the AWS Glue Data Catalog output from running the job.
+        :param dataset_name: The name of the dataset to use for the job.
+        :param encryption_key_arn: The Amazon Resource Name (ARN) of an encryption key that is used to protect the job output. For more information, see `Encrypting data written by DataBrew jobs <https://docs.aws.amazon.com/databrew/latest/dg/encryption-security-configuration.html>`_
+        :param encryption_mode: The encryption mode for the job, which can be one of the following:. - ``SSE-KMS`` - Server-side encryption with keys managed by AWS KMS . - ``SSE-S3`` - Server-side encryption with keys managed by Amazon S3.
+        :param job_name: The name of a preexisting DataBrew job to run. If None, a DataBrew job is created.
+        :param job_role_arn: The Arn of the job execution role. Required if job_name is None.
+        :param job_sample: A sample configuration for profile jobs only, which determines the number of rows on which the profile job is run. If a ``JobSample`` value isn't provided, the default value is used. The default value is CUSTOM_ROWS for the mode parameter and 20,000 for the size parameter.
+        :param job_type: The type of job to run. Required if job_name is None.
+        :param log_subscription: The current status of Amazon CloudWatch logging for the job.
+        :param max_capacity: The maximum number of nodes that can be consumed when the job processes data.
+        :param max_retries: The maximum number of times to retry the job after a job run fails.
+        :param output_location: ``AWS::DataBrew::Job.OutputLocation``.
+        :param outputs: The output properties for the job.
+        :param profile_configuration: Configuration for profile jobs. Configuration can be used to select columns, do evaluations, and override default parameters of evaluations. When configuration is undefined, the profile job will apply default settings to all supported columns.
+        :param project_name: The name of the project that the job is associated with.
+        :param recipe: The recipe to be used by the DataBrew job which is a series of data transformation steps.
+        :param tags: Metadata tags that have been applied to the job.
+        :param timeout: The job's timeout in minutes. A job that attempts to run longer than this timeout period ends with a status of ``TIMEOUT`` .
+        :param validation_configurations: List of validation configurations that are applied to the profile job.
         '''
         if isinstance(job_sample, dict):
             job_sample = _aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty(**job_sample)
         if isinstance(output_location, dict):
             output_location = _aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty(**output_location)
         if isinstance(profile_configuration, dict):
             profile_configuration = _aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty(**profile_configuration)
@@ -5529,178 +5849,281 @@
         if timeout is not None:
             self._values["timeout"] = timeout
         if validation_configurations is not None:
             self._values["validation_configurations"] = validation_configurations
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def additional_role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
         result = self._values.get("additional_role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
         result = self._values.get("state_machine_input")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
         result = self._values.get("state_machine_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def create_job(self) -> typing.Optional[builtins.bool]:
+        '''Whether to create the DataBrew job or not.'''
         result = self._values.get("create_job")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def database_outputs(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty]]:
+        '''Represents a list of JDBC database output objects which defines the output destination for a DataBrew recipe job to write into.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-databaseoutputs
+        '''
         result = self._values.get("database_outputs")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty]], result)
 
     @builtins.property
     def data_catalog_outputs(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty]]:
+        '''One or more artifacts that represent the AWS Glue Data Catalog output from running the job.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-datacatalogoutputs
+        '''
         result = self._values.get("data_catalog_outputs")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty]], result)
 
     @builtins.property
     def dataset_name(self) -> typing.Optional[builtins.str]:
+        '''The name of the dataset to use for the job.'''
         result = self._values.get("dataset_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def encryption_key_arn(self) -> typing.Optional[builtins.str]:
+        '''The Amazon Resource Name (ARN) of an encryption key that is used to protect the job output.
+
+        For more information, see `Encrypting data written by DataBrew jobs <https://docs.aws.amazon.com/databrew/latest/dg/encryption-security-configuration.html>`_
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-encryptionkeyarn
+        '''
         result = self._values.get("encryption_key_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def encryption_mode(self) -> typing.Optional[builtins.str]:
+        '''The encryption mode for the job, which can be one of the following:.
+
+        - ``SSE-KMS`` - Server-side encryption with keys managed by AWS KMS .
+        - ``SSE-S3`` - Server-side encryption with keys managed by Amazon S3.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-encryptionmode
+        '''
         result = self._values.get("encryption_mode")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_name(self) -> typing.Optional[builtins.str]:
+        '''The name of a preexisting DataBrew job to run.
+
+        If None, a DataBrew job is created.
+        '''
         result = self._values.get("job_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_role_arn(self) -> typing.Optional[builtins.str]:
+        '''The Arn of the job execution role.
+
+        Required if job_name is None.
+        '''
         result = self._values.get("job_role_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_sample(
         self,
     ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty]:
+        '''A sample configuration for profile jobs only, which determines the number of rows on which the profile job is run.
+
+        If a ``JobSample`` value isn't provided, the default value is used. The default value is CUSTOM_ROWS for the mode parameter and 20,000 for the size parameter.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-jobsample
+        '''
         result = self._values.get("job_sample")
         return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty], result)
 
     @builtins.property
     def job_type(self) -> typing.Optional[builtins.str]:
+        '''The type of job to run.
+
+        Required if job_name is None.
+        '''
         result = self._values.get("job_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def log_subscription(self) -> typing.Optional[builtins.str]:
+        '''The current status of Amazon CloudWatch logging for the job.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-logsubscription
+        '''
         result = self._values.get("log_subscription")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_capacity(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of nodes that can be consumed when the job processes data.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-maxcapacity
+        '''
         result = self._values.get("max_capacity")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def max_retries(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of times to retry the job after a job run fails.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-maxretries
+        '''
         result = self._values.get("max_retries")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def output_location(
         self,
     ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty]:
+        '''``AWS::DataBrew::Job.OutputLocation``.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-outputlocation
+        '''
         result = self._values.get("output_location")
         return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty], result)
 
     @builtins.property
     def outputs(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty]]:
+        '''The output properties for the job.'''
         result = self._values.get("outputs")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty]], result)
 
     @builtins.property
     def profile_configuration(
         self,
     ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty]:
+        '''Configuration for profile jobs.
+
+        Configuration can be used to select columns, do evaluations, and override default parameters of evaluations. When configuration is undefined, the profile job will apply default settings to all supported columns.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-profileconfiguration
+        '''
         result = self._values.get("profile_configuration")
         return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty], result)
 
     @builtins.property
     def project_name(self) -> typing.Optional[builtins.str]:
+        '''The name of the project that the job is associated with.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-projectname
+        '''
         result = self._values.get("project_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def recipe(
         self,
     ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty]:
+        '''The recipe to be used by the DataBrew job which is a series of data transformation steps.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-recipe
+        '''
         result = self._values.get("recipe")
         return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.CfnTag]]:
+        '''Metadata tags that have been applied to the job.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-tags
+        '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.CfnTag]], result)
 
     @builtins.property
     def timeout(self) -> typing.Optional[jsii.Number]:
+        '''The job's timeout in minutes.
+
+        A job that attempts to run longer than this timeout period ends with a status of ``TIMEOUT`` .
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-timeout
+        '''
         result = self._values.get("timeout")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def validation_configurations(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty]]:
+        '''List of validation configurations that are applied to the profile job.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-databrew-job.html#cfn-databrew-job-validationconfigurations
+        '''
         result = self._values.get("validation_configurations")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5713,29 +6136,52 @@
 
 
 class DataStage(
     Stage,
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="aws-ddk-core.DataStage",
 ):
+    '''Class that represents a data stage within a data pipeline.
+
+    To create a DataStage, inherit from this class, add infrastructure required by the stage,
+    and implement ``eventPatterns`` and ``targets`` properties.
+
+    Example::
+
+        class MyStage extends DataStage:
+          readonly queue: sqs.Queue;
+        
+          constructor(scope: Construct, id: string, props: MyStageProps) {
+             super(scope, id, props);
+        
+             this.queue = sqs.Queue(this, "Queue");
+        
+             this.eventPatterns = {
+               detail_type: ["my-detail-type"],
+             };
+             this.targets = [new events_targets.SqsQueue(this.queue)];
+          }
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param alarms_enabled: 
-        :param description: 
-        :param name: 
+        '''Constructs the stage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a7ee0133925b96b521f696b544f087847c2e6916f79bbdcf76306ed73653fdb2)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DataStageProps(
             alarms_enabled=alarms_enabled, description=description, name=name
@@ -5749,20 +6195,23 @@
         id: builtins.str,
         *,
         metric: _aws_cdk_aws_cloudwatch_ceddda9d.IMetric,
         comparison_operator: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.ComparisonOperator] = None,
         evaluation_periods: typing.Optional[jsii.Number] = None,
         threshold: typing.Optional[jsii.Number] = None,
     ) -> "DataStage":
-        '''
-        :param id: -
-        :param metric: 
-        :param comparison_operator: 
-        :param evaluation_periods: 
-        :param threshold: 
+        '''Add a CloudWatch alarm for the DataStage.
+
+        :param id: Identifier of the CloudWatch Alarm.
+        :param metric: Metric to use for creating the stage's CloudWatch Alarm.
+        :param comparison_operator: Comparison operator to use for alarm. Default: GREATER_THAN_THRESHOLD
+        :param evaluation_periods: The value against which the specified alarm statistic is compared. Default: 5
+        :param threshold: The number of periods over which data is compared to the specified threshold. Default: 1
+
+        :return: this DataStage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dfe170c2325021dad043fac92cbbedf46c28aacb0956794521a87dbad31593a0)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = AlarmProps(
             metric=metric,
             comparison_operator=comparison_operator,
@@ -5771,19 +6220,21 @@
         )
 
         return typing.cast("DataStage", jsii.invoke(self, "addAlarm", [id, props]))
 
     @builtins.property
     @jsii.member(jsii_name="alarmsEnabled")
     def alarms_enabled(self) -> builtins.bool:
+        '''Flag indicating whether the alarms are enabled for this stage.'''
         return typing.cast(builtins.bool, jsii.get(self, "alarmsEnabled"))
 
     @builtins.property
     @jsii.member(jsii_name="cloudwatchAlarms")
     def cloudwatch_alarms(self) -> typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.Alarm]:
+        '''List of CloudWatch Alarms linked to the stage.'''
         return typing.cast(typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.Alarm], jsii.get(self, "cloudwatchAlarms"))
 
 
 class _DataStageProxy(
     DataStage,
     jsii.proxy_for(Stage), # type: ignore[misc]
 ):
@@ -5806,18 +6257,19 @@
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param alarms_enabled: 
+        '''Properties for the ``DataStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1cf78e5b7c077cc8d8a6b8227060c5d2b68df15e3f29e358244b75ef0b897e42)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -5826,24 +6278,30 @@
         if name is not None:
             self._values["name"] = name
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in a DataStage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5856,41 +6314,67 @@
 
 
 class EventStage(
     Stage,
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="aws-ddk-core.EventStage",
 ):
+    '''Class that represents an event stage within a data pipeline.
+
+    To create an EventStage, inherit from this class, add infrastructure required by the stage,
+    and implement the ``eventPattern`` property.
+
+    The ``targets`` property will be set to null.
+
+    Example::
+
+        class MyStage extends EventStage:
+          constructor(scope: Construct, id: string, props: MyStageProps) {
+             super(scope, id, props);
+        
+             this.eventPatterns = {
+               source: ["aws.s3"],
+               detail: props.detail,
+               detail_type: props.detail_type,
+             };
+          }
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param description: 
-        :param name: 
+        '''Constructs event stage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__41f4bcf520b1f5e4739a71110428c14cbff5ea45be37a68ea1fe04dbffd91d83)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = EventStageProps(description=description, name=name)
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 class _EventStageProxy(
     EventStage,
     jsii.proxy_for(Stage), # type: ignore[misc]
 ):
@@ -5908,35 +6392,38 @@
 class EventStageProps(StageProps):
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
+        '''Properties for the event stage.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f2768fcf39322e444b8b05e9cfa0508e071c34b9e8a29e28fc79130506d7aeb6)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5949,14 +6436,16 @@
 
 
 class FirehoseToS3Stage(
     DataStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.FirehoseToS3Stage",
 ):
+    '''DDK Kinesis Firehose Delivery stream to S3 stage, with an optional Kinesis Data Stream.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         data_output_prefix: typing.Optional[builtins.str] = None,
         data_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream] = None,
@@ -5968,30 +6457,31 @@
         kinesis_firehose_destinations_s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
         s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param data_output_prefix: 
-        :param data_stream: 
-        :param data_stream_enabled: 
-        :param delivery_stream_data_freshness_errors_alarm_threshold: 
-        :param delivery_stream_data_freshness_errors_evaluation_periods: 
-        :param firehose_delivery_stream: 
-        :param firehose_delivery_stream_props: 
-        :param kinesis_firehose_destinations_s3_bucket_props: 
-        :param s3_bucket: 
-        :param s3_bucket_props: 
-        :param alarms_enabled: 
-        :param description: 
-        :param name: 
+        '''Constructs ``FirehoseToS3Stage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param data_output_prefix: A prefix that Kinesis Data Firehose evaluates and adds to records before writing them to S3. This prefix appears immediately following the bucket name. Default: “YYYY/MM/DD/HH”
+        :param data_stream: Preexisting Kinesis Data Stream to use in stage before Delivery Stream. Setting this parameter will override any creation of Kinesis Data Streams in this stage. The ``dataStreamEnabled`` parameter will have no effect.
+        :param data_stream_enabled: Add Kinesis Data Stream to front Firehose Delivery. Default: false
+        :param delivery_stream_data_freshness_errors_alarm_threshold: Threshold for Cloudwatch Alarm created for this stage. Default: 900
+        :param delivery_stream_data_freshness_errors_evaluation_periods: Evaluation period value for Cloudwatch alarm created for this stage. Default: 1
+        :param firehose_delivery_stream: Firehose Delivery stream. If no stram is provided, a new one is created.
+        :param firehose_delivery_stream_props: Properties of the Firehose Delivery stream to be created.
+        :param kinesis_firehose_destinations_s3_bucket_props: Props for defining an S3 destination of a Kinesis Data Firehose delivery stream.
+        :param s3_bucket: Preexisting S3 Bucket to use as a destination for the Firehose Stream. If no bucket is provided, a new one is created. Amazon EventBridge notifications must be enabled on the bucket in order for this stage to produce events after its completion.
+        :param s3_bucket_props: Properties of the S3 Bucket to be created as a delivery destination. Amazon EventBridge notifications must be enabled on the bucket in order for this stage to produce events after its completion.
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3f9217104050cf03ef7cf7519808ce659edfe6c1ba00722ea6601239921cfd56)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FirehoseToS3StageProps(
             data_output_prefix=data_output_prefix,
@@ -6029,21 +6519,30 @@
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream], jsii.get(self, "dataStream"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.FirehoseToS3StageProps",
     jsii_struct_bases=[DataStageProps],
     name_mapping={
@@ -6076,28 +6575,29 @@
         delivery_stream_data_freshness_errors_evaluation_periods: typing.Optional[jsii.Number] = None,
         firehose_delivery_stream: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream] = None,
         firehose_delivery_stream_props: typing.Optional[typing.Union[DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
         kinesis_firehose_destinations_s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
         s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param alarms_enabled: 
-        :param data_output_prefix: 
-        :param data_stream: 
-        :param data_stream_enabled: 
-        :param delivery_stream_data_freshness_errors_alarm_threshold: 
-        :param delivery_stream_data_freshness_errors_evaluation_periods: 
-        :param firehose_delivery_stream: 
-        :param firehose_delivery_stream_props: 
-        :param kinesis_firehose_destinations_s3_bucket_props: 
-        :param s3_bucket: 
-        :param s3_bucket_props: 
+        '''Properties for ``FirehoseToS3Stage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param data_output_prefix: A prefix that Kinesis Data Firehose evaluates and adds to records before writing them to S3. This prefix appears immediately following the bucket name. Default: “YYYY/MM/DD/HH”
+        :param data_stream: Preexisting Kinesis Data Stream to use in stage before Delivery Stream. Setting this parameter will override any creation of Kinesis Data Streams in this stage. The ``dataStreamEnabled`` parameter will have no effect.
+        :param data_stream_enabled: Add Kinesis Data Stream to front Firehose Delivery. Default: false
+        :param delivery_stream_data_freshness_errors_alarm_threshold: Threshold for Cloudwatch Alarm created for this stage. Default: 900
+        :param delivery_stream_data_freshness_errors_evaluation_periods: Evaluation period value for Cloudwatch alarm created for this stage. Default: 1
+        :param firehose_delivery_stream: Firehose Delivery stream. If no stram is provided, a new one is created.
+        :param firehose_delivery_stream_props: Properties of the Firehose Delivery stream to be created.
+        :param kinesis_firehose_destinations_s3_bucket_props: Props for defining an S3 destination of a Kinesis Data Firehose delivery stream.
+        :param s3_bucket: Preexisting S3 Bucket to use as a destination for the Firehose Stream. If no bucket is provided, a new one is created. Amazon EventBridge notifications must be enabled on the bucket in order for this stage to produce events after its completion.
+        :param s3_bucket_props: Properties of the S3 Bucket to be created as a delivery destination. Amazon EventBridge notifications must be enabled on the bucket in order for this stage to produce events after its completion.
         '''
         if isinstance(firehose_delivery_stream_props, dict):
             firehose_delivery_stream_props = DeliveryStreamProps(**firehose_delivery_stream_props)
         if isinstance(kinesis_firehose_destinations_s3_bucket_props, dict):
             kinesis_firehose_destinations_s3_bucket_props = _aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps(**kinesis_firehose_destinations_s3_bucket_props)
         if isinstance(s3_bucket_props, dict):
             s3_bucket_props = _aws_cdk_aws_s3_ceddda9d.BucketProps(**s3_bucket_props)
@@ -6142,82 +6642,130 @@
         if s3_bucket is not None:
             self._values["s3_bucket"] = s3_bucket
         if s3_bucket_props is not None:
             self._values["s3_bucket_props"] = s3_bucket_props
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in a DataStage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def data_output_prefix(self) -> typing.Optional[builtins.str]:
+        '''A prefix that Kinesis Data Firehose evaluates and adds to records before writing them to S3.
+
+        This prefix appears immediately following the bucket name.
+
+        :default: “YYYY/MM/DD/HH”
+        '''
         result = self._values.get("data_output_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def data_stream(self) -> typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream]:
+        '''Preexisting Kinesis Data Stream to use in stage before Delivery Stream.
+
+        Setting this parameter will override any creation of Kinesis Data Streams
+        in this stage.
+        The ``dataStreamEnabled`` parameter will have no effect.
+        '''
         result = self._values.get("data_stream")
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream], result)
 
     @builtins.property
     def data_stream_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Add Kinesis Data Stream to front Firehose Delivery.
+
+        :default: false
+        '''
         result = self._values.get("data_stream_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def delivery_stream_data_freshness_errors_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''Threshold for Cloudwatch Alarm created for this stage.
+
+        :default: 900
+        '''
         result = self._values.get("delivery_stream_data_freshness_errors_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def delivery_stream_data_freshness_errors_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''Evaluation period value for Cloudwatch alarm created for this stage.
+
+        :default: 1
+        '''
         result = self._values.get("delivery_stream_data_freshness_errors_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def firehose_delivery_stream(
         self,
     ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream]:
+        '''Firehose Delivery stream.
+
+        If no stram is provided, a new one is created.
+        '''
         result = self._values.get("firehose_delivery_stream")
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream], result)
 
     @builtins.property
     def firehose_delivery_stream_props(self) -> typing.Optional[DeliveryStreamProps]:
+        '''Properties of the Firehose Delivery stream to be created.'''
         result = self._values.get("firehose_delivery_stream_props")
         return typing.cast(typing.Optional[DeliveryStreamProps], result)
 
     @builtins.property
     def kinesis_firehose_destinations_s3_bucket_props(
         self,
     ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps]:
+        '''Props for defining an S3 destination of a Kinesis Data Firehose delivery stream.'''
         result = self._values.get("kinesis_firehose_destinations_s3_bucket_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps], result)
 
     @builtins.property
     def s3_bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+        '''Preexisting S3 Bucket to use as a destination for the Firehose Stream.
+
+        If no bucket is provided, a new one is created.
+
+        Amazon EventBridge notifications must be enabled on the bucket in order
+        for this stage to produce events after its completion.
+        '''
         result = self._values.get("s3_bucket")
         return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
 
     @builtins.property
     def s3_bucket_props(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.BucketProps]:
+        '''Properties of the S3 Bucket to be created as a delivery destination.
+
+        Amazon EventBridge notifications must be enabled on the bucket in order
+        for this stage to produce events after its completion.
+        '''
         result = self._values.get("s3_bucket_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.BucketProps], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -6276,35 +6824,36 @@
         job_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_alpha_ce674d29.JobProps, typing.Dict[builtins.str, typing.Any]]] = None,
         job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
         state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
         targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param crawler_allow_failure: 
-        :param crawler_name: 
-        :param crawler_props: 
-        :param crawler_role: 
-        :param database_name: 
-        :param job_name: 
-        :param job_props: 
-        :param job_run_args: 
-        :param state_machine_retry_backoff_rate: 
-        :param state_machine_retry_interval: 
-        :param state_machine_retry_max_attempts: 
-        :param targets: 
+        '''Properties for ``GlueTransformStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param crawler_allow_failure: Argument to allow stepfunction success for crawler failures/execption like Glue.CrawlerRunningException. Default: true
+        :param crawler_name: The name of a preexisting Glue crawler to run. If None, a Glue crawler is created.
+        :param crawler_props: Properties for the Glue Crawler.
+        :param crawler_role: The crawler execution role.
+        :param database_name: The name of the database in which the crawler's output is stored.
+        :param job_name: The name of a preexisting Glue job to run. If None, a Glue job is created.
+        :param job_props: Additional Glue job properties. For complete list of properties refer to CDK Documentation
+        :param job_run_args: The input arguments to the Glue job.
+        :param state_machine_retry_backoff_rate: Multiplication for how much longer the wait interval gets on every retry. Default: 2
+        :param state_machine_retry_interval: How many seconds to wait initially before retrying. Default: cdk.Duration.seconds(1)
+        :param state_machine_retry_max_attempts: How many times to retry this particular error. Default: 3
+        :param targets: A collection of targets to crawl.
         '''
         if isinstance(crawler_props, dict):
             crawler_props = _aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps(**crawler_props)
         if isinstance(job_props, dict):
             job_props = _aws_cdk_aws_glue_alpha_ce674d29.JobProps(**job_props)
         if isinstance(targets, dict):
             targets = _aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty(**targets)
@@ -6370,123 +6919,179 @@
         if state_machine_retry_max_attempts is not None:
             self._values["state_machine_retry_max_attempts"] = state_machine_retry_max_attempts
         if targets is not None:
             self._values["targets"] = targets
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def additional_role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
         result = self._values.get("additional_role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
         result = self._values.get("state_machine_input")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
         result = self._values.get("state_machine_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def crawler_allow_failure(self) -> typing.Optional[builtins.bool]:
+        '''Argument to allow stepfunction success for crawler failures/execption like Glue.CrawlerRunningException.
+
+        :default: true
+        '''
         result = self._values.get("crawler_allow_failure")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def crawler_name(self) -> typing.Optional[builtins.str]:
+        '''The name of a preexisting Glue crawler to run.
+
+        If None, a Glue crawler is created.
+        '''
         result = self._values.get("crawler_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def crawler_props(
         self,
     ) -> typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps]:
+        '''Properties for the Glue Crawler.
+
+        :link: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_glue.CfnCrawler.html
+        '''
         result = self._values.get("crawler_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps], result)
 
     @builtins.property
     def crawler_role(self) -> typing.Optional[builtins.str]:
+        '''The crawler execution role.'''
         result = self._values.get("crawler_role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def database_name(self) -> typing.Optional[builtins.str]:
+        '''The name of the database in which the crawler's output is stored.'''
         result = self._values.get("database_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_name(self) -> typing.Optional[builtins.str]:
+        '''The name of a preexisting Glue job to run.
+
+        If None, a Glue job is created.
+        '''
         result = self._values.get("job_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_props(self) -> typing.Optional[_aws_cdk_aws_glue_alpha_ce674d29.JobProps]:
+        '''Additional Glue job properties.
+
+        For complete list of properties refer to CDK Documentation
+
+        :aws-cdk_aws-glue-alpha: .Job.html
+        :link: https://docs.aws.amazon.com/cdk/api/v2/docs/
+        '''
         result = self._values.get("job_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_glue_alpha_ce674d29.JobProps], result)
 
     @builtins.property
     def job_run_args(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''The input arguments to the Glue job.'''
         result = self._values.get("job_run_args")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_retry_backoff_rate(self) -> typing.Optional[jsii.Number]:
+        '''Multiplication for how much longer the wait interval gets on every retry.
+
+        :default: 2
+        '''
         result = self._values.get("state_machine_retry_backoff_rate")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_retry_interval(
         self,
     ) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''How many seconds to wait initially before retrying.
+
+        :default: cdk.Duration.seconds(1)
+        '''
         result = self._values.get("state_machine_retry_interval")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def state_machine_retry_max_attempts(self) -> typing.Optional[jsii.Number]:
+        '''How many times to retry this particular error.
+
+        :default: 3
+        '''
         result = self._values.get("state_machine_retry_max_attempts")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def targets(
         self,
     ) -> typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty]:
+        '''A collection of targets to crawl.'''
         result = self._values.get("targets")
         return typing.cast(typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -6531,28 +7136,29 @@
         state_machine_name: typing.Optional[builtins.str] = None,
         redshift_cluster_identifier: builtins.str,
         sql_statements: typing.Sequence[builtins.str],
         database_name: typing.Optional[builtins.str] = None,
         database_user: typing.Optional[builtins.str] = None,
         polling_time: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param redshift_cluster_identifier: 
-        :param sql_statements: 
-        :param database_name: 
-        :param database_user: 
-        :param polling_time: 
+        '''Properties for ``RedshiftDataApiStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param redshift_cluster_identifier: Identifier of the Redshift cluster.
+        :param sql_statements: List of SQL statements to execute.
+        :param database_name: Name of the database in Redshift. Default: "dev"
+        :param database_user: Database user. Default: "awsuser"
+        :param polling_time: Waiting time between checking whether the statements have finished executing. Default: cdk.Duration.seconds(15)
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__defbc9333f2b8b3e2d55373f9b0155e5f6e83609e9153dc24f619d747ca4f133)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
@@ -6590,84 +7196,115 @@
         if database_user is not None:
             self._values["database_user"] = database_user
         if polling_time is not None:
             self._values["polling_time"] = polling_time
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def additional_role_policy_statements(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
         result = self._values.get("additional_role_policy_statements")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_failed_executions_alarm_threshold(
         self,
     ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
         result = self._values.get("state_machine_failed_executions_alarm_threshold")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
         result = self._values.get("state_machine_input")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
 
     @builtins.property
     def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
         result = self._values.get("state_machine_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def redshift_cluster_identifier(self) -> builtins.str:
+        '''Identifier of the Redshift cluster.'''
         result = self._values.get("redshift_cluster_identifier")
         assert result is not None, "Required property 'redshift_cluster_identifier' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def sql_statements(self) -> typing.List[builtins.str]:
+        '''List of SQL statements to execute.'''
         result = self._values.get("sql_statements")
         assert result is not None, "Required property 'sql_statements' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def database_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the database in Redshift.
+
+        :default: "dev"
+        '''
         result = self._values.get("database_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def database_user(self) -> typing.Optional[builtins.str]:
+        '''Database user.
+
+        :default: "awsuser"
+        '''
         result = self._values.get("database_user")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def polling_time(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''Waiting time between checking whether the statements have finished executing.
+
+        :default: cdk.Duration.seconds(15)
+        '''
         result = self._values.get("polling_time")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -6680,33 +7317,39 @@
 
 
 class S3EventStage(
     EventStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.S3EventStage",
 ):
+    '''Stage implements an S3 event pattern based on event names, a bucket name and optional key prefix.
+
+    Amazon EventBridge notifications must be enabled on the bucket in order to use this construct.
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         bucket: typing.Union[_aws_cdk_aws_s3_ceddda9d.IBucket, typing.Sequence[_aws_cdk_aws_s3_ceddda9d.IBucket]],
         event_names: typing.Sequence[builtins.str],
         key_prefix: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param bucket: 
-        :param event_names: 
-        :param key_prefix: 
-        :param description: 
-        :param name: 
+        '''Constructs ``S3EventStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param bucket: S3 Bucket or list of buckets. Amazon EventBridge notifications must be enabled on the bucket in order to use this construct.
+        :param event_names: The list of events to capture, for example: ["Object Created"].
+        :param key_prefix: The S3 prefix or list of prefixes. Capture root level prefix ("/") by default.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__faeff4d3ae690cf668837c5bb7641744355445bfe3e6990816e841afad5a577f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = S3EventStageProps(
             bucket=bucket,
@@ -6719,14 +7362,19 @@
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.S3EventStageProps",
     jsii_struct_bases=[EventStageProps],
     name_mapping={
@@ -6743,20 +7391,21 @@
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         bucket: typing.Union[_aws_cdk_aws_s3_ceddda9d.IBucket, typing.Sequence[_aws_cdk_aws_s3_ceddda9d.IBucket]],
         event_names: typing.Sequence[builtins.str],
         key_prefix: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param bucket: 
-        :param event_names: 
-        :param key_prefix: 
+        '''Properties for ``S3EventStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param bucket: S3 Bucket or list of buckets. Amazon EventBridge notifications must be enabled on the bucket in order to use this construct.
+        :param event_names: The list of events to capture, for example: ["Object Created"].
+        :param key_prefix: The S3 prefix or list of prefixes. Capture root level prefix ("/") by default.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b66fa30f9df5c5a39526206778107c9f4992a0d357e41d5469d45e647a206a90)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
             check_type(argname="argument event_names", value=event_names, expected_type=type_hints["event_names"])
@@ -6770,40 +7419,54 @@
         if name is not None:
             self._values["name"] = name
         if key_prefix is not None:
             self._values["key_prefix"] = key_prefix
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def bucket(
         self,
     ) -> typing.Union[_aws_cdk_aws_s3_ceddda9d.IBucket, typing.List[_aws_cdk_aws_s3_ceddda9d.IBucket]]:
+        '''S3 Bucket or list of buckets.
+
+        Amazon EventBridge notifications must be enabled on the bucket in order to use this construct.
+        '''
         result = self._values.get("bucket")
         assert result is not None, "Required property 'bucket' is missing"
         return typing.cast(typing.Union[_aws_cdk_aws_s3_ceddda9d.IBucket, typing.List[_aws_cdk_aws_s3_ceddda9d.IBucket]], result)
 
     @builtins.property
     def event_names(self) -> typing.List[builtins.str]:
+        '''The list of events to capture, for example: ["Object Created"].
+
+        :link: https://docs.aws.amazon.com/AmazonS3/latest/userguide/EventBridge.html
+        '''
         result = self._values.get("event_names")
         assert result is not None, "Required property 'event_names' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def key_prefix(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, typing.List[builtins.str]]]:
+        '''The S3 prefix or list of prefixes.
+
+        Capture root level prefix ("/") by default.
+        '''
         result = self._values.get("key_prefix")
         return typing.cast(typing.Optional[typing.Union[builtins.str, typing.List[builtins.str]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -6816,14 +7479,16 @@
 
 
 class SqsToLambdaStage(
     DataStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.SqsToLambdaStage",
 ):
+    '''Stage implements an Amazon SQS queue connected to an AWS Lambda function, with an optional DLQ.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         batch_size: typing.Optional[jsii.Number] = None,
         dlq_enabled: typing.Optional[builtins.bool] = None,
@@ -6834,29 +7499,30 @@
         message_group_id: typing.Optional[builtins.str] = None,
         sqs_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
         sqs_queue_props: typing.Optional[typing.Union[_aws_cdk_aws_sqs_ceddda9d.QueueProps, typing.Dict[builtins.str, typing.Any]]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param batch_size: 
-        :param dlq_enabled: 
-        :param lambda_function: 
-        :param lambda_function_props: 
-        :param max_batching_window: 
-        :param max_receive_count: 
-        :param message_group_id: 
-        :param sqs_queue: 
-        :param sqs_queue_props: 
-        :param alarms_enabled: 
-        :param description: 
-        :param name: 
+        '''Constructs ``SqsToLambdaStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param batch_size: The maximum number of records retrieved from the event source at the function invocation time. Default: 10
+        :param dlq_enabled: Determines if DLQ is enabled. Default: false
+        :param lambda_function: Preexisting Lambda Function to use in stage. If not provided, a new function will be created.
+        :param lambda_function_props: Properties for the Lambda Function that will be created by this construct (if ``lambdaFunction`` is not provided).
+        :param max_batching_window: The maximum amount of time to gather records before invoking the function. Valid Range: Minimum value of 0 minutes, maximum value of 5 minutes. Default: - no batching window.
+        :param max_receive_count: The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue. Default: 1
+        :param message_group_id: Message Group ID for messages sent to this queue. Required for FIFO queues.
+        :param sqs_queue: Preexisting SQS Queue to use in stage. If not provided, a new queue will be created.
+        :param sqs_queue_props: Properties for the SQS Queue that will be created by this construct (if ``sqsQueue`` is not provided).
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b5be1a85b67aa2deae08f66dcc56eb002282a0b357ba91df9339c1c9e2cb7401)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SqsToLambdaStageProps(
             batch_size=batch_size,
@@ -6891,21 +7557,30 @@
         return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue], jsii.get(self, "deadLetterQueue"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.SqsToLambdaStageProps",
     jsii_struct_bases=[DataStageProps],
     name_mapping={
@@ -6936,27 +7611,28 @@
         lambda_function_props: typing.Optional[typing.Union[SqsToLambdaStageFunctionProps, typing.Dict[builtins.str, typing.Any]]] = None,
         max_batching_window: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         max_receive_count: typing.Optional[jsii.Number] = None,
         message_group_id: typing.Optional[builtins.str] = None,
         sqs_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
         sqs_queue_props: typing.Optional[typing.Union[_aws_cdk_aws_sqs_ceddda9d.QueueProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param alarms_enabled: 
-        :param batch_size: 
-        :param dlq_enabled: 
-        :param lambda_function: 
-        :param lambda_function_props: 
-        :param max_batching_window: 
-        :param max_receive_count: 
-        :param message_group_id: 
-        :param sqs_queue: 
-        :param sqs_queue_props: 
+        '''Properties for ``SqsToLambdaStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param batch_size: The maximum number of records retrieved from the event source at the function invocation time. Default: 10
+        :param dlq_enabled: Determines if DLQ is enabled. Default: false
+        :param lambda_function: Preexisting Lambda Function to use in stage. If not provided, a new function will be created.
+        :param lambda_function_props: Properties for the Lambda Function that will be created by this construct (if ``lambdaFunction`` is not provided).
+        :param max_batching_window: The maximum amount of time to gather records before invoking the function. Valid Range: Minimum value of 0 minutes, maximum value of 5 minutes. Default: - no batching window.
+        :param max_receive_count: The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue. Default: 1
+        :param message_group_id: Message Group ID for messages sent to this queue. Required for FIFO queues.
+        :param sqs_queue: Preexisting SQS Queue to use in stage. If not provided, a new queue will be created.
+        :param sqs_queue_props: Properties for the SQS Queue that will be created by this construct (if ``sqsQueue`` is not provided).
         '''
         if isinstance(lambda_function_props, dict):
             lambda_function_props = SqsToLambdaStageFunctionProps(**lambda_function_props)
         if isinstance(sqs_queue_props, dict):
             sqs_queue_props = _aws_cdk_aws_sqs_ceddda9d.QueueProps(**sqs_queue_props)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6ea408fc3fa64f721e1e8e8f5dba2b0b6340914a77963785a7642a5943b0a04a)
@@ -6996,71 +7672,108 @@
         if sqs_queue is not None:
             self._values["sqs_queue"] = sqs_queue
         if sqs_queue_props is not None:
             self._values["sqs_queue_props"] = sqs_queue_props
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in a DataStage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def batch_size(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of records retrieved from the event source at the function invocation time.
+
+        :default: 10
+        '''
         result = self._values.get("batch_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def dlq_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Determines if DLQ is enabled.
+
+        :default: false
+        '''
         result = self._values.get("dlq_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def lambda_function(
         self,
     ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction]:
+        '''Preexisting Lambda Function to use in stage.
+
+        If not provided, a new function will be created.
+        '''
         result = self._values.get("lambda_function")
         return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction], result)
 
     @builtins.property
     def lambda_function_props(self) -> typing.Optional[SqsToLambdaStageFunctionProps]:
+        '''Properties for the Lambda Function that will be created by this construct (if ``lambdaFunction`` is not provided).'''
         result = self._values.get("lambda_function_props")
         return typing.cast(typing.Optional[SqsToLambdaStageFunctionProps], result)
 
     @builtins.property
     def max_batching_window(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''The maximum amount of time to gather records before invoking the function.
+
+        Valid Range: Minimum value of 0 minutes, maximum value of 5 minutes.
+        Default: - no batching window.
+        '''
         result = self._values.get("max_batching_window")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def max_receive_count(self) -> typing.Optional[jsii.Number]:
+        '''The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue.
+
+        :default: 1
+        '''
         result = self._values.get("max_receive_count")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def message_group_id(self) -> typing.Optional[builtins.str]:
+        '''Message Group ID for messages sent to this queue.
+
+        Required for FIFO queues.
+        '''
         result = self._values.get("message_group_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sqs_queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue]:
+        '''Preexisting SQS Queue to use in stage.
+
+        If not provided, a new queue will be created.
+        '''
         result = self._values.get("sqs_queue")
         return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue], result)
 
     @builtins.property
     def sqs_queue_props(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.QueueProps]:
+        '''Properties for the SQS Queue that will be created by this construct (if ``sqsQueue`` is not provided).'''
         result = self._values.get("sqs_queue_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.QueueProps], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -7073,39 +7786,42 @@
 
 
 class StateMachineStage(
     DataStage,
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="aws-ddk-core.StateMachineStage",
 ):
+    '''DataStage with helper methods to simplify StateMachine stages creation.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs state machine stage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c9ccc4da0d6d8eb11cda39b2839889ebd93235f90bbfbdd93a92a3f816c9fd60)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = StateMachineStageProps(
             additional_role_policy_statements=additional_role_policy_statements,
@@ -7130,24 +7846,27 @@
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> CreateStateMachineResult:
-        '''
-        :param definition: -
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs a state machine from the definition.
+
+        :param definition: Steps for the state machine.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+
+        :return: Dictionary with event pattern, targets and state machine construct.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__642bc4c0673f5b0f2331c42eaeb1c12c1c4fce53646416b8e239dd0bd724b5d2)
             check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
         props = StateMachineStageProps(
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
@@ -7161,35 +7880,42 @@
 
         return typing.cast(CreateStateMachineResult, jsii.invoke(self, "createStateMachine", [definition, props]))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     @abc.abstractmethod
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         ...
 
 
 class _StateMachineStageProxy(
     StateMachineStage,
     jsii.proxy_for(DataStage), # type: ignore[misc]
 ):
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, StateMachineStage).__jsii_proxy_class__ = lambda : _StateMachineStageProxy
 
 
 class AppFlowIngestionStage(
     StateMachineStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.AppFlowIngestionStage",
 ):
+    '''Stage that contains a step function that runs an AppFlow flow ingestion.
+
+    If the AppFlow flow name is not supplied, then the flow is created.
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         destination_flow_config: typing.Optional[typing.Union[_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         flow_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
@@ -7201,30 +7927,31 @@
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param destination_flow_config: 
-        :param flow_execution_status_check_period: 
-        :param flow_name: 
-        :param flow_tasks: 
-        :param source_flow_config: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs AppFlowIngestionStage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param destination_flow_config: The flow ``appflow.CfnFlow.DestinationFlowConfigProperty`` properties.
+        :param flow_execution_status_check_period: Time to wait between flow execution status checks. Default: aws_cdk.Duration.seconds(15)
+        :param flow_name: Name of the AppFlow flow to run. If None, an AppFlow flow is created.
+        :param flow_tasks: The flow tasks properties.
+        :param source_flow_config: The flow ``appflow.CfnFlow.SourceFlowConfigProperty`` properties.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__75fdc83ac05ea2b4078c2c89fa4beb028f1353a28c899b42364d275a692f3594)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = AppFlowIngestionStageProps(
             destination_flow_config=destination_flow_config,
@@ -7253,88 +7980,104 @@
     @jsii.member(jsii_name="flowObject")
     def flow_object(self) -> _aws_cdk_aws_stepfunctions_tasks_ceddda9d.CallAwsService:
         return typing.cast(_aws_cdk_aws_stepfunctions_tasks_ceddda9d.CallAwsService, jsii.get(self, "flowObject"))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 class AthenaSQLStage(
     StateMachineStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.AthenaSQLStage",
 ):
+    '''Stage that contains a step function that execute Athena SQL query.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         catalog_name: typing.Optional[builtins.str] = None,
         database_name: typing.Optional[builtins.str] = None,
         encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key] = None,
         encryption_option: typing.Optional[_aws_cdk_aws_stepfunctions_tasks_ceddda9d.EncryptionOption] = None,
         output_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
-        query_string: typing.Optional[builtins.str] = None,
+        parallel: typing.Optional[builtins.bool] = None,
+        query_string: typing.Optional[typing.Sequence[builtins.str]] = None,
         query_string_path: typing.Optional[builtins.str] = None,
         work_group: typing.Optional[builtins.str] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param catalog_name: 
-        :param database_name: 
-        :param encryption_key: 
-        :param encryption_option: 
-        :param output_location: 
-        :param query_string: 
-        :param query_string_path: 
-        :param work_group: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs ``AthenaSQLStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param catalog_name: Catalog name.
+        :param database_name: Database name.
+        :param encryption_key: Encryption KMS key.
+        :param encryption_option: Encryption configuration.
+        :param output_location: Output S3 location.
+        :param parallel: flag to determine parallel or sequential execution. Default: false
+        :param query_string: SQL queries that will be started.
+        :param query_string_path: dynamic path in statemachine for SQL query to be started.
+        :param work_group: Athena workgroup name.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__51d1732123dc8ece0c4c19240b905f56cb50227d150f624d8b798a82b65cbe29)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = AthenaToSQLStageProps(
             catalog_name=catalog_name,
             database_name=database_name,
             encryption_key=encryption_key,
             encryption_option=encryption_option,
             output_location=output_location,
+            parallel=parallel,
             query_string=query_string,
             query_string_path=query_string_path,
             work_group=work_group,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
@@ -7345,48 +8088,60 @@
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
 
     @builtins.property
     @jsii.member(jsii_name="eventBridgeEventPath")
     def event_bridge_event_path(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "eventBridgeEventPath"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachineInput")
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "stateMachineInput"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 class DataBrewTransformStage(
     StateMachineStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.DataBrewTransformStage",
 ):
+    '''Stage that contains a step function that runs DataBrew job.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         create_job: typing.Optional[builtins.bool] = None,
         database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
@@ -7414,46 +8169,47 @@
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param create_job: 
-        :param database_outputs: 
-        :param data_catalog_outputs: 
-        :param dataset_name: 
-        :param encryption_key_arn: 
-        :param encryption_mode: 
-        :param job_name: 
-        :param job_role_arn: 
-        :param job_sample: 
-        :param job_type: 
-        :param log_subscription: 
-        :param max_capacity: 
-        :param max_retries: 
-        :param output_location: 
-        :param outputs: 
-        :param profile_configuration: 
-        :param project_name: 
-        :param recipe: 
-        :param tags: 
-        :param timeout: 
-        :param validation_configurations: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs ``DataBrewTransformStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param create_job: Whether to create the DataBrew job or not.
+        :param database_outputs: Represents a list of JDBC database output objects which defines the output destination for a DataBrew recipe job to write into.
+        :param data_catalog_outputs: One or more artifacts that represent the AWS Glue Data Catalog output from running the job.
+        :param dataset_name: The name of the dataset to use for the job.
+        :param encryption_key_arn: The Amazon Resource Name (ARN) of an encryption key that is used to protect the job output. For more information, see `Encrypting data written by DataBrew jobs <https://docs.aws.amazon.com/databrew/latest/dg/encryption-security-configuration.html>`_
+        :param encryption_mode: The encryption mode for the job, which can be one of the following:. - ``SSE-KMS`` - Server-side encryption with keys managed by AWS KMS . - ``SSE-S3`` - Server-side encryption with keys managed by Amazon S3.
+        :param job_name: The name of a preexisting DataBrew job to run. If None, a DataBrew job is created.
+        :param job_role_arn: The Arn of the job execution role. Required if job_name is None.
+        :param job_sample: A sample configuration for profile jobs only, which determines the number of rows on which the profile job is run. If a ``JobSample`` value isn't provided, the default value is used. The default value is CUSTOM_ROWS for the mode parameter and 20,000 for the size parameter.
+        :param job_type: The type of job to run. Required if job_name is None.
+        :param log_subscription: The current status of Amazon CloudWatch logging for the job.
+        :param max_capacity: The maximum number of nodes that can be consumed when the job processes data.
+        :param max_retries: The maximum number of times to retry the job after a job run fails.
+        :param output_location: ``AWS::DataBrew::Job.OutputLocation``.
+        :param outputs: The output properties for the job.
+        :param profile_configuration: Configuration for profile jobs. Configuration can be used to select columns, do evaluations, and override default parameters of evaluations. When configuration is undefined, the profile job will apply default settings to all supported columns.
+        :param project_name: The name of the project that the job is associated with.
+        :param recipe: The recipe to be used by the DataBrew job which is a series of data transformation steps.
+        :param tags: Metadata tags that have been applied to the job.
+        :param timeout: The job's timeout in minutes. A job that attempts to run longer than this timeout period ends with a status of ``TIMEOUT`` .
+        :param validation_configurations: List of validation configurations that are applied to the profile job.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a9214d4641d831e11d83d601cf5e13ef25bd3d55977b689c3cefd7aaa9fb0fb5)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DataBrewTransformStageProps(
             create_job=create_job,
@@ -7498,41 +8254,56 @@
     @jsii.member(jsii_name="jobName")
     def job_name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "jobName"))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="job")
     def job(self) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob]:
         return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob], jsii.get(self, "job"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 class GlueTransformStage(
     StateMachineStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.GlueTransformStage",
 ):
+    '''Stage that contains a step function that runs Glue job, and a Glue crawler afterwards.
+
+    If the Glue job or crawler names are not supplied, then they are created.
+    '''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         crawler_allow_failure: typing.Optional[builtins.bool] = None,
         crawler_name: typing.Optional[builtins.str] = None,
@@ -7551,37 +8322,38 @@
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param crawler_allow_failure: 
-        :param crawler_name: 
-        :param crawler_props: 
-        :param crawler_role: 
-        :param database_name: 
-        :param job_name: 
-        :param job_props: 
-        :param job_run_args: 
-        :param state_machine_retry_backoff_rate: 
-        :param state_machine_retry_interval: 
-        :param state_machine_retry_max_attempts: 
-        :param targets: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs ``GlueTransformStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param crawler_allow_failure: Argument to allow stepfunction success for crawler failures/execption like Glue.CrawlerRunningException. Default: true
+        :param crawler_name: The name of a preexisting Glue crawler to run. If None, a Glue crawler is created.
+        :param crawler_props: Properties for the Glue Crawler.
+        :param crawler_role: The crawler execution role.
+        :param database_name: The name of the database in which the crawler's output is stored.
+        :param job_name: The name of a preexisting Glue job to run. If None, a Glue job is created.
+        :param job_props: Additional Glue job properties. For complete list of properties refer to CDK Documentation
+        :param job_run_args: The input arguments to the Glue job.
+        :param state_machine_retry_backoff_rate: Multiplication for how much longer the wait interval gets on every retry. Default: 2
+        :param state_machine_retry_interval: How many seconds to wait initially before retrying. Default: cdk.Duration.seconds(1)
+        :param state_machine_retry_max_attempts: How many times to retry this particular error. Default: 3
+        :param targets: A collection of targets to crawl.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8ddc56c43fee5e5dc6737d945cf18cb6800a5b74340125036ae173083ba761f2)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = GlueTransformStageProps(
             crawler_allow_failure=crawler_allow_failure,
@@ -7612,41 +8384,53 @@
     @jsii.member(jsii_name="glueJob")
     def glue_job(self) -> _aws_cdk_aws_glue_alpha_ce674d29.IJob:
         return typing.cast(_aws_cdk_aws_glue_alpha_ce674d29.IJob, jsii.get(self, "glueJob"))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
 
     @builtins.property
     @jsii.member(jsii_name="crawler")
     def crawler(self) -> typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler]:
         return typing.cast(typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler], jsii.get(self, "crawler"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 class RedshiftDataApiStage(
     StateMachineStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.RedshiftDataApiStage",
 ):
+    '''Stage that contains a step function that executes Redshift Data API statements.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         redshift_cluster_identifier: builtins.str,
         sql_statements: typing.Sequence[builtins.str],
@@ -7658,30 +8442,31 @@
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param redshift_cluster_identifier: 
-        :param sql_statements: 
-        :param database_name: 
-        :param database_user: 
-        :param polling_time: 
-        :param additional_role_policy_statements: 
-        :param alarms_enabled: 
-        :param state_machine_failed_executions_alarm_evaluation_periods: 
-        :param state_machine_failed_executions_alarm_threshold: 
-        :param state_machine_input: 
-        :param state_machine_name: 
-        :param description: 
-        :param name: 
+        '''Constructs ``RedshiftDataApiStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param redshift_cluster_identifier: Identifier of the Redshift cluster.
+        :param sql_statements: List of SQL statements to execute.
+        :param database_name: Name of the database in Redshift. Default: "dev"
+        :param database_user: Database user. Default: "awsuser"
+        :param polling_time: Waiting time between checking whether the statements have finished executing. Default: cdk.Duration.seconds(15)
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2e1a2de894e37c9f2da01cc73a49a2d2fe9ec89a86ba3d42531baaa26002a1a7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = RedshiftDataApiStageProps(
             redshift_cluster_identifier=redshift_cluster_identifier,
@@ -7700,48 +8485,60 @@
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="stateMachine")
     def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
         return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
 
     @builtins.property
     @jsii.member(jsii_name="eventBridgeEventPath")
     def event_bridge_event_path(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "eventBridgeEventPath"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="stateMachineInput")
     def state_machine_input(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "stateMachineInput"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 class SnsSqsToLambdaStage(
     SqsToLambdaStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.SnsSqsToLambdaStage",
 ):
+    '''Stage implements an SNS Topic connected to an Amazon SQS queue and an AWS Lambda function, with an optional DLQ.'''
+
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         disable_default_topic_policy: typing.Optional[builtins.bool] = None,
         filter_policy: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_sns_ceddda9d.SubscriptionFilter]] = None,
@@ -7758,35 +8555,36 @@
         message_group_id: typing.Optional[builtins.str] = None,
         sqs_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
         sqs_queue_props: typing.Optional[typing.Union[_aws_cdk_aws_sqs_ceddda9d.QueueProps, typing.Dict[builtins.str, typing.Any]]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''
-        :param scope: -
-        :param id: -
-        :param disable_default_topic_policy: 
-        :param filter_policy: 
-        :param raw_message_delivery: 
-        :param sns_dlq_enabled: 
-        :param sns_topic: 
-        :param sns_topic_props: 
-        :param batch_size: 
-        :param dlq_enabled: 
-        :param lambda_function: 
-        :param lambda_function_props: 
-        :param max_batching_window: 
-        :param max_receive_count: 
-        :param message_group_id: 
-        :param sqs_queue: 
-        :param sqs_queue_props: 
-        :param alarms_enabled: 
-        :param description: 
-        :param name: 
+        '''Constructs ``SnsSqsToLambdaStage``.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param disable_default_topic_policy: Whether to disable the default topic policy generated by SnsFactory. Default: false
+        :param filter_policy: The filter policy. Default: - all messages are delivered
+        :param raw_message_delivery: The message to the queue is the same as it was sent to the topic. If false, the message will be wrapped in an SNS envelope. Default: false
+        :param sns_dlq_enabled: Queue to be used as dead letter queue. If not passed no dead letter queue is enabled. Default: - No dead letter queue enabled.
+        :param sns_topic: Preexisting SNS Topic to use in stage. If not provided, a new one will be created.
+        :param sns_topic_props: Properties for the SNS Topic that will be created by this construct (if ``snsTopic`` is not provided).
+        :param batch_size: The maximum number of records retrieved from the event source at the function invocation time. Default: 10
+        :param dlq_enabled: Determines if DLQ is enabled. Default: false
+        :param lambda_function: Preexisting Lambda Function to use in stage. If not provided, a new function will be created.
+        :param lambda_function_props: Properties for the Lambda Function that will be created by this construct (if ``lambdaFunction`` is not provided).
+        :param max_batching_window: The maximum amount of time to gather records before invoking the function. Valid Range: Minimum value of 0 minutes, maximum value of 5 minutes. Default: - no batching window.
+        :param max_receive_count: The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue. Default: 1
+        :param message_group_id: Message Group ID for messages sent to this queue. Required for FIFO queues.
+        :param sqs_queue: Preexisting SQS Queue to use in stage. If not provided, a new queue will be created.
+        :param sqs_queue_props: Properties for the SQS Queue that will be created by this construct (if ``sqsQueue`` is not provided).
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param description: Description of the stage.
+        :param name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f1f6169c1775457f18465db8ac58b6e948ab3cee732db9fb369eb57e96e8b7ef)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SnsToLambdaStageProps(
             disable_default_topic_policy=disable_default_topic_policy,
@@ -7817,26 +8615,35 @@
         return typing.cast(_aws_cdk_aws_sns_ceddda9d.ITopic, jsii.get(self, "topic"))
 
     @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
         return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
 
     @builtins.property
     @jsii.member(jsii_name="snsDeadLetterQueue")
     def sns_dead_letter_queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue]:
         return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue], jsii.get(self, "snsDeadLetterQueue"))
 
     @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.SnsToLambdaStageProps",
     jsii_struct_bases=[SqsToLambdaStageProps],
     name_mapping={
@@ -7879,33 +8686,34 @@
         disable_default_topic_policy: typing.Optional[builtins.bool] = None,
         filter_policy: typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_sns_ceddda9d.SubscriptionFilter]] = None,
         raw_message_delivery: typing.Optional[builtins.bool] = None,
         sns_dlq_enabled: typing.Optional[builtins.bool] = None,
         sns_topic: typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic] = None,
         sns_topic_props: typing.Optional[typing.Union[_aws_cdk_aws_sns_ceddda9d.TopicProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''
-        :param description: 
-        :param name: 
-        :param alarms_enabled: 
-        :param batch_size: 
-        :param dlq_enabled: 
-        :param lambda_function: 
-        :param lambda_function_props: 
-        :param max_batching_window: 
-        :param max_receive_count: 
-        :param message_group_id: 
-        :param sqs_queue: 
-        :param sqs_queue_props: 
-        :param disable_default_topic_policy: 
-        :param filter_policy: 
-        :param raw_message_delivery: 
-        :param sns_dlq_enabled: 
-        :param sns_topic: 
-        :param sns_topic_props: 
+        '''Properties for ``SnsSqsToLambdaStage``.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param alarms_enabled: Enable/Disable all alarms in a DataStage. Default: true
+        :param batch_size: The maximum number of records retrieved from the event source at the function invocation time. Default: 10
+        :param dlq_enabled: Determines if DLQ is enabled. Default: false
+        :param lambda_function: Preexisting Lambda Function to use in stage. If not provided, a new function will be created.
+        :param lambda_function_props: Properties for the Lambda Function that will be created by this construct (if ``lambdaFunction`` is not provided).
+        :param max_batching_window: The maximum amount of time to gather records before invoking the function. Valid Range: Minimum value of 0 minutes, maximum value of 5 minutes. Default: - no batching window.
+        :param max_receive_count: The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue. Default: 1
+        :param message_group_id: Message Group ID for messages sent to this queue. Required for FIFO queues.
+        :param sqs_queue: Preexisting SQS Queue to use in stage. If not provided, a new queue will be created.
+        :param sqs_queue_props: Properties for the SQS Queue that will be created by this construct (if ``sqsQueue`` is not provided).
+        :param disable_default_topic_policy: Whether to disable the default topic policy generated by SnsFactory. Default: false
+        :param filter_policy: The filter policy. Default: - all messages are delivered
+        :param raw_message_delivery: The message to the queue is the same as it was sent to the topic. If false, the message will be wrapped in an SNS envelope. Default: false
+        :param sns_dlq_enabled: Queue to be used as dead letter queue. If not passed no dead letter queue is enabled. Default: - No dead letter queue enabled.
+        :param sns_topic: Preexisting SNS Topic to use in stage. If not provided, a new one will be created.
+        :param sns_topic_props: Properties for the SNS Topic that will be created by this construct (if ``snsTopic`` is not provided).
         '''
         if isinstance(lambda_function_props, dict):
             lambda_function_props = SqsToLambdaStageFunctionProps(**lambda_function_props)
         if isinstance(sqs_queue_props, dict):
             sqs_queue_props = _aws_cdk_aws_sqs_ceddda9d.QueueProps(**sqs_queue_props)
         if isinstance(sns_topic_props, dict):
             sns_topic_props = _aws_cdk_aws_sns_ceddda9d.TopicProps(**sns_topic_props)
@@ -7965,103 +8773,167 @@
         if sns_topic is not None:
             self._values["sns_topic"] = sns_topic
         if sns_topic_props is not None:
             self._values["sns_topic_props"] = sns_topic_props
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in a DataStage.
+
+        :default: true
+        '''
         result = self._values.get("alarms_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def batch_size(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of records retrieved from the event source at the function invocation time.
+
+        :default: 10
+        '''
         result = self._values.get("batch_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def dlq_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Determines if DLQ is enabled.
+
+        :default: false
+        '''
         result = self._values.get("dlq_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def lambda_function(
         self,
     ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction]:
+        '''Preexisting Lambda Function to use in stage.
+
+        If not provided, a new function will be created.
+        '''
         result = self._values.get("lambda_function")
         return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction], result)
 
     @builtins.property
     def lambda_function_props(self) -> typing.Optional[SqsToLambdaStageFunctionProps]:
+        '''Properties for the Lambda Function that will be created by this construct (if ``lambdaFunction`` is not provided).'''
         result = self._values.get("lambda_function_props")
         return typing.cast(typing.Optional[SqsToLambdaStageFunctionProps], result)
 
     @builtins.property
     def max_batching_window(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''The maximum amount of time to gather records before invoking the function.
+
+        Valid Range: Minimum value of 0 minutes, maximum value of 5 minutes.
+        Default: - no batching window.
+        '''
         result = self._values.get("max_batching_window")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def max_receive_count(self) -> typing.Optional[jsii.Number]:
+        '''The number of times a message can be unsuccessfully dequeued before being moved to the dead-letter queue.
+
+        :default: 1
+        '''
         result = self._values.get("max_receive_count")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def message_group_id(self) -> typing.Optional[builtins.str]:
+        '''Message Group ID for messages sent to this queue.
+
+        Required for FIFO queues.
+        '''
         result = self._values.get("message_group_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sqs_queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue]:
+        '''Preexisting SQS Queue to use in stage.
+
+        If not provided, a new queue will be created.
+        '''
         result = self._values.get("sqs_queue")
         return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue], result)
 
     @builtins.property
     def sqs_queue_props(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.QueueProps]:
+        '''Properties for the SQS Queue that will be created by this construct (if ``sqsQueue`` is not provided).'''
         result = self._values.get("sqs_queue_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.QueueProps], result)
 
     @builtins.property
     def disable_default_topic_policy(self) -> typing.Optional[builtins.bool]:
+        '''Whether to disable the default topic policy generated by SnsFactory.
+
+        :default: false
+
+        :see: SnsFactory.secureSnsTopicPolicy
+        '''
         result = self._values.get("disable_default_topic_policy")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def filter_policy(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_sns_ceddda9d.SubscriptionFilter]]:
+        '''The filter policy.
+
+        :default: - all messages are delivered
+        '''
         result = self._values.get("filter_policy")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, _aws_cdk_aws_sns_ceddda9d.SubscriptionFilter]], result)
 
     @builtins.property
     def raw_message_delivery(self) -> typing.Optional[builtins.bool]:
+        '''The message to the queue is the same as it was sent to the topic.
+
+        If false, the message will be wrapped in an SNS envelope.
+
+        :default: false
+        '''
         result = self._values.get("raw_message_delivery")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def sns_dlq_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Queue to be used as dead letter queue.
+
+        If not passed no dead letter queue is enabled.
+
+        :default: - No dead letter queue enabled.
+        '''
         result = self._values.get("sns_dlq_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def sns_topic(self) -> typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic]:
+        '''Preexisting SNS Topic to use in stage.
+
+        If not provided, a new one will be created.
+        '''
         result = self._values.get("sns_topic")
         return typing.cast(typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic], result)
 
     @builtins.property
     def sns_topic_props(self) -> typing.Optional[_aws_cdk_aws_sns_ceddda9d.TopicProps]:
+        '''Properties for the SNS Topic that will be created by this construct (if ``snsTopic`` is not provided).'''
         result = self._values.get("sns_topic_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_sns_ceddda9d.TopicProps], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -8102,19 +8974,19 @@
     "DataBrewTransformStageProps",
     "DataPipeline",
     "DataPipelineProps",
     "DataStage",
     "DataStageProps",
     "DeliveryStreamProps",
     "EnvironmentConfiguration",
-    "EnvironmentResult",
     "EventStage",
     "EventStageProps",
     "FirehoseToS3Stage",
     "FirehoseToS3StageProps",
+    "GetConfigProps",
     "GetEnvConfigProps",
     "GetEnvironmentProps",
     "GetSynthActionProps",
     "GetTagsProps",
     "GlueFactory",
     "GlueTransformStage",
     "GlueTransformStageProps",
@@ -8269,14 +9141,22 @@
     environment_id: typing.Optional[builtins.str] = None,
     prefix: typing.Optional[builtins.str] = None,
     qualifier: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__b2efe5dde2538acae1f48243a64a4ddfc2bc79e8400b2883ddf4986fbd5984c8(
+    exported_value: typing.Any,
+    *,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__a429ca722d1fec889b8120d065d6c339e922faac9a9e70454e565500ff82514c(
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
@@ -8434,14 +9314,15 @@
 
 def _typecheckingstub__daeed9e6cb5e50c39b922933d297c173f25183423bf700dfd9f8b0fe3765c923(
     *,
     environments: typing.Mapping[builtins.str, typing.Union[EnvironmentConfiguration, typing.Dict[builtins.str, typing.Any]]],
     account: typing.Optional[builtins.str] = None,
     bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ddk_bootstrap_config_key: typing.Optional[builtins.str] = None,
+    props: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     region: typing.Optional[builtins.str] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__83dd06108e5a02547d07299060f92123340b3d7ec7e9e6f36a8e28ce02b22a22(
@@ -8510,25 +9391,25 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__cf306c436463dcb56197f32e9c4793604595ef2ca8f42b2d72de058d5806870c(
     *,
     account: typing.Optional[builtins.str] = None,
     bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    props: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     region: typing.Optional[builtins.str] = None,
     resources: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c2515674b45134976862352edd7f3a4f56dddd10e860df69a14d633b55dfe768(
+def _typecheckingstub__5dba6810d9499d40d626ee84f10a13e1cade1e4a1602afa74c9dd333695965bd(
     *,
-    account: typing.Optional[builtins.str] = None,
-    region: typing.Optional[builtins.str] = None,
+    config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__392d4bf9e0a3416c4cbfe2cfcca884cc2b98f96b99a23a03e386497b6cfd2fef(
     *,
     config_path: builtins.str,
@@ -8797,15 +9678,16 @@
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     catalog_name: typing.Optional[builtins.str] = None,
     database_name: typing.Optional[builtins.str] = None,
     encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key] = None,
     encryption_option: typing.Optional[_aws_cdk_aws_stepfunctions_tasks_ceddda9d.EncryptionOption] = None,
     output_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
-    query_string: typing.Optional[builtins.str] = None,
+    parallel: typing.Optional[builtins.bool] = None,
+    query_string: typing.Optional[typing.Sequence[builtins.str]] = None,
     query_string_path: typing.Optional[builtins.str] = None,
     work_group: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f6be6b9ec4e805f427307a7bc1c743a3f56ffd52c0cc37a1436d75ce69e31b9f(
@@ -9096,15 +9978,16 @@
     id: builtins.str,
     *,
     catalog_name: typing.Optional[builtins.str] = None,
     database_name: typing.Optional[builtins.str] = None,
     encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.Key] = None,
     encryption_option: typing.Optional[_aws_cdk_aws_stepfunctions_tasks_ceddda9d.EncryptionOption] = None,
     output_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
-    query_string: typing.Optional[builtins.str] = None,
+    parallel: typing.Optional[builtins.bool] = None,
+    query_string: typing.Optional[typing.Sequence[builtins.str]] = None,
     query_string_path: typing.Optional[builtins.str] = None,
     work_group: typing.Optional[builtins.str] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
```

### Comparing `aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/__init__.py` & `aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 import aws_cdk.aws_glue_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii
 import aws_cdk.integ_tests_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "aws-ddk-core",
-    "1.0.0-beta.1",
-    __name__[0:-6],
-    "aws-ddk-core@1.0.0-beta.1.jsii.tgz",
+    "aws-ddk-core", "1.0.0-rc.0", __name__[0:-6], "aws-ddk-core@1.0.0-rc.0.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

