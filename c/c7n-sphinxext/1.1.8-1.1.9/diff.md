# Comparing `tmp/c7n_sphinxext-1.1.8-py3-none-any.whl.zip` & `tmp/c7n_sphinxext-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8867 bytes, number of entries: 14
+Zip file size: 8881 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx       81 b- defN 20-Nov-17 16:47 c7n_sphinxext/__init__.py
 -rw-rw-r--  2.0 unx    11906 b- defN 20-Nov-17 16:47 c7n_sphinxext/docgen.py
 -rw-rw-r--  2.0 unx      520 b- defN 20-Sep-08 15:42 c7n_sphinxext/_templates/provider-common-elements.rst
 -rw-rw-r--  2.0 unx      242 b- defN 20-Sep-08 15:42 c7n_sphinxext/_templates/provider-group.rst
 -rw-rw-r--  2.0 unx      428 b- defN 20-Sep-08 15:42 c7n_sphinxext/_templates/provider-index.rst
 -rw-rw-r--  2.0 unx      378 b- defN 20-Oct-15 17:51 c7n_sphinxext/_templates/provider-mode.rst
 -rw-rw-r--  2.0 unx      119 b- defN 20-Sep-08 15:42 c7n_sphinxext/_templates/provider-resource.rst
 -rw-rw-r--  2.0 unx     1228 b- defN 20-Oct-15 17:51 c7n_sphinxext/_templates/resource.rst
 -rw-rw-r--  2.0 unx      247 b- defN 20-Sep-08 15:42 c7n_sphinxext/_templates/schema.rst
--rw-rw-r--  2.0 unx     3534 b- defN 20-Dec-14 16:37 c7n_sphinxext-1.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Dec-14 16:37 c7n_sphinxext-1.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       61 b- defN 20-Dec-14 16:37 c7n_sphinxext-1.1.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       14 b- defN 20-Dec-14 16:37 c7n_sphinxext-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1276 b- defN 20-Dec-14 16:37 c7n_sphinxext-1.1.8.dist-info/RECORD
-14 files, 20126 bytes uncompressed, 6691 bytes compressed:  66.8%
+-rw-rw-r--  2.0 unx     3674 b- defN 21-Jan-11 16:55 c7n_sphinxext-1.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Jan-11 16:55 c7n_sphinxext-1.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       61 b- defN 21-Jan-11 16:55 c7n_sphinxext-1.1.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       14 b- defN 21-Jan-11 16:55 c7n_sphinxext-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1276 b- defN 21-Jan-11 16:55 c7n_sphinxext-1.1.9.dist-info/RECORD
+14 files, 20266 bytes uncompressed, 6705 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: c7n_sphinxext/_templates/resource.rst
 Comment: 
 
 Filename: c7n_sphinxext/_templates/schema.rst
 Comment: 
 
-Filename: c7n_sphinxext-1.1.8.dist-info/METADATA
+Filename: c7n_sphinxext-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_sphinxext-1.1.8.dist-info/WHEEL
+Filename: c7n_sphinxext-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_sphinxext-1.1.8.dist-info/entry_points.txt
+Filename: c7n_sphinxext-1.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_sphinxext-1.1.8.dist-info/top_level.txt
+Filename: c7n_sphinxext-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: c7n_sphinxext-1.1.8.dist-info/RECORD
+Filename: c7n_sphinxext-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `c7n_sphinxext-1.1.8.dist-info/METADATA` & `c7n_sphinxext-1.1.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: c7n-sphinxext
-Version: 1.1.8
+Version: 1.1.9
 Summary: Cloud Custodian - Sphinx Extensions
 Home-page: https://cloudcustodian.io
 Author: Cloud Custodian Project
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
 Requires-Dist: alabaster (==0.7.12)
 Requires-Dist: argcomplete (==1.12.2)
 Requires-Dist: attrs (==20.3.0)
-Requires-Dist: boto3 (==1.16.32)
-Requires-Dist: botocore (==1.19.32)
-Requires-Dist: c7n (==0.9.8)
+Requires-Dist: boto3 (==1.16.42)
+Requires-Dist: botocore (==1.19.42)
+Requires-Dist: c7n (==0.9.10)
 Requires-Dist: certifi (==2020.12.5)
-Requires-Dist: chardet (==3.0.4)
 Requires-Dist: commonmark (==0.9.1)
-Requires-Dist: importlib-metadata (==1.7.0)
+Requires-Dist: importlib-metadata (==3.3.0)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonpickle (==1.3)
 Requires-Dist: jsonschema (==3.2.0)
 Requires-Dist: pyrsistent (==0.17.3)
 Requires-Dist: python-dateutil (==2.8.1)
 Requires-Dist: pytz (==2020.4)
 Requires-Dist: pyyaml (==5.3.1)
 Requires-Dist: recommonmark (==0.6.0)
 Requires-Dist: s3transfer (==0.3.3)
 Requires-Dist: six (==1.15.0)
 Requires-Dist: snowballstemmer (==2.0.0)
 Requires-Dist: sphinx-markdown-tables (==0.0.12)
 Requires-Dist: sphinx-rtd-theme (==0.4.3)
 Requires-Dist: tabulate (==0.8.7)
+Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: urllib3 (==1.26.2)
 Requires-Dist: zipp (==3.4.0)
 Requires-Dist: pyparsing (==2.4.7) ; python_version >= "2.6" and python_full_version < "3.0.0" or python_full_version >= "3.3.0"
 Requires-Dist: babel (==2.9.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: idna (==2.10) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: imagesize (==1.2.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: markdown (==3.0.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
 Requires-Dist: markupsafe (==1.1.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
-Requires-Dist: packaging (==20.7) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
+Requires-Dist: packaging (==20.8) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.4.0"
+Requires-Dist: chardet (==4.0.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: click (==7.1.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: colorama (==0.4.4) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: docutils (==0.16) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: jinja2 (==2.11.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
-Requires-Dist: requests (==2.25.0) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
+Requires-Dist: requests (==2.25.1) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0"
 Requires-Dist: urllib3 (==1.26.2) ; python_version >= "2.7" and python_full_version < "3.0.0" or python_full_version >= "3.5.0" and python_version < "4"
 Requires-Dist: pygments (==2.7.3) ; python_version >= "3.5"
 Requires-Dist: sphinx (==3.0.4) ; python_version >= "3.5"
 Requires-Dist: sphinxcontrib-applehelp (==1.0.2) ; python_version >= "3.5"
 Requires-Dist: sphinxcontrib-devhelp (==1.0.2) ; python_version >= "3.5"
 Requires-Dist: sphinxcontrib-htmlhelp (==1.0.3) ; python_version >= "3.5"
 Requires-Dist: sphinxcontrib-jsmath (==1.0.1) ; python_version >= "3.5"
```

## Comparing `c7n_sphinxext-1.1.8.dist-info/RECORD` & `c7n_sphinxext-1.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 c7n_sphinxext/_templates/provider-common-elements.rst,sha256=B1tNJeNZGpBwQZuXkER45Xi5b1qpA2fvKruDHJawH7E,520
 c7n_sphinxext/_templates/provider-group.rst,sha256=Yk4RsQnojWv1rVJmeIjoUl-l_LM6z8j2p-oSkxzfqrI,242
 c7n_sphinxext/_templates/provider-index.rst,sha256=kSWPLb6oMcXyW9llKDy9I42KgUPIu_8sPiQtZqC8iVw,428
 c7n_sphinxext/_templates/provider-mode.rst,sha256=vNQN2WSX2JMnsQejZZj5TjKe_oHwEjolw1wEuoOJq40,378
 c7n_sphinxext/_templates/provider-resource.rst,sha256=kIozWHSfVNsk8oy_D6gUCR_3SS0vwBvgK0m1j3A5jLk,119
 c7n_sphinxext/_templates/resource.rst,sha256=Ix7mlugGYxGUsTl89IjWW2RlTEqDWDSJtgIltIYpDJs,1228
 c7n_sphinxext/_templates/schema.rst,sha256=SZQiMZAOS4YJj8Atfsuqdbw3RqAAlAYdTvqADXQOuZo,247
-c7n_sphinxext-1.1.8.dist-info/METADATA,sha256=yk4XzbZf-7jajmM37Q_CjA0-qADy_Rqj9eUc2GtTbgQ,3534
-c7n_sphinxext-1.1.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-c7n_sphinxext-1.1.8.dist-info/entry_points.txt,sha256=mvZUN5aIv36_dV3pzLxNX4ffnUktyA5j4xUJi9PmOAQ,61
-c7n_sphinxext-1.1.8.dist-info/top_level.txt,sha256=2vUgRlr3tLvPy6drUvG2bIdBpdGC7YRhR22etGAs_tg,14
-c7n_sphinxext-1.1.8.dist-info/RECORD,,
+c7n_sphinxext-1.1.9.dist-info/METADATA,sha256=P_ZyropDtXkGP34zXu3waEvVKatHJbt7HJUgj50nqDo,3674
+c7n_sphinxext-1.1.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+c7n_sphinxext-1.1.9.dist-info/entry_points.txt,sha256=mvZUN5aIv36_dV3pzLxNX4ffnUktyA5j4xUJi9PmOAQ,61
+c7n_sphinxext-1.1.9.dist-info/top_level.txt,sha256=2vUgRlr3tLvPy6drUvG2bIdBpdGC7YRhR22etGAs_tg,14
+c7n_sphinxext-1.1.9.dist-info/RECORD,,
```

