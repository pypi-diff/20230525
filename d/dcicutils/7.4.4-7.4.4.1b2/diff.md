# Comparing `tmp/dcicutils-7.4.4.tar.gz` & `tmp/dcicutils-7.4.4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.4.4.tar", max compression
+gzip compressed data, was "dcicutils-7.4.4.1b2.tar", max compression
```

## Comparing `dcicutils-7.4.4.tar` & `dcicutils-7.4.4.1b2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1098 2023-05-25 13:59:33.106910 dcicutils-7.4.4/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-25 13:59:33.106910 dcicutils-7.4.4/README.rst
--rw-r--r--   0        0        0        0 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-25 13:59:33.106910 dcicutils-7.4.4/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20234 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   154684 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    12771 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-25 13:59:33.110910 dcicutils-7.4.4/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3944 2023-05-25 13:59:33.114910 dcicutils-7.4.4/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 dcicutils-7.4.4/setup.py
--rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/README.rst
+-rw-r--r--   0        0        0        0 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-05-23 21:00:08.071694 dcicutils-7.4.4.1b2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-05-23 21:00:08.075695 dcicutils-7.4.4.1b2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20234 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   154684 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    11525 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3948 2023-05-23 21:00:08.079695 dcicutils-7.4.4.1b2/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 dcicutils-7.4.4.1b2/setup.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 dcicutils-7.4.4.1b2/PKG-INFO
```

### Comparing `dcicutils-7.4.4/LICENSE.txt` & `dcicutils-7.4.4.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/README.rst` & `dcicutils-7.4.4.1b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/base.py` & `dcicutils-7.4.4.1b2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/beanstalk_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/cloudformation_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/codebuild_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/command_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/common.py` & `dcicutils-7.4.4.1b2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/creds_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/data_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/deployment_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/diff_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/docker_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/ecr_scripts.py` & `dcicutils-7.4.4.1b2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/ecr_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/ecs_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/env_base.py` & `dcicutils-7.4.4.1b2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/env_manager.py` & `dcicutils-7.4.4.1b2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/env_scripts.py` & `dcicutils-7.4.4.1b2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/env_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/env_utils_legacy.py` & `dcicutils-7.4.4.1b2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/es_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/exceptions.py` & `dcicutils-7.4.4.1b2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/ff_mocks.py` & `dcicutils-7.4.4.1b2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/ff_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/function_cache_decorator.py` & `dcicutils-7.4.4.1b2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/glacier_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/jh_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/kibana/dashboards.json` & `dcicutils-7.4.4.1b2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/kibana/readme.md` & `dcicutils-7.4.4.1b2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/lang_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/log_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/misc_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/obfuscation_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/opensearch_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/qa_checkers.py` & `dcicutils-7.4.4.1b2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/qa_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/redis_tools.py` & `dcicutils-7.4.4.1b2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/redis_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/s3_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.4.4.1b2/dcicutils/scripts/publish_to_pypi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,59 @@
 # Script to publish the Python package in the CURRENT git repo to PyPi.
 # Does the following checks before allowing a publish:
 #
-# 0. Current directory MUST be a git repo.
 # 1. The git repo MUST NOT contain unstaged changes.
 # 2. The git repo MUST NOT contain staged but uncommitted changes.
 # 3. The git repo MUST NOT contain committed but unpushed changes.
 # 4. The git repo package directories MUST NOT contain untracked files,
 #    OR if they do contain untracked files then you must confirm this is OK.
 # 5. The version being published must NOT have already been published.
 #
-# ASSUMES you have these credentials environment variables correctly set for PyPi publishing;
-# although a --username and --password are also supported to set these via command-line.
+# ASSUMES you have these environment variables correctly set for PyPi publishing:
 #
 # - PYPI_USER
 # - PYPI_PASSWORD
 #
-# Prints a warning if the username is NOT "__token__" meaning a PyPi API token is being
-# used, as using a simple username/password (as opposed to API token) is deprecated.
-#
 # Prompts for yes or no before publish is actually done. There is a --noconfirm
 # option to skip this confimation, however it is only allowed when running in the
 # context of GitHub actions - it checks for the GITHUB_ACTIONS environment variable.
 #
-# Prints warning if PY
-#
 # FYI: This was created late April 2023 after a junk file containing development
 # logging output containing passwords was accidentally published to PyPi;
 # item #4 above specifically addresses/prevents this. Perhaps better
 # would be if publishing only happened via GitHub actions.
 
 import argparse
 import os
 import requests
 import subprocess
 import toml
 from typing import Tuple, Union
 
 
-PYPI_BASE_URL = "https://pypi.org"
 DEBUG = False
+PRINT = print
 
 
 def main() -> None:
 
     def is_github_actions_context():
         return "GITHUB_ACTIONS" in os.environ
 
     argp = argparse.ArgumentParser()
     argp.add_argument("--noconfirm", required=False, dest="noconfirm", action="store_true")
     argp.add_argument("--debug", required=False, dest="debug", action="store_true")
-    argp.add_argument("--username", required=False, dest="username")
-    argp.add_argument("--password", required=False, dest="password")
     args = argp.parse_args()
 
     if args.debug:
         global DEBUG
         DEBUG = True
 
     if args.noconfirm and not is_github_actions_context():
-        ERROR_PRINT("The --noconfirm flag is only allowed within GitHub actions!")
+        PRINT("The --noconfirm flag is only allowed within GitHub actions!")
         exit_with_no_action()
 
     if not verify_git_repo():
         exit_with_no_action()
 
     if not verify_unstaged_changes():
         exit_with_no_action()
@@ -87,156 +78,148 @@
 
     if not args.noconfirm:
         if not answered_yes_to_confirmation(f"Do you want to publish {package_name} {package_version} to PyPi?"):
             exit_with_no_action()
 
     PRINT(f"Publishing {package_name} {package_version} to PyPi ...")
 
-    if not publish_package(args.username, args.password):
+    if not publish_package():
         exit_with_no_action()
 
     PRINT(f"Publishing {package_name} {package_version} to PyPi complete.")
 
 
 def publish_package(pypi_username: str = None, pypi_password: str = None) -> bool:
     if not pypi_username:
         pypi_username = os.environ.get("PYPI_USER")
     if not pypi_password:
         pypi_password = os.environ.get("PYPI_PASSWORD")
     if not pypi_username or not pypi_password:
-        ERROR_PRINT(f"No PyPi credentials; you should set the PYPI_USER and PYPI_PASSWORD environment variables.")
+        PRINT(f"No PyPi credentials. You must have PYPI_USER and PYPI_PASSWORD environment variables set.")
         return False
-    if pypi_username != "__token__":
-        WARNING_PRINT(f"Publishing with username/pasword is deprecated; should use be using API token instead.")
     poetry_publish_command = [
         "poetry", "publish",
         "--no-interaction", "--build",
         f"--username={pypi_username}", f"--password={pypi_password}"
     ]
     poetry_publish_results, status_code = execute_command(poetry_publish_command)
     PRINT("\n".join(poetry_publish_results))
     if status_code != 0:
-        # TODO: Maybe retry once or twice (with prompt) if (perhaps spurious) failure.
-        ERROR_PRINT(f"Publish to PyPi failed!")
+        PRINT(f"Publish to PyPi failed!")
         return False
     return True
 
 
 def verify_git_repo() -> bool:
     """
     If this (the current directory) looks like a git repo then return True,
-    otherwise prints an error message and returns False.
+    otherwise prints a warning and returns False.
     """
     _, status = execute_command("git rev-parse --is-inside-work-tree")
     if status != 0:
-        ERROR_PRINT("You are not in a git repo directory!")
+        PRINT("You are not in a git repo directory!")
         return False
     return True
 
 
 def verify_unstaged_changes() -> bool:
     """
     If the current git repo has no unstaged changes then returns True,
-    otherwise prints an error message and returns False.
+    otherwise prints a warning and returns False.
     """
-    git_diff_results, _ = execute_command("git diff")
+    git_diff_results, _ = execute_command(["git", "diff"])
     if git_diff_results:
-        ERROR_PRINT("You have changes to this branch that you have not staged for commit.")
+        PRINT("You have changes to this branch that you have not staged for commit.")
         return False
     return True
 
 
 def verify_uncommitted_changes() -> bool:
     """
     If the current git repo has no staged but uncommitted changes then returns True,
-    otherwise prints an error message and returns False.
+    otherwise prints a warning and returns False.
     """
-    git_diff_staged_results, _ = execute_command("git diff --staged")
+    git_diff_staged_results, _ = execute_command(["git", "diff", "--staged"])
     if git_diff_staged_results:
-        ERROR_PRINT("You have changes to this branch that you have staged but not committed.")
+        PRINT("You have changes to this branch that you have staged but not committed.")
         return False
     return True
 
 
 def verify_unpushed_changes() -> bool:
     """
     If the current git repo committed but unpushed changes then returns True,
-    otherwise prints an error message and returns False.
+    otherwise prints a warning and returns False.
     """
-    git_uno_results, _ = execute_command("git status -uno", lines_containing="is ahead of")
+    git_uno_results, _ = execute_command(["git", "status", "-uno"], lines_containing="is ahead of")
     if git_uno_results:
-        ERROR_PRINT("You have committed changes to this branch that you committed but not pushed.")
+        PRINT("You have committed changes to this branch that you committed but not pushed.")
         return False
     return True
 
 
 def verify_tagged() -> bool:
     """
     If the current git repo has a tag as its most recent commit then returns True,
-    otherwise prints an error message and returns False.
+    otherwise prints a warning and returns False.
     """
-    git_most_recent_commit, _ = execute_command("git log -1 --decorate", lines_containing="tag:")
+    git_most_recent_commit, _ = execute_command(["git", "log", "-1", "--decorate"], lines_containing="tag:")
     if not git_most_recent_commit:
-        ERROR_PRINT("You can only publish a tagged commit.")
+        PRINT("You can only publish a tagged commit.")
         return False
     return True
 
 
 def verify_untracked_files() -> bool:
     """
     If the current git repo has no untracked files then returns True,
-    otherwise prints an error message, with the list of untracked files,
+    otherwise prints a warning, and with the list of untracked files,
     and prompts the user for a yes/no confirmation on whether or to
     continue, and returns True for a yes response, otherwise returns False.
     """
     untracked_files = get_untracked_files()
     if untracked_files:
-        PRINT(f"You are about to PUBLISH the following ({len(untracked_files)})"
+        PRINT(f"WARNING: You are about to PUBLISH the following ({len(untracked_files)})"
               f" UNTRACKED file{'' if len(untracked_files) == 1 else 's' } -> SECURITY risk:")
         for untracked_file in untracked_files:
             PRINT(f"-- {untracked_file}")
         PRINT("DO NOT continue UNLESS you KNOW what you are doing!")
         if not answered_yes_to_confirmation("Do you really want to continue?"):
             return False
     return True
 
 
 def verify_not_already_published(package_name: str, package_version: str) -> bool:
     """
     If the given package and version has not already been published to PyPi then returns True,
-    otherwise prints an error message and returns False.
+    otherwise prints a warning and returns False.
     """
-    url = f"{PYPI_BASE_URL}/project/{package_name}/{package_version}/"
-    DEBUG_PRINT(f"curl {url}")
-    response = requests.get(url)
+    response = requests.get(f"https://pypi.org/project/{package_name}/{package_version}/")
     if response.status_code == 200:
-        ERROR_PRINT(f"Package {package_name} {package_version} has already been published to PyPi.")
+        PRINT(f"Package {package_name} {package_version} has already been published to PyPi.")
         return False
     return True
 
 
 def get_untracked_files() -> list:
     """
-    Returns a list of untracked files for the current git repo; empty list if no untracked changes.
-    We ignore __pycache__ directories for this which are already excluded by poetry publish.
+    Returns a list of untracked files for the current git repo; empty list of no untracked changes.
+    We ignore __pycache__ directories which are excluded by poetry publish.
     We ignore the .gitignore file for this.
     """
     package_directories = get_package_directories()
     untracked_files = []
     for package_directory in package_directories:
-        # Note that the output of "git status -s --ignored" looks something like this:
-        # ?? chalicelib_fourfront/some_untracked_file.py
-        # !! chalicelib_fourfront/__pycache__/
-        # Note that the --ignored option ignores the .gitignore file.
-        git_status_results, _ = execute_command(f"git status -s --ignored {package_directory}")
+        # The --ignored option ignores the .gitignore file.
+        git_status_results, _ = execute_command(["git", "status", "-s", "--ignored", package_directory])
         for git_status_result in git_status_results:
             if git_status_result and (git_status_result.startswith("??") or git_status_result.startswith("!!")):
                 untracked_file = git_status_result[2:].strip()
                 if untracked_file:
-                    # Ignore any __pycache__ directories as they are already ignored by poetry publish.
+                    # Ignore any __pycache__ directories as the are ignored by poetry publish.
                     if os.path.isdir(untracked_file) and os.path.basename(untracked_file.rstrip("/")) == "__pycache__":
                         continue
                     untracked_files.append(untracked_file)
     return untracked_files
 
 
 def get_package_version() -> str:
@@ -251,15 +234,15 @@
     return package_version
 
 
 def get_package_name() -> str:
     """
     Returns the base name of the current git repo name.
     """
-    package_name, _ = execute_command("git config --get remote.origin.url")
+    package_name, _ = execute_command("git config --get remote.origin.url".split(" "))
     package_name = os.path.basename(package_name[0])
     if package_name.endswith(".git"):
         package_name = package_name[:-4]
     return package_name
 
 
 def get_package_directories() -> list:
@@ -287,15 +270,16 @@
     is the list of lines from the output of the command, and the second element is the exit status code.
     """
     def cleanup_funny_output(output: str) -> str:
         return output.replace("('", "").replace("',)", "").replace("\\n\\n", "\n").replace("\\n", "\n")
 
     if isinstance(command_argv, str):
         command_argv = [arg for arg in command_argv.split(" ") if arg.strip()]
-    DEBUG_PRINT(" ".join(command_argv))
+    if DEBUG:
+        PRINT(f"DEBUG: {' '.join(command_argv)}")
     result = subprocess.run(command_argv, stdout=subprocess.PIPE,
                             stderr=subprocess.STDOUT)
     lines = result.stdout.decode("utf-8").split("\n")
     if lines_containing:
         lines = [line for line in lines if lines_containing in line]
     return [cleanup_funny_output(line.strip()) for line in lines if line.strip()], result.returncode
 
@@ -316,26 +300,9 @@
     Exits this process immediately with status 1;
     first prints a message saying no action was taken.
     """
     PRINT("Exiting without taking action.")
     exit(1)
 
 
-def PRINT(s):
-    print(s)
-
-
-def WARNING_PRINT(s):
-    PRINT(f"WARNING: {s}")
-
-
-def ERROR_PRINT(s):
-    PRINT(f"ERROR: {s}")
-
-
-def DEBUG_PRINT(s):
-    if DEBUG:
-        PRINT(f"DEBUG: {s}")
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `dcicutils-7.4.4/dcicutils/secrets_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/snapshot_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/task_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/dcicutils/trace_utils.py` & `dcicutils-7.4.4.1b2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.4.4/pyproject.toml` & `dcicutils-7.4.4.1b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.4.4"
+version = "7.4.4.1b2"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.4.4/setup.py` & `dcicutils-7.4.4.1b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.4.4',
+    'version': '7.4.4.1b2',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.4.4/PKG-INFO` & `dcicutils-7.4.4.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.4.4
+Version: 7.4.4.1b2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

