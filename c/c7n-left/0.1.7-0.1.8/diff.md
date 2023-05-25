# Comparing `tmp/c7n_left-0.1.7-py3-none-any.whl.zip` & `tmp/c7n_left-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 19614 bytes, number of entries: 15
+Zip file size: 19618 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     2977 b- defN 80-Jan-01 00:00 c7n_left/cli.py
 -rw-r--r--  2.0 unx    11560 b- defN 80-Jan-01 00:00 c7n_left/core.py
 -rw-r--r--  2.0 unx      142 b- defN 80-Jan-01 00:00 c7n_left/entry.py
 -rw-r--r--  2.0 unx     4315 b- defN 80-Jan-01 00:00 c7n_left/filters.py
--rw-r--r--  2.0 unx    11802 b- defN 80-Jan-01 00:00 c7n_left/output.py
+-rw-r--r--  2.0 unx    11824 b- defN 80-Jan-01 00:00 c7n_left/output.py
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/__init__.py
 -rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/graph.py
 -rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/provider.py
 -rw-r--r--  2.0 unx      945 b- defN 80-Jan-01 00:00 c7n_left/providers/terraform/resource.py
 -rw-r--r--  2.0 unx     7208 b- defN 80-Jan-01 00:00 c7n_left/test.py
 -rw-r--r--  2.0 unx      732 b- defN 80-Jan-01 00:00 c7n_left/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.7.dist-info/METADATA
-?rw-------  2.0 unx     1206 b- defN 23-Apr-12 11:00 c7n_left-0.1.7.dist-info/RECORD
-15 files, 58040 bytes uncompressed, 17632 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_left-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 80-Jan-01 00:00 c7n_left-0.1.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    12065 b- defN 16-Jan-01 00:00 c7n_left-0.1.8.dist-info/METADATA
+?rw-------  2.0 unx     1206 b- defN 23-May-25 11:15 c7n_left-0.1.8.dist-info/RECORD
+15 files, 58062 bytes uncompressed, 17636 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: c7n_left/test.py
 Comment: 
 
 Filename: c7n_left/utils.py
 Comment: 
 
-Filename: c7n_left-0.1.7.dist-info/WHEEL
+Filename: c7n_left-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_left-0.1.7.dist-info/entry_points.txt
+Filename: c7n_left-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_left-0.1.7.dist-info/METADATA
+Filename: c7n_left-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: c7n_left-0.1.7.dist-info/RECORD
+Filename: c7n_left-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_left/output.py

```diff
@@ -2,23 +2,23 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 import json
 from collections import Counter
 from pathlib import Path
 import time
 
-import jmespath
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.text import Text
 
 from .core import CollectionRunner, PolicyMetadata
 from .utils import SEVERITY_LEVELS
 from c7n.output import OutputRegistry
+from c7n.utils import jmespath_search
 
 
 report_outputs = OutputRegistry("left")
 
 
 def get_reporter(config):
     for k, v in report_outputs.items():
@@ -352,15 +352,15 @@
 
     def on_results(self, results):
         self.results.extend(results)
 
     def on_execution_ended(self):
         formatted_results = [self.format_result(r) for r in self.results]
         if self.config.output_query:
-            formatted_results = jmespath.search(
+            formatted_results = jmespath_search(
                 self.config.output_query, formatted_results
             )
         self.config.output_file.write(
             json.dumps({"results": formatted_results}, cls=JSONEncoder, indent=2)
         )
 
     def format_result(self, result):
```

## Comparing `c7n_left-0.1.7.dist-info/METADATA` & `c7n_left-0.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c7n-left
-Version: 0.1.7
+Version: 0.1.8
 Summary: Custodian policies for IAAC definitions
 Home-page: https://cloudcustodian.io
 License: Apache-2
 Author: Cloud Custodian Project
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
@@ -12,41 +12,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: c7n (==0.9.26) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: boto3 (==1.26.109) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: c7n (==0.9.27) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: click (==8.1.3) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: rich (==13.3.5) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: tfparse (==0.5.0) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: argcomplete (==3.0.8) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: boto3 (==1.26.139) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: docutils (==0.18.1) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: importlib-metadata (==5.2.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: jsonschema (==4.17.3) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: argcomplete (==3.0.5) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: python-dateutil (==2.8.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pyyaml (==6.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: tabulate (==0.9.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: importlib-metadata (==5.2.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: docutils (==0.18.1) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: botocore (==1.29.109) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: urllib3 (==1.26.16) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: colorama (==0.4.6) ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
+Requires-Dist: markdown-it-py (==2.2.0) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: pygments (==2.15.1) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: typing-extensions (==4.6.1) ; python_version >= "3.7" and python_version < "3.9"
+Requires-Dist: cffi (==1.15.1) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: botocore (==1.29.139) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: jmespath (==1.0.1) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: s3transfer (==0.6.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: attrs (==22.2.0) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: s3transfer (==0.6.1) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: zipp (==3.15.0) ; python_version >= "3.7" and python_version < "4.0"
+Requires-Dist: attrs (==23.1.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: importlib-resources (==5.12.0) ; python_version >= "3.7" and python_version < "3.9"
 Requires-Dist: pkgutil-resolve-name (==1.3.10) ; python_version >= "3.7" and python_version < "3.9"
 Requires-Dist: pyrsistent (==0.19.3) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: typing-extensions (==4.5.0) ; python_version >= "3.7" and python_version < "3.9"
 Requires-Dist: six (==1.16.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: zipp (==3.15.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: urllib3 (==1.26.15) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: click (==8.1.3) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: rich (==13.3.3) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: tfparse (==0.5.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: colorama (==0.4.6) ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
-Requires-Dist: markdown-it-py (==2.2.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: pygments (==2.14.0) ; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: cffi (==1.15.1) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: mdurl (==0.1.2) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pycparser (==2.21) ; python_version >= "3.7" and python_version < "4.0"
 Project-URL: Documentation, https://cloudcustodian.io/docs/
 Project-URL: Repository, https://github.com/cloud-custodian/cloud-custodian
 Description-Content-Type: text/markdown
 
 # Custodian policies for Infrastructure Code
```

## Comparing `c7n_left-0.1.7.dist-info/RECORD` & `c7n_left-0.1.8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 c7n_left/cli.py,sha256=Ve97mFA__pIr7cVh5KUHpGVpk7N9bS0AnMXYfjYrgEE,2977
 c7n_left/core.py,sha256=HYj2zIa4p9DYWkh78SqRhTOQj4qN_ezMalQu4CfrYG4,11560
 c7n_left/entry.py,sha256=qnxA1j66drB8YISyJQmRiv0DKG0lv5SOogIuL2IDE6M,142
 c7n_left/filters.py,sha256=8yYvVBBtiozDpi8_KWSfJWflbqm6Fp9BvtPrsN2fIQk,4315
-c7n_left/output.py,sha256=aeaPfPFzLhQyc3HRnXY5l88HXUtIkmxPloAleEK2qVM,11802
+c7n_left/output.py,sha256=CFEOF65v4EJgTm0ShjUBS1fJAn8U1q0XNKltpgWCqQU,11824
 c7n_left/providers/terraform/__init__.py,sha256=BPUsPHvPInkb9N5fqhYccTRt_dWnFsdSEkFSDwgAFlY,121
 c7n_left/providers/terraform/graph.py,sha256=b47aqwKM6QCjdfRwWwteciplflNER-WKw86JTB-F1Gc,3282
 c7n_left/providers/terraform/provider.py,sha256=5etOLvG-3nssOsfw1Dfs08QPTmujiBb6RvfZ1v_7Ve4,1552
 c7n_left/providers/terraform/resource.py,sha256=6sZhzlHrZ8unJKJViHsQkalQAspCzUyMAL8mjzngR98,945
 c7n_left/test.py,sha256=iOW7nQLjCk9Luk4LhjAqKfKBnoy_tJCUrMPO9qKW20I,7208
 c7n_left/utils.py,sha256=V8yRbNRjKmuz24ZrfYwtYSLdyLMlZ0MVIhAkZdMwFbQ,732
-c7n_left-0.1.7.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
-c7n_left-0.1.7.dist-info/entry_points.txt,sha256=BP7MM3oxRCtY3qaC9GsUqrYj3962epelsmHx4XkQ6pY,45
-c7n_left-0.1.7.dist-info/RECORD,,
-c7n_left-0.1.7.dist-info/METADATA,sha256=ktOHViWiooXV9QPjXfIw1fENbJIMNKQsMnDYrogOQf4,12065
+c7n_left-0.1.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+c7n_left-0.1.8.dist-info/entry_points.txt,sha256=BP7MM3oxRCtY3qaC9GsUqrYj3962epelsmHx4XkQ6pY,45
+c7n_left-0.1.8.dist-info/RECORD,,
+c7n_left-0.1.8.dist-info/METADATA,sha256=GTkpHvgwm6WfacDecQ7GOkiD0EvP4kDJ15YEYaS9vUI,12065
```

