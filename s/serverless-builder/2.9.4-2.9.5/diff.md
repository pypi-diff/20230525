# Comparing `tmp/serverless-builder-2.9.4.tar.gz` & `tmp/serverless-builder-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverless-builder-2.9.4.tar", last modified: Mon Jul 18 11:24:36 2022, max compression
+gzip compressed data, was "serverless-builder-2.9.5.tar", last modified: Tue Jul 26 19:29:58 2022, max compression
```

## Comparing `serverless-builder-2.9.4.tar` & `serverless-builder-2.9.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1067 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/LICENSE
--rw-r--r--   0        0        0     3417 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/README.md
--rw-r--r--   0        0        0     1155 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/pyproject.toml
--rw-r--r--   0        0        0       98 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/alerts/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/alerts/sqs.py
--rw-r--r--   0        0        0      445 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/auth.py
--rw-r--r--   0        0        0      105 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/features/__init__.py
--rw-r--r--   0        0        0      645 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/features/api_handler.py
--rw-r--r--   0        0        0      884 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/features/api_keys.py
--rw-r--r--   0        0        0     3482 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/features/encryption.py
--rw-r--r--   0        0        0     8962 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/features/stepfunctions.py
--rw-r--r--   0        0        0      374 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/features/xray.py
--rw-r--r--   0        0        0        0 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/functions/__init__.py
--rw-r--r--   0        0        0     1761 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/functions/dynamodb.py
--rw-r--r--   0        0        0     1444 2022-07-18 11:24:19.992998 serverless-builder-2.9.4/serverless/aws/functions/event_bridge.py
--rw-r--r--   0        0        0     8653 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/functions/generic.py
--rw-r--r--   0        0        0     1704 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/functions/http.py
--rw-r--r--   0        0        0     1936 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/functions/kinesis.py
--rw-r--r--   0        0        0      959 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/functions/s3.py
--rw-r--r--   0        0        0     1176 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/functions/sqs.py
--rw-r--r--   0        0        0     2803 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/__init__.py
--rw-r--r--   0        0        0      734 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/apigw.py
--rw-r--r--   0        0        0     2461 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/dynamodb.py
--rw-r--r--   0        0        0      640 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/event_bridge.py
--rw-r--r--   0        0        0     1414 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/kinesis.py
--rw-r--r--   0        0        0     1454 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/redshift.py
--rw-r--r--   0        0        0      674 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/secrets_manager.py
--rw-r--r--   0        0        0      528 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/sqs.py
--rw-r--r--   0        0        0      562 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/iam/xray.py
--rw-r--r--   0        0        0     7392 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/provider.py
--rw-r--r--   0        0        0      967 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/__init__.py
--rw-r--r--   0        0        0     4597 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/dynamodb.py
--rw-r--r--   0        0        0      955 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/iam.py
--rw-r--r--   0        0        0     1196 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/kinesis.py
--rw-r--r--   0        0        0      498 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/kms.py
--rw-r--r--   0        0        0     1085 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/logs.py
--rw-r--r--   0        0        0     1831 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/s3.py
--rw-r--r--   0        0        0      919 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/resources/sqs.py
--rw-r--r--   0        0        0     1656 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/aws/types.py
--rw-r--r--   0        0        0     5352 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/cli.py
--rw-r--r--   0        0        0        0 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/feature.py
--rw-r--r--   0        0        0      175 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/integration/__init__.py
--rw-r--r--   0        0        0     1739 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/integration/event_dispatcher.py
--rw-r--r--   0        0        0      409 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/integration/powertools.py
--rw-r--r--   0        0        0      529 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/integration/sentry.py
--rw-r--r--   0        0        0      647 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/plugins.py
--rw-r--r--   0        0        0       60 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/provider.py
--rw-r--r--   0        0        0     4212 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/__init__.py
--rw-r--r--   0        0        0      217 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/configuration.py
--rw-r--r--   0        0        0      313 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/environment.py
--rw-r--r--   0        0        0      477 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/functions.py
--rw-r--r--   0        0        0      287 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/package.py
--rw-r--r--   0        0        0      805 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/__init__.py
--rw-r--r--   0        0        0     1477 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/code_sign.py
--rw-r--r--   0        0        0      303 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/composed_vars.py
--rw-r--r--   0        0        0     1679 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/deployment_bucket.py
--rw-r--r--   0        0        0      935 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/domain_manager.py
--rw-r--r--   0        0        0      531 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/dynamodb.py
--rw-r--r--   0        0        0      230 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/export_env.py
--rw-r--r--   0        0        0      431 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/generic.py
--rw-r--r--   0        0        0      344 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/iam_roles.py
--rw-r--r--   0        0        0     1015 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/kms.py
--rw-r--r--   0        0        0      246 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/lambda_dlq.py
--rw-r--r--   0        0        0     1024 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/localstack.py
--rw-r--r--   0        0        0      495 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/prune.py
--rw-r--r--   0        0        0     1139 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/python_requirements.py
--rw-r--r--   0        0        0      967 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/scriptable.py
--rw-r--r--   0        0        0      743 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/secrets.py
--rw-r--r--   0        0        0      293 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/step_functions.py
--rw-r--r--   0        0        0     1320 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/plugins/vpc_discovery.py
--rw-r--r--   0        0        0     2428 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/resources.py
--rw-r--r--   0        0        0     3833 2022-07-18 11:24:19.996998 serverless-builder-2.9.4/serverless/service/types.py
--rw-r--r--   0        0        0     4611 2022-07-18 11:24:36.306793 serverless-builder-2.9.4/setup.py
--rw-r--r--   0        0        0     4286 2022-07-18 11:24:36.307604 serverless-builder-2.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-07-26 19:29:40.247512 serverless-builder-2.9.5/LICENSE
+-rw-r--r--   0        0        0     3417 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/README.md
+-rw-r--r--   0        0        0     1155 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/alerts/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/alerts/sqs.py
+-rw-r--r--   0        0        0      445 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/auth.py
+-rw-r--r--   0        0        0      105 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/features/__init__.py
+-rw-r--r--   0        0        0      645 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/features/api_handler.py
+-rw-r--r--   0        0        0      884 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/features/api_keys.py
+-rw-r--r--   0        0        0     3482 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/features/encryption.py
+-rw-r--r--   0        0        0     8962 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/features/stepfunctions.py
+-rw-r--r--   0        0        0      374 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/features/xray.py
+-rw-r--r--   0        0        0        0 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/__init__.py
+-rw-r--r--   0        0        0     1761 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/dynamodb.py
+-rw-r--r--   0        0        0     1444 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/event_bridge.py
+-rw-r--r--   0        0        0     8652 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/generic.py
+-rw-r--r--   0        0        0     1704 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/http.py
+-rw-r--r--   0        0        0     1936 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/kinesis.py
+-rw-r--r--   0        0        0      959 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/s3.py
+-rw-r--r--   0        0        0     1176 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/functions/sqs.py
+-rw-r--r--   0        0        0     2803 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/__init__.py
+-rw-r--r--   0        0        0      734 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/apigw.py
+-rw-r--r--   0        0        0     2461 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/dynamodb.py
+-rw-r--r--   0        0        0      640 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/event_bridge.py
+-rw-r--r--   0        0        0     1414 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/kinesis.py
+-rw-r--r--   0        0        0     1454 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/redshift.py
+-rw-r--r--   0        0        0      674 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/secrets_manager.py
+-rw-r--r--   0        0        0      528 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/sqs.py
+-rw-r--r--   0        0        0      562 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/iam/xray.py
+-rw-r--r--   0        0        0     7392 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/provider.py
+-rw-r--r--   0        0        0      967 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/__init__.py
+-rw-r--r--   0        0        0     4597 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/dynamodb.py
+-rw-r--r--   0        0        0      955 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/iam.py
+-rw-r--r--   0        0        0     1196 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/kinesis.py
+-rw-r--r--   0        0        0      498 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/kms.py
+-rw-r--r--   0        0        0     1085 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/logs.py
+-rw-r--r--   0        0        0     1831 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/s3.py
+-rw-r--r--   0        0        0      919 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/resources/sqs.py
+-rw-r--r--   0        0        0     1656 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/aws/types.py
+-rw-r--r--   0        0        0     5352 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/cli.py
+-rw-r--r--   0        0        0        0 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/feature.py
+-rw-r--r--   0        0        0      175 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/integration/__init__.py
+-rw-r--r--   0        0        0     1739 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/integration/event_dispatcher.py
+-rw-r--r--   0        0        0      409 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/integration/powertools.py
+-rw-r--r--   0        0        0      529 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/integration/sentry.py
+-rw-r--r--   0        0        0      647 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/plugins.py
+-rw-r--r--   0        0        0       60 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/provider.py
+-rw-r--r--   0        0        0     4212 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/__init__.py
+-rw-r--r--   0        0        0      217 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/configuration.py
+-rw-r--r--   0        0        0      313 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/environment.py
+-rw-r--r--   0        0        0      477 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/functions.py
+-rw-r--r--   0        0        0      287 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/package.py
+-rw-r--r--   0        0        0      805 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/__init__.py
+-rw-r--r--   0        0        0     1477 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/code_sign.py
+-rw-r--r--   0        0        0      303 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/composed_vars.py
+-rw-r--r--   0        0        0     1679 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/deployment_bucket.py
+-rw-r--r--   0        0        0      935 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/domain_manager.py
+-rw-r--r--   0        0        0      531 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/dynamodb.py
+-rw-r--r--   0        0        0      230 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/export_env.py
+-rw-r--r--   0        0        0      431 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/generic.py
+-rw-r--r--   0        0        0      344 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/iam_roles.py
+-rw-r--r--   0        0        0     1015 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/kms.py
+-rw-r--r--   0        0        0      246 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/lambda_dlq.py
+-rw-r--r--   0        0        0     1024 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/localstack.py
+-rw-r--r--   0        0        0      495 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/prune.py
+-rw-r--r--   0        0        0     1139 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/python_requirements.py
+-rw-r--r--   0        0        0      967 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/scriptable.py
+-rw-r--r--   0        0        0      743 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/secrets.py
+-rw-r--r--   0        0        0      293 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/step_functions.py
+-rw-r--r--   0        0        0     1320 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/plugins/vpc_discovery.py
+-rw-r--r--   0        0        0     2428 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/resources.py
+-rw-r--r--   0        0        0     3833 2022-07-26 19:29:40.251512 serverless-builder-2.9.5/serverless/service/types.py
+-rw-r--r--   0        0        0     4611 2022-07-26 19:29:58.604783 serverless-builder-2.9.5/setup.py
+-rw-r--r--   0        0        0     4286 2022-07-26 19:29:58.605560 serverless-builder-2.9.5/PKG-INFO
```

### Comparing `serverless-builder-2.9.4/LICENSE` & `serverless-builder-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/README.md` & `serverless-builder-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/pyproject.toml` & `serverless-builder-2.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "serverless-builder"
-version = "2.9.4"
+version = "2.9.5"
 description = "Python interface to easily generate `serverless.yml`."
 keywords = ["library", "serverless"]
 authors = ["Epsy <engineering@epsyhealth.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://epsylabs.github.io/serverless-builder/"
 repository = "https://github.com/epsylabs/serverless-builder"
```

### Comparing `serverless-builder-2.9.4/serverless/aws/features/api_handler.py` & `serverless-builder-2.9.5/serverless/aws/features/api_handler.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/features/api_keys.py` & `serverless-builder-2.9.5/serverless/aws/features/api_keys.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/features/encryption.py` & `serverless-builder-2.9.5/serverless/aws/features/encryption.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/features/stepfunctions.py` & `serverless-builder-2.9.5/serverless/aws/features/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/dynamodb.py` & `serverless-builder-2.9.5/serverless/aws/functions/dynamodb.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/event_bridge.py` & `serverless-builder-2.9.5/serverless/aws/functions/event_bridge.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/generic.py` & `serverless-builder-2.9.5/serverless/aws/functions/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             force_name
             if force_name
             else Identifier(self._service.service.spinal.lower() + "-${sls:stage}" + "-" + self.key.spinal.lower())
         )
         self.description = description
 
         if not handler:
-            handler = f"{self._service.service.snake}.{self.key.spinal}.handler"
+            handler = f"{self._service.service.snake}.{self.key.snake}.handler"
 
         self.handler = handler
         self.events = []
 
         if self._service.plugins.get(IAMRoles):
             self.iamRoleStatements = FunctionPolicyBuilder(self.name, self._service)
             self.iamRoleStatementsName = self.iamRoleStatements.role
```

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/http.py` & `serverless-builder-2.9.5/serverless/aws/functions/http.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/kinesis.py` & `serverless-builder-2.9.5/serverless/aws/functions/kinesis.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/s3.py` & `serverless-builder-2.9.5/serverless/aws/functions/s3.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/functions/sqs.py` & `serverless-builder-2.9.5/serverless/aws/functions/sqs.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/__init__.py` & `serverless-builder-2.9.5/serverless/aws/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/apigw.py` & `serverless-builder-2.9.5/serverless/aws/iam/apigw.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/dynamodb.py` & `serverless-builder-2.9.5/serverless/aws/iam/dynamodb.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/event_bridge.py` & `serverless-builder-2.9.5/serverless/aws/iam/event_bridge.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/kinesis.py` & `serverless-builder-2.9.5/serverless/aws/iam/kinesis.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/redshift.py` & `serverless-builder-2.9.5/serverless/aws/iam/redshift.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/secrets_manager.py` & `serverless-builder-2.9.5/serverless/aws/iam/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/sqs.py` & `serverless-builder-2.9.5/serverless/aws/iam/sqs.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/iam/xray.py` & `serverless-builder-2.9.5/serverless/aws/iam/xray.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/provider.py` & `serverless-builder-2.9.5/serverless/aws/provider.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/__init__.py` & `serverless-builder-2.9.5/serverless/aws/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/dynamodb.py` & `serverless-builder-2.9.5/serverless/aws/resources/dynamodb.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/iam.py` & `serverless-builder-2.9.5/serverless/aws/resources/iam.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/kinesis.py` & `serverless-builder-2.9.5/serverless/aws/resources/kinesis.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/logs.py` & `serverless-builder-2.9.5/serverless/aws/resources/logs.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/s3.py` & `serverless-builder-2.9.5/serverless/aws/resources/s3.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/resources/sqs.py` & `serverless-builder-2.9.5/serverless/aws/resources/sqs.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/aws/types.py` & `serverless-builder-2.9.5/serverless/aws/types.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/cli.py` & `serverless-builder-2.9.5/serverless/cli.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/integration/event_dispatcher.py` & `serverless-builder-2.9.5/serverless/integration/event_dispatcher.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/integration/sentry.py` & `serverless-builder-2.9.5/serverless/integration/sentry.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/plugins.py` & `serverless-builder-2.9.5/serverless/plugins.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/__init__.py` & `serverless-builder-2.9.5/serverless/service/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/__init__.py` & `serverless-builder-2.9.5/serverless/service/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/code_sign.py` & `serverless-builder-2.9.5/serverless/service/plugins/code_sign.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/deployment_bucket.py` & `serverless-builder-2.9.5/serverless/service/plugins/deployment_bucket.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/domain_manager.py` & `serverless-builder-2.9.5/serverless/service/plugins/domain_manager.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/dynamodb.py` & `serverless-builder-2.9.5/serverless/service/plugins/dynamodb.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/kms.py` & `serverless-builder-2.9.5/serverless/service/plugins/kms.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/localstack.py` & `serverless-builder-2.9.5/serverless/service/plugins/localstack.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/python_requirements.py` & `serverless-builder-2.9.5/serverless/service/plugins/python_requirements.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/scriptable.py` & `serverless-builder-2.9.5/serverless/service/plugins/scriptable.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/secrets.py` & `serverless-builder-2.9.5/serverless/service/plugins/secrets.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/plugins/vpc_discovery.py` & `serverless-builder-2.9.5/serverless/service/plugins/vpc_discovery.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/resources.py` & `serverless-builder-2.9.5/serverless/service/resources.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/serverless/service/types.py` & `serverless-builder-2.9.5/serverless/service/types.py`

 * *Files identical despite different names*

### Comparing `serverless-builder-2.9.4/setup.py` & `serverless-builder-2.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'troposphere>=3.2,<3.3']
 
 entry_points = \
 {'console_scripts': ['slscli = serverless.cli:cli']}
 
 setup_kwargs = {
     'name': 'serverless-builder',
-    'version': '2.9.4',
+    'version': '2.9.5',
     'description': 'Python interface to easily generate `serverless.yml`.',
     'long_description': '<h2 align="center">serverless-builder</h2>\n<p align="center">\n<a href="https://pypi.org/project/serverless-builder/"><img alt="PyPI" src="https://img.shields.io/pypi/v/serverless-builder"></a>\n<a href="https://pypi.org/project/serverless-builder/"><img alt="Python" src="https://img.shields.io/pypi/pyversions/serverless-builder.svg"></a>\n<a href="https://github.com/epsylabs/serverless-builder/blob/master/LICENSE"><img alt="License" src="https://img.shields.io/pypi/l/serverless-builder.svg"></a>\n</p>\n\nPython interface to easily generate [serverless.yml](https://www.serverless.com/) file.\n\nTo read more about features, visit [📜 our documentation](https://epsylabs.github.io/serverless-builder/).\n\n## Installation\n```shell\npip install serverless-builder\n```\n\n## Features\n* [plugin management](https://epsylabs.github.io/serverless-builder/plugins/) with autoconfiguration\n* [function factory](https://epsylabs.github.io/serverless-builder/usage/#lambda-functions) with some best practice hints\n* autoconfiguration of some provider specific features like AWS X-Ray\n* easy resource manipulation with [troposphere lib](https://github.com/cloudtools/troposphere) (but if you want you can use old good dict)\n* easier IAM management with predefined permission sets\n* built-in support for any serverless attributes\n* integration with [aws lambda powertools](https://awslabs.github.io/aws-lambda-powertools-python/latest/)\n\n## Example of use\n\n```python\nfrom serverless.aws.functions.event_bridge import RetryPolicy\nfrom serverless.aws.functions.http import HTTPFunction\nfrom serverless import Service\nfrom serverless.provider import AWSProvider\nfrom serverless.aws.features import XRay\nfrom serverless.aws.iam.dynamodb import DynamoDBReader\nfrom serverless.plugins import ComposedVars, PythonRequirements, Prune\n\nfrom troposphere.dynamodb import Table, AttributeDefinition, KeySchema\n\nservice = Service(\n    "service-name",\n    "some dummy service",\n    AWSProvider()\n)\nservice.plugins.add(ComposedVars())\nservice.plugins.add(Prune())\nservice.plugins.add(PythonRequirements())\n\ntable = Table(\n    "TestTable",\n    BillingMode="PAY_PER_REQUEST",\n    AttributeDefinitions=[\n        AttributeDefinition(AttributeName="name", AttributeType="S")\n    ],\n    KeySchema=[KeySchema(AttributeName="name", KeyType="HASH")]\n)\n\nservice.enable(XRay())\nservice.provider.iam.apply(DynamoDBReader(table))\n\nservice.builder.function.generic("test", "description")\nservice.builder.function.http("test", "description", "/", HTTPFunction.POST)\n\n# Multiple events with different paths and/or methods can be set up for the same handler\n# This will add the same handler to all of these: POST /, POST /alias, PUT /, PUT /alias\nservice.builder.function.http("test", "description", ["/", "/alias"], ["POST", "PUT"], handler="shared.handler")\n\n# Context with pre-defined setup\nwith service.preset(\n    layers=[{"Ref": "PythonRequirementsLambdaLayer"}],\n    handler="test.handlers.custom_handler.handle"\n) as p:\n    p.http_get("test-list", "List all tests", "/")\n    p.http_get("test-get", "Get one test", "/{test_id}")\n\nevent_bridge_function = service.builder.function.event_bridge(\n    "event_bridge_function",\n    "sample event bridge function",\n    "epsy",\n    {"source": ["saas.external"]},\n)\n\nevent_bridge_function.use_delivery_dlq(RetryPolicy(5, 300))\nevent_bridge_function.use_async_dlq()\n\nservice.resources.add(table)\n\nservice.render()\n```\n',
     'author': 'Epsy',
     'author_email': 'engineering@epsyhealth.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://epsylabs.github.io/serverless-builder/',
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 ['serverless', 'serverless.aws', 'serverless.aws.alerts',
 'serverless.aws.features', 'serverless.aws.functions', 'serverless.aws.iam',
 'serverless.aws.resources', 'serverless.integration', 'serverless.service',
 'serverless.service.plugins'] package_data = \ {'': ['*']} install_requires = \
 ['PyYAML>=6.0,<7.0', 'awacs>=2.1.0,<3.0.0', 'inflection>=0.5.1,<0.6.0',
 'troposphere>=3.2,<3.3'] entry_points = \ {'console_scripts': ['slscli =
 serverless.cli:cli']} setup_kwargs = { 'name': 'serverless-builder', 'version':
-'2.9.4', 'description': 'Python interface to easily generate
+'2.9.5', 'description': 'Python interface to easily generate
 `serverless.yml`.', 'long_description': '
                         ***** serverless-builder *****
 \n
                         \n[PyPI]\n[Python]\n[License]\n
 \n\nPython interface to easily generate [serverless.yml](https://
 www.serverless.com/) file.\n\nTo read more about features, visit [ð our
 documentation](https://epsylabs.github.io/serverless-builder/).\n\n##
```

### Comparing `serverless-builder-2.9.4/PKG-INFO` & `serverless-builder-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-builder
-Version: 2.9.4
+Version: 2.9.5
 Summary: Python interface to easily generate `serverless.yml`.
 Home-page: https://epsylabs.github.io/serverless-builder/
 License: MIT
 Keywords: library,serverless
 Author: Epsy
 Author-email: engineering@epsyhealth.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: serverless-builder Version: 2.9.4 Summary: Python
+Metadata-Version: 2.1 Name: serverless-builder Version: 2.9.5 Summary: Python
 interface to easily generate `serverless.yml`. Home-page: https://
 epsylabs.github.io/serverless-builder/ License: MIT Keywords:
 library,serverless Author: Epsy Author-email: engineering@epsyhealth.com
 Requires-Python: >=3.8,<4.0 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
```

