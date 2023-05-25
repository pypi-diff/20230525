# Comparing `tmp/c7n_policystream-0.4.8-py3-none-any.whl.zip` & `tmp/c7n_policystream-0.4.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 12354 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    32843 b- defN 20-Nov-17 16:47 policystream.py
--rw-rw-r--  2.0 unx     5994 b- defN 20-Dec-14 16:37 c7n_policystream-0.4.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_policystream-0.4.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       55 b- defN 20-Dec-14 16:37 c7n_policystream-0.4.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 20-Dec-14 16:37 c7n_policystream-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      511 b- defN 20-Dec-14 16:37 c7n_policystream-0.4.8.dist-info/RECORD
-6 files, 39508 bytes uncompressed, 11420 bytes compressed:  71.1%
+Zip file size: 12303 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    32583 b- defN 21-Jan-11 16:47 policystream.py
+-rw-rw-r--  2.0 unx     6134 b- defN 21-Jan-11 16:55 c7n_policystream-0.4.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_policystream-0.4.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       55 b- defN 21-Jan-11 16:55 c7n_policystream-0.4.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 21-Jan-11 16:55 c7n_policystream-0.4.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      511 b- defN 21-Jan-11 16:55 c7n_policystream-0.4.9.dist-info/RECORD
+6 files, 39388 bytes uncompressed, 11369 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: policystream.py
 Comment: 
 
-Filename: c7n_policystream-0.4.8.dist-info/METADATA
+Filename: c7n_policystream-0.4.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_policystream-0.4.8.dist-info/WHEEL
+Filename: c7n_policystream-0.4.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_policystream-0.4.8.dist-info/entry_points.txt
+Filename: c7n_policystream-0.4.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_policystream-0.4.8.dist-info/top_level.txt
+Filename: c7n_policystream-0.4.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_policystream-0.4.8.dist-info/RECORD
+Filename: c7n_policystream-0.4.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## policystream.py

```diff
@@ -395,19 +395,15 @@
                     current_policies += self.policy_files[f]
             elif delta.status == GIT_DELTA_INVERT['GIT_DELTA_MODIFIED']:
                 change_policies += self._policy_file_rev(f, change)
                 if f in self.policy_files:
                     current_policies += self.policy_files[f]
             elif delta.status == GIT_DELTA_INVERT['GIT_DELTA_DELETED']:
                 if f in self.policy_files:
-                    # if the policies were moved, only add in policies
-                    # that are not already accounted for.
-                    current_policies += self.policy_files[f].select(
-                        set(current_policies.keys()).difference(
-                            self.policy_files[f].keys()))
+                    current_policies += self.policy_files[f]
                     removed.add(f)
             elif delta.status == GIT_DELTA_INVERT['GIT_DELTA_RENAMED']:
                 change_policies += self._policy_file_rev(f, change)
                 current_policies += self.policy_files[delta.old_file.path]
                 removed.add(delta.old_file.path)
             else:
                 log.info(
```

## Comparing `c7n_policystream-0.4.8.dist-info/METADATA` & `c7n_policystream-0.4.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: c7n-policystream
-Version: 0.4.8
+Version: 0.4.9
 Summary: Cloud Custodian - Git Commits as Logical Policy Changes
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
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
+Requires-Dist: c7n (==0.9.10)
 Requires-Dist: certifi (==2020.12.5)
 Requires-Dist: cffi (==1.14.4)
-Requires-Dist: chardet (==3.0.4)
-Requires-Dist: importlib-metadata (==1.7.0)
+Requires-Dist: importlib-metadata (==3.3.0)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonpickle (==1.3)
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: pygit2 (==1.0.3)
 Requires-Dist: pyrsistent (==0.17.3)
 Requires-Dist: python-dateutil (==2.8.1)
 Requires-Dist: pyyaml (==5.3.1)
 Requires-Dist: s3transfer (==0.3.3)
 Requires-Dist: six (==1.15.0)
 Requires-Dist: tabulate (==0.8.7)
+Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: urllib3 (==1.26.2)
 Requires-Dist: zipp (==3.4.0)
 Requires-Dist: jmespath (==0.10.0) ; python_version >= "2.6" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: python-dateutil (==2.8.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: six (==1.15.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: idna (==2.10) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: pycparser (==2.20) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
+Requires-Dist: chardet (==4.0.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: click (==7.1.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: pyyaml (==5.3.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
-Requires-Dist: requests (==2.25.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
+Requires-Dist: requests (==2.25.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: urllib3 (==1.26.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version < "4"
 
 # c7n-policystream: Policy Changes from Git
 
 [//]: # (         !!! IMPORTANT !!!                    )
 [//]: # (This file is moved during document generation.)
 [//]: # (Only edit the original document at ./tools/c7n_policystream/README.md)
```

