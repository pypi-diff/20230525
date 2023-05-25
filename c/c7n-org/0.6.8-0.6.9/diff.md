# Comparing `tmp/c7n_org-0.6.8-py3-none-any.whl.zip` & `tmp/c7n_org-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10971 bytes, number of entries: 8
+Zip file size: 11000 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       79 b- defN 20-Sep-08 15:42 c7n_org/__init__.py
--rw-rw-r--  2.0 unx    25442 b- defN 20-Nov-17 16:47 c7n_org/cli.py
+-rw-rw-r--  2.0 unx    25470 b- defN 21-Jan-11 16:47 c7n_org/cli.py
 -rw-rw-r--  2.0 unx      771 b- defN 20-Nov-17 16:47 c7n_org/utils.py
--rw-rw-r--  2.0 unx     6761 b- defN 20-Dec-14 16:37 c7n_org-0.6.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_org-0.6.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       45 b- defN 20-Dec-14 16:37 c7n_org-0.6.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 20-Dec-14 16:37 c7n_org-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      610 b- defN 20-Dec-14 16:37 c7n_org-0.6.8.dist-info/RECORD
-8 files, 33808 bytes uncompressed, 9907 bytes compressed:  70.7%
+-rw-rw-r--  2.0 unx     6807 b- defN 21-Jan-11 16:55 c7n_org-0.6.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_org-0.6.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       45 b- defN 21-Jan-11 16:55 c7n_org-0.6.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 21-Jan-11 16:55 c7n_org-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      610 b- defN 21-Jan-11 16:55 c7n_org-0.6.9.dist-info/RECORD
+8 files, 33882 bytes uncompressed, 9936 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: c7n_org/cli.py
 Comment: 
 
 Filename: c7n_org/utils.py
 Comment: 
 
-Filename: c7n_org-0.6.8.dist-info/METADATA
+Filename: c7n_org-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_org-0.6.8.dist-info/WHEEL
+Filename: c7n_org-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_org-0.6.8.dist-info/entry_points.txt
+Filename: c7n_org-0.6.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_org-0.6.8.dist-info/top_level.txt
+Filename: c7n_org-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_org-0.6.8.dist-info/RECORD
+Filename: c7n_org-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_org/cli.py

```diff
@@ -25,15 +25,15 @@
 from c7n.credentials import assumed_session, SessionFactory
 from c7n.executor import MainThreadExecutor
 from c7n.config import Config
 from c7n.policy import PolicyCollection
 from c7n.provider import get_resource_class
 from c7n.reports.csvout import Formatter, fs_record_set
 from c7n.resources import load_available
-from c7n.utils import CONN_CACHE, dumps
+from c7n.utils import CONN_CACHE, dumps, filter_empty
 
 from c7n_org.utils import environ, account_tags
 
 log = logging.getLogger('c7n_org')
 
 # Workaround OSX issue, note this exists for py2 but there
 # isn't anything we can do in that case.
@@ -396,15 +396,15 @@
         env['AWS_DEFAULT_REGION'] = region
         env['AWS_ACCOUNT_ID'] = account["account_id"]
     elif account["provider"] == 'azure':
         env['AZURE_SUBSCRIPTION_ID'] = account["account_id"]
     elif account["provider"] == 'gcp':
         env['GOOGLE_CLOUD_PROJECT'] = account["account_id"]
         env['CLOUDSDK_CORE_PROJECT'] = account["account_id"]
-    return env
+    return filter_empty(env)
 
 
 def run_account_script(account, region, output_dir, debug, script_args):
 
     try:
         session = get_session(account, "org-script", region)
     except ClientError:
```

## Comparing `c7n_org-0.6.8.dist-info/METADATA` & `c7n_org-0.6.9.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: c7n-org
-Version: 0.6.8
+Version: 0.6.9
 Summary: Cloud Custodian - Parallel Execution
 Home-page: https://cloudcustodian.io
 Author: Cloud Custodian Project
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
 Requires-Dist: argcomplete (==1.12.2)
 Requires-Dist: attrs (==20.3.0)
-Requires-Dist: boto3 (==1.16.32)
-Requires-Dist: botocore (==1.19.32)
-Requires-Dist: c7n (==0.9.8)
-Requires-Dist: importlib-metadata (==1.7.0)
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
+Requires-Dist: c7n (==0.9.10)
+Requires-Dist: importlib-metadata (==3.3.0)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonpickle (==1.3)
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: pyrsistent (==0.17.3)
 Requires-Dist: python-dateutil (==2.8.1)
 Requires-Dist: pyyaml (==5.3.1)
 Requires-Dist: s3transfer (==0.3.3)
 Requires-Dist: six (==1.15.0)
 Requires-Dist: tabulate (==0.8.7)
+Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: urllib3 (==1.26.2)
 Requires-Dist: zipp (==3.4.0)
 Requires-Dist: click (==7.1.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 
 # c7n-org: Multi Account Custodian Execution
 
 [//]: # (         !!! IMPORTANT !!!                    )
```

